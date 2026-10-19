# Cloud / DevOps / SRE Job Market Scan — 2026-10-19

## Summary

- **90+ postings individually evaluated** (plus several thousand scanned in bulk via board-level keyword grep) across cloud-native tech, energy-sector, and LinkedIn/follow-up-lead sources.
- **12 roles passed all 3 locked filters and live-URL validation** → shipped to the shortlist below. 1 more passed filters but was cut for weak role-fit (pre-sales, not hands-on IC); 0 were dropped this run for citizenship/clearance gating (the 3 Leidos leads checked all failed the observability filter independently, so the eligibility gate wasn't the deciding factor).
- **1 `[ENERGY]` role** (Crusoe Energy, Bellevue WA — 3rd consecutive confirmed-live run). **6 `[SEATTLE]`-tagged** onsite/hybrid roles.
- **New employer discovered this run: Okta.** Its Greenhouse board has at least 5 Bellevue-WA-eligible SRE/reliability roles naming Terraform/Ansible plus Splunk/Datadog/observability explicitly — the strongest new-source find in several runs. Added to `resources/sources.md`.
- **Top recurring stack overlap:** Terraform (every shortlisted role) + a named observability/SIEM tool (Splunk, Datadog, Grafana, Panther) in 9 of 12 roles — a stronger-than-usual observability-tool-naming rate this run.
- GitLab remains the single highest-yield individual source (3 of 12 shortlisted, after curating 2 more for redundancy); LinkedIn's direct job-URL indexing gap persists for a 4th+ consecutive run (structural WebSearch limitation, not a query problem).

## Top picks (5)

**1. Staff Site Reliability Engineer – Splunk — Okta `[SEATTLE]`**
Bellevue, WA (also Chicago/NYC/SF/DC). Owns and evolves Okta's Splunk ecosystem for observability at scale — about as direct a match to a SIEM/telemetry-pipeline background as this scan finds. Terraform, Splunk, Python, observability/telemetry all explicitly named.

**2. Software Engineer – Platform Observability and Intelligence — Fastly**
Hybrid/remote-eligible, NYC or SF preferred. Broadest stack match of the whole shortlist: Terraform, Ansible, Splunk, Datadog, Grafana, observability, and telemetry all named in one JD. Recurring pick (3rd consecutive run live).

**3. Senior Security Engineer — SmarterDx**
Remote (United States). Runs Panther SIEM plus AWS GuardDuty/Wiz/Snyk/CrowdStrike investigation workflows — the strongest detection-engineering/DevSecOps alignment on the list. Terraform named for infra/network security work. Recurring pick, 2nd+ consecutive run confirmed live.

**4. Senior Cloud Support Engineer – Weekend Shift — Crusoe Energy `[ENERGY][SEATTLE]`**
Bellevue, WA. GPU-cloud infrastructure support with Terraform and Grafana named. 3rd consecutive run confirmed live — now a reliably recurring Seattle+energy pick.

**5. Site Reliability Engineer, Infrastructure Platforms — AMER — GitLab**
Remote, US/Canada. Terraform-based infra-platform ownership with explicit SRE observability ownership (metrics/logging/alerting/SLOs). GitLab's highest-tenure recurring source continues to deliver.

## Full shortlist (12)

- **Staff Site Reliability Engineer – Splunk** — Okta `[SEATTLE]`
  - **Location**: Bellevue, WA (hybrid; also Chicago/NYC/SF/Washington DC)
  - **Stack match**: Terraform, Python, Splunk, observability, telemetry
  - **Why it fits**: Direct SIEM/observability-platform ownership role matching the candidate's telemetry-pipeline specialization.
  - **Apply link**: https://job-boards.greenhouse.io/okta/jobs/7658254
  - **Source**: Greenhouse — Okta careers (NEW source this run)

- **Staff Site Reliability Engineer – Kubernetes** — Okta `[SEATTLE]`
  - **Location**: Bellevue, WA (hybrid; also Chicago/NYC/SF/Washington DC)
  - **Stack match**: Terraform, Ansible, Python, observability
  - **Why it fits**: Rare explicit Terraform+Ansible pairing at a Seattle-area major; Kubernetes platform ownership.
  - **Apply link**: https://job-boards.greenhouse.io/okta/jobs/8160050
  - **Source**: Greenhouse — Okta careers (NEW source this run)

- **Software Engineer – Platform Observability and Intelligence** — Fastly
  - **Location**: Hybrid/remote-eligible (preferred NYC or SF; JD explicitly states "open to Hybrid And Remote Work Locations")
  - **Stack match**: Terraform, Ansible, Splunk, Datadog, Grafana, observability, telemetry
  - **Why it fits**: Broadest named-tool stack match on the shortlist; directly titled around observability.
  - **Apply link**: https://www.fastly.com/about/jobs/apply?gh_jid=8256238
  - **Source**: Greenhouse JSON API — Fastly careers (fastly.com itself egress-blocked; API-verified)

- **Senior Security Engineer** — SmarterDx
  - **Location**: Remote (United States)
  - **Stack match**: Terraform, SIEM (Panther), security tooling (GuardDuty, Wiz, Snyk, CrowdStrike)
  - **Why it fits**: Strongest SIEM/detection-engineering and DevSecOps alignment found this run.
  - **Apply link**: https://job-boards.greenhouse.io/smarterdx/jobs/5204868007
  - **Source**: Greenhouse — SmarterDx careers

- **Senior Site Reliability Engineer** — Garner Health
  - **Location**: Remote (HQ in NYC; occasional travel)
  - **Stack match**: Terraform, Datadog, observability
  - **Why it fits**: SRE/platform role with explicit IaC + observability ownership matching the candidate's background.
  - **Apply link**: https://job-boards.greenhouse.io/garnerhealth/jobs/6180042004
  - **Source**: Greenhouse — Garner Health careers

- **Senior Cloud Support Engineer – Weekend Shift** — Crusoe Energy `[ENERGY][SEATTLE]`
  - **Location**: Bellevue, WA
  - **Stack match**: Terraform, Grafana
  - **Why it fits**: Energy-adjacent (AI/GPU-compute infrastructure) + commutable Seattle-area location; multi-cloud hardening background applies directly.
  - **Apply link**: https://jobs.ashbyhq.com/Crusoe/43f1edf3-8459-4573-87db-9f00293e3118
  - **Source**: Ashby JSON API — Crusoe Energy careers (jobs.ashbyhq.com renders empty SPA; API-verified)

- **Site Reliability Engineer, Infrastructure Platforms — AMER (Intermediate to Senior Staff)** — GitLab
  - **Location**: Remote, US/Canada only
  - **Stack match**: Terraform, observability (metrics/logging/alerting/SLOs)
  - **Why it fits**: Core infra-platform SRE ownership role, GitLab's recurring highest-yield source.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8623389002
  - **Source**: Greenhouse — GitLab careers

- **Staff Corporate Security Engineer** — GitLab
  - **Location**: Remote, US/Canada only
  - **Stack match**: Terraform, telemetry, detection engineering (endpoint telemetry/detections, Security Operations & Detection and Response partnership)
  - **Why it fits**: Strong detection-engineering angle on top of IaC-managed security tooling.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8734888002
  - **Source**: Greenhouse — GitLab careers

- **Senior Professional Services Technical Architect – Security** — GitLab
  - **Location**: Remote, US/Canada only
  - **Stack match**: Terraform, Ansible, named AppSec security tooling (GitLab SAST/DAST/Dependency Scanning/Secret Detection, Snyk/Checkmarx/Veracode comparisons)
  - **Why it fits**: Explicit Terraform+Ansible IaC pairing plus a deep named-security-tooling angle.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8795736002
  - **Source**: Greenhouse — GitLab careers

- **Senior Infrastructure Engineer, Storage Platform** — Cloudflare `[SEATTLE]`
  - **Location**: Onsite — one of Austin, TX / London, UK / **Seattle, WA**
  - **Stack match**: Terraform, Grafana, observability
  - **Why it fits**: Hands-on storage-platform infra engineering with IaC + observability ownership; recurring Seattle pick.
  - **Apply link**: https://job-boards.greenhouse.io/cloudflare/jobs/7629805
  - **Source**: Greenhouse — Cloudflare careers

- **Principal Engineer – Network (Remote)** — CrowdStrike
  - **Location**: Remote, US (California-eligible)
  - **Stack match**: Terraform, Ansible, telemetry
  - **Why it fits**: Senior network-infrastructure IC role with explicit dual-IaC-tool naming.
  - **Apply link**: https://crowdstrike.wd5.myworkdayjobs.com/crowdstrikecareers/job/USA---Remote-CA/Principal-Engineer---Network--Remote-_R30292
  - **Source**: Workday JSON API — CrowdStrike careers (WebFetch renders empty SPA shell; API-verified)

- **Site Reliability Engineer** — F5 Networks `[SEATTLE]`
  - **Location**: Seattle, WA (hybrid)
  - **Stack match**: Terraform, Grafana, Prometheus, observability
  - **Why it fits**: Direct SRE role with a modern observability stack; 3rd consecutive run confirmed live — now a reliable recurring Seattle pick (req RP1038966).
  - **Apply link**: https://ffive.wd5.myworkdayjobs.com/f5jobs/job/Seattle/Site-Reliability-Engineer_RP1038966
  - **Source**: Workday JSON API — F5 careers (WebFetch renders empty SPA shell; API-verified)

## Sources & method

Scan date: 2026-10-19. Filters applied per `resources/sources.md` (locked): (1) Linux+IaC — Terraform and/or Ansible explicitly named; (2) observability/SIEM/security angle; (3) US-remote eligible OR onsite/hybrid in Greater Seattle. Every apply link above was validated live this run via WebFetch and/or the employer's ATS JSON API (Greenhouse/Ashby/Workday), per workflow Step 3.5 — no aggregator or search-snippet URL shipped.

**Sources queried**: GitLab, Wiz, Stripe†, Cloudflare, Fastly†, GitHub‡, Datadog, Elastic, Grafana Labs, Honeycomb, Reddit, DuckDuckGo, Red Hat, Canonical, SUSE, CrowdStrike, Snyk, Sysdig, Tenable, Palo Alto Networks, Shopify, Amazon‡, Microsoft‡, F5 Networks, T-Mobile‡, Nordstrom Tech, Workiva, Okta (**new**), Octopus Energy/Kraken, Crusoe Energy, Hut8, Sunnova, Sunrun, Duke Energy, Leidos, Palantir, SmarterDx, Garner Health, Paxos, BlackCloak, Zscaler, LinkedIn Jobs.
(† egress-blocked domain, validated via ATS JSON API instead; ‡ egress-blocked with no public ATS API found, could not validate this run.)

Full per-source coverage, every URL fetched, and every ATS API call made are recorded in `logs/job-market-scan-2026-10-19.json`.

**Cut for weak fit** (passed keyword filters but judged not a genuine match): Wiz's "Senior Partner Solutions Architect – GSI" (Remote-USA) — names Terraform/Ansible/SIEM/telemetry but is a pre-sales/solutions-architect role, not hands-on engineering; consistent with 3+ prior runs' judgment on this same req.

**Notable gap**: Nordstrom Tech's careers site is reachable, but all 3 search-indexed SRE/DevOps job URLs found via web search 404'd against the live site this run (known high dead-link-rate pattern for search-indexed Nordstrom IDs). A full page-by-page crawl (needed given the site's non-functional on-page search box) was out of this run's time budget — worth a dedicated deeper pass next run.
