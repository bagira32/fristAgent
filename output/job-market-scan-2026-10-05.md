# Job Market Scan — 2026-10-05

Weekly Cloud/DevOps/SRE US-remote (or Seattle-area onsite/hybrid) scan for a senior
Linux Systems Engineer profile (multi-cloud hardening, Terraform/Ansible, Python,
SIEM/log pipelines, observability, DevSecOps).

## Summary

- **27** roles passed all three locked filters (Linux+IaC, observability/SIEM/security,
  US-remote-or-Seattle) across ~60 individually-evaluated postings (many hundreds more
  scanned in bulk at board-level without opening each JD); curated to a **15-role
  shortlist** for quality/fit/dedup after dropping weak-fit sales/presales/support
  roles and one eligibility-gated role (below).
- **1 role tagged `[ENERGY]`** (Crusoe Energy, Bellevue WA — borderline, titled as
  cloud-support not pure DevOps/SRE but passes all three filters).
- **5 roles tagged `[SEATTLE]`** (onsite/hybrid, no remote requirement needed): F5,
  2× Stripe, 2× Cloudflare, plus Crusoe above.
- **Top recurring stack overlap**: Terraform named in every shortlisted role;
  security-tooling/detection-and-response language (Wiz, GitLab Security, SmarterDx)
  was the strongest observability-filter signal this run, ahead of classic
  SIEM-platform mentions.
- **GitLab remains the single highest-yield employer** (4th consecutive run) — 4 of
  15 shortlisted roles. **Excluded, not shipped**: a strong-fit Zscaler "Staff SRE
  (Production Engineer) – Federal" role (Ansible, telemetry/OTel, lists Bellevue WA
  as an eligible office) explicitly requires **US citizenship** — a material
  eligibility gate outside the locked filters that couldn't be verified for this
  candidate, so it's flagged here rather than shipped: https://job-boards.greenhouse.io/zscaler/jobs/5029669007

## Top picks (4)

### 1. Site Reliability Engineer, Infrastructure Platforms — AMER (Intermediate–Senior Staff) — GitLab
- **Location**: US-remote (Canada/US)
- **Stack match**: Terraform (modules, automation); observability
- **Why it fits**: Direct infra-platform reliability ownership — a recurring
  high-value GitLab lead across multiple scan runs, still open and re-confirmed live.
- **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8623389002
- **Source**: Greenhouse — GitLab careers (verified via Greenhouse JSON API,
  `boards-api.greenhouse.io/v1/boards/gitlab/jobs/8623389002?content=true`, 200,
  re-confirmed 2026-10-05)

### 2. Security Engineer — F5 Networks `[SEATTLE]`
- **Location**: Seattle, WA (hybrid; San Jose also listed)
- **Stack match**: Terraform, Ansible, Puppet, Chef explicitly named; security
  tooling (administers the CrowdStrike EDR platform enterprise-wide)
- **Why it fits**: Hands-on EDR/security-tooling administration plus a full IaC
  stack is the closest 1:1 match to the candidate's DevSecOps background among all
  Seattle-area roles found.
- **Apply link**: https://ffive.wd5.myworkdayjobs.com/f5jobs/job/Seattle/Security-Engineer_RP1038142
- **Source**: Workday — F5 careers, tenant `ffive.wd5.myworkdayjobs.com`, site
  `f5jobs` (verified via Workday search API + direct job page, 200, re-confirmed
  2026-10-05)

### 3. Senior Security Engineer — SmarterDx
- **Location**: US-remote (no state exclusions found)
- **Stack match**: Terraform; SIEM (runs Panther SIEM explicitly), detection
  engineering, AWS GuardDuty/Wiz investigation
- **Why it fits**: Hands-on SIEM/detection-engineering ownership is a near-exact
  match to the candidate's SOC/telemetry-pipeline specialization.
- **Apply link**: https://job-boards.greenhouse.io/smarterdx/jobs/5204868007
- **Source**: Greenhouse — SmarterDx careers (verified via Greenhouse JSON API,
  `api.greenhouse.io/v1/boards/smarterdx/jobs/5204868007?content=true`, 200,
  re-confirmed 2026-10-05)

### 4. Security Engineer, Product & Production Infrastructure — Wiz
- **Location**: US-remote
- **Stack match**: Terraform; security tooling, detection & response
- **Why it fits**: Cloud-security engineering ownership of production
  infrastructure maps directly to the candidate's multi-cloud hardening background.
- **Apply link**: https://job-boards.greenhouse.io/wizinc/jobs/4711762006 — **note**:
  Wiz's own wiz.io apply-page redirect has a live template bug (unsubstituted
  `:title` placeholder in the URL); use this Greenhouse-hosted URL instead.
- **Source**: Greenhouse — Wiz careers, token `wizinc` (verified via Greenhouse
  JSON API, `boards-api.greenhouse.io/v1/boards/wizinc/jobs/4711762006?content=true`,
  200, re-confirmed 2026-10-05)

## Full shortlist (15)

1. **Senior Platform Engineer, GitLab Orbit** — GitLab
   - Location: US-remote (Canada/US)
   - Stack match: Terraform, Kubernetes/Helm; observability (owns platform reliability)
   - Why it fits: Core platform-engineering role, strong IaC + reliability overlap.
   - Apply: https://job-boards.greenhouse.io/gitlab/jobs/8771527002
   - Source: Greenhouse — GitLab careers (full-board JSON API pull, 200, 2026-10-05)

2. **Staff Corporate Security Engineer** — GitLab
   - Location: US-remote (Canada/US)
   - Stack match: Terraform/GitOps (endpoint security via IaC); security tooling,
     security operations, detection and response
   - Why it fits: Security-engineering ownership with an explicit IaC delivery model.
   - Apply: https://job-boards.greenhouse.io/gitlab/jobs/8734888002
   - Source: Greenhouse — GitLab careers (full-board JSON API pull, 200, 2026-10-05)

3. **Senior Site Reliability Engineer** — Garner Health
   - Location: US-remote (HQ NYC, explicitly remote-eligible with occasional travel)
   - Stack match: Terraform; Datadog, observability/SLO ownership
   - Why it fits: Platform-engineering SRE role, AWS/Kubernetes reliability ownership.
   - Apply: https://job-boards.greenhouse.io/garnerhealth/jobs/6180042004
   - Source: Greenhouse — Garner Health careers (verified via Greenhouse JSON API,
     200, 2026-10-05)

4. **Software Engineer, Product Security Data Platforms** — Stripe `[SEATTLE]`
   - Location: Seattle, WA (onsite/hybrid)
   - Stack match: Terraform; observability, security operations
   - Why it fits: Security-data-platform engineering with an IaC + observability angle.
   - Apply: https://job-boards.greenhouse.io/stripe/jobs/7761694
   - Source: Greenhouse — Stripe careers (full-board JSON API pull, 200, 2026-10-05;
     stripe.com's own apply domain is proxy-blocked in this session — this
     Greenhouse-hosted URL is the confirmed-live direct link)

5. **Senior Professional Services Technical Architect – Security** — GitLab
   - Location: US-remote (Canada/US)
   - Stack match: Terraform + Ansible (both explicit); security tooling
   - Why it fits: Consulting/PS role rather than pure IC, but strong stack match —
     included as a secondary option.
   - Apply: https://job-boards.greenhouse.io/gitlab/jobs/8795736002
   - Source: Greenhouse — GitLab careers (full-board JSON API pull, 200, 2026-10-05)

6. **Compliance Engineer – US Public Sector** — Wiz
   - Location: US-remote
   - Stack match: Terraform/OpenTofu; SIEM, observability, security operations
   - Why it fits: Compliance-leaning but strong keyword overlap with candidate's
     security-intelligence background.
   - Apply: https://job-boards.greenhouse.io/wizinc/jobs/4707353006
   - Source: Greenhouse — Wiz careers, token `wizinc` (full-board JSON API pull,
     200, 2026-10-05)

7. **Staff Software Engineer, Deployment Platform** — Stripe `[SEATTLE]`
   - Location: Seattle, WA (onsite/hybrid)
   - Stack match: Terraform ("Infrastructure as Code at scale"); observability
   - Why it fits: Deployment-platform engineering with explicit IaC-at-scale ownership.
   - Apply: https://job-boards.greenhouse.io/stripe/jobs/8038771
   - Source: Greenhouse — Stripe careers (full-board JSON API pull, 200, 2026-10-05)

8. **Distributed Systems Engineer – Data Platform** — Cloudflare `[SEATTLE]`
   - Location: Hybrid, incl. Seattle, WA
   - Stack match: Terraform; observability, Grafana
   - Why it fits: Platform/data-infrastructure engineering with IaC + Grafana
     monitoring ownership.
   - Apply: https://boards.greenhouse.io/cloudflare/jobs/7462801?gh_jid=7462801
   - Source: Greenhouse — Cloudflare careers (full-board JSON API pull, 200, 2026-10-05)

9. **Senior Infrastructure Engineer, Storage Platform** — Cloudflare `[SEATTLE]`
   - Location: In-office, incl. Seattle, WA
   - Stack match: Terraform; observability, Grafana
   - Why it fits: Storage/infrastructure engineering with IaC + monitoring ownership.
   - Apply: https://boards.greenhouse.io/cloudflare/jobs/7629805?gh_jid=7629805
   - Source: Greenhouse — Cloudflare careers (full-board JSON API pull, 200, 2026-10-05)

10. **Software Engineer with Systems Depth** — Datadog
    - Location: Multiple US locations incl. remote
    - Stack match: Terraform (Chef/Consul/Terraform/K8s/large infra deployments);
      observability, Datadog, Elastic
    - Why it fits: Generic systems-infra "track" req that reads close to the
      candidate's build-tooling/large-fleet background.
    - Apply: https://careers.datadoghq.com/detail/4452918/?gh_jid=4452918
    - Source: Greenhouse — Datadog careers (full-board JSON API pull, 200, 2026-10-05)

11. **Sr. Cloud Support Engineer – Weekend Shift** — Crusoe Energy `[ENERGY]` `[SEATTLE]`
    - Location: Bellevue, WA — hybrid (on-site required weekday/weekend shift rotation)
    - Stack match: Terraform ("workload management, e.g., Slurm, Terraform");
      Grafana ("monitoring tools")
    - Why it fits: Linux CLI + cloud-support role touching Terraform-managed GPU-cloud
      infra and Grafana monitoring with 24/7 incident ownership — titled as support
      rather than pure DevOps/SRE, borderline but passes all three filters.
    - Apply: https://jobs.ashbyhq.com/Crusoe/43f1edf3-8459-4573-87db-9f00293e3118
    - Source: Ashby — Crusoe Energy careers, org slug `Crusoe` (verified via Ashby
      posting API, full JD in payload, 200, 2026-10-05)

## Flagged, not shipped

- **Staff Site Reliability Engineer (Production Engineer) – Federal** — Zscaler.
  Passes all three locked filters (Ansible + Python/Go named; telemetry/Prometheus/
  OpenTelemetry for observability; location list includes **Bellevue, WA** alongside
  San Jose/Boston/Denver/NYC — qualifying under the Seattle-area clause) but the JD
  states **"US Citizenship is required (due to the nature of assigned customers)"**
  — an eligibility condition outside the locked filter criteria that this scan has
  no way to verify against the candidate. Surfacing it here rather than silently
  dropping or silently shipping it: https://job-boards.greenhouse.io/zscaler/jobs/5029669007
  (verified via Greenhouse JSON API, 200, 2026-10-05). Confirm citizenship
  eligibility before applying.

## Sources & method

Queried in this order per `workflows/job-market-scan.md`:

1. **Cloud-native tech + Seattle-area major employers** (parallel subagent): Datadog,
   Elastic, Grafana Labs, Chronosphere, Honeycomb, Cloudflare, Fastly, GitLab, GitHub,
   Red Hat, Canonical, SUSE, CrowdStrike, Wiz, Snyk, Sysdig, Tenable, Palo Alto
   Networks, Stripe, Shopify, Reddit, DuckDuckGo, HashiCorp, Amazon, Microsoft, F5
   Networks, T-Mobile, Nordstrom Tech, Workiva — via employer ATS JSON APIs
   (Greenhouse/Workday/Ashby/Lever) where available, WebSearch/WebFetch otherwise.
2. **Energy-sector employers** (parallel subagent): Octopus Energy/Kraken, Palantir,
   Hut8, Crusoe Energy, ChargePoint, EVgo, Sunnova, Enphase, Sunrun, Constellation,
   NextEra, Duke Energy, Exelon, Schneider Electric, Siemens Energy, Uplight,
   AutoGrid, GridX, Arcadia, David Energy, Tesla Energy, Southwest Power Pool, Leidos.
3. **LinkedIn + prior-run follow-up leads** (parallel subagent): LinkedIn Jobs search
   (returned no direct `linkedin.com/jobs` URLs this run — an apparent indexing gap,
   noted below), plus re-chased leads: Bungie, SmarterDx, Garner Health, Attain,
   Zscaler, Fivetran, BlackCloak, Epic Games, Qlik, Experian, Paxos, Chainlink Labs.

Every apply link above was validated live via the employer's own ATS JSON API
(Greenhouse/Ashby/Workday) with `content=true`/full-JD payloads confirming the exact
title and the Terraform/Ansible + observability/SIEM keywords, per the project's
Step 3.5 URL-validation rule — no aggregator or search-snippet URL was shipped. The
4 top picks received a second, independent re-fetch today (2026-10-05) as the Step 6
final spot-check immediately before this report was written.

Full collection/validation detail (every endpoint hit, every egress block, every
dead link, and the full reasoning for every dropped or excluded role) is recorded in
`logs/job-market-scan-2026-10-05.json`.
