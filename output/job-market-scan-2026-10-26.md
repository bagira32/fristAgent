# Cloud / DevOps / SRE Job Market Scan — 2026-10-26

## Summary

- **~510 postings individually keyword-evaluated** (plus several thousand more scanned in bulk via board-level keyword grep — e.g. Cloudflare 451, Stripe 717, Datadog 426, Elastic 402, Okta 389, Zscaler 350, Crusoe 349, Palantir 309, Canonical 314, GitLab 239) across cloud-native tech, Seattle-area majors, energy-sector, and new-lead/aggregator sources.
- **17 roles passed all 3 locked filters and live-URL validation.** Curated down to **14 shipped** after cutting 3 for redundancy (a 4th GitLab security-adjacent req, a 3rd Okta req, and a 2nd Cloudflare req — all genuinely qualifying but duplicative of a stronger shortlisted pick from the same employer). **2 additional roles passed the 3 filters but were correctly excluded as citizenship/clearance-gated**: CrowdStrike's "Principal Engineer – Network" (requires US citizenship or Green Card) and Leidos's "Cloud Architect/Engineer" (requires US citizenship + Public Trust clearance).
- **1 `[ENERGY]` role** (Crusoe Energy, Bellevue WA — 4th consecutive confirmed-live run). **7 `[SEATTLE]`-tagged** onsite/hybrid roles.
- **4 new finds this run**: GitLab's "Cloud Platform Engineer", a 2nd distinct qualifying Wiz role (hands-on DevSecOps, separate from the recurring pre-sales req that keeps getting cut), and **Stripe's first-ever qualifying role in this scan's history** — a Seattle-based Staff Software Engineer role. A 4th, Cloudflare's "Senior Network Engineer" (also Seattle-eligible), passed filters but was cut in curation for redundancy — worth shipping next run if the shortlist has room.
- **Top recurring stack overlap:** Terraform named in all 14 shortlisted roles; a named observability/SIEM tool (Splunk, Datadog, Grafana, Prometheus, Panther, OpenTelemetry) in 12 of 14.

## Top picks (5)

**1. Software Engineer – Platform Observability and Intelligence — Fastly**
Hybrid/remote-eligible, NYC or SF preferred. Broadest stack match of the whole shortlist: Terraform, Ansible, Splunk, Datadog, Grafana, observability, and telemetry all named in one JD. Recurring pick, reconfirmed live again this run.

**2. Staff Site Reliability Engineer – Splunk — Okta `[SEATTLE]`**
Bellevue, WA (also Chicago/NYC/SF/DC). Owns and evolves Okta's Splunk ecosystem for observability at scale — about as direct a match to a SIEM/telemetry-pipeline background as this scan finds. Terraform, Splunk, Python, observability all explicitly named. Recurring pick.

**3. Production Engineer — Zscaler `[SEATTLE]`**
Hybrid, Bellevue, WA or Santa Clara/San Jose, CA (3 days/week). Near-literal match to the candidate's own profile line: hardening multi-cloud infrastructure (AWS, GCP, bare-metal) with Terraform + Ansible, and maturing observability (Prometheus, Grafana, OpenTelemetry). Reconfirmed clean — no citizenship/clearance gate in the JD. Recurring pick.

**4. Senior Security Engineer — SmarterDx**
Remote (United States). Runs Panther SIEM plus AWS GuardDuty/Wiz/Snyk/CrowdStrike investigation workflows — the strongest detection-engineering/DevSecOps alignment on the list. Terraform named for infra/network security work. Recurring pick.

**5. Security Engineer, Product & Production Infrastructure — Wiz**
Remote (USA). **New this run** — distinct from Wiz's recurring pre-sales req that has been cut 4+ consecutive runs for weak IC fit. This one is genuine hands-on DevSecOps engineering: Terraform/IaC + Python + detection-and-response ownership.

## Full shortlist (14)

- **Cloud Platform Engineer** — GitLab `[NEW]`
  - **Location**: Remote, US/Canada
  - **Stack match**: Terraform, Kubernetes, observability
  - **Why it fits**: Hands-on IaC + GitOps + observability platform ownership, a direct match to multi-cloud hardening work.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8889193002
  - **Source**: Verified via Greenhouse JSON API — GitLab careers (2026-10-26)

- **Site Reliability Engineer, Infrastructure Platforms — AMER** — GitLab
  - **Location**: Remote, US/Canada only
  - **Stack match**: Terraform, observability (metrics/logging/alerting/SLOs)
  - **Why it fits**: Core infra-platform SRE ownership role; GitLab is this scan's highest-tenure recurring source.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8623389002
  - **Source**: Verified via Greenhouse JSON API — GitLab careers

- **Senior Professional Services Technical Architect – Security** — GitLab
  - **Location**: Remote, US/Canada only
  - **Stack match**: Terraform, Ansible, named AppSec tooling (GitLab SAST/DAST/Dependency Scanning/Secret Detection, Snyk/Checkmarx/Veracode comparisons)
  - **Why it fits**: Explicit dual Terraform+Ansible IaC pairing plus a deep named-security-tooling angle.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8795736002
  - **Source**: Verified via Greenhouse JSON API — GitLab careers

- **Security Engineer, Product & Production Infrastructure** — Wiz `[NEW]`
  - **Location**: Remote (USA)
  - **Stack match**: Terraform/IaC, Python, detection and response
  - **Why it fits**: Hands-on DevSecOps engineering combining IaC ownership with detection/response; distinct from Wiz's recurring pre-sales req.
  - **Apply link**: https://job-boards.greenhouse.io/wizinc/jobs/4711762006
  - **Source**: Verified via Greenhouse JSON API — Wiz careers (wiz.io's own apply-page redirect has a known `:title` template bug; use the Greenhouse-hosted URL)

- **Staff Software Engineer, Deployment Platform** — Stripe `[SEATTLE][NEW]`
  - **Location**: Seattle, WA
  - **Stack match**: Terraform, observability
  - **Why it fits**: First-ever qualifying Stripe role found in this scan's history; deployment-platform ownership fits an IaC background directly.
  - **Apply link**: https://job-boards.greenhouse.io/stripe/jobs/8038771
  - **Source**: Verified via Greenhouse JSON API — Stripe careers (stripe.com itself is egress-blocked in this environment)

- **Senior Infrastructure Engineer, Storage Platform** — Cloudflare `[SEATTLE]`
  - **Location**: Onsite — one of Seattle, WA / Austin, TX / NYC / SF / London
  - **Stack match**: Terraform, Grafana, observability
  - **Why it fits**: Hands-on storage-platform infra engineering with IaC + observability ownership; recurring Seattle pick.
  - **Apply link**: https://job-boards.greenhouse.io/cloudflare/jobs/7629805
  - **Source**: Verified via Greenhouse JSON API — Cloudflare careers

- **Software Engineer – Platform Observability and Intelligence** — Fastly
  - **Location**: Hybrid/remote-eligible (preferred NYC or SF)
  - **Stack match**: Terraform, Ansible, Splunk, Datadog, Grafana, observability, telemetry
  - **Why it fits**: Broadest named-tool stack match on the shortlist; directly titled around observability.
  - **Apply link**: https://www.fastly.com/about/jobs/apply?gh_jid=8256238
  - **Source**: Verified via Greenhouse JSON API — Fastly careers (fastly.com itself egress-blocked)

- **Staff Site Reliability Engineer – Splunk** — Okta `[SEATTLE]`
  - **Location**: Bellevue, WA (hybrid; also Chicago/NYC/SF/Washington DC)
  - **Stack match**: Terraform, Python, Splunk, observability
  - **Why it fits**: Direct SIEM/observability-platform ownership role matching the candidate's telemetry-pipeline specialization.
  - **Apply link**: https://job-boards.greenhouse.io/okta/jobs/7658254
  - **Source**: Verified via Greenhouse JSON API — Okta careers (okta.com itself egress-blocked)

- **Senior Database Reliability Engineer (DBRE)** — Okta `[SEATTLE]`
  - **Location**: Bellevue, WA (hybrid; also other hub cities)
  - **Stack match**: Terraform, Ansible, Datadog, Grafana, Python
  - **Why it fits**: Rare explicit dual Terraform+Ansible pairing at a Seattle-area major with a full observability stack.
  - **Apply link**: https://job-boards.greenhouse.io/okta/jobs/7617976
  - **Source**: Verified via Greenhouse JSON API — Okta careers

- **Production Engineer** — Zscaler `[SEATTLE]`
  - **Location**: Hybrid, 3 days/week — Bellevue, WA or Santa Clara/San Jose, CA
  - **Stack match**: Linux, Terraform, Ansible, Prometheus, Grafana, OpenTelemetry (multi-cloud: AWS, GCP, bare-metal)
  - **Why it fits**: Near-literal match to the candidate's own specialization — hardening multi-cloud infrastructure with Terraform/Ansible and maturing observability/telemetry to reduce MTTM.
  - **Apply link**: https://job-boards.greenhouse.io/zscaler/jobs/5158936007
  - **Source**: Verified via Greenhouse JSON API — Zscaler careers; reconfirmed clean of any citizenship/clearance gate

- **Site Reliability Engineer** — F5 Networks `[SEATTLE]`
  - **Location**: Seattle, WA (hybrid)
  - **Stack match**: Terraform, Prometheus, Grafana, observability
  - **Why it fits**: Direct SRE role with a modern observability stack; 4th consecutive run confirmed live — a fully reliable recurring Seattle pick (req RP1038966).
  - **Apply link**: https://ffive.wd5.myworkdayjobs.com/f5jobs/job/Seattle/Site-Reliability-Engineer_RP1038966
  - **Source**: Verified via Workday JSON API — F5 careers (WebFetch renders an empty SPA shell)

- **Senior Cloud Support Engineer – Weekend Shift** — Crusoe Energy `[ENERGY][SEATTLE]`
  - **Location**: Bellevue, WA
  - **Stack match**: Terraform, Grafana
  - **Why it fits**: Energy-adjacent (AI/GPU-compute infrastructure) + commutable Seattle-area location; multi-cloud hardening background applies directly. 4th consecutive run confirmed live.
  - **Apply link**: https://jobs.ashbyhq.com/Crusoe/43f1edf3-8459-4573-87db-9f00293e3118
  - **Source**: Verified via Ashby JSON API — Crusoe Energy careers (jobs.ashbyhq.com renders an empty SPA)

- **Senior Security Engineer** — SmarterDx
  - **Location**: Remote (United States)
  - **Stack match**: Terraform, SIEM (Panther), security tooling (GuardDuty, Wiz, Snyk, CrowdStrike)
  - **Why it fits**: Strongest SIEM/detection-engineering and DevSecOps alignment found this run.
  - **Apply link**: https://job-boards.greenhouse.io/smarterdx/jobs/5204868007
  - **Source**: Verified via Greenhouse JSON API — SmarterDx careers

- **Senior Site Reliability Engineer** — Garner Health
  - **Location**: Remote (HQ in NYC)
  - **Stack match**: Terraform, Datadog, observability
  - **Why it fits**: SRE/platform role with explicit IaC + observability ownership matching the candidate's background.
  - **Apply link**: https://job-boards.greenhouse.io/garnerhealth/jobs/6180042004
  - **Source**: Verified via Greenhouse JSON API — Garner Health careers

## Sources & method

Scan date: 2026-10-26. Filters applied per `resources/sources.md` (locked): (1) Linux+IaC — Terraform and/or Ansible explicitly named; (2) observability/SIEM/security angle; (3) US-remote eligible OR onsite/hybrid in Greater Seattle. Every apply link above was validated live this run via the employer's ATS JSON API (Greenhouse/Ashby/Workday) per workflow Step 3.5 — no aggregator or search-snippet URL shipped.

**Sources queried**: GitLab, Wiz, Stripe†, Cloudflare, Fastly†, GitHub‡, Datadog, Elastic, Grafana Labs, Honeycomb, Reddit, DuckDuckGo, Red Hat, Canonical, SUSE, CrowdStrike, Snyk, Sysdig, Tenable, Palo Alto Networks, Shopify, Amazon‡, Microsoft‡, F5 Networks, T-Mobile‡, Nordstrom Tech, Workiva, Okta†, Zscaler, Octopus Energy/Kraken, Crusoe Energy, Hut8, Sunnova, Sunrun, Duke Energy, Siemens Energy‡, EVgo‡, Enphase‡, ChargePoint‡, Constellation Energy‡, NextEra Energy‡, David Energy‡, Exelon‡, Schneider Electric, Arcadia, Tesla Energy, Leidos, Palantir, SmarterDx, Garner Health, Paxos, BlackCloak, Aalyria/Rippling‡, DigitalOcean‡, Epic Games‡, Qlik‡, Experian‡, LinkedIn Jobs.
(† egress-blocked domain, validated via ATS JSON API instead; ‡ egress-blocked with no public ATS API reachable this run, could not validate.)

Full per-source coverage, every URL fetched, and every ATS API call made are recorded in `logs/job-market-scan-2026-10-26.json`.

**Cut for redundancy** (passed all 3 filters, live-validated, but cut in curation for being duplicative of a stronger shortlisted pick from the same employer): GitLab's "Staff Corporate Security Engineer" (8734888002 — redundant with the shortlisted PS Technical Architect – Security req's security-tooling angle); Okta's "Senior Site Reliability Engineer – EPG" (8268917 — redundant with the shortlisted Splunk and DBRE reqs); Cloudflare's "Senior Network Engineer" (7992903, also `[SEATTLE]`-eligible — redundant with the shortlisted Storage Platform req). Any of the three would be a reasonable swap-in next run if a shortlisted role goes stale.

**Flagged eligibility-gated, not shipped**: CrowdStrike's "Principal Engineer – Network (Remote)" (`R30292`) — Terraform+Ansible+telemetry all named, but the JD explicitly requires "US Citizenship or Green Card holder status"; this req had been shipped on prior runs' shortlists without that flag, now corrected. Leidos's "Cloud Architect/Engineer" (`R-00192064`, Remote US) — Terraform+Ansible+Datadog+observability all named, but requires US citizenship + Public Trust clearance. Neither is shipped without confirming the candidate's eligibility.

**Notable gaps**: Nordstrom Tech's careers site remains reachable (200), but the on-page keyword search still doesn't filter server-side and search-indexed job URLs continue to 404 — a full ~139-page crawl is needed to reliably surface a current qualifying role, which has now exceeded the time budget of 4+ consecutive runs. Octopus Energy/Kraken had zero DevOps/SRE/Infra-titled reqs for a 3rd consecutive run (173 postings, structurally non-technical board). Palantir and Paxos/BlackCloak hit a 5th consecutive non-qualifying run — the latter two have been formally demoted to spot-check-only this run per the 3-strikes convention (see `resources/sources.md`).
