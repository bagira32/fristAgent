# Job Hunt Sources & Filter Criteria

Reusable seed list for the **Cloud / DevOps / SRE — US-Remote** market scan.
Last reviewed: 2026-05-12.

## Candidate profile (anchors the filter)

Linux Systems Engineer · multi-cloud hardening · Terraform / Ansible · Python ·
SIEM / log pipelines · global-scale observability · DevSecOps.

## Locked filter criteria

A role must hit **ALL three** must-haves to make a shortlist:

1. **Linux + IaC** — Terraform and/or Ansible explicitly named in the JD.
2. **Observability / SIEM / security angle** — SIEM, SOAR, detection engineering,
   log/telemetry pipelines, or strong observability ownership.
3. **US-remote eligible** — open to US-based remote applicants, no state exclusion
   blocking the candidate's location.

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
