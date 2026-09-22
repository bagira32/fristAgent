# Job Hunt Sources & Filter Criteria

Reusable seed list for the **Cloud / DevOps / SRE — US-Remote or Seattle-area**
market scan.
Last reviewed: 2026-09-21.

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
  no qualifying role yet after 4 runs — see maintenance notes below. F5's Workday
  tenant is now known (`ffive.wd5.myworkdayjobs.com`, site `f5jobs`) — 3 Seattle
  security roles found 2026-09-21 but none cleared both must-have filters.

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
