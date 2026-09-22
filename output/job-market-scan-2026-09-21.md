# Job Market Scan — 2026-09-21

## Summary

- **~39 raw hits** collected across 3 source groups (8 energy-sector, 18 cloud-native tech/Seattle-majors, ~9 LinkedIn — plus 4 additional GitLab roles surfaced during my own full-board re-check).
- **11 roles survived filtering + live validation** — within the 10–15 target, and the best-quality run yet (vs. 7 on 2026-09-14, 3 on 2026-09-10, 1 on 2026-09-09). No padding with unverified links was needed this time.
- **[ENERGY]**: 1 of 11 (Octopus Energy/Kraken). **[SEATTLE]**: 0 of 11 — several Seattle-area candidates (Palantir Seattle ×2, F5 Seattle ×3) existed but all failed the Linux+IaC or observability filter; F5's Workday tenant is now confirmed working (`ffive.wd5.myworkdayjobs.com`/`f5jobs`) for future runs.
- Top recurring stack overlap: Terraform named in 10 of 11; Ansible confirmed in 4 of 11; observability/security-tooling angle present in all 11. **GitLab remains the single highest-yield source, 3rd run in a row** (6 of 11 shortlisted roles).
- **New reliable source this run**: CrowdStrike surfaced a second strong role beyond its usual SRE post — a "Sr. Linux Systems Engineer – Object Storage" req that's an unusually direct title match to the candidate's own role.

## Top picks (5 of 11)

- **Sr Engineer, SRE TechOps CICD (Remote)** — CrowdStrike
  Strongest stack match in the batch — Terraform, Ansible, Splunk, Datadog, and observability all explicitly named. Direct hit on the candidate's IaC/telemetry-pipeline background. Repeat strong match, still live.
- **Sr. Linux Systems Engineer – Object Storage (Remote)** — CrowdStrike
  Title is an almost exact match to the candidate's own "Linux Systems Engineer" specialization. Ansible, Python, and a Prometheus/Grafana/ELK observability stack all confirmed in the live JD.
- **Staff Infrastructure Security Engineer (USA)** — GitLab
  Terraform + Ansible + Python confirmed; infrastructure-security ownership maps directly to the candidate's multi-cloud hardening/DevSecOps background. 3rd run in a row this exact role has stayed live and validated.
- **Platform Engineer II** — Octopus Energy (Kraken Technologies) `[ENERGY]`
  Terraform, Python, Datadog, and observability all explicitly named at a grid-tech energy platform — strong SIEM/telemetry-pipeline overlap. Only energy-sector role to survive validation this run, 3rd run in a row.
- **Staff Corporate Security Engineer** — GitLab
  Terraform + Python + detection-engineering language named; a new GitLab req (not seen in prior runs) with a direct DevSecOps/detection-engineering angle.

## Full shortlist

- **Sr Engineer, SRE TechOps CICD (Remote)** — CrowdStrike
  - **Location**: US-remote
  - **Stack match**: Terraform ✅ · Ansible ✅ · Python ✅ · SIEM/observability ✅ (Splunk, Datadog, observability all named)
  - **Why it fits**: CI/CD + SRE TechOps ownership with the full IaC/observability toolchain named is a direct line to the candidate's automated-infrastructure and telemetry-pipeline background.
  - **Apply link**: https://crowdstrike.wd5.myworkdayjobs.com/crowdstrikecareers/job/USA---Remote/Sr-Engineer--SRE-TechOps-CICD--Remote-_R29733
  - **Source**: Workday — CrowdStrike careers
  - **Verified via**: Workday JSON API — per-job fetch (`crowdstrike.wd5.myworkdayjobs.com/wday/cxs/crowdstrike/crowdstrikecareers/job/.../_R29733`) (2026-09-21), 200 OK, full JD body, Terraform/Ansible/Python/Splunk/Datadog/observability confirmed in body text; re-confirmed live at Step 6 spot-check.

- **Sr. Linux Systems Engineer – Object Storage (Remote)** — CrowdStrike
  - **Location**: US-remote
  - **Stack match**: Terraform — not confirmed · Ansible ✅ · Python ✅ · SIEM/observability ✅ (Prometheus, Grafana, ELK, observability all named)
  - **Why it fits**: Object-storage systems engineering with Ansible automation and a Prometheus/Grafana/ELK telemetry stack is a near-exact match for the candidate's Linux Systems Engineer title and background.
  - **Apply link**: https://crowdstrike.wd5.myworkdayjobs.com/crowdstrikecareers/job/USA---Remote/Sr-Linux-Systems-Engineer---Object-Storage--Remote-_R29937
  - **Source**: Workday — CrowdStrike careers
  - **Verified via**: Workday JSON API — per-job fetch (`crowdstrike.wd5.myworkdayjobs.com/wday/cxs/crowdstrike/crowdstrikecareers/job/.../_R29937`) (2026-09-21), 200 OK, full JD body, Ansible/Python/Prometheus/Grafana/ELK/observability confirmed; re-confirmed live at Step 6 spot-check.

- **Staff Infrastructure Security Engineer (USA)** — GitLab
  - **Location**: US-remote
  - **Stack match**: Terraform ✅ · Ansible ✅ · Python ✅ · SIEM/observability — security-tooling clause (infrastructure security ownership)
  - **Why it fits**: Infrastructure-security ownership + IaC tooling is a direct line to the candidate's multi-cloud hardening and DevSecOps background.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8769103002
  - **Source**: Greenhouse — GitLab careers
  - **Verified via**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/gitlab/jobs/8769103002` (2026-09-21), title/location/content confirmed live, Terraform + Ansible + Python present in body text; re-confirmed live at Step 6 spot-check.

- **Staff Corporate Security Engineer** — GitLab
  - **Location**: US-remote (also open to Canada)
  - **Stack match**: Terraform ✅ · Ansible ❌ (not named) · Python ✅ · SIEM/observability ✅ (detection-engineering language)
  - **Why it fits**: Corporate/detection-engineering security ownership with named Terraform + Python overlaps directly with the candidate's SIEM/security-tooling and automation background.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8734888002
  - **Source**: Greenhouse — GitLab careers
  - **Verified via**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/gitlab/jobs/8734888002` (2026-09-21), title/location/content confirmed live, Terraform/Python/detection-engineering present in body text; re-confirmed live at Step 6 spot-check.

- **Site Reliability Engineer, Infrastructure Platforms — AMER (Intermediate to Senior Staff)** — GitLab
  - **Location**: US-remote (also open to Canada)
  - **Stack match**: Terraform ✅ · Ansible ❌ (not named) · SIEM/observability ✅ (observability stack, metrics/logs/SLOs ownership)
  - **Why it fits**: SRE ownership of infrastructure platforms with explicit Terraform and observability language matches the candidate's SRE/IaC profile. Repeat strong match, still live 3rd run in a row.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8623389002
  - **Source**: Greenhouse — GitLab careers
  - **Verified via**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/gitlab/jobs/8623389002` (2026-09-21), Terraform + observability present in body text.

- **Senior Platform Engineer, GitLab Orbit** — GitLab
  - **Location**: US-remote (also open to Canada)
  - **Stack match**: Terraform ✅ · Ansible ❌ (not named) · SIEM/observability ✅ (observability stack ownership)
  - **Why it fits**: Platform engineering with named Terraform and observability ownership overlaps with the candidate's IaC/observability profile. Repeat strong match, still live 3rd run in a row.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8771527002
  - **Source**: Greenhouse — GitLab careers
  - **Verified via**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/gitlab/jobs/8771527002` (2026-09-21), title/location/content confirmed live, Terraform + observability present in body text.

- **Platform Engineer II** — Octopus Energy (Kraken Technologies) `[ENERGY]`
  - **Location**: US-remote
  - **Stack match**: Terraform ✅ · Ansible ❌ (not named) · Python ✅ · SIEM/observability ✅ (Datadog, observability explicitly named)
  - **Why it fits**: Grid-tech energy platform engineering with Terraform + Datadog/telemetry ownership overlaps directly with the candidate's SIEM/log-pipeline and multi-cloud hardening background.
  - **Apply link**: https://jobs.lever.co/octoenergy/e2a5dba5-53ec-4623-8b25-85efcfed3d19
  - **Source**: Lever — Octopus Energy / Kraken Technologies careers
  - **Verified via**: Lever JSON API — `api.lever.co/v0/postings/octoenergy` (2026-09-21), posting present in current live array, Terraform/Python/Datadog/observability confirmed in body text; re-confirmed present at Step 6 spot-check.

- **Platform Engineer - Kubernetes** — Elastic
  - **Location**: United States (pay band varies by metro; no state exclusion found)
  - **Stack match**: Terraform ✅ (named alongside Crossplane as IaC tooling) · Ansible ❌ · SIEM/observability ✅ (observability explicitly named)
  - **Why it fits**: Kubernetes platform engineering with named IaC tooling and observability ownership matches the candidate's infra-automation and telemetry background.
  - **Apply link**: https://jobs.elastic.co/jobs?gh_jid=8047349
  - **Source**: Greenhouse — Elastic careers
  - **Verified via**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/elastic/jobs?content=true` (2026-09-21), job ID present, title/location confirmed, Terraform + observability present in body text.

- **Senior Professional Services Technical Architect - Security** — GitLab
  - **Location**: US-remote (also open to Canada)
  - **Stack match**: Terraform ✅ · Ansible ✅ · SIEM/observability — security-controls/CI-CD-integration angle
  - **Why it fits**: Hands-on Ansible + Terraform configuration-management work integrating security controls into CI/CD lines up with the candidate's DevSecOps and infrastructure-hardening background, though this is a customer-facing consulting role rather than pure internal ops.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8795736002
  - **Source**: Greenhouse — GitLab careers
  - **Verified via**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/gitlab/jobs/8795736002` (2026-09-21), Ansible + Terraform + security/CI-CD integration present in body text.

- **Staff Forward Deployed Engineer** — GitLab
  - **Location**: US-remote
  - **Stack match**: Terraform ✅ · Ansible ❌ · SIEM/observability ✅ (Linux, networking, observability, and performance analysis explicitly listed)
  - **Why it fits**: Explicit "Linux, networking, observability, and performance analysis" plus Terraform/GitLab CI-CD/runner architecture is a strong technical-skills match, though the role is customer-facing (forward-deployed) rather than internal SRE.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8512432002
  - **Source**: Greenhouse — GitLab careers
  - **Verified via**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/gitlab/jobs/8512432002` (2026-09-21), Terraform/Linux/observability present in body text.

- **Tech Lead, Agent Framework - Observability** — Elastic
  - **Location**: United States (pay band varies by metro; no state exclusion found)
  - **Stack match**: Terraform — named as nice-to-have ("experience with cloudformation, terraform, or other IaC tooling") · Ansible ❌ · SIEM/observability ✅ (Observability team, pipeline execution models, logstash/fluent)
  - **Why it fits**: Weakest fit of the eleven — this is a dev/SWE-leaning Tech Lead role on Elastic's Observability team rather than an infra/ops role, but it clears all three must-haves and the observability-domain overlap is genuine.
  - **Apply link**: https://jobs.elastic.co/jobs?gh_jid=8071641
  - **Source**: Greenhouse — Elastic careers
  - **Verified via**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/elastic/jobs?content=true` (2026-09-21), job ID present, title/location confirmed, Terraform + observability present in body text.

## Roles found but dropped in validation (for the record)

| Role — Company | Reason dropped |
|---|---|
| Cybersecurity Engineer II \| SIEM and EDR (Remote) — Home Depot | Confirmed LIVE via direct curl fetch (title matched, full 1.2MB page retrieved) — strong SIEM/EDR match (Cortex XSIAM, Splunk, CrowdStrike all named) but **zero occurrences of "Terraform" or "Ansible" anywhere on the page**. Fails Linux+IaC filter despite live posting and strong SIEM angle. |
| Senior Cybersecurity Engineer \| GCP, DevOps — Home Depot | Terraform/Ansible explicit per snippet, but Austin, TX-based, not remote and not Seattle-area. Fails geography filter. |
| Site Reliability Engineer, Infrastructure Platforms — UK — GitLab | Found during full-board re-check; Terraform + observability confirmed, but Remote-UK only. Fails US-remote/Seattle geography filter. |
| Forward Deployed Engineer, AI and Agentic SDLC — GitLab | Terraform/Ansible/AWS/GCP/Azure named, US-remote — but role is AI/Agentic-SDLC customer engineering, a materially weaker profile match than the other 6 GitLab roles. Deprioritized rather than shortlisted, to keep the list at reasonable quality; worth reconsidering if the list needs padding in a future run. |
| Sr. Infrastructure Engineer, TechOps CICD (Remote) — CrowdStrike (R30075) | Confirmed live — Terraform + Ansible named, but no SIEM/observability keyword found in JD. Fails observability filter. |
| Security Engineer (RP1038142) — F5 | Seattle onsite — Terraform + Ansible + Puppet/Chef named, but no SIEM/observability keyword found. Fails observability filter. |
| Principal Security Engineer – Incident Response (RP1038430); Security Engineer – Incident Response (RP1038431) — F5 | Seattle onsite — strong SIEM/telemetry/observability language, but no Terraform/Ansible named. Fails Linux+IaC filter. |
| Software Reliability Engineer; Site Reliability Engineer; Systems Reliability Engineer (×3) — T-Mobile | Terraform/Ansible/Python named per search snippets, but `careers.t-mobile.com` returns HTTP 403 to WebFetch (inconclusive) and T-Mobile has no public ATS API. Per validation rule, dropped rather than shipped on an unverified snippet. |
| Senior Site Reliability Engineer, FedRAMP Cloud Platform (×2 postings) — Splunk | `splunk.com` job URLs now 301-redirect to `careers.cisco.com/global/en/splunk` (Splunk is now under Cisco) — and `careers.cisco.com` is blocked by this session's network egress policy. Inconclusive, dropped. |
| Senior Site Reliability Engineer — Qlik | `careerhub.qlik.com` blocked by network egress policy; no public ATS API found. Inconclusive, dropped. |
| Senior Site Reliability Engineer (Remote) — Experian | `jobs.experian.com` blocked by network egress policy; no public ATS API found. Inconclusive, dropped. |
| Staff Site Reliability Engineer — Workiva | Workday tenant found (`workiva.wd1.myworkdayjobs.com`) but no guessed site slug resolves (`External`/`Careers`/`workiva`/`Workiva` all 422); `www.workiva.com` itself is egress-blocked so the correct site slug couldn't be looked up. Inconclusive, dropped rather than guessing further. |
| DevOps Engineer — EVgo | `jobs.jobvite.com/evgo/...` now 302-redirects to a generic invalid-search page — 2nd run in a row this board is broken. Dead, dropped. |
| Senior DevOps & Infrastructure Engineer — Enphase Energy | `jobs.jobvite.com/enphase-energy/...` returns a 303 redirect to an empty page. Dead, dropped. |
| Senior/Principal DevOps Architect – AWS — Sunnova | Only found via aggregator (BuiltIn); no direct employer ATS URL located. Per rule, aggregator-only means drop. |
| Staff Site Reliability Engineer — David Energy | Dropped at the Step 2 collection-time sanity check — job ID not present on the employer's current live Ashby board (only 2 unrelated postings open). |
| Information Security Engineer; Senior Software Engineer, Network Infrastructure — Palantir (Seattle, WA) `[SEATTLE]` | Confirmed live via Lever API — but neither JD names Terraform or Ansible. Fails Linux+IaC filter. |
| DevOps Engineer — Palantir (Washington, D.C.) | Onsite/hybrid DC only, not remote and not Seattle-area. Fails geography filter. |
| Platform Engineer II — Octopus Energy (Houston, TX onsite) `[ENERGY]` | Same JD as the shortlisted remote posting, but this req is Houston-onsite. Fails geography filter. |
| Systems Engineer, Product Platform Tools — Cloudflare | Austin, TX-based; not remote, not Seattle-area. Fails geography filter. |
| Sr. Site Reliability Engineer — Blackpoint Cyber | Live Ashby posting confirmed — but Remote-Canada, not US. Fails geography filter. |
| Sr./Senior DevOps Engineer, OGS — Epic Games (Bellevue, WA) `[SEATTLE]` | LinkedIn-only; Epic's actual ATS is Avature but no current job ID could be located there this round. Dropped per "aggregator/LinkedIn-only doesn't count" rule. |
| Senior DevSecOps Engineer — Hyperproof | Strong stack fit (Terraform/Terragrunt, Ansible, CI/CD security) per aggregator listing (RemoteRocketship), but no direct Greenhouse/Lever/Ashby URL found. Dropped per aggregator rule. |
| Senior SRE, Cloud Platform — Semperis; Senior SRE - Software Engineering — Bungie `[SEATTLE]` | Both LinkedIn hits are stale — live ATS boards for each currently carry zero SRE/DevOps postings. |
| HashiCorp, Grafana Labs, Fastly, Datadog, Stripe, Reddit, Canonical, Cloudflare (remaining board), Webflow, Sysdig, Wiz, Tenable | Live boards checked (where reachable), no qualifying US-remote/Seattle role this run — consistent with prior runs. |
| GitHub, SUSE, Snyk, DuckDuckGo | No usable public ATS API found (Greenhouse/Lever/Ashby all 404 or placeholder) — dead ends, consistent with prior runs. |
| Chainlink Labs, Paxos | Ashby/Greenhouse boards still unresolvable under any guessed slug — 3rd+ run in a row. |
| Amazon, Microsoft | No direct ATS URL located this round; both domains also egress-blocked. 3rd run in a row with no locatable direct listing. |
| ChargePoint, Duke Energy, Sunrun, Uplight, Crusoe Energy, Hut 8, Tesla Energy, Schneider Electric, Leidos, Siemens Energy, Southwest Power Pool, GridX, AutoGrid, Arcadia | Checked (ATS reachable for most), no qualifying or independently validatable role found this run. |
| Constellation Energy, NextEra Energy, Exelon | Workday tenant-guessing still returns 422. **New finding**: Exelon's careers site is actually on iCIMS (`careers-exeloncorp.icims.com`), not Workday — explains the persistent 422s for that one. Constellation/NextEra ATS still unconfirmed. |

## Sources & method

- **Date run**: 2026-09-21
- **Sources queried**: `resources/sources.md` full list — energy-sector employers, cloud-native tech employers, Seattle-area majors (Amazon, Microsoft, F5, T-Mobile, Nordstrom), LinkedIn Jobs (remote + Seattle-area query templates), plus a full re-check of GitLab's live Greenhouse board (all 200+ jobs) and ad-hoc checks for Splunk/Qlik/Experian/Workiva/Home Depot/Epic Games/Hyperproof surfaced via LinkedIn search
- **Filter criteria applied**: Terraform and/or Ansible explicitly named · SIEM/observability/security-tooling angle named · US-remote eligible **or** onsite/hybrid in the Greater Seattle area
- **Validation method**: Greenhouse/Lever/Workday JSON APIs (primary — worked reliably for all API-hosted candidates this run), WebFetch and raw curl for non-API hosts. Splunk's career page (now under Cisco), Qlik, Experian, Workiva, and Cisco's careers domain were unreachable this session (egress-blocked or unresolvable tenant); T-Mobile returned HTTP 403 to WebFetch with no ATS API fallback available. All such roles were dropped rather than shipped unverified.

## Notes for the workflow (Step 7 follow-ups)

- **Home Depot's domain is reachable again this session** (unlike 2026-09-14's hard block) and its SIEM/EDR role is confirmed genuinely live — but it fails the Linux+IaC filter on the merits (no Terraform/Ansible anywhere in the JD), not on validation grounds. Worth noting since the role looked strong by title alone.
- **Splunk's career site now redirects to Cisco** (`careers.cisco.com/global/en/splunk`) following the Cisco acquisition, and Cisco's careers domain is egress-blocked this session. Splunk should be treated as effectively unreachable until either the block lifts or a Cisco-hosted ATS API is identified.
- **T-Mobile continues to 403 WebFetch with no public ATS API** — 2nd run in a row this specific host can't be validated even when the domain itself isn't hard-blocked. Recommend deprioritizing further manual search-snippet chasing for T-Mobile unless a direct ATS is found.
- **Exelon is on iCIMS, not Workday** (`careers-exeloncorp.icims.com`) — this explains 2+ runs of 422s from Workday tenant-guessing. Recommend updating `sources.md` to try iCIMS-pattern lookups for Exelon specifically next run; Constellation/NextEra's correct ATS is still unconfirmed.
- **F5's correct Workday tenant/site is now known**: `ffive.wd5.myworkdayjobs.com` / site `f5jobs` (previous 422s were from guessing the wrong site name). Three Seattle-based F5 security roles were found this run but none cleared both must-have filters — worth rechecking this tenant directly in future runs now that it's resolvable.
- **CrowdStrike's Workday site slug is `crowdstrikecareers`**, not `crowdstrike` (a bare `crowdstrike` site guess 404s) — worth recording precisely since this run found a 2nd strong CrowdStrike role (Object Storage Linux Systems Engineer) beyond the usual SRE TechOps req.
- **GitLab remains the dominant source, 3rd run in a row** (6 of 11 shortlisted roles this run) — a full re-check of its entire live board (beyond the specific titles found by search/collection agents) surfaced 2 additional qualifying roles (Corporate Security Engineer, Professional Services Security Architect, Staff Forward Deployed Engineer) not caught by keyword search alone. Recommend future runs always pull GitLab's full board via the Greenhouse API rather than relying only on search-indexed titles.
- **Workiva** is a promising novel lead (found via LinkedIn, Terraform/GCP/AWS stack per snippet) but its Workday site slug couldn't be resolved this run and its main domain is egress-blocked. Revisit next run — if the block lifts, one WebFetch to `workiva.com/careers` should reveal the correct tenant/site.
- **Qlik and Experian** are both egress-blocked this session with no ATS API alternative found — both had promising snippets (Qlik: Terraform/Crossplane/Ansible/Prometheus/OTel/Splunk; Experian: 3+ yrs Terraform). Revisit if the block lifts.
- **Epic Games** (Bellevue, WA `[SEATTLE]`) surfaced again via LinkedIn with a strong stack per snippet (Terraform, Ansible, Python/Go/Bash) but its actual ATS (Avature) couldn't be pinned to a current job ID. Worth dedicated ATS-hunting effort next run given the Seattle-area fit.
- Reviewed 2026-09-14 → 2026-09-21.
