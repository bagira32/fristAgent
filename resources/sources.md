# Job Hunt Sources & Filter Criteria

Reusable seed list for the **Cloud / DevOps / SRE — US-Remote or Seattle-area**
market scan.
Last reviewed: 2026-09-28.

## Candidate profile (anchors the filter)

Linux Systems Engineer · multi-cloud hardening · Terraform / Ansible · Python ·
SIEM / log pipelines · global-scale observability · DevSecOps.

## Locked filter criteria

A role must hit **ALL three** must-haves to make a shortlist:

1. **Linux + IaC** — Terraform and/or Ansible explicitly named in the JD.
2. **Observability / SIEM / security angle** — SIEM, SOAR, detection engineering,
   log/telemetry pipelines, or strong observability ownership.
3. **US-remote eligible, OR onsite/hybrid in the Seattle area** — either open to
   US-based remote applicants (no state exclusion blocking the candidate's
   location), or based in the Greater Seattle area — Seattle, Bellevue, Redmond,
   Kirkland, Renton, Tacoma, Everett, or listed generically as "Seattle, WA" /
   "Puget Sound." The candidate can commute to onsite/hybrid roles in this area,
   so remote eligibility is not required for them. A city restriction *outside*
   this area (e.g. "must be in Austin") still disqualifies a role.

Nice-to-have (boost a match but not required):

- Python in the stack
- Senior / Staff IC ladder (skip pure manager unless IC-track)
- Energy-sector employer → tag `[ENERGY]`

## Source list

### Energy-sector employers (check career pages directly)

- Octopus Energy / Kraken Technologies — `octopus.energy/careers`, `kraken.tech/careers`
- Tesla Energy — `tesla.com/careers`
- Sunrun, Sunnova, Enphase — solar/storage
- ChargePoint, EVgo — EV charging
- Constellation, NextEra, Duke Energy, Exelon — US utilities
- Schneider Electric, Siemens Energy — grid/industrial
- Uplight, AutoGrid (Schneider), GridX — grid-edge SaaS
- Arcadia, David Energy — energy-data platforms
- Crusoe Energy, Hut 8 — energy/compute crossover
- Palantir (energy / Foundry) — `palantir.com/careers`

### Cloud-native tech employers (senior Linux/SRE remote-friendly)

- Observability / data: HashiCorp, Datadog, Elastic, Grafana Labs, Chronosphere, Honeycomb
- Infra / edge: Cloudflare, Fastly, GitLab, GitHub
- Linux vendors: Red Hat, Canonical, SUSE
- Security: CrowdStrike, Wiz, Snyk, Sysdig, Tenable, Palo Alto Networks (Cortex)
- Product cos with strong SRE culture: Stripe, Shopify, Reddit, DuckDuckGo

### Seattle-area major employers (onsite/hybrid OK per commute-range filter, added 2026-09-10)

- Amazon (AWS), Microsoft, F5 Networks, T-Mobile, Nordstrom Tech — high role volume but
  JDs at this scale often don't name specific IaC tools (internal tooling common).
  F5's Workday tenant is `ffive.wd5.myworkdayjobs.com`, site `f5jobs` — first
  qualifying F5 role found 2026-09-28 ("Security Engineer", RP1038142: Terraform +
  Ansible + Python + security tooling, Seattle hybrid) after 2 prior runs of
  near-misses. Amazon and Microsoft's own career domains (`amazon.jobs`,
  `jobs.careers.microsoft.com`) were egress-blocked in the 2026-09-28 session
  specifically (a new finding vs. prior runs, which just found "no ATS") — retry
  next run. T-Mobile still 403s with no public ATS API found (3 runs running).

### Aggregators / boards

- **LinkedIn Jobs** — query template:
  `("Senior" OR "Staff") ("SRE" OR "DevOps" OR "Cloud Engineer" OR "Platform Engineer" OR "Site Reliability") "remote" "United States"`
  Filters: Remote · United States · Experience: Senior+ · Date: past week

## Search query cheatsheet

For WebSearch / Google:

- `site:boards.greenhouse.io "Senior" ("SRE" OR "DevOps") remote terraform`
- `site:jobs.lever.co staff site reliability engineer remote terraform ansible`
- `site:ashbyhq.com senior platform engineer remote linux observability`
- `site:greenhouse.io energy senior devops terraform remote`
- `"hiring" "remote" "senior" ("SRE" OR "DevOps") "terraform" 2026`

## Maintenance notes

- Re-review this file quarterly — employers shut down hiring or change ATS hosts.
- If a company appears 3+ runs in a row with no qualifying role, drop it.
- Add new finds under the right section; keep alphabetical inside each group.

### From 2026-09-28 run

- **New confirmed ATS slugs/tenants this run** (previously unlisted or wrong):
  Wiz's Greenhouse board token is `wizinc`, not `wiz` (`wiz` 404s); also Wiz's
  own `absolute_url` field on wiz.io is malformed (literal `:title`
  placeholder) — always use the `boards.greenhouse.io/wizinc/jobs/<id>` form.
  Tenable's Greenhouse token is `tenableinc`. SUSE is on Workday, tenant
  `suse.wd3.myworkdayjobs.com`, site `Jobsatsuse` (26 reqs, thin on
  SRE/DevOps). DuckDuckGo is on Ashby, org slug `duck-duck-go` (hyphenated,
  only 10 reqs total). Hut8's ATS is Greenhouse, token `hut8` (43 reqs) — a
  prior Lever guess was wrong. Crusoe Energy is on Ashby, org slug `Crusoe`
  (350 reqs) — but the entire board is confirmed onsite-only (SF/Denver/
  Dublin), no remote/Seattle reqs exist structurally, future runs can
  deprioritize re-checking Crusoe for remote roles. Sysdig is on Lever, slug
  `sysdig` (28 reqs). Duke Energy's Workday tenant is
  `dukeenergy.wd1.myworkdayjobs.com`, site `Search`. Sunrun's correct Workday
  tenant is `sunrun.wd5.myworkdayjobs.com`, site `Sunrun_Careers` (a prior
  `wd1` guess was wrong host). Siemens Energy runs its own "Careers
  Marketplace" portal at `jobs.siemens-energy.com` (not Workday) — has
  Terraform/Ansible/Kubernetes DevOps roles but only in Romania/India so far,
  no US req found yet. Datadog (`datadog`), Grafana Labs (`grafanalabs`,
  skews EU/UK for SRE), Cloudflare (`cloudflare`), Fastly (`fastly`), Stripe
  (`stripe`), Reddit (`reddit`), Honeycomb (`honeycomb`) Greenhouse tokens
  all reconfirmed working with zero qualifying yield this run.
- **Workiva's Workday site slug is `careers` (lowercase)** —
  `workiva.wd1.myworkdayjobs.com/careers` — correcting prior runs' failed
  guesses of `External`/`Careers`/`workiva`/`Workiva`. Could not be exercised
  this run (Workday had a platform-wide maintenance outage across all
  tenants at validation time) — worth a fresh full-board pull next run now
  that the slug is confirmed. Leads seen: R8280 "Staff Site Reliability
  Engineer", R9272-3 "Staff Software Engineer - Site Reliability", R10266
  "Senior Software Engineer - Site Reliability" (USA-Remote).
- **LinkedIn-sourced job IDs had an unusually high dead-link rate this run**:
  5 distinct "new employer" leads found via LinkedIn/web search — Bungie
  (`boards.greenhouse.io/bungie/jobs/3460177`), SmarterDx, Zscaler ("Staff
  SRE - Federal"), Garner Health, and Attain — all 404'd against the
  employer's own current Greenhouse board when validated, despite fresh-
  looking search snippets. In 3 of the 5 cases (Zscaler, Garner Health,
  Attain) a similarly-titled role existed at a *different* job ID on the
  same board, but with worse geography (hybrid-only, non-Seattle) or a
  different seniority tier — so they still wouldn't have qualified even as
  substitutes. Treat LinkedIn-sourced job IDs as leads only, never as
  apply-ready, and always re-derive the current ID from the employer's own
  board rather than trusting the linked ID.
- **Bungie, SmarterDx, Garner Health, Attain, Zscaler**: not added to the
  formal source list yet (only 1 appearance each, and that appearance was a
  dead link) — worth a second look next run by pulling each company's full
  live Greenhouse board directly (tokens: `bungie`, `smarterdx`,
  `garnerhealth`, `attain`, `zscaler`) rather than trusting search-indexed
  job IDs again.
- **Session-level egress blocks observed this run** (may vary session to
  session — retry next run before assuming permanent): `icims.com` (blocked
  entirely — explains repeated Exelon/Constellation/NextEra iCIMS-guess
  failures), `careers.se.com` (Schneider Electric — now confirmed hard
  blocked, not intermittent), `canonical.com`, `jobs.experian.com` (and its
  suspected backend `api.smartrecruiters.com` also blocked at the proxy
  layer), `qlik.com`, `epicgames.avature.net`, `github.careers`, `snyk.io`,
  `www.t-mobile.com`, `www.amazon.jobs` (new block — wasn't blocked before,
  was previously just "no ATS found"), `jobs.careers.microsoft.com` (also a
  new block). Working fine this session: `jobs.paloaltonetworks.com`,
  `shopify.com` (though Shopify still has no discoverable JSON API).
- **GridX, AutoGrid, Arcadia**: 3rd consecutive run with zero resolvable ATS
  via token-guessing or web search — per the "3 runs no qualifying source"
  convention, recommend dropping automated-search budget on these three and
  relying on manual/LinkedIn spot-checks only going forward.
- **Palantir** (Lever, slug `palantir`): checked 6 current DevOps/SRE/
  InfoSec reqs this run — all hybrid DC/NY/Seattle-onsite/Palo-Alto, none
  remote, and none name Terraform/Ansible explicitly in the JD body. Same
  pattern as the 2026-09-21 run. Consider deprioritizing unless a remote or
  Seattle-based req appears.
- **Shopify, GitHub, Snyk**: no public Greenhouse/Lever/Ashby board found via
  token-guessing (all 404). Worth trying SmartRecruiters/Workable APIs next
  run, or treat like Amazon/Microsoft/Nordstrom as "no queryable ATS."
- Reviewed 2026-09-21 → 2026-09-28.

### From 2026-09-21 run

- **GitLab full-board re-check surfaced 2 additional qualifying roles missed by keyword/search-based collection**: a "Staff Corporate Security Engineer", "Senior Professional Services Technical Architect - Security", and "Staff Forward Deployed Engineer" all passed the three must-haves but weren't found by the earlier collection agents' targeted searches. **Recommend future runs always pull GitLab's full live Greenhouse board (`boards-api.greenhouse.io/v1/boards/gitlab/jobs?content=true`) and grep for Terraform/Ansible + observability/security keywords across every open req**, not just search-indexed or obviously-titled postings — GitLab is now 3 runs in a row as the single highest-yield source (6 of 11 shortlisted roles this run).
- **CrowdStrike's Workday site slug is `crowdstrikecareers`** (not bare `crowdstrike`, which 404s) — `crowdstrike.wd5.myworkdayjobs.com/wday/cxs/crowdstrike/crowdstrikecareers/...`. Found a 2nd strong, distinct CrowdStrike role this run beyond the usual SRE TechOps req: "Sr. Linux Systems Engineer – Object Storage (Remote)" (R29937) — an unusually direct title match to the candidate's own specialization. Worth searching this tenant's full job list each run, not just the previously-known req IDs.
- **F5's correct Workday tenant/site found**: `ffive.wd5.myworkdayjobs.com`, site `f5jobs` (prior runs' 422s were from guessing wrong site names like `f5` or `careers`). Yielded 3 Seattle-based security roles this run, none of which cleared both must-have filters, but the tenant is now directly queryable for future runs.
- **Exelon is on iCIMS, not Workday**: `careers-exeloncorp.icims.com`. This explains 2+ runs of 422 Unprocessable Entity from Workday tenant-name guessing for Exelon specifically. Constellation Energy and NextEra Energy's correct ATS platforms remain unconfirmed — try iCIMS-pattern lookups for them too next run before continuing to guess Workday tenants.
- **Splunk's career site now redirects to Cisco** (`splunk.com/en_us/careers/jobs/*.html` → 301 → `careers.cisco.com/global/en/splunk`, reflecting the Cisco acquisition), and `careers.cisco.com` is blocked by this session's network egress policy. Splunk is effectively unreachable until the block lifts or a Cisco-hosted ATS API is identified — do not keep budgeting search time on `splunk.com` URLs directly.
- **T-Mobile continues to return HTTP 403 to WebFetch with no public ATS API found**, 2nd run in a row it can't be validated despite the domain itself not being hard network-blocked. Deprioritize further manual chasing of T-Mobile search snippets unless a direct ATS is discovered.
- **New promising leads, not yet formalized (need a 2nd qualifying appearance)**: **Workiva** (Terraform/GCP/AWS stack per LinkedIn snippet for a "Staff Site Reliability Engineer" — Workday tenant `workiva.wd1.myworkdayjobs.com` confirmed to exist but the site slug wasn't resolvable this run and `workiva.com` is egress-blocked, so the correct slug couldn't be looked up); **Epic Games** `[SEATTLE]` (Bellevue, WA — Terraform/Ansible/Python/Go/Bash per LinkedIn snippet for a Sr./Senior DevOps Engineer role; actual ATS is Avature but no current job ID pinned yet — do not confuse with Epic Systems/careers.epic.com, a different company); **Qlik** and **Experian** (both egress-blocked this session with no ATS API alternative, but both had strong stack snippets — Qlik: Terraform/Crossplane/Ansible/Prometheus/OTel/Splunk; Experian: 3+ yrs Terraform).
- Home Depot's `careers.homedepot.com` was reachable this run (unlike the 2026-09-14 hard block) — confirmed its SIEM/EDR "Cybersecurity Engineer II" role is genuinely live, but it fails the Linux+IaC filter on the merits: zero mentions of Terraform or Ansible anywhere in the full JD despite the strong SIEM/EDR/Cortex/XSIAM language.
- Reviewed 2026-09-14 → 2026-09-21.

### From 2026-09-09 run

- **RemoteOK, WeWorkRemotely, and Wellfound removed from the source list.** RemoteOK returned zero usable postings (tag-page searches only surfaced "hire a freelancer" pages); WeWorkRemotely and Wellfound both block automated fetch (403/410), so collection could only rely on unverifiable WebSearch snippets for them. All three produced hits that repeatedly failed Step 3.5 validation. Revisit only if their fetch-blocking or listing quality changes.
- A high proportion of Greenhouse/Workday/Ashby job IDs surfaced by web search this run were stale (404 or removed) even on established boards (GitLab, Grafana Labs, Honeycomb, Wiz, Close, The Farmer's Dog) — validate job IDs against the employer's live ATS listing, not just the search snippet.
- Candidate additions surfaced this run (not yet added, need a second qualifying appearance first per the 3-strikes-you're-in convention): **Southwest Power Pool** `[ENERGY]` (grid/utility, strong Terraform/Linux stack fit, but posting could not be independently validated — JS-blocked career portal) and **Leidos** (gov/energy-adjacent DevOps).

### From 2026-09-14 run

- **Session network egress policy blocked ~10 major-employer domains entirely this run** (Home Depot, T-Mobile, Nordstrom, Palo Alto Networks, Splunk, Shopify, Tesla, Sunrun, Schneider Electric, Jobvite) — confirmed via both WebFetch and raw curl (`connect_rejected`, gateway 403 on CONNECT), not a dead-link condition. This forced several strong-looking candidates (notably Home Depot's SIEM/EDR Cybersecurity Engineer II and T-Mobile's Terraform/Ansible-named Software Reliability Engineer) to be dropped as unvalidatable rather than shipped unverified. This is environment-dependent and may not recur on future runs from a different session — re-attempt these sources next run before assuming they need removal.
- **Red Hat added as a confirmed-working source**: its Workday tenant (`redhat.wd5.myworkdayjobs.com`, site `Jobs`) is directly queryable and yielded a strong match this run (Terraform+Ansible+Splunk+observability). Search-indexed Red Hat job IDs were stale; query the Workday tenant search API directly instead.
- **CrowdStrike's Workday per-job detail endpoint is now working** (200, full JD body) for the two IDs re-tested this run, reversing the 403/empty-SPA finding from 2026-09-09/09-10. Treat CrowdStrike as a normal Workday source going forward rather than flagging it for manual review.
- **GitLab remains the highest-yield single source** — 3 of 7 shortlisted roles this run came from GitLab's Greenhouse board (`gitlab`), each with Terraform and/or Ansible plus observability language explicitly named.
- **Paxos's Greenhouse board no longer resolves under any guessed token** (`paxos`, `joinpaxos`, `paxosinc`, `paxostrust` all 404) — possible ATS migration; the specific Staff SRE posting found via LinkedIn/search could not be validated. Re-check next run before dropping as a candidate source.
- **Chainlink Labs' Ashby board is not resolvable via the public posting API** under any guessed org slug, and its hosted job page renders no extractable content via WebFetch (client-side SPA). No viable automated validation path found — do not add to the formal source list yet.
- **Utility-sector Workday tenants (Constellation Energy, NextEra Energy, Exelon) remain unresolved** — tenant-name guessing returned 422 Unprocessable Entity rather than confirming/denying. Needs the correct tenant slug (typically findable from the employer's own careers page) before these can be queried directly.
- Reviewed 2026-09-10 → 2026-09-14.

### From 2026-09-10 run

- **Filter criteria updated**: onsite/hybrid Seattle-area roles now qualify without remote eligibility (candidate can commute) — see Locked filter criteria above. 0 Seattle-area roles passed validation this run despite genuine effort (Amazon ×2 live but no Terraform/Ansible named; Boeing/Qualtrics dead; Microsoft/T-Mobile no locatable live URL) — this looks like a real pattern (big employers at this scale rarely name specific IaC tools) worth a follow-up decision on whether to loosen the IaC-tool wording for Seattle-area roles specifically.
- **Southwest Power Pool and Leidos both struck out again on validation** (2nd appearance for SPP, Leidos not previously formalized) — SPP's UltiPro portal serves a browser-incompatibility page instead of content to automated fetch, and Leidos's `careers.leidos.com` 403s with no public ATS API. Recommend NOT adding either to the formal source list — they surface plausible-looking hits repeatedly but have no viable automated validation path, which defeats the point of the source list.
- **HashiCorp's two postings** flagged live-but-rate-limited (429) on 2026-09-09 are now confirmed dead (404) — a data point that a 429 shouldn't be read as "probably real, just blocked."
- **CrowdStrike remains only partially checkable, 2nd run in a row**: Workday's listings-index search reliably confirms a job is live + its title, but the per-job detail endpoint 403s and WebFetch gets an empty SPA render every time. Automated stack-keyword validation isn't possible here without a different approach (e.g. a logged-in browser session) — flag for manual review if pursuing CrowdStrike specifically, rather than continuing to spend automation budget on it.
- Reviewed 2026-05-12 → 2026-09-10.
