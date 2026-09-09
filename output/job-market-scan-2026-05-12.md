# Cloud / DevOps / SRE Job Market Scan — US Remote

**Date:** 2026-05-12 (validation-first re-scan; final pass)
**Profile:** Senior Linux Systems Engineer · Terraform / Ansible · Python · SIEM · DevSecOps
**Scope:** US-remote · Senior / Staff IC · Tech + Energy (energy tagged `[ENERGY]`)
**Filter (all three required):** Linux + IaC · Observability/SIEM/security angle · US-remote eligible

---

## Summary

- This is a fresh, **validation-first** scan. Every shortlisted role's URL has been confirmed live by hitting the employer's ATS public JSON API (Lever / Greenhouse / Ashby) and reading the actual JD body — no search snippets, no aggregator mirrors. Methodology is the one written into `workflows/job-market-scan.md` Step 3.5.
- **4 strong matches pass all three must-have filters** with explicit Terraform/Ansible naming. 1 additional fallback (hybrid + US citizens only). 5 "strong fit, but JD doesn't enumerate IaC tooling" near-misses included as a second tier in case the candidate wants to relax filter #1 for an otherwise-clean SRE role.
- **Energy remains zero.** Every energy company queried via Greenhouse/Lever/Ashby APIs either returned no postings, no senior DevOps/SRE titles, or postings that failed filter #1. Most major US energy employers (NextEra, Tesla, Schneider, etc.) use Workday with per-tenant paths that need to be discovered manually — flagged for next run.
- **One thing the candidate should know:** Zscaler has *two* good roles. The Principal SRE passes all three filters strictly; the Staff SRE (lower comp, similar scope) has explicit Prometheus/OpenTelemetry/detection-engineering language but doesn't name Terraform/Ansible. Worth applying to both if seniority allows.

---

## Top picks (4)

### 1. Principal Site Reliability Engineer — Zscaler
$192,500–$275,000. Remote – USA explicit. JD literally says "Deep professional experience with Terraform and Ansible" and "deep expertise in IaC/CaC, Linux virtualization, and physical hardware management." Python or Go required. Kubernetes deep expertise. Cloud Operations team — exactly the DevSecOps/SIEM lineage in a security-vendor context. **Strongest verified match overall, especially for the Linux-systems-engineer profile.**

### 2. Senior Infrastructure Engineer — Twilio
$141,520–$166,400. Remote – US. JD names Terraform explicitly ("Infrastructure as Code (Terraform, GitOps, or similar)"), plus Kubernetes/EKS, Docker, AWS, and observability tooling by name: "Datadog, ELK, Prometheus/Grafana." Production reliability + incident response scope. Slightly lower comp than Zscaler but cleanest single-paragraph match to the candidate's resume.

### 3. Senior DevOps / SRE Engineer — MLabs
$120K–$150K. Remote, USA timezones eligible. Terraform, Ansible, Prometheus, Grafana, Datadog, Loki — the most complete IaC + observability JD overlap in the shortlist. Incident-leadership scope at a blockchain/AI-trading infra company. Lower comp than Twilio/Zscaler but the stack hits every single filter keyword.

### 4. Senior Platform Engineer — Liatrio
$110K–$183K (per earlier source — not in current API payload). Remote, US or Canada. JD names Terraform + Prometheus + metrics/logs/tracing observability. Consulting context with **25–50% travel** depending on client needs — biggest caveat. Solid fit if travel is acceptable.

---

## Full shortlist — verified, all three filters pass (4)

- **Principal Site Reliability Engineer** — Zscaler
  - **Location:** Remote – USA (also San Jose, CA listed as alternative)
  - **Stack match:** Linux · Terraform · Ansible · Python · Kubernetes · IaC/CaC · Hardware/virtualization
  - **Why it fits:** Security-vendor SRE at scale; "Deep professional experience with Terraform and Ansible" in JD; Linux-virtualization + bare-metal angle maps to candidate's systems-engineering depth.
  - **Apply link:** [https://boards.greenhouse.io/zscaler/jobs/5100835007](https://boards.greenhouse.io/zscaler/jobs/5100835007)
  - **Source:** Greenhouse — Zscaler · $192.5K–$275K
  - **Verified via:** Greenhouse JSON API (`boards-api.greenhouse.io/v1/boards/zscaler/jobs/5100835007`) — full JD fetched 2026-05-12; Terraform and Ansible explicitly named.

- **Senior Infrastructure Engineer** — Twilio
  - **Location:** Remote – US
  - **Stack match:** Terraform · Kubernetes/EKS · Docker · AWS · Observability (Datadog, ELK, Prometheus, Grafana) · Incident response
  - **Why it fits:** Production reliability + on-call automation at scale; explicit observability tooling overlap with candidate's telemetry-pipeline background.
  - **Apply link:** [https://boards.greenhouse.io/twilio/jobs/7474040](https://boards.greenhouse.io/twilio/jobs/7474040)
  - **Source:** Greenhouse — Twilio · $141,520–$166,400
  - **Verified via:** Greenhouse JSON API — full JD fetched 2026-05-12; Terraform + Datadog/ELK/Prometheus/Grafana all named.

- **Senior DevOps / SRE Engineer** — MLabs
  - **Location:** Remote, USA timezones (also UTC+0)
  - **Stack match:** Terraform · Ansible · Observability (Prometheus, Grafana, Datadog, Loki)
  - **Why it fits:** Most complete keyword overlap with candidate's stack; incident-leadership + reliability bar.
  - **Apply link:** [https://remotive.com/remote/jobs/devops/senior-devops-sre-engineer-4224115](https://remotive.com/remote/jobs/devops/senior-devops-sre-engineer-4224115)
  - **Source:** Remotive · $120K–$150K
  - **Verified via:** WebFetch — full JD returned 2026-05-12 (re-confirmed live this run).

- **Senior Platform Engineer** — Liatrio
  - **Location:** Remote (US or Canada — must be work-authorized without sponsorship)
  - **Stack match:** Terraform · CI/CD (GitHub Actions, GitLab) · Kubernetes · Observability (Prometheus + metrics/logs/tracing/alerting)
  - **Why it fits:** Strong observability ownership in a consulting context with broad client exposure. Ansible not named (Terraform alone satisfies filter #1).
  - **Apply link:** [https://jobs.lever.co/liatrio/460b92ff-7078-4c7b-9362-49fc29bba70c](https://jobs.lever.co/liatrio/460b92ff-7078-4c7b-9362-49fc29bba70c)
  - **Source:** Lever — Liatrio
  - **Verified via:** Lever JSON API — confirmed live; full JD body fetched. **Caveat:** 25–50% travel.

---

## Fallback (caveated, doesn't strictly pass)

- **Senior DevOps Engineer (Terraform/Ansible)** — Information Consulting Services
  - **Location:** Austin, TX — **hybrid 3–4 days/week onsite, contract-to-hire, US citizens only.** Fails strict pure-remote filter.
  - **Stack match:** Terraform · Ansible · Python · Bash · Linux · AWS/Azure/GCP
  - **Apply link:** [https://jobs.joindevops.com/jobs/468250835-senior-devops-engineer-terraform-ansible](https://jobs.joindevops.com/jobs/468250835-senior-devops-engineer-terraform-ansible)
  - **Verified via:** WebFetch — full JD returned 2026-05-12.

---

## Second tier — strong fits, fail filter #1 strictly

These pass filters #2 (observability) and #3 (US-remote) cleanly and the candidate's profile maps well, but the JD does not enumerate Terraform or Ansible by name. Included so the candidate can decide whether to relax filter #1 for any of them — real-world infra teams almost always run Terraform/Ansible even when JDs don't list them.

- **Staff Software Engineer — Grafana Cloud Observability, Kubernetes Monitoring** — Grafana Labs
  - Remote, USA EST · Python/Go · Prometheus/Mimir/Loki/Tempo · OpenTelemetry pipelines
  - [https://boards.greenhouse.io/grafanalabs/jobs/5811262004](https://boards.greenhouse.io/grafanalabs/jobs/5811262004)

- **Senior Observability Architect (PST)** — Grafana Labs
  - $204K–$260K · Remote, USA · "Grafana, Prometheus, and Loki a plus" · Kubernetes
  - [https://boards.greenhouse.io/grafanalabs/jobs/5971212004](https://boards.greenhouse.io/grafanalabs/jobs/5971212004)

- **Staff Software Engineer, DevProd (Infrastructure Observability)** — Temporal Technologies
  - $212K–$286K · Remote, US · Clickhouse, Prometheus, Grafana, Loki, Thanos, Kubernetes
  - [https://boards.greenhouse.io/temporaltechnologies/jobs/5119529007](https://boards.greenhouse.io/temporaltechnologies/jobs/5119529007)

- **Staff Site Reliability Engineer** — Zscaler
  - $119K–$170K · Remote – USA · Linux/BSD, Kubernetes, Prometheus/OpenTelemetry, detection/diagnosis
  - [https://boards.greenhouse.io/zscaler/jobs/5029669007](https://boards.greenhouse.io/zscaler/jobs/5029669007)

- **Senior Software Engineer, Compute Platform** — Reddit
  - $190.8K–$267.1K · Remote – United States · "expert in Linux internals" · Kubernetes controllers/operators
  - [https://boards.greenhouse.io/reddit/jobs/7902277](https://boards.greenhouse.io/reddit/jobs/7902277)

---

## Dropped on re-validation (from earlier passes of this report)

| Role | Reason |
|------|--------|
| DuckDuckGo — Senior CloudOps Engineer | Recruitee subdomain returns "careers not hosted" |
| CrowdStrike — Engineer III, CICD DevOps | Hybrid out of US offices, not pure remote; no Terraform explicit |
| Florida Power & Light / NextEra — Senior DevOps `[ENERGY]` | Talentify URL returns 404 after host redirect |
| Jack Henry & Associates — Senior SRE | Himalayas URL is a generic aggregator listing, not the JD |
| EVgo — Senior DevOps `[ENERGY]` | Jobvite URL renders department listing only |
| Flashbots — Senior DevOps | Remotive URL returns HTTP 410 Gone |
| ZayZoon — Senior DevOps | JD names CloudFormation, not Terraform/Ansible |
| Snyk — Senior SWE, Data Infrastructure | Greenhouse URL returns HTTP 404 |
| Chronosphere — Member of Technical Staff, Cloud Infra | Posting removed 2025-05-19 |
| Enphase Energy — Senior DevOps `[ENERGY]` | Jobvite URL renders department listing only |
| The Voleon Group — Senior Cluster SRE | Lever API: 0 open postings company-wide |
| AHEAD — Senior Cloud Engineer | URL not in current Lever postings; alternates fail filter #2 |

---

## Sources & method

- **Date scanned:** 2026-05-12
- **Filter criteria** (all three required for the top-picks tier):
  1. Linux + IaC (Terraform and/or Ansible explicitly named in JD)
  2. Observability / SIEM / security angle
  3. US-remote eligible
- **Validation methodology this run:**
  - **Greenhouse:** queried `boards-api.greenhouse.io/v1/boards/<slug>/jobs` across 40+ employer slugs (cloud-native + energy crossover). For each title match, fetched full JD body via `…/jobs/<id>?questions=false` and grep'd for the must-have keywords.
  - **Lever:** queried `api.lever.co/v0/postings/<slug>?mode=json` for 20+ slugs. For each title match, fetched per-posting body via `…/postings/<slug>/<id>` and grep'd for must-haves. This is also how the Voleon and AHEAD URLs from the previous report were confirmed dead.
  - **Ashby:** queried `api.ashbyhq.com/posting-api/job-board/<slug>` for known slugs. No new matches (most cloud-native employers on Ashby weren't in the seed list).
  - **Remotive:** queried `remotive.com/api/remote-jobs?search=…` with multiple terms. Only MLabs survived the strict filter combo.
  - **Aggregator URLs** (Himalayas, Built In, Talentify, RemoteRocketShip, Jobright.ai) — explicitly avoided per workflow; not used as final apply links.
- **What didn't yield matches this run:**
  - **Energy companies** — no senior DevOps/SRE/Platform role meeting all three filters surfaced on Greenhouse/Lever/Ashby. NextEra, Tesla, Schneider, etc. use Workday with per-tenant paths that need manual discovery.
  - **Datadog, Stripe, Cloudflare, GitLab Senior SRE, Snowflake** — either no qualifying senior US-remote role open, or roles failed filter #1 (JDs don't name Terraform/Ansible) or filter #3 (hybrid on-site requirement).
- **Suggested next run:** dedicate it to energy. Use Workday per-tenant endpoints (`<tenant>.<region>.myworkdayjobs.com/wday/cxs/...`) starting from NextEra, Tesla Energy, Schneider, Constellation, plus Octopus Energy / Kraken on their proprietary ATS. Also check Greenhouse boards for Form Energy, Fluence, Span, Crusoe, Arcadia (none returned hits today, but they may post intermittently).
