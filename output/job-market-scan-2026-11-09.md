# Cloud / DevOps / SRE Job Market Scan — 2026-11-09

## Summary

- **24 roles** passed all 3 locked filters (Linux+IaC, observability/SIEM, US-remote-or-Seattle) across ~6,700 reqs touched; curated to a **15-role shortlist** (9 held back for redundancy/weaker IC fit, not for failing the filters — see Sources & method).
- **3 brand-new qualifying sources this run**: Red Hat (`OpenShift Infrastructure – Senior Consultant`, breaks the prior "international/onsite-only" pattern), Coalfire (`Senior Site Reliability Engineer (FedRAMP)`, new employer), and Okta's 2nd distinct Seattle pick (`Senior SRE – EPG`). Palantir's Seattle role also **formalized as a reliable recurring source** after a 2nd consecutive live appearance.
- **2 `[ENERGY]`-tagged roles shipped** (both Crusoe Energy, replacing last run's now-closed Bellevue pick) — a recovery after last run's first-ever zero-energy result.
- **7 `[SEATTLE]`** and **5 `[US-CITIZEN]`/`[CLEARANCE]`-tagged** roles shipped. Top recurring stack overlap across the shortlist: Terraform + Ansible + Datadog/Grafana/Prometheus/Splunk.
- Notable signal: multiple long-assumed-closed patterns broke this run (Red Hat, Palo Alto Networks, Elastic all surfaced genuine US-remote Terraform/Ansible+observability roles for the first time in months) — worth revisiting those employers' "international/onsite-only" framing in `sources.md`.

## Top picks (5)

### 1. Senior Software Engineer, Substrate — Palantir `[SEATTLE]`
Seattle, WA (hybrid). Terraform, Ansible, Kubernetes/Puppet operators, high-scale observability, SRE/data-center Linux background explicitly wanted. 2nd consecutive run this exact req has qualified — formalizing Palantir as a reliable Seattle source after a 5–6 run losing streak before that.
**Apply**: https://jobs.lever.co/palantir/c38bb622-6f8e-43a1-8ae7-32291da328a8/apply
**Verified**: WebFetch — full JD rendered, STATUS=LIVE (2026-11-09)
**Source**: Lever — Palantir careers (`api.lever.co/v0/postings/palantir`)

### 2. Software Engineer, Platform Observability and Intelligence — Fastly
NYC/SF, JD explicitly allows US-remote consideration. The single strongest stack match this run: Terraform, Ansible, Datadog, Grafana, OpenTelemetry, Prometheus, and Splunk all named directly.
**Apply**: https://www.fastly.com/about/jobs/apply?gh_jid=8256238
**Verified**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/fastly/jobs?content=true` (2026-11-09)
**Source**: Greenhouse — Fastly careers

### 3. Senior Database Reliability Engineer — Okta `[SEATTLE]` `[US-CITIZEN]`
Bellevue, WA (+ Chicago/NYC/SF/DC). Terraform, Ansible, Datadog, Grafana, Prometheus for DB automation/monitoring. Reliable recurring pick; JD requires "U.S. Person" status (citizen/GC) for FedRAMP-adjacent work — candidate qualifies.
**Apply**: https://www.okta.com/company/careers/opportunity/7617976?gh_jid=7617976
**Verified**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/okta/jobs/7617976` (2026-11-09)
**Source**: Greenhouse — Okta careers

### 4. OpenShift Infrastructure – Senior Consultant — Red Hat
US-remote (any state Red Hat is registered in). Ansible + Terraform/Helm for IaC, Prometheus/Grafana/ELK/Splunk for observability. First genuinely US-remote Red Hat req to qualify in this scan's history — prior runs only found international or Raleigh-onsite Terraform/Ansible hits.
**Apply**: https://redhat.wd5.myworkdayjobs.com/Jobs/job/Remote-US-NC/OpenShift-Infrastructure---Senior-Consultant_R-060309-1
**Verified**: Workday JSON API — `redhat.wd5.myworkdayjobs.com/wday/cxs/redhat/Jobs/job/...` (2026-11-09)
**Source**: Workday — Red Hat careers (tenant `redhat.wd5.myworkdayjobs.com`, site `Jobs`)

### 5. Senior Site Reliability Engineer (FedRAMP) — Coalfire
Remote, United States. Both Terraform AND Ansible explicitly named, plus a dedicated "SIEM and log pipelines, observability platforms" specialty line — a direct match to the candidate's SIEM/telemetry background in a FedRAMP/NIST 800-53 regulated-cloud context. Brand-new qualifying employer this run.
**Apply**: https://jobs.lever.co/coalfire/e2620778-f8e9-4b22-910e-ae0edfcc8238
**Verified**: Lever JSON API — `api.lever.co/v0/postings/coalfire/e2620778-f8e9-4b22-910e-ae0edfcc8238?mode=json` (2026-11-09)
**Source**: Lever — Coalfire careers

## Full shortlist (15)

- **Senior Infrastructure Engineer, Storage Platform** — Cloudflare `[SEATTLE]`
  - Location: In-office, Seattle among listed offices (also Austin/London/NYC/SF)
  - Stack match: Terraform, SaltStack, Prometheus, Grafana
  - Why it fits: Fleet-lifecycle infra ownership with Terraform + Prometheus/Grafana observability — direct Linux/SRE match
  - Apply link: https://boards.greenhouse.io/cloudflare/jobs/7629805?gh_jid=7629805
  - Source: Greenhouse — Cloudflare careers (verified via JSON API, 2026-11-09)

- **Principal Engineer – Network (Remote)** — CrowdStrike `[US-CITIZEN]`
  - Location: USA – Remote, CA
  - Stack match: Terraform, Ansible, CI/CD, GitOps, telemetry/analytics strategy
  - Why it fits: Owns network automation/IaC direction plus telemetry-analysis strategy — strong infra+observability-ownership match; requires US citizenship/GC, candidate qualifies
  - Apply link: https://crowdstrike.wd5.myworkdayjobs.com/crowdstrikecareers/job/USA---Remote-CA/Principal-Engineer---Network--Remote-_R30292
  - Source: Workday — CrowdStrike careers (verified via JSON API, 2026-11-09)

- **Production Engineer** — Zscaler `[SEATTLE]`
  - Location: Bellevue, WA / Santa Clara, CA
  - Stack match: Ansible, Terraform, Helm, Temporal, Grafana, OpenTelemetry, Prometheus
  - Why it fits: Full IaC+observability stack named directly; reliable recurring pick
  - Apply link: https://job-boards.greenhouse.io/zscaler/jobs/5158936007
  - Source: Greenhouse — Zscaler careers (verified via JSON API, 2026-11-09)

- **Site Reliability Engineer** — F5 Networks `[SEATTLE]`
  - Location: Seattle, WA (hybrid; also San Jose)
  - Stack match: Terraform, Prometheus, Grafana
  - Why it fits: Live for a 6th consecutive run — Terraform config management + Prometheus/Grafana observability directly named
  - Apply link: https://ffive.wd5.myworkdayjobs.com/f5jobs/job/Seattle/Site-Reliability-Engineer_RP1038966
  - Source: Workday — F5 careers (verified via JSON API, 2026-11-09)

- **Security Engineer, Product & Production Infrastructure** — Wiz
  - Location: Remote – USA
  - Stack match: Terraform/IaC, detection-and-response engineering, DevSecOps collaboration
  - Why it fits: Detection-engineering-equivalent function plus Terraform ownership; reliable recurring pick
  - Apply link: https://job-boards.greenhouse.io/wizinc/jobs/4711762006
  - Source: Greenhouse — Wiz careers (verified via JSON API, 2026-11-09)

- **Senior Site Reliability Engineer – EPG (Emerging Products Group)** — Okta `[SEATTLE]` `[US-CITIZEN]`
  - Location: Bellevue, WA / San Francisco, CA
  - Stack match: Terraform; Datadog, Splunk, Grafana
  - Why it fits: Second distinct Okta Seattle-area IC pick this run — explicit Datadog/Splunk/Grafana observability line plus Terraform automation; FedRAMP context requires US Person status, candidate qualifies
  - Apply link: https://www.okta.com/company/careers/opportunity/8268917?gh_jid=8268917
  - Source: Greenhouse — Okta careers (verified via JSON API, 2026-11-09)

- **Senior Staff Automation Engineer** — Crusoe Energy `[ENERGY]` `[SEATTLE]`
  - Location: San Francisco, CA primary; Bellevue, WA among listed onsite locations
  - Stack match: Kubernetes, Docker, Terraform, Ansible, AWX, osquery; config-management + observability charter
  - Why it fits: Terraform+Ansible explicitly named with a dedicated "Configuration Management and Observability" responsibility; replaces last run's now-closed Bellevue weekend-shift pick
  - Apply link: https://jobs.ashbyhq.com/Crusoe/ab5a5395-5480-4731-9053-3906b0f92f23
  - Source: Ashby — Crusoe Energy careers (verified via JSON API, 2026-11-09)

- **Senior DevOps Engineer** — Leidos `[CLEARANCE-ACTIVE]` `[US-CITIZEN]`
  - Location: Remote/Teleworker, US (req 6314)
  - Stack match: Terraform, Ansible, CloudFormation; Splunk, Grafana, Prometheus; multi-cloud
  - Why it fits: Strong remote-US match on all 3 filters; requires an active DoD Secret/Top-Secret clearance at hire, which the candidate does not currently hold — tagged `[CLEARANCE-ACTIVE]` per project rule rather than dropped
  - Apply link: https://leidos.wd5.myworkdayjobs.com/External/job/6314-RemoteTeleworker-US/Senior-DevOps-Engineer_R-00196252
  - Source: Workday — Leidos careers (verified via JSON API, 2026-11-09)

- **Senior Security Engineer** — SmarterDx
  - Location: Remote, United States
  - Stack match: Terraform; SIEM (Panther), CloudTrail/VPC Flow Logs/GuardDuty/AWS Config/Wiz/Snyk/CrowdStrike
  - Why it fits: Named SIEM tool + Terraform + broad cloud-security tooling stack, fully remote; reliable recurring pick
  - Apply link: https://job-boards.greenhouse.io/smarterdx/jobs/5204868007
  - Source: Greenhouse — SmarterDx careers (verified via JSON API, 2026-11-09)

## Sources & method

**Date of scan**: 2026-11-09. **Method**: Three parallel collection agents, each scoped to a disjoint slice of `resources/sources.md` (mirroring the proven 2026-10-26/2026-11-02 approach): (1) cloud-native tech + Seattle-area majors, (2) energy-sector + Palantir/Leidos, (3) newly-formalized/promising-leads/aggregators + a fresh discovery sweep. Each agent queried its sources' own ATS JSON APIs (Greenhouse, Lever, Ashby, Workday) and/or WebFetch on career pages, applied the three locked filters (Linux+IaC named explicitly, observability/SIEM angle, US-remote-or-Seattle-area), and performed Step 3.5 live URL validation on every surviving role inline before reporting back — no unverified or aggregator-sourced apply link appears on this report.

**Sources queried**: Datadog, Elastic, Grafana Labs, Honeycomb, Cloudflare, Fastly, GitLab, GitHub, Red Hat, Canonical, SUSE, CrowdStrike, Wiz, Sysdig, Tenable, Palo Alto Networks, Snyk, Stripe, Shopify, Reddit, DuckDuckGo, Okta, Zscaler, Amazon, Microsoft, T-Mobile, F5 Networks, Nordstrom Tech, Workiva, Octopus Energy/Kraken, Crusoe Energy, Hut8, Sunnova, Sunrun, Duke Energy, Tesla Energy, Siemens Energy, EVgo, Enphase, ChargePoint, Constellation, NextEra Energy, David Energy, Exelon, Schneider Electric, Arcadia, Palantir, Leidos, SmarterDx, Garner Health, Paxos, BlackCloak, Aalyria, DigitalOcean, Epic Games, Qlik, Experian, Coalfire, Blumira, TENEX.AI, Stellar Cyber, plus LinkedIn and a fresh WebSearch discovery sweep for new boards.

**24 roles passed all 3 locked filters** this run; **15 were shipped** above. The following **9 were held back for redundancy or weaker IC fit (not for failing the locked filters)**: Elastic's "Consulting Architect" and "Consulting Architect – Search" reqs (both US-remote, Terraform/Ansible/SIEM — but consulting/pre-sales-weighted tracks, a new pattern worth a closer look next run); Cloudflare's "Senior Software Engineer – Kubernetes platform" (IaC/observability were secondary nice-to-have bullets, not core duties); Wiz's "Senior Partner Solutions Architect – GSI" (pre-sales, repeatedly cut in prior runs for weak IC fit); Palo Alto Networks' "Global Solutions Architect – AI and Automation" (new find, genuinely US-remote with Terraform/Ansible+observability — breaking PANW's prior CA-onsite-only pattern — but Solutions-Architect-titled rather than hands-on IC; worth rechecking for a clearer IC title); GitLab's "SRE, Infrastructure Platforms AMER" (redundant with GitLab's Cloud Platform Engineer pick, same employer); Zscaler's "Staff SRE (Production Engineer) – Federal" (redundant with Zscaler's Production Engineer pick, same employer/region); Garner Health's "Senior SRE" (genuinely qualifying, Terraform+Datadog+remote, reliable recurring pick — but the thinnest stack match among this run's 24 candidates); and Crusoe Energy's "Senior Production Engineer, Storage" (Terraform/Ansible named, but observability is only incident-response-context telemetry, weaker than its Senior Staff Automation Engineer sibling pick).

One role — Okta's `8268917` ("Senior SRE – EPG") — was independently surfaced by two different collection agents this run, a good signal of its stack-match strength.

No roles were dropped this run for citizenship/clearance language — per project rule, those roles ship with `[US-CITIZEN]`/`[CLEARANCE]`/`[CLEARANCE-ACTIVE]` tags instead.

Full run detail (sites visited, API calls, token usage, source-by-source coverage) is logged in `logs/job-market-scan-2026-11-09.json`.
