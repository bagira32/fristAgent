# Cloud / DevOps / SRE Job Market Scan — 2026-10-12

Weekly scan for a Linux Systems Engineer profile (multi-cloud hardening,
Terraform/Ansible, Python, SIEM/log pipelines, observability, DevSecOps).
US-remote eligible, or onsite/hybrid in Greater Seattle.

## Summary

- **26 roles passed all 3 locked filters** this run (23 fully shippable after
  live validation + 3 eligibility-gated); curated down to a **15-role final
  shortlist** after cutting weak-fit and redundant picks.
- **Terraform** was the dominant IaC signal (named in 13 of 15 shortlisted
  roles); **Ansible** explicitly named in 4; observability tooling
  (Prometheus/Grafana/Datadog/Splunk) anchored most matches, and 2 roles
  carried genuine named-**SIEM** language (Panther at SmarterDx, Wiz at
  Garner Health — the latter cut in curation for redundancy).
- **GitLab remains the single highest-yield source** — 3 of 15 shortlisted
  roles, a 4th consecutive run as top source. **Nordstrom Tech** newly
  resolved as a directly-crawlable source (after 2+ runs of dead
  search-indexed links), yielding a strong new `[SEATTLE]` pick.
- Tags: **1 `[ENERGY]`** match (Crusoe Energy, Bellevue — 2nd consecutive
  run this req has been live) and **4 `[SEATTLE]`** matches (Stripe,
  Cloudflare, F5, Nordstrom), one of which (Crusoe) is dual-tagged.
- **3 strong candidates found but not shipped** due to unverifiable
  eligibility gates — 2 Leidos reqs (US citizenship / secret clearance)
  and 1 Zscaler req (US citizenship) — flagged below rather than silently
  dropped or shipped unverified.

## Top picks (5)

1. **Site Reliability Engineer, Infrastructure Platforms — AMER (Intermediate to Senior Staff)** — GitLab
   - Core SRE role building net-new Terraform modules and owning the full
     observability stack (metrics, logs, SLOs/SLIs) for GitLab's
     user-facing production systems — about as direct a match to the
     candidate's IaC + observability-ownership background as this run found.
   - Remote, US/Canada.

2. **Software Engineer - Platform Observability and Intelligence** — Fastly
   - Owns Fastly's own internal observability stack end-to-end, explicitly
     naming Terraform, Ansible, Prometheus, Grafana, Splunk, Datadog, and
     OpenTelemetry — the single strongest stack-breadth match in this run.
   - NYC/SF listed, hybrid/remote-US candidates considered.

3. **Senior Specialist Solution Architect** — Red Hat
   - Builds automation with Red Hat Ansible Automation Platform + Terraform,
     plus OpenShift Service Mesh observability (mTLS, canary deploys) — a
     direct hit on the Ansible/Terraform/observability profile from a
     flagship Linux vendor. JD states "telecommuting role to be performed
     anywhere in the U.S."

4. **Sr Engineering Manager – Network Infrastructure (Hybrid - Seattle)** — Nordstrom Tech `[SEATTLE]`
   - Network-infrastructure automation role explicitly naming
     Ansible/Terraform/NAPALM IaC tooling plus Datadog/Splunk/New Relic
     monitoring and "observability and monitoring practices" — found via a
     direct site crawl after Nordstrom's ATS was undiscoverable in prior runs.
   - Hybrid, Seattle WA (1600 7th Avenue).

5. **Senior Security Engineer** — SmarterDx
   - Direct SIEM/detection-engineering ownership (runs Panther SIEM) plus
     cloud security tooling (AWS GuardDuty, Wiz) on a Terraform-managed AWS
     stack — the cleanest SIEM-angle match this run.
   - Remote, United States.

## Full shortlist (15)

- **Staff Forward Deployed Engineer** — GitLab
  - **Location**: Remote, US
  - **Stack match**: Linux, Terraform, observability
  - **Why it fits**: JD explicitly lists "Linux, networking, observability, and performance analysis" plus Terraform and GitLab CI/CD.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8512432002
  - **Source / Verified via**: Greenhouse JSON API + WebFetch — full JD returned (2026-10-12)

- **Site Reliability Engineer, Infrastructure Platforms — AMER (Intermediate to Senior Staff)** — GitLab — TOP PICK
  - **Location**: Remote, US/Canada (candidates must be based in the US or Canada)
  - **Stack match**: Terraform, observability (metrics/logs/SLOs)
  - **Why it fits**: Builds net-new Terraform modules and owns production reliability/observability at scale.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8623389002
  - **Source / Verified via**: Re-confirmed live via WebFetch, Step 6 spot-check (2026-10-12) + Greenhouse JSON API

- **Senior Platform Engineer, GitLab Orbit** — GitLab
  - **Location**: Remote, Canada; Remote, US
  - **Stack match**: Terraform, observability
  - **Why it fits**: Owns deployment, monitoring, and ops of a distributed platform (Kubernetes/Helm/Terraform) with an explicit observability/incident-readiness mandate.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8771527002
  - **Source / Verified via**: Greenhouse JSON API + WebFetch — full JD returned (2026-10-12)

- **Staff Software Engineer, Deployment Platform** — Stripe `[SEATTLE]`
  - **Location**: Seattle (onsite)
  - **Stack match**: Terraform, observability
  - **Why it fits**: Builds IaC-at-scale deployment-platform tooling with observability integration.
  - **Apply link**: https://job-boards.greenhouse.io/stripe/jobs/8038771
  - **Source / Verified via**: Verified via Greenhouse JSON API (2026-10-12) — this URL 302-redirects to stripe.com's job-search page since stripe.com is proxy-egress-blocked in this environment; the Greenhouse JSON record is the confirmed-live source of truth.

- **Senior Infrastructure Engineer, Storage Platform** — Cloudflare `[SEATTLE]`
  - **Location**: In-office — one of Austin TX / London UK / Seattle WA
  - **Stack match**: Terraform, observability (Prometheus/Grafana)
  - **Why it fits**: Fleet lifecycle automation and production observability for object-storage clusters.
  - **Apply link**: https://job-boards.greenhouse.io/cloudflare/jobs/7629805
  - **Source / Verified via**: WebFetch — full JD returned, STATUS=LIVE (2026-10-12)

- **Senior Engineer - Cloud and Container Services** — Fastly
  - **Location**: Denver, CO / NYC / SF; JD states it may consider remote candidates within the US, UK, or Canada
  - **Stack match**: Terraform, observability (Datadog/Grafana/Prometheus)
  - **Why it fits**: CNCF-space infra engineering with explicit Terraform and Prometheus/Datadog/Grafana monitoring ownership.
  - **Apply link**: https://www.fastly.com/about/jobs/apply?gh_jid=8226276
  - **Source / Verified via**: Verified via Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/fastly/jobs/8226276` (2026-10-12). fastly.com itself is egress-blocked in this environment (DNS failure on direct WebFetch, re-confirmed on spot-check).

- **Software Engineer - Platform Observability and Intelligence** — Fastly — TOP PICK
  - **Location**: NYC / SF; JD states it is open to hybrid and remote work locations and may consider remote candidates within the US
  - **Stack match**: Terraform, Ansible, observability (Prometheus/Grafana/Splunk/Datadog/OpenTelemetry)
  - **Why it fits**: Owns Fastly's own internal observability stack end-to-end with Terraform/Ansible/Chef IaC.
  - **Apply link**: https://www.fastly.com/about/jobs/apply?gh_jid=8256238
  - **Source / Verified via**: Verified via Greenhouse JSON API, re-confirmed by main-thread curl re-fetch (`boards-api.greenhouse.io/v1/boards/fastly/jobs/8256238?questions=true`, HTTP 200, 2026-10-12). fastly.com domain itself egress-blocked.

- **Senior Specialist Solution Architect** — Red Hat — TOP PICK
  - **Location**: "Telecommuting role to be performed anywhere in the U.S." (listed office: Raleigh, NC)
  - **Stack match**: Ansible (Red Hat Ansible Automation Platform), Terraform, observability (OpenShift Service Mesh — mTLS, canary deploys)
  - **Why it fits**: Builds automation using Ansible AAP + Terraform + Service Mesh observability — a direct hit on the candidate's core tool set.
  - **Apply link**: https://redhat.wd5.myworkdayjobs.com/Jobs/job/Raleigh/Senior-Specialist-Solution-Architect_R-059619
  - **Source / Verified via**: Verified via Workday JSON API, re-confirmed by main-thread curl re-fetch (2026-10-12). WebFetch renders an empty client-side SPA shell on this Workday tenant (known limitation).

- **Sr. Software Engineer, Infrastructure (Remote)** — CrowdStrike
  - **Location**: USA - Remote
  - **Stack match**: Terraform, observability (Prometheus/Grafana/Alertmanager)
  - **Why it fits**: Infrastructure engineering with Terraform/Pulumi IaC and Prometheus/Alertmanager/Grafana monitoring ownership.
  - **Apply link**: https://crowdstrike.wd5.myworkdayjobs.com/crowdstrikecareers/job/USA---Remote/Sr-Software-Engineer--Infrastructure--Remote-_R30377-1
  - **Source / Verified via**: Verified via Workday JSON API — full JD returned (2026-10-12). WebFetch renders empty SPA shell (known Workday limitation).

- **Principal Engineer, Networking (Remote)** — CrowdStrike
  - **Location**: USA - Remote
  - **Stack match**: Terraform, Ansible, telemetry/log pipelines
  - **Why it fits**: Sets direction for network automation/IaC (Terraform, Ansible, GitOps) and telemetry/analytics strategy.
  - **Apply link**: https://crowdstrike.wd5.myworkdayjobs.com/crowdstrikecareers/job/USA---Remote/Principal-Engineer--Networking--Remote-_R30382
  - **Source / Verified via**: Verified via Workday JSON API — full JD returned (2026-10-12).

- **Site Reliability Engineer** — F5 Networks `[SEATTLE]`
  - **Location**: Seattle, Hybrid
  - **Stack match**: Terraform, observability (Prometheus/Grafana)
  - **Why it fits**: SRE role naming Terraform + Prometheus/Grafana, hybrid in Seattle — replaces the previously-tracked req RP1038142, now confirmed closed.
  - **Apply link**: https://ffive.wd5.myworkdayjobs.com/f5jobs/job/Seattle/Site-Reliability-Engineer_RP1038966
  - **Source / Verified via**: Verified via Workday JSON API — full JD returned (2026-10-12). WebFetch renders empty SPA shell.

- **Sr Engineering Manager – Network Infrastructure (Hybrid - Seattle)** — Nordstrom Tech `[SEATTLE]` — TOP PICK
  - **Location**: Hybrid, Seattle WA (1600 7th Avenue)
  - **Stack match**: Ansible, Terraform, observability/SIEM-adjacent (Datadog, Splunk, New Relic)
  - **Why it fits**: Network-infrastructure automation role naming Ansible/Terraform/NAPALM IaC plus Datadog/Splunk/New Relic monitoring and explicit "observability and monitoring practices" language.
  - **Apply link**: https://careers.nordstrom.com/sr-engineering-manager-network-infrastructure-hybrid-seattle/job/3BA5007ABE9964372C9C59203D511185
  - **Source / Verified via**: Re-confirmed live via WebFetch, Step 6 spot-check (2026-10-12) — direct crawl of careers.nordstrom.com (no ATS API found; custom careers site)

- **Sr. Cloud Support Engineer - Weekend Shift** — Crusoe Energy `[ENERGY]` `[SEATTLE]`
  - **Location**: Bellevue, WA (onsite, weekend shift)
  - **Stack match**: Terraform, Grafana (observability), Linux CLI, Kubernetes
  - **Why it fits**: Linux CLI + Terraform/IaC + Grafana observability ownership in an incident-response/SRE-adjacent role at an energy/AI-infra crossover employer; Bellevue is in commute range. 2nd consecutive run this exact req has been live.
  - **Apply link**: https://jobs.ashbyhq.com/Crusoe/43f1edf3-8459-4573-87db-9f00293e3118
  - **Source / Verified via**: Verified via Ashby JSON API — `api.ashbyhq.com/posting-api/job-board/Crusoe` (2026-10-12). WebFetch renders title only (empty SPA) — inconclusive by itself, confirmed via API per Step 3.5 fallback.

- **Senior Security Engineer** — SmarterDx — TOP PICK
  - **Location**: Remote (United States)
  - **Stack match**: Terraform, SIEM (Panther), AWS GuardDuty, Wiz
  - **Why it fits**: Direct SIEM/detection-engineering ownership plus cloud security tooling and Terraform — the cleanest SIEM-angle match this run.
  - **Apply link**: https://job-boards.greenhouse.io/smarterdx/jobs/5204868007
  - **Source / Verified via**: Re-confirmed live via WebFetch, Step 6 spot-check (2026-10-12)

- **Senior Site Reliability Engineer** — Garner Health
  - **Location**: Remote (HQ New York City; occasional HQ travel)
  - **Stack match**: Terraform, Datadog
  - **Why it fits**: SRE/platform role with Terraform-driven IaC and Datadog observability ownership.
  - **Apply link**: https://job-boards.greenhouse.io/garnerhealth/jobs/6180042004
  - **Source / Verified via**: WebFetch — full JD returned, STATUS=LIVE (2026-10-12)

## Flagged — not shipped (pass all 3 filters, unverifiable eligibility gate)

- **Cloud Architect/Engineer** — Leidos `[ENERGY]` — Remote, US — Terraform/Ansible/Datadog/Grafana all named, but JD requires **US citizenship** and a public-trust clearance. https://leidos.wd5.myworkdayjobs.com/en-US/External/job/Remote-US/Cloud-Architect-Engineer_R-00192064
- **DevSecOps Engineer – Intelligent Platforms & Agents** — Leidos `[ENERGY]` — Remote/Teleworker, US — Terraform + compliance-as-code named, but JD requires an active **secret clearance**. https://leidos.wd5.myworkdayjobs.com/en-US/External/job/6314-RemoteTeleworker-US/DevSecOps-Engineer---Intelligent-Platforms---Agents_R-00192493
- **Staff Site Reliability Engineer (Production Engineer) – Federal** — Zscaler `[SEATTLE]` — Bellevue WA (one of 9 eligible offices) — Ansible named, but JD requires **US citizenship** "due to the nature of assigned customers." Unchanged from the 2026-10-05 flag; a fresh full-board sweep found no substitute non-gated role. https://job-boards.greenhouse.io/zscaler/jobs/5029669007

## Dropped in curation (passed filters + validation, cut for weak fit or redundancy)

- GitLab — Director of Engineering, Database Excellence (Terraform/observability listed only as "a plus," not a requirement; manager-track)
- GitLab — Senior CX Platform Engineer (genuine match but redundant with 3 stronger GitLab picks above)
- Wiz — Senior Partner Solutions Architect – GSI (partner/pre-sales facing, not hands-on ops)
- Elastic — Agentic AI Engineer (tangential AI/ML infra role; no security/SIEM angle)
- Reddit — Senior Staff Machine Learning Engineer, GenAI Platform (ML-platform role; no security/SIEM angle)
- Cloudflare — Senior Software Engineer, Distributed Databases (same stack/offices as the shortlisted Storage Platform role — redundant)
- CrowdStrike — Principal Engineer - Network (Remote), CA-specific req (near-duplicate JD of the shortlisted Networking req, different req ID only)
- Garner Health — Staff Security Engineer (genuine match but redundant with the shortlisted Garner Health SRE role from the same employer)

## Sources & method

**Three-must-have filter** (all required): (1) Terraform and/or Ansible explicitly named; (2) SIEM/SOAR/detection-engineering/log-telemetry/observability-ownership or a named tool (Datadog/Splunk/Elastic/Grafana/etc.); (3) US-remote eligible, or onsite/hybrid in Greater Seattle. Criteria per `resources/sources.md`, unchanged since 2026-10-05.

**Sources queried** (via three parallel collection passes, each doing its own Step 3.5 live-URL validation):

- *Cloud-native + Seattle-majors*: GitLab, Wiz, Stripe, Cloudflare, Datadog, Reddit, Elastic, Grafana Labs, Honeycomb, Fastly, GitHub (blocked), Red Hat, Canonical, SUSE, CrowdStrike, Snyk, Sysdig, Tenable, Palo Alto Networks, Shopify (no ATS found), DuckDuckGo, Amazon (blocked), Microsoft (blocked), F5 Networks, T-Mobile (blocked), Nordstrom Tech, Workiva (unresolved 422, 3rd run).
- *Energy sector*: Octopus Energy/Kraken, Crusoe Energy, Hut8, Sunnova, Enphase (blocked), Sunrun, ChargePoint (blocked), EVgo (blocked), Constellation/NextEra (blocked), Duke Energy, Exelon (blocked), Schneider Electric (blocked), Siemens Energy (blocked), Arcadia (confirmed gone), David Energy (blocked), Tesla Energy (403), Leidos, Palantir.
- *LinkedIn + follow-up leads*: LinkedIn search (zero direct URLs — indexing gap persists, 3rd+ consecutive run), SmarterDx, Garner Health, Paxos, BlackCloak, Aalyria (new ATS found: Rippling, blocked), DigitalOcean (ATS still unknown — ruled out Greenhouse/Lever/Ashby), Epic Games (Avature now blocked, no live req found), Zscaler, Qlik (blocked), Experian (blocked).

Every apply URL on this report was validated live on 2026-10-12 via WebFetch, with ATS JSON API fallback (Greenhouse/Lever/Ashby/Workday) where WebFetch returned an empty SPA shell or a blocked domain — see "Verified via" field per role above. Full validation detail, source coverage, and API call logs are in `logs/job-market-scan-2026-10-12.json`.

Aggregator/mirror links (LinkedIn, Built In, Himalayas, TheMuse, etc.) were used only to discover leads, never as the shipped apply link — every shortlisted role resolves to the employer's own ATS or careers site.
