# Cloud / DevOps / SRE Job Market Scan — 2026-09-28

Weekly US-remote (or onsite/hybrid Seattle-area) scan for a Senior Linux
Systems Engineer profile (multi-cloud hardening, Terraform/Ansible, Python,
SIEM/log pipelines, DevSecOps, observability).

## Summary

- **50 raw hits** collected across cloud-native tech, energy-sector, and
  LinkedIn sources; **10 passed all 3 must-have filters + live URL
  validation** — down from 11 last run, mainly because GitLab's board
  yielded fewer qualifying reqs this week and several new LinkedIn-sourced
  leads (Bungie, SmarterDx, Zscaler, Garner Health, Attain) turned out to be
  **dead/stale job IDs** caught by Step 3.5 validation (search snippets do
  not equal live postings — see Sources & method).
- **1 energy-tagged** `[ENERGY]` role (Octopus Energy/Kraken) — Palantir (6
  reqs) and Crusoe Energy (4 reqs) both had strong-looking energy-sector
  postings this run but every one failed on geography (DC/NY hybrid or
  SF/Dublin onsite) or missing explicit Terraform/Ansible.
- **1 Seattle-tagged** `[SEATTLE]` role (F5 Networks) — the only Seattle
  hybrid role this run to clear both must-have filters, out of 4 F5
  candidates and 1 Hut8 candidate checked.
- **Top recurring stack overlap**: Terraform + observability/telemetry
  ownership (metrics/logs/traces/SLOs) is the dominant pattern across
  GitLab's 4 qualifying roles; CrowdStrike continues to be the strongest
  direct "Linux Systems Engineer" title match two runs running.
- **Notable signal**: three "new employer" leads surfaced via LinkedIn/web
  search this run (Bungie, SmarterDx, Zscaler-Federal, Garner Health,
  Attain) all resolved to 404 against their employer's own live Greenhouse
  board when validated — a reminder that LinkedIn/search-snippet job IDs
  have a high stale rate and must never ship without the Step 3.5 API
  cross-check.

## Top picks (5)

- **Sr. Linux Systems Engineer - Object Storage (Remote)** — CrowdStrike
  - **Location**: US-remote
  - **Stack match**: Linux (title-level), Ansible, Python, observability (Prometheus, Grafana, ELK stack)
  - **Why it fits**: Closest direct title match to the candidate's own specialization — Linux systems engineering at global scale, with explicit observability-tool ownership.
  - **Apply link**: https://crowdstrike.wd5.myworkdayjobs.com/crowdstrikecareers/job/USA---Remote/Sr-Linux-Systems-Engineer---Object-Storage--Remote-_R29937
  - **Source**: Workday — CrowdStrike careers (tenant `crowdstrike`, site `crowdstrikecareers`)

- **Staff Corporate Security Engineer** — GitLab
  - **Location**: US-remote (also open to Canada)
  - **Stack match**: Terraform, GitOps/IaC for device management, detection & response telemetry, Python/Go/PowerShell security tooling
  - **Why it fits**: Genuine detection-engineering and endpoint-telemetry work (not just DevSecOps buzzwords) paired with Terraform-driven device management — a strong SIEM/telemetry-pipeline analog to the candidate's SOC/observability background.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8734888002
  - **Source**: Greenhouse — GitLab careers (board `gitlab`)

- **Security Engineer** — F5 Networks `[SEATTLE]`
  - **Location**: Seattle, WA — onsite/hybrid (candidate can commute)
  - **Stack match**: Terraform, Ansible, Python, security tooling (CrowdStrike + other detection/response tools)
  - **Why it fits**: Direct Terraform+Ansible+security-tooling overlap in a Seattle-based role the candidate can work without a remote-eligibility requirement.
  - **Apply link**: https://ffive.wd5.myworkdayjobs.com/f5jobs/job/Seattle/Security-Engineer_RP1038142
  - **Source**: Workday — F5 careers (tenant `ffive`, site `f5jobs`)

- **Security Engineer, Product & Production Infrastructure** — Wiz
  - **Location**: US-remote
  - **Stack match**: Terraform, detection & response operations, policy-as-code/security tooling
  - **Why it fits**: A cloud-security company building its own Terraform-driven infra with a genuine detection-and-response mandate — DevSecOps positioning that maps directly to the candidate's hardening + SIEM background.
  - **Apply link**: https://boards.greenhouse.io/wizinc/jobs/4711762006
  - **Source**: Greenhouse — Wiz careers (board `wizinc` — note: NOT `wiz`, which 404s)

- **Site Reliability Engineer, Infrastructure Platforms — AMER (Intermediate to Senior Staff)** — GitLab
  - **Location**: US/Canada-remote
  - **Stack match**: Terraform, observability (metrics/logs/SLOs to detect symptoms early)
  - **Why it fits**: Explicit observability-ownership mandate (SLOs, early-symptom detection) on Terraform-managed infrastructure, at a title band (Intermediate–Senior Staff) that fits a senior IC.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8623389002
  - **Source**: Greenhouse — GitLab careers (board `gitlab`)

## Full shortlist (10)

- **Senior Platform Engineer, GitLab Orbit** — GitLab
  - **Location**: US/Canada-remote
  - **Stack match**: Terraform, Kubernetes/Helm, observability (metrics/logs/traces/dashboards/alerts, incident readiness)
  - **Why it fits**: Direct observability-ownership + Terraform overlap on GitLab's internal deployment platform.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8771527002
  - **Source**: Greenhouse — GitLab careers (board `gitlab`)

- **Site Reliability Engineer, Infrastructure Platforms — AMER (Intermediate to Senior Staff)** — GitLab
  - **Location**: US/Canada-remote — see Top picks above for detail.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8623389002
  - **Source**: Greenhouse — GitLab careers

- **Staff Corporate Security Engineer** — GitLab — see Top picks above for detail.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8734888002
  - **Source**: Greenhouse — GitLab careers

- **Senior Professional Services Technical Architect – Security** — GitLab
  - **Location**: US/Canada-remote
  - **Stack match**: Terraform, Ansible, security tooling (leads migration of AppSec/SAST-DAST tooling such as Snyk, Checkmarx, Secret Detection)
  - **Why it fits**: Security-tooling migration and hardening work aligns with the candidate's DevSecOps background, though the angle is AppSec/CI-CD scanning rather than SIEM/log-pipelines specifically — **flagged borderline on the observability/SIEM must-have**: it passes on "security tooling" language but doesn't hit SIEM/SOAR/telemetry directly. Included because the JD's security-tooling content is substantive, not a buzzword match.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8795736002
  - **Source**: Greenhouse — GitLab careers

- **Sr Engineer, SRE TechOps CICD (Remote)** — CrowdStrike
  - **Location**: US-remote
  - **Stack match**: Ansible, Chef, Puppet, Salt, Terraform (IaC provisioning); Datadog, Grafana, Humio/LogScale, Honeycomb, New Relic, Prometheus, Splunk (observability)
  - **Why it fits**: Broad IaC + observability-tool breadth mirrors the candidate's telemetry-pipeline background.
  - **Apply link**: https://crowdstrike.wd5.myworkdayjobs.com/crowdstrikecareers/job/USA---Remote/Sr-Engineer--SRE-TechOps-CICD--Remote-_R29733
  - **Source**: Workday — CrowdStrike careers

- **Sr. Linux Systems Engineer - Object Storage (Remote)** — CrowdStrike — see Top picks above for detail.
  - **Apply link**: https://crowdstrike.wd5.myworkdayjobs.com/crowdstrikecareers/job/USA---Remote/Sr-Linux-Systems-Engineer---Object-Storage--Remote-_R29937
  - **Source**: Workday — CrowdStrike careers

- **Security Engineer** — F5 Networks `[SEATTLE]` — see Top picks above for detail.
  - **Apply link**: https://ffive.wd5.myworkdayjobs.com/f5jobs/job/Seattle/Security-Engineer_RP1038142
  - **Source**: Workday — F5 careers

- **Security Engineer, Product & Production Infrastructure** — Wiz — see Top picks above for detail.
  - **Apply link**: https://boards.greenhouse.io/wizinc/jobs/4711762006
  - **Source**: Greenhouse — Wiz careers

- **Platform Engineer II** — Octopus Energy / Kraken Technologies `[ENERGY]`
  - **Location**: US-remote
  - **Stack match**: Terraform (or similar IaC), Datadog (or similar monitoring/logging)
  - **Why it fits**: Energy-sector software platform with direct IaC + observability overlap. **Note**: "II" level reads as more mid-level than the candidate's senior/staff band — included for stack/geography fit but ranked lower on seniority match.
  - **Apply link**: https://jobs.lever.co/octoenergy/e2a5dba5-53ec-4623-8b25-85efcfed3d19
  - **Source**: Lever — Octopus Energy/Kraken careers (slug `octoenergy`)

- **Director of Security Engineering** — Sysdig
  - **Location**: US-remote
  - **Stack match**: Terraform (Kubernetes/multi-cloud hardening via Terraform + CI/CD), detection & response, telemetry
  - **Why it fits**: Hardening-and-detection mandate is a strong background match. **Note**: Director-level title is above a typical senior/staff IC band — flagged for seniority fit, included because stack/geography/domain match is otherwise strong.
  - **Apply link**: https://jobs.lever.co/sysdig/49b38de8-5034-4bd1-a5eb-a206a2866516
  - **Source**: Lever — Sysdig careers (slug `sysdig`)

## Sources & method

Scan date: 2026-09-28. Filter criteria per `resources/sources.md` (Locked
filter criteria, last reviewed 2026-09-21): (1) Terraform and/or Ansible
explicitly named, (2) SIEM/SOAR/detection-engineering/log-pipeline/
observability/security-tooling angle explicitly named, (3) US-remote
eligible or onsite/hybrid in Greater Seattle.

**Sources queried** (Step 2, in order): cloud-native tech employers
(HashiCorp, Datadog, Elastic, Grafana Labs, Chronosphere, Honeycomb,
Cloudflare, Fastly, GitLab, GitHub, Red Hat, Canonical, SUSE, CrowdStrike,
Wiz, Snyk, Sysdig, Tenable, Palo Alto Networks, Stripe, Shopify, Reddit,
DuckDuckGo) + Seattle-area majors (Amazon, Microsoft, F5 Networks,
T-Mobile, Nordstrom Tech); energy-sector employers (Octopus Energy/Kraken,
Tesla Energy, Sunrun, Sunnova, Enphase, ChargePoint, EVgo, Constellation,
NextEra, Duke Energy, Exelon, Schneider Electric, Siemens Energy, Uplight,
AutoGrid, GridX, Arcadia, David Energy, Crusoe Energy, Hut8, Palantir);
LinkedIn Jobs (query template + SIEM/Seattle variants + targeted searches
on 4 promising unformalized leads from the 2026-09-21 run).

**Every apply link above was validated live** on 2026-09-28 via the
employer's ATS JSON API (Greenhouse `boards-api.greenhouse.io/v1/boards/
<token>/jobs/<id>?content=true`, Workday tenant job-detail endpoint, or
Lever `api.lever.co/v0/postings/<slug>?mode=json`), confirming HTTP
200/live status, exact job title, and that Terraform/Ansible +
SIEM/observability language actually appears in the full JD body (not just
a search snippet). The 5 Top Picks were re-confirmed live a second time
immediately before this report was written (Step 6 spot-check). No
aggregator/mirror link or unverified search-snippet URL appears above.

**Validation drops worth noting**: Bungie, SmarterDx, Zscaler ("Staff SRE -
Federal"), Garner Health, and Attain job IDs surfaced by LinkedIn/web
search all 404'd against the employer's current live Greenhouse board —
dropped as dead links, not shipped. Workiva (Workday platform-wide
maintenance outage this session), Experian (`jobs.experian.com` and the
SmartRecruiters API both egress-blocked), Epic Games (Avature tenant
unreachable), and Qlik (egress-blocked, Raleigh-NC-based with unconfirmed
remote eligibility) were dropped as inconclusive rather than guessed at.
BlackCloak had no direct-ATS URL, only an aggregator listing — dropped.

30 raw hits failed a must-have filter outright after inspection (wrong
geography — DC/NY/SF/Dublin/Austin/Santa Clara/Chicago/Miami with no
remote or Seattle option — or no explicit Terraform/Ansible, or no
substantive SIEM/observability/security-tooling language beyond company
boilerplate). Full breakdown is in `logs/job-market-scan-2026-09-28.json`.

See `resources/sources.md` for the full locked criteria and this run's
new source-list findings (added below).
