# Job Hunt Sources & Filter Criteria

Reusable seed list for the **Cloud / DevOps / SRE — US-Remote or Seattle-area**
market scan.
Last reviewed: 2026-09-10.

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
  JDs at this scale often don't name specific IaC tools (internal tooling common);
  1st appearance this run, no qualifying role yet — see 2026-09-10 maintenance notes.

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

### From 2026-09-09 run

- **RemoteOK, WeWorkRemotely, and Wellfound removed from the source list.** RemoteOK returned zero usable postings (tag-page searches only surfaced "hire a freelancer" pages); WeWorkRemotely and Wellfound both block automated fetch (403/410), so collection could only rely on unverifiable WebSearch snippets for them. All three produced hits that repeatedly failed Step 3.5 validation. Revisit only if their fetch-blocking or listing quality changes.
- A high proportion of Greenhouse/Workday/Ashby job IDs surfaced by web search this run were stale (404 or removed) even on established boards (GitLab, Grafana Labs, Honeycomb, Wiz, Close, The Farmer's Dog) — validate job IDs against the employer's live ATS listing, not just the search snippet.
- Candidate additions surfaced this run (not yet added, need a second qualifying appearance first per the 3-strikes-you're-in convention): **Southwest Power Pool** `[ENERGY]` (grid/utility, strong Terraform/Linux stack fit, but posting could not be independently validated — JS-blocked career portal) and **Leidos** (gov/energy-adjacent DevOps).

### From 2026-09-10 run

- **Filter criteria updated**: onsite/hybrid Seattle-area roles now qualify without remote eligibility (candidate can commute) — see Locked filter criteria above. 0 Seattle-area roles passed validation this run despite genuine effort (Amazon ×2 live but no Terraform/Ansible named; Boeing/Qualtrics dead; Microsoft/T-Mobile no locatable live URL) — this looks like a real pattern (big employers at this scale rarely name specific IaC tools) worth a follow-up decision on whether to loosen the IaC-tool wording for Seattle-area roles specifically.
- **Southwest Power Pool and Leidos both struck out again on validation** (2nd appearance for SPP, Leidos not previously formalized) — SPP's UltiPro portal serves a browser-incompatibility page instead of content to automated fetch, and Leidos's `careers.leidos.com` 403s with no public ATS API. Recommend NOT adding either to the formal source list — they surface plausible-looking hits repeatedly but have no viable automated validation path, which defeats the point of the source list.
- **HashiCorp's two postings** flagged live-but-rate-limited (429) on 2026-09-09 are now confirmed dead (404) — a data point that a 429 shouldn't be read as "probably real, just blocked."
- **CrowdStrike remains only partially checkable, 2nd run in a row**: Workday's listings-index search reliably confirms a job is live + its title, but the per-job detail endpoint 403s and WebFetch gets an empty SPA render every time. Automated stack-keyword validation isn't possible here without a different approach (e.g. a logged-in browser session) — flag for manual review if pursuing CrowdStrike specifically, rather than continuing to spend automation budget on it.
- Reviewed 2026-05-12 → 2026-09-10.
