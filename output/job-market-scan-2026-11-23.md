# Cloud / DevOps / SRE Job Market Scan — 2026-11-23

## Summary

- **24 roles** passed all 3 locked filters (Linux+IaC, observability/SIEM, US-remote-or-Seattle) across ~6,400 reqs touched; curated to a **15-role shortlist** (9 held back for redundancy/weaker fit/quality — see Sources & method).
- **1 brand-new qualifying source**: **Corelight** (network detection/security company, Greenhouse) — strong Terraform + Prometheus/Grafana + FedRAMP-context match, found via a fresh discovery sweep. Also, **DigitalOcean's long-mysterious ATS is finally resolved** (Greenhouse token `digitalocean98` — ends a 5+ run "unresolvable" streak), though it yielded 0 qualifying roles this run.
- **Leidos staged a strong recovery** after shipping zero last run: a fresh full remote-facet sweep surfaced **3 distinct new qualifying remote-US roles**, 2 of which ship here (`R-00197276`, `R-00197465`) — all three require an *active* DoD Secret clearance plus US citizenship at hire, tagged `[CLEARANCE-ACTIVE][US-CITIZEN]` per project rule (never dropped for this).
- **Fastly's long-standing top pick (`8256238`) is now confirmed DEAD** (404, absent from the live board) — no replacement of similar stack quality was found this run, a real loss.
- **6 `[SEATTLE]`-tagged**, **1 `[ENERGY]`-tagged**, **6 `[US-CITIZEN]`-tagged**, and **2 `[CLEARANCE-ACTIVE]`-tagged** roles shipped. Top recurring stack overlap: Terraform + Ansible + Datadog/Splunk/Grafana/Prometheus/SIEM. Okta and Palantir remain the most reliable recurring sources (Palantir's Substrate req is now live for a 5th consecutive run).

## Top picks (5)

### 1. Sr Software Engineer, Cloud Infrastructure/SRE — Corelight (brand-new qualifying source) `[US-CITIZEN]`
North America (role requires physical presence in the US). Terraform, Kubernetes, Prometheus, Grafana all named directly for a FedRAMP-context federal cloud security platform — a clean, strong match to the candidate's telemetry/observability and security-platform background. JD requires US citizenship (no active-clearance requirement found).
**Apply**: https://job-boards.greenhouse.io/corelight/jobs/8369707
**Verified**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/corelight/jobs/8369707` + WebFetch confirmation (2026-11-23)
**Source**: Greenhouse — Corelight careers (new source, found via fresh discovery sweep)

### 2. Orchestration Application Performance Engineer - Mid — Leidos `[CLEARANCE-ACTIVE]` `[US-CITIZEN]`
Remote/Teleworker, US. The strongest of 3 new Leidos finds this run: Terraform, Ansible, SIEM, telemetry, Splunk, and Elastic all explicitly named. Requires an active DoD Secret clearance and US citizenship at hire — candidate is a US citizen but holds no active clearance today, flagged accordingly per project rule (still shipped, never dropped for this).
**Apply**: https://leidos.wd5.myworkdayjobs.com/External/job/6314-RemoteTeleworker-US/Orchestration-Application-Performance-Engineer---Mid_R-00197276
**Verified**: Workday JSON API — job-detail endpoint, HTTP 200 (2026-11-23); WebFetch inconclusive (empty SPA render), API used per protocol
**Source**: Workday — Leidos careers

### 3. Senior Software Engineer, Substrate — Palantir `[SEATTLE]`
Seattle, WA (hybrid). Terraform, Ansible, Puppet, Kubernetes, and high-scale observability all named. Live for a 5th consecutive run — the most reliably recurring Seattle source alongside Okta.
**Apply**: https://jobs.lever.co/palantir/c38bb622-6f8e-43a1-8ae7-32291da328a8
**Verified**: WebFetch — full JD returned, STATUS=LIVE (2026-11-23); cross-checked against Lever JSON API `api.lever.co/v0/postings/palantir?mode=json`
**Source**: Lever — Palantir careers

### 4. Senior Database Reliability Engineer (DBRE) — Okta `[SEATTLE]` `[US-CITIZEN]`
Bellevue, WA (+ Chicago/NYC/SF/DC). Terraform, Ansible, Kubernetes Operators, Prometheus/Grafana/Datadog for DB automation and monitoring. Okta's most reliable recurring pick, live for 7+ consecutive runs; JD requires "U.S. Person" status — candidate qualifies.
**Apply**: https://job-boards.greenhouse.io/okta/jobs/7617976
**Verified**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/okta/jobs/7617976?content=true` (2026-11-23)
**Source**: Greenhouse — Okta careers (`okta.com` itself is egress-blocked; this Greenhouse-hosted URL is the canonical apply link)

### 5. Senior Staff Automation Engineer — Crusoe Energy `[ENERGY]` `[SEATTLE]`
San Francisco, CA (primary); Bellevue, WA + Sunnyvale, CA (secondary onsite locations). Terraform, Ansible, AWX, osquery, with a dedicated "Configuration Management and Observability" charter — a direct match to the candidate's IaC + observability-ownership background. Live for another consecutive run.
**Apply**: https://jobs.ashbyhq.com/Crusoe/ab5a5395-5480-4731-9053-3906b0f92f23
**Verified**: Ashby JSON API — `api.ashbyhq.com/posting-api/job-board/Crusoe`, `descriptionPlain` field (2026-11-23)
**Source**: Ashby — Crusoe Energy careers

## Full shortlist (15)

- **Senior Site Reliability Engineer - EPG** — Okta `[SEATTLE]` `[US-CITIZEN]`
  - Location: Bellevue, WA / San Francisco, CA
  - Stack match: Terraform; Datadog, Splunk, Grafana; FedRAMP
  - Why it fits: Okta's 2nd distinct Seattle-area IC pick, reconfirmed live again this run
  - Apply link: https://job-boards.greenhouse.io/okta/jobs/8268917
  - Source: Greenhouse — Okta careers (verified via JSON API, 2026-11-23)

- **Principal Engineer – Network (Remote)** — CrowdStrike `[US-CITIZEN]`
  - Location: USA – Remote, CA
  - Stack match: Terraform, Ansible, CI/CD, GitOps, telemetry/analytics strategy
  - Why it fits: Owns network automation/IaC direction plus telemetry-analysis strategy; requires US citizenship/GC, candidate qualifies. Per-job detail endpoint returned a clean 200 this run (no 403 flake, as seen in some prior runs).
  - Apply link: https://crowdstrike.wd5.myworkdayjobs.com/crowdstrikecareers/job/USA---Remote-CA/Principal-Engineer---Network--Remote-_R30292
  - Source: Workday — CrowdStrike careers (verified via JSON API, 2026-11-23)

- **Site Reliability Engineer** — F5 Networks `[SEATTLE]`
  - Location: Seattle, WA (hybrid)
  - Stack match: Terraform, Prometheus, Grafana
  - Why it fits: Live for an 8th+ consecutive run — Terraform config management + Prometheus/Grafana observability directly named
  - Apply link: https://ffive.wd5.myworkdayjobs.com/f5jobs/job/Seattle/Site-Reliability-Engineer_RP1038966
  - Source: Workday — F5 careers (verified via JSON API, 2026-11-23)

- **Senior Infrastructure Engineer, Storage Platform** — Cloudflare `[SEATTLE]`
  - Location: In-office, Seattle among listed offices (also Austin/London/NYC/SF)
  - Stack match: Terraform, SaltStack, Prometheus, Grafana
  - Why it fits: Fleet-lifecycle infra ownership with Terraform + Prometheus/Grafana observability — direct Linux/SRE match
  - Apply link: https://boards.greenhouse.io/cloudflare/jobs/7629805?gh_jid=7629805
  - Source: Greenhouse — Cloudflare careers (verified via JSON API, 2026-11-23)

- **Cloud Platform Engineer** — GitLab
  - Location: Remote, US/Canada
  - Stack match: Terraform, platform observability
  - Why it fits: Reliable recurring pick; direct IaC + observability ownership
  - Apply link: https://job-boards.greenhouse.io/gitlab/jobs/8889193002
  - Source: Greenhouse — GitLab careers (verified via JSON API, 2026-11-23)

- **Security Engineer, Product & Production Infrastructure** — Wiz
  - Location: Remote – USA
  - Stack match: Terraform/IaC, detection-and-response-equivalent security tooling
  - Why it fits: Detection-engineering-equivalent function plus Terraform ownership; reliable recurring pick
  - Apply link: https://job-boards.greenhouse.io/wizinc/jobs/4711762006
  - Source: Greenhouse — Wiz careers (verified via JSON API, 2026-11-23)

- **Senior Site Reliability Engineer (FedRAMP)** — Coalfire
  - Location: Remote, United States
  - Stack match: Terraform AND Ansible (now in a "Bonus Points" section after a JD reword — still explicitly named); SIEM/log-pipeline language
  - Why it fits: Direct match to the candidate's FedRAMP/NIST 800-53 + SIEM background. Reconfirmed live for another consecutive run.
  - Apply link: https://jobs.lever.co/coalfire/e2620778-f8e9-4b22-910e-ae0edfcc8238
  - Source: Lever — Coalfire careers (verified via JSON API, 2026-11-23)

- **Staff Site Reliability Engineer** — TENEX.AI
  - Location: Remote, USA
  - Stack match: Terraform, SIEM, Datadog
  - Why it fits: TENEX.AI is an AI-native MDR provider — this SRE role builds the observability/detection platform itself, a strong domain match
  - Apply link: https://jobs.ashbyhq.com/tenex/fc7c5446-8d7d-4f8e-97fa-14a7e4ac3ad6
  - Source: Ashby — TENEX.AI careers (verified via JSON API, 2026-11-23)

- **Senior DevOps Engineer** — DigiCert
  - Location: United States - Remote
  - Stack match: Terraform AND Ansible both named, plus Splunk
  - Why it fits: Strongest IaC-tool match of this run's recurring picks — infra-automation/reliability-and-scale charter, genuinely remote
  - Apply link: https://job-boards.greenhouse.io/digicert/jobs/8885889002
  - Source: Greenhouse — DigiCert careers (verified via JSON API, 2026-11-23; `digicert.com` itself is egress-blocked, use this Greenhouse-hosted URL)

- **Cryptography & Security Infrastructure Engineer – Mid-Level** — Leidos `[CLEARANCE-ACTIVE]` `[US-CITIZEN]`
  - Location: Remote/Teleworker, US
  - Stack match: Terraform, Ansible, SIEM
  - Why it fits: Second of 3 new Leidos finds this run — direct SIEM term plus both IaC tools named. Requires active DoD Secret clearance + US citizenship at hire.
  - Apply link: https://leidos.wd5.myworkdayjobs.com/External/job/6314-RemoteTeleworker-US/Cryptography---Security-Infrastructure-Engineer---Mid-Level_R-00197465
  - Source: Workday — Leidos careers (verified via JSON API, 2026-11-23)

## Sources & method

**Date of scan**: 2026-11-23. **Method**: Three parallel collection agents, each scoped to a disjoint slice of `resources/sources.md`: (1) cloud-native tech + Seattle-area majors, (2) energy-sector + Palantir/Leidos, (3) newly-formalized/promising-leads/aggregators + a fresh discovery sweep for brand-new sources. Each agent queried its sources' own ATS JSON APIs (Greenhouse, Lever, Ashby, Workday) and/or WebFetch on career pages, applied the three locked filters, and performed Step 3.5 live URL validation on every surviving role inline before reporting back. No unverified or aggregator-sourced apply link appears on this report.

**Sources queried**: Datadog, Elastic, Grafana Labs, Honeycomb, Cloudflare, Fastly, GitLab, GitHub, Red Hat, Canonical, SUSE, CrowdStrike, Wiz, Sysdig, Tenable, Palo Alto Networks, Snyk, Stripe, Shopify, Reddit, DuckDuckGo, Okta, Zscaler, Amazon, Microsoft, T-Mobile, F5 Networks, Nordstrom Tech, Workiva, Octopus Energy/Kraken (quick existence check only, per monthly-cadence decision), Crusoe Energy, Hut8 (quick existence check only), Sunnova, Sunrun, Duke Energy, Tesla Energy, Siemens Energy, EVgo, Enphase, ChargePoint, Constellation Energy, NextEra Energy, David Energy, Exelon, Schneider Electric, Arcadia, Palantir, Leidos, SmarterDx, Garner Health, Paxos, Aalyria/Rippling, DigitalOcean, Epic Games, Qlik, Experian, Coalfire, TENEX.AI, Stellar Cyber, Netlify, Stacklok, Bugcrowd, ScienceLogic, Pondurance, Chainguard, Corelight, remote.com, Blackpoint Cyber, plus LinkedIn and a fresh discovery sweep. (BlackCloak was skipped entirely — dropped from rotation 2026-11-16.)

**24 roles passed all 3 locked filters** this run; **15 were shipped** above. The following **9 were held back for redundancy, weaker fit, or quality curation (not for failing the locked filters)**:
- GitLab "SRE, Infrastructure Platforms — AMER" (`8623389002`) — redundant with the shipped GitLab pick (same company, similar role)
- Okta "Staff Site Reliability Engineer" (`8385706`) — redundant with the shipped Okta EPG pick (same Bellevue FedRAMP team)
- Cloudflare "Senior Software Engineer – Kubernetes platform" (`8263016`) — redundant with the shipped Cloudflare pick; Ansible is only a "such as" nice-to-have, a weaker IaC commitment than most shipped roles
- Crusoe Energy "Senior Software Engineer, Platform Networking" (`d0a11984-9ed0-42e1-99af-e63113b3681c`) — Terraform/Ansible only a nice-to-have, and the named telemetry is network telemetry (gNMI/gRPC/NETCONF), not security/observability telemetry — weaker fit than its shipped sibling
- Leidos "Senior Network Support Engineer Remote" (`R-00196293`) — weakest of the 3 new Leidos finds (Elastic+Grafana only, no SIEM term), held back given 2 stronger Leidos picks already shipped
- Red Hat "Site Reliability Engineer" (`R-060248`) — a genuine new nationwide-US-remote find (Red Hat's first non-dead lead in 2 runs), but no Terraform named (Ansible only), entry/mid-level (2 yrs experience, below the candidate's senior profile), and observability named only generically
- SmarterDx "Senior Security Engineer, Security Automation" (`5204868007`) — a reliable long-standing recurring pick, held back this run purely for shortlist-size curation given an unusually strong week (2 new sources + a Leidos recovery); worth re-shipping next run
- Garner Health "Senior Staff Site Reliability Engineer" (`6261236004`) — a new replacement pick (the prior recurring SRE pick is gone from the board), but the Greenhouse `title` field says "SRE" while the JD body opens "Senior Staff Platform Engineer" — a JD inconsistency worth confirming before shipping
- Nordstrom Technology "Senior Identity Security Engineer" (`R-898894`, Seattle) — Terraform is explicitly named, but the observability/SIEM angle is thin (ITDR/ITSM tooling and KQL only, no named SIEM/SOAR/Datadog/Splunk/Elastic/Grafana term) — borderline on filter 2, held back pending a clearer match rather than shipped on a close call

**Notable source changes this run**: Fastly's long-standing top pick `8256238` is confirmed **dead** (404), with no replacement of similar quality found among its 6 remaining Terraform/observability-matching reqs (all city-specific-onsite or international). DigitalOcean's ATS is **finally resolved** — Greenhouse token `digitalocean98` (not a guessable plain "digitalocean" token, explaining 5+ runs of failure) — 0 qualifying roles found among its 132 open reqs this run, but it should be queried directly going forward. Leidos recovered from zero to 3 new qualifying remote-US roles via a fresh full remote-facet sweep. Crusoe's previously-tracked "Senior Production Engineer, Storage" (`fb0c1911...`) is confirmed gone from the board entirely. Hut8 is confirmed to have zero technical roles for a 3rd consecutive check and has been formally dropped from the rotation (see `resources/sources.md`).

No roles were dropped this run for citizenship/clearance language — per project rule, those roles ship with `[US-CITIZEN]`/`[CLEARANCE]`/`[CLEARANCE-ACTIVE]` tags instead.

Full run detail (sites visited, API calls, token usage, source-by-source coverage) is logged in `logs/job-market-scan-2026-11-23.json`.
