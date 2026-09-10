# Workflow: Cloud / DevOps / SRE Job Market Scan

A plain-English recipe to produce a curated US-remote job shortlist for a
senior Linux Systems Engineer profile. Designed to be re-run weekly.

## Inputs (load before running)

- `resources/sources.md` — source list and locked filter criteria
- `CLAUDE.md` — candidate profile and project rules
- Today's date (used for the output filename and "Sources & method" section)

## Step 1 — Confirm scope hasn't drifted

Before running, glance at `resources/sources.md` and confirm:

- Filter criteria still match user intent (Linux+IaC, observability/SIEM, US-remote).
- No major source has been retired (e.g. board shut down) — if so, prune.

Ask the user only if criteria are unclear or have visibly changed since last run.

## Step 2 — Query each source group

Run in this order, capturing raw hits before filtering:

1. **Cloud-native tech employers** — for each company in `sources.md`,
   query their careers page or run `site:<ats-host> <company> remote senior devops terraform`.
   Prefer the employer's own ATS URL (Greenhouse / Lever / Ashby / Workday) over
   aggregator mirrors (Himalayas, Built In, Talentify, RemoteRocketShip,
   Jobright.ai). Aggregator URLs go stale silently and are not acceptable as
   the final apply link on the report.
2. **Energy-sector employers** — same approach; bias toward companies with a
   clear software platform (Kraken/Octopus, Uplight, Arcadia, NextEra Digital).
3. **Aggregators / boards** — none currently in `sources.md`. RemoteOK,
   WeWorkRemotely, and Wellfound were removed 2026-09-09: all three routinely
   return 403/410 to automated fetch, RemoteOK's tag pages have been observed
   returning "hire a freelancer" placeholder pages instead of real listings,
   and hits sourced from them repeatedly failed Step 3.5 validation. Skip this
   step unless `sources.md` lists a replacement aggregator.
4. **LinkedIn** — last, because hits often duplicate earlier ATS finds. Use it
   to surface postings missed by the company-page sweep.

Capture for each hit: title, company, JD URL, location/remote text, date posted,
key stack keywords. Don't filter yet — collect first.

**Collection-time sanity check (do this before recording the hit, not just in
Step 3.5):** web search frequently indexes Greenhouse/Ashby/Lever job IDs for
postings that have already been removed — this has produced a high dead-link
rate on well-known boards (GitLab, Grafana Labs, Honeycomb, Wiz, Close, The
Farmer's Dog all 404'd in one run despite fresh-looking search snippets). Before
adding a specific Greenhouse/Ashby/Lever job ID to the raw-hits list, cross-check
it against that employer's current listing, not just the search snippet:

- **Greenhouse** — `https://api.greenhouse.io/v1/boards/<board-token>/jobs`
  (fall back to `boards-api.greenhouse.io` if that 404s) and confirm the job ID
  is present.
- **Ashby** — `https://api.ashbyhq.com/posting-api/job-board/<org-slug>` and
  confirm the job ID/title is present. If this returns "Unauthorized," the
  board isn't public via API — fall back to WebFetch on the `jobs.ashbyhq.com`
  URL directly and treat it as inconclusive (not a pass) if that renders empty.
- **Lever** — `https://api.lever.co/v0/postings/<company-slug>?mode=json` and
  confirm the posting is in the array.

If the ID isn't in the current listing, drop it now rather than carrying a dead
hit through Steps 3–4. This is a cheap check (one API call per company, not per
hit) and catches most of the dead-link volume before the expensive per-role
validation in Step 3.5.

## Step 3 — Apply the three must-have filters

Drop any role that fails any of:

1. **Linux + IaC** — JD must name Terraform and/or Ansible explicitly. Generic
   "IaC experience" alone is not enough (too vague to verify fit).
2. **Observability / SIEM / security angle** — JD must mention at least one of:
   SIEM, SOAR, detection engineering, log pipelines, telemetry, observability
   ownership, Datadog/Splunk/Elastic/Grafana, security tooling.
3. **US-remote eligible, OR onsite/hybrid in the Seattle area** — either the JD
   doesn't exclude US-remote applicants (watch for "must be in [specific city]"
   or "EU only" disqualifiers; state exclusions like "not CA/CO/NY" only matter
   if they hit the candidate's state), OR the role is based in the Greater
   Seattle area (Seattle, Bellevue, Redmond, Kirkland, Renton, Tacoma, Everett,
   or listed generically as "Seattle, WA"/"Puget Sound") — the candidate can
   commute, so onsite/hybrid is fine there specifically. A city restriction
   *outside* the Seattle area still disqualifies a role even if remote isn't
   required elsewhere in the JD.

Tag any energy-sector match with `[ENERGY]`, and any Seattle-area onsite/hybrid
match with `[SEATTLE]`, for the report.

## Step 3.5 — URL validation (REQUIRED, no role goes on the report without it)

**Every** apply link that will appear on the final report must be validated
before inclusion. No exceptions. This step exists because aggregator and ATS
URLs go dead silently — a posting can be removed but the URL still resolves
to a generic listing or department index, which previously caused this report
to ship dead links.

For each candidate role:

1. **Hit the URL with WebFetch** and ask it to confirm STATUS=LIVE/DEAD, quote
   the exact job title, and confirm Terraform/Ansible/observability are named.
   Run validations in parallel — they're independent.
2. **Classify the response:**
   - `STATUS=LIVE` with the right title and stack → **PASS**. Note the
     verification source as "WebFetch — full JD returned (YYYY-MM-DD)".
   - `STATUS=DEAD` / 404 / 410 / "no longer accepting" → **FAIL**. Drop the role.
   - Redirect to a different host → re-fetch the redirect target once. If that
     also fails, drop the role.
   - HTTP 403 / empty SPA render → **inconclusive via WebFetch**. This is
     common on Lever, Workday, Ashby and some Greenhouse instances. Fall back
     to step 3.
3. **Fallback for ATS hosts that block WebFetch:** use the ATS's public JSON
   API. Search-engine snippets are **not** sufficient — they happily quote
   cached or removed postings and have produced false positives on this
   project before. Use these endpoints from Bash via curl:
   - **Lever** — `https://api.lever.co/v0/postings/<company-slug>?mode=json`
     returns the full current postings list with `text` (title), `hostedUrl`,
     `categories.location`, `workplaceType`, plus `description`/`lists`/
     `additional` fields containing the full JD. If a posting isn't in the
     returned array, it's not open. This is the canonical validator for any
     Lever URL.
   - **Greenhouse** — `https://api.greenhouse.io/v1/boards/<board-token>/jobs`
     lists current openings; append `/<job-id>?questions=true` for the full
     JD body.
   - **Ashby** — `https://api.ashbyhq.com/posting-api/job-board/<org-slug>`
     returns current openings; per-job detail at
     `https://api.ashbyhq.com/posting-api/job-board/<org-slug>/<job-id>`.
   - **Workday** has a JSON endpoint per tenant, typically at
     `https://<tenant>.<region>.myworkdayjobs.com/wday/cxs/<tenant>/<site>/jobs`
     for the listings index — verify the specific job ID is still present.
     **Known issue:** some tenants (e.g. CrowdStrike) return `403 permission
     denied` on a direct per-job fetch even though the listings-index POST
     works — don't treat that 403 as proof the job is dead, but also don't
     treat it as a pass. If the job ID doesn't turn up in the listings-index
     search either, mark it inconclusive and drop it rather than guessing.
   - For any ATS without a usable public API, the URL must instead be
     verifiable directly via WebFetch.
   When validating via an ATS API, confirm: (a) the URL is still in the
   current list, (b) the title matches, (c) Terraform/Ansible and the
   observability/SIEM angle appear in the JD body. Label these roles
   "Verified via <ATS> JSON API — `api.<host>.../<id>`".
4. **Aggregator/mirror pages do not count** as validation. Himalayas, Built In,
   Glassdoor, Jobright.ai, Talentify, RemoteRocketShip, etc. often mirror dead
   listings. If the only live evidence is on an aggregator, search for the
   posting on the employer's own ATS and use that URL instead. If no employer
   ATS URL can be found, drop the role.
5. **Record the verification status per role** in the report under a
   "Verified via" field, so the trail is auditable on the next run.

If validation drops the shortlist below the target volume, do not pad it with
unverified URLs. Surface the gap honestly in the report's "Summary" section
and offer to do a fresh scan.

## Step 4 — Rank and shortlist (target: 10–15)

Score each surviving role on:

- **Stack fit** — how many of {Linux, Terraform, Ansible, Python, SIEM,
  observability} are explicitly named (higher = better).
- **Profile match** — DevSecOps / SIEM / telemetry-pipeline language in the JD
  maps directly to candidate's background.
- **Signal quality** — direct ATS link > LinkedIn rewrite > aggregator link.

Pick top 10–15. Among those, designate **3–5 top picks** with strongest match.

## Step 5 — Write the report

Output path: `output/job-market-scan-YYYY-MM-DD.md` (use today's date).

Sections (in order):

1. **Summary** — ≤5 bullets: total found, energy-tagged count, Seattle-tagged
   count, top recurring stack overlaps, any notable industry signal.
2. **Top picks (3–5)** — each with 2–3 lines of rationale.
3. **Full shortlist (10–15)** — bullet-per-role format below.
4. **Sources & method** — list of sources actually queried, date, filter
   criteria applied. Required by the "cite sources" project rule.

### Per-role bullet format

- **Title** — Company `[ENERGY]` / `[SEATTLE]` if applicable
- **Location**: US-remote, or onsite/hybrid Seattle area (note any state/city restrictions)
- **Stack match**: which of Linux / Terraform / Ansible / Python / SIEM / observability are explicitly named in the JD
- **Why it fits**: one line tying the role to the candidate's background
- **Apply link**: direct JD URL
- **Source**: where it was found (e.g. Greenhouse — HashiCorp careers)

## Step 6 — Final spot-check before delivering

The bulk URL validation already happened in Step 3.5. This step is a sanity
pass on the **top picks specifically** — open each top-pick link in a browser
context (via WebFetch) one more time and confirm the JD is still the one
you summarized. If a top-pick link is dead, swap it for the next-best match
from the shortlist and re-validate before delivering.

## Step 7 — Note follow-ups

If you discover new strong employers or new dead sources during the run, update
`resources/sources.md` before finishing. This keeps the seed list current and
the next run cheaper.

## Step 8 — Log the run

Write `logs/job-market-scan-YYYY-MM-DD.json` (same date as the report) so runs
are comparable over time and the monitor dashboard has data to show. Follow the
schema in the most recent existing file under `logs/` — capture:

- **results** — raw hits collected, how many passed filtering + validation, final
  shortlist size.
- **token_usage** — exact `tokens`/`tool_uses`/`duration_ms` for every subagent
  used (from its completion notification). Main-thread usage is not measurable
  precisely — report a tool-call-count proxy (WebFetch/curl/WebSearch counts) and
  say so explicitly; never present the proxy as an exact figure.
- **timing** — approximate minutes per major step (collection, filter+validation,
  report writing), and say it's approximate.
- **source_coverage** — per source group in `resources/sources.md`: which
  companies/boards were queried, which yielded raw hits, which yielded nothing.
- **sites_visited** — every distinct URL fetched directly (WebFetch), with status
  and outcome (dead / filter-fail / inconclusive / pass).
- **api_hits** — every ATS JSON API call (Greenhouse/Ashby/Lever/Workday), with
  endpoint, status, and outcome.

Then update the monitor dashboard: read every file under `logs/`, and republish
the dashboard Artifact (URL and update instructions in `resources/monitor.md`)
with the combined data so it reflects all runs to date, not just the latest one.

## Project rules to honor (from CLAUDE.md)

- Ask clarifying questions only if scope is genuinely unclear.
- Show the plan before executing on a fresh complex task.
- Keep the report concise; bullet points preferred.
- Save all output to `output/`.
- Cite sources.
