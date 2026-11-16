# Cloud / DevOps / SRE Job Market Scan — 2026-11-16

## Summary

- **23 roles** passed all 3 locked filters (Linux+IaC, observability/SIEM, US-remote-or-Seattle) across ~5,500 reqs touched; curated to a **14-role shortlist** (9 held back for redundancy/weaker fit/manager-tier, not for failing the filters — see Sources & method).
- **2 brand-new qualifying sources this run**: **TENEX.AI** (AI-native MDR provider, Ashby org slug `tenex`) and **DigiCert** (Greenhouse, strongest IaC-tool match of the run — Terraform AND Ansible both named plus Splunk).
- **Three previously-reliable recurring picks died with no replacement found**: Red Hat's formalized US-remote pick (`R-060309-1`), Leidos's only remote-US pick (`R-00196252`), and both of Zscaler's tracked picks (`5158936007` closed, `5029669007` lost its Bellevue/remote eligibility). Red Hat, Leidos, and Zscaler all ship **zero** roles this run — a rougher week for several long-tracked sources.
- **1 `[ENERGY]`-tagged role** (Crusoe Energy), **6 `[SEATTLE]`-tagged**, and **3 `[US-CITIZEN]`-tagged** roles shipped. Top recurring stack overlap: Terraform + Ansible + Datadog/Grafana/Prometheus/Splunk.
- Notable signal: Okta and Palantir remain the most reliable recurring sources (Okta shipped 2 distinct Seattle picks again; Palantir's Substrate req is now live for a 4th consecutive run). BlackCloak is recommended for full removal from the source rotation after an 8th consecutive non-qualifying run.

## Top picks (5)

### 1. Software Engineer, Platform Observability and Intelligence — Fastly
NYC/SF, JD explicitly allows US-remote consideration. The single strongest stack match this run: Terraform, Ansible, Datadog, Grafana, OpenTelemetry, Prometheus, and Splunk all named directly — a near 1:1 map to the candidate's telemetry-pipeline/observability background.
**Apply**: https://www.fastly.com/about/jobs/apply?gh_jid=8256238
**Verified**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/fastly/jobs/8256238` (2026-11-16)
**Source**: Greenhouse — Fastly careers

### 2. Senior Site Reliability Engineer (FedRAMP) — Coalfire
Remote, United States. Both Terraform AND Ansible explicitly named, plus a dedicated SIEM/log-pipeline/observability specialty line — a direct match to the candidate's FedRAMP/NIST 800-53 + SIEM background. Reconfirmed live for another consecutive run.
**Apply**: https://jobs.lever.co/coalfire/e2620778-f8e9-4b22-910e-ae0edfcc8238
**Verified**: Lever JSON API — `api.lever.co/v0/postings/coalfire` (2026-11-16)
**Source**: Lever — Coalfire careers

### 3. Senior Database Reliability Engineer (DBRE) — Okta `[SEATTLE]` `[US-CITIZEN]`
Bellevue, WA (+ Chicago/NYC/SF/DC). Terraform, Ansible, Datadog, Grafana, Prometheus for DB automation/monitoring. Reliable recurring pick, live for 6+ consecutive runs; JD requires "U.S. Person" status (citizen/GC) — candidate qualifies.
**Apply**: https://www.okta.com/company/careers/opportunity/7617976?gh_jid=7617976
**Verified**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/okta/jobs/7617976` (2026-11-16)
**Source**: Greenhouse — Okta careers

### 4. Senior Software Engineer, Substrate — Palantir `[SEATTLE]`
Seattle, WA (hybrid). Terraform, Ansible, Kubernetes, high-scale observability, SRE/Linux experience explicitly wanted. Live for a 4th consecutive run — fully formalized as a reliable recurring Seattle source.
**Apply**: https://jobs.lever.co/palantir/c38bb622-6f8e-43a1-8ae7-32291da328a8
**Verified**: Lever JSON API — `api.lever.co/v0/postings/palantir?mode=json` (2026-11-16)
**Source**: Lever — Palantir careers

### 5. Staff Site Reliability Engineer — TENEX.AI (brand-new qualifying source)
Remote, USA. Terraform, SIEM, and Datadog observability named directly. TENEX.AI is an AI-native MDR (managed detection and response) provider — this SRE role builds/automates the observability and detection platform itself, an unusually direct match to the candidate's SIEM/telemetry-pipeline specialization. Previously flagged "unresolvable ATS" in prior runs — resolved this run under Ashby org slug `tenex`.
**Apply**: https://jobs.ashbyhq.com/tenex/fc7c5446-8d7d-4f8e-97fa-14a7e4ac3ad6
**Verified**: Ashby JSON API — `api.ashbyhq.com/posting-api/job-board/tenex` (2026-11-16)
**Source**: Ashby — TENEX.AI careers

## Full shortlist (14)

- **Senior Site Reliability Engineer - EPG** — Okta `[SEATTLE]` `[US-CITIZEN]`
  - Location: Bellevue, WA / San Francisco, CA
  - Stack match: Terraform; Datadog, Splunk, Grafana
  - Why it fits: Okta's 2nd distinct Seattle-area IC pick, reconfirmed live again this run
  - Apply link: https://www.okta.com/company/careers/opportunity/8268917?gh_jid=8268917
  - Source: Greenhouse — Okta careers (verified via JSON API, 2026-11-16)

- **Principal Engineer – Network (Remote)** — CrowdStrike `[US-CITIZEN]`
  - Location: USA – Remote, CA
  - Stack match: Terraform, Ansible, CI/CD, GitOps, telemetry/analytics strategy
  - Why it fits: Owns network automation/IaC direction plus telemetry-analysis strategy; requires US citizenship/GC, candidate qualifies
  - Apply link: https://crowdstrike.wd5.myworkdayjobs.com/crowdstrikecareers/job/USA---Remote-CA/Principal-Engineer---Network--Remote-_R30292
  - Source: Workday — CrowdStrike careers (verified via JSON API, 2026-11-16)

- **Site Reliability Engineer** — F5 Networks `[SEATTLE]`
  - Location: Seattle, WA (hybrid)
  - Stack match: Terraform, Prometheus, Grafana
  - Why it fits: Live for a 7th+ consecutive run — Terraform config management + Prometheus/Grafana observability directly named
  - Apply link: https://ffive.wd5.myworkdayjobs.com/f5jobs/job/Seattle/Site-Reliability-Engineer_RP1038966
  - Source: Workday — F5 careers (verified via JSON API, 2026-11-16)

- **Senior Infrastructure Engineer, Storage Platform** — Cloudflare `[SEATTLE]`
  - Location: In-office, Seattle among listed offices (also Austin/London/NYC/SF)
  - Stack match: Terraform, SaltStack, Prometheus, Grafana
  - Why it fits: Fleet-lifecycle infra ownership with Terraform + Prometheus/Grafana observability — direct Linux/SRE match
  - Apply link: https://boards.greenhouse.io/cloudflare/jobs/7629805?gh_jid=7629805
  - Source: Greenhouse — Cloudflare careers (verified via JSON API, 2026-11-16)

- **Cloud Platform Engineer** — GitLab
  - Location: Remote, US/Canada
  - Stack match: Terraform, Kubernetes, observability
  - Why it fits: Reliable recurring pick; direct IaC + observability ownership
  - Apply link: https://job-boards.greenhouse.io/gitlab/jobs/8889193002
  - Source: Greenhouse — GitLab careers (verified via JSON API, 2026-11-16)

- **Security Engineer, Product & Production Infrastructure** — Wiz
  - Location: Remote – USA
  - Stack match: Terraform/IaC, detection-and-response engineering, DevSecOps collaboration
  - Why it fits: Detection-engineering-equivalent function plus Terraform ownership; reliable recurring pick
  - Apply link: https://job-boards.greenhouse.io/wizinc/jobs/4711762006
  - Source: Greenhouse — Wiz careers (verified via JSON API, 2026-11-16)

- **Senior Staff Automation Engineer** — Crusoe Energy `[ENERGY]` `[SEATTLE]`
  - Location: San Francisco, CA primary; Bellevue, WA + Sunnyvale, CA secondary onsite locations
  - Stack match: Terraform, Ansible, AWX, osquery, Kubernetes/Docker; dedicated config-management/observability charter
  - Why it fits: Terraform+Ansible explicitly named with a dedicated "Configuration Management and Observability" responsibility; live for a 2nd consecutive run
  - Apply link: https://jobs.ashbyhq.com/Crusoe/ab5a5395-5480-4731-9053-3906b0f92f23
  - Source: Ashby — Crusoe Energy careers (verified via JSON API, 2026-11-16)

- **Senior Security Engineer** — SmarterDx
  - Location: Remote, United States
  - Stack match: Terraform; SIEM (Panther), CloudTrail/VPC Flow Logs/GuardDuty/AWS Config/Wiz/Snyk/CrowdStrike
  - Why it fits: Named SIEM tool + Terraform + broad cloud-security tooling stack, fully remote; reliable recurring pick
  - Apply link: https://job-boards.greenhouse.io/smarterdx/jobs/5204868007
  - Source: Greenhouse — SmarterDx careers (verified via JSON API, 2026-11-16)

- **Senior DevOps Engineer** — DigiCert (brand-new qualifying source)
  - Location: United States - Remote
  - Stack match: Terraform AND Ansible both named, plus Splunk and observability language
  - Why it fits: Strongest IaC-tool match of this run's new finds — infra-automation/reliability-and-scale charter, genuinely remote
  - Apply link: https://job-boards.greenhouse.io/digicert/jobs/8885889002
  - Source: Greenhouse — DigiCert careers (verified via JSON API, 2026-11-16; `digicert.com` itself is egress-blocked, use this Greenhouse-hosted URL)

## Sources & method

**Date of scan**: 2026-11-16. **Method**: Three parallel collection agents, each scoped to a disjoint slice of `resources/sources.md`: (1) cloud-native tech + Seattle-area majors, (2) energy-sector + Palantir/Leidos, (3) newly-formalized/promising-leads/aggregators + a fresh discovery sweep for brand-new sources. Each agent queried its sources' own ATS JSON APIs (Greenhouse, Lever, Ashby, Workday) and/or WebFetch on career pages, applied the three locked filters (Linux+IaC named explicitly, observability/SIEM angle, US-remote-or-Seattle-area), and performed Step 3.5 live URL validation on every surviving role inline before reporting back. All 5 top picks were re-verified live a second time (Step 6 spot-check) immediately before this report was written. No unverified or aggregator-sourced apply link appears on this report.

**Sources queried**: Datadog, Elastic, Grafana Labs, Honeycomb, Cloudflare, Fastly, GitLab, GitHub, Red Hat, Canonical, SUSE, CrowdStrike, Wiz, Sysdig, Tenable, Palo Alto Networks, Snyk, Stripe, Shopify, Reddit, DuckDuckGo, Okta, Zscaler, Amazon, Microsoft, T-Mobile, F5 Networks, Nordstrom Tech, Workiva, Octopus Energy/Kraken, Crusoe Energy, Hut8 (quick existence check only), Sunnova, Sunrun, Duke Energy, Tesla Energy, Siemens Energy, EVgo, Enphase, ChargePoint, Constellation Energy, NextEra Energy, David Energy, Exelon, Schneider Electric, Arcadia, Palantir, Leidos, SmarterDx, Garner Health, Paxos, BlackCloak, Aalyria/Rippling, DigitalOcean, Epic Games, Qlik, Experian, Coalfire, Blumira, TENEX.AI, Stellar Cyber, plus LinkedIn and a fresh discovery sweep (ScienceLogic, Pondurance, DigiCert).

**23 roles passed all 3 locked filters** this run; **14 were shipped** above. The following **9 were held back for redundancy, weaker fit, or wrong track (not for failing the locked filters)**: Palo Alto Networks "Global Solutions Architect – AI and Automation" `JR-023885-1` (Solutions-Architect-titled, not hands-on IC); Wiz "Senior Partner Solutions Architect – GSI" `4703947006` (pre-sales); GitLab "SRE, Infrastructure Platforms — AMER" `8623389002` (redundant with the shipped GitLab pick); Elastic "Consulting Architect" `8325389` and "Consulting Architect – Search" `8352728` (consulting/pre-sales track); Cloudflare "Senior Software Engineer – Kubernetes platform" `8263016` (IaC only a secondary bullet); Crusoe Energy "Senior Production Engineer, Storage" `fb0c1911-c752-49df-84ef-4ff5309e8590` (observability is incident-context-only, weaker than its shipped sibling); and Garner Health's "Senior Security Engineer" `6238004004` and "Staff Security Engineer" `6200743004` (Terraform + named security tools, but no SIEM/SOAR/detection-engineering term beyond generic "security monitoring" — borderline, held back).

**Three previously-reliable sources went to zero this run, with no qualifying replacement found despite a dedicated search**: Red Hat's formalized US-remote pick `R-060309-1` is confirmed closed (a new lead, `R-060411`, names Terraform+Ansible but has no observability/SIEM term and fails filter 2); Leidos's only tracked remote-US pick `R-00196252` is confirmed closed (5 searchText variants swept, closest candidate `R-00193640` fails the observability filter and is junior-level); and Zscaler's two tracked picks are both gone — `5158936007` is 404'd off the board entirely, and `5029669007` now requires strict Santa Clara onsite with no Bellevue/remote language, failing filter 3.

No roles were dropped this run for citizenship/clearance language — per project rule, those roles ship with `[US-CITIZEN]`/`[CLEARANCE]`/`[CLEARANCE-ACTIVE]` tags instead.

Full run detail (sites visited, API calls, token usage, source-by-source coverage) is logged in `logs/job-market-scan-2026-11-16.json`.
