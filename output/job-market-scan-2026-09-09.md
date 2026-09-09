# Job Market Scan — 2026-09-09

## Summary

- **Agent test run** of `workflows/job-market-scan.md`, executed end-to-end (collection → filter → URL validation → ranking → report).
- **60 raw hits** collected across all 4 source groups (9 energy, 30 cloud-native tech, 21 aggregators/LinkedIn).
- **After Step 3 filtering + Step 3.5 URL validation, only 1 role survived** as a verified, live, must-have-passing posting. This is far below the 10–15 target — per the workflow's explicit rule, the shortfall is being surfaced honestly rather than padded with unverified links.
- **Root cause**: most specific job-board URLs/IDs surfaced by web search (Greenhouse, Workday, Ashby) were dead, redirected to generic career hubs, or simply not present when checked against the ATS's own JSON API — even when posted only minutes earlier by the collection pass. Aggregators (RemoteOK, WeWorkRemotely, Wellfound) largely block direct fetch (403/410), and their mirrors of postings that *were* real had already gone stale by validation time (e.g. Close, Farmer's Dog).
- **Recommendation**: treat this as a workflow finding, not just a market finding — see "Notes for the workflow" below before relying on this recipe for a real weekly run.

## Top pick (1)

- **Senior Site Reliability Engineer** — Garner Health
  Owns reliability/performance/resilience of the cloud infra behind Garner's product and AI/ML workloads on the Platform Engineering team — direct fit for a Linux/IaC background with an SRE ownership mandate (SLOs, incident response, automation standards).

## Full shortlist (1 of 10–15 target)

- **Senior Site Reliability Engineer** — Garner Health
  - **Location**: US-remote (Greenhouse `location.name = "Remote"`, no state restriction stated)
  - **Stack match**: Terraform ✅ · Ansible ❌ (not named) · Python — not confirmed · SIEM/observability — ✅ (Datadog + general observability language) · Linux — implied by SRE/platform role, not separately confirmed
  - **Why it fits**: Direct SRE ownership of cloud reliability/SLOs/incident response maps closely to the candidate's SRE/DevSecOps background; Terraform + Datadog give partial IaC/observability confirmation (2 of 3 nice-to-haves).
  - **Apply link**: https://job-boards.greenhouse.io/garnerhealth/jobs/6180042004
  - **Source**: Greenhouse — Garner Health careers (found via Wellfound mirror, re-sourced to direct ATS per sourcing rule)
  - **Verified via**: Greenhouse JSON API — `api.greenhouse.io/v1/boards/garnerhealth/jobs/6180042004` (2026-09-09), title and content confirmed live and matching

## Roles found but dropped in validation (for the record)

| Role — Company | Reason dropped |
|---|---|
| Staff SRE, Ads — Reddit | Confirmed live via Greenhouse API, but location is San Francisco, CA (onsite) — fails US-remote filter |
| Senior Systems Engineer — Cloudflare | Confirmed live via Greenhouse API, but location is Hybrid (Atlanta/Austin/Denver/Seattle/DC) — fails US-remote filter |
| Site Reliability/GitOps Engineer — Canonical | Confirmed live, fully remote — but no Terraform/Ansible named anywhere in the JD (Prometheus/Grafana/Elasticsearch only) — fails Linux+IaC filter |
| Senior SRE, Environment Automation / Tenant Services — GitLab (x2) | Greenhouse API returns 404 on both job IDs — dead/removed |
| Platform InfraSec / Platform Productivity — Grafana Labs (x2) | Greenhouse API returns 404 on both job IDs — dead/removed |
| Senior SRE — Honeycomb | Greenhouse API returns 404 — dead/removed |
| Staff SRE, Energy Software — Tesla Energy | Both known URLs (`en_SA` locale and US variant) return HTTP 403 to automated fetch; other Tesla SRE/Energy Software listings found are Palo Alto or Amsterdam (onsite/relocation) — inconclusive, dropped |
| Senior SRE, AI Infra Engineer, SRE Cloud (Remote) — CrowdStrike (x3) | Workday SPA returns empty render to WebFetch; Workday's own `cxs` job API returns `403 permission denied` on direct job fetch and doesn't surface these req IDs via search — inconclusive on both primary and fallback method, dropped per validation rule |
| Senior Site Reliability Engineer — DuckDuckGo | WebFetch returns empty SPA shell; Ashby posting-api returns "Unauthorized" for the org slug — inconclusive, dropped |
| Site Reliability Engineer (Ashby) — Close | Ashby's current public job list for Close does not include this posting (and the Wellfound mirror had already gone 410) — dead |
| Senior Platform Engineer — The Farmer's Dog | Direct Greenhouse URL (found via search) returns 404 — dead |
| Senior DevOps Engineer — EVgo | Jobvite URL redirects to `search.jobvite.com/?invalid=1` — dead |
| Senior DevOps Engineer (Multiple Locations) — Schneider Electric | `careers.se.com` blocks automated fetch (403) — inconclusive, dropped |
| Senior DevSecOps Engineer — Hyperproof | Wellfound mirror returns 410; no live specific posting locatable on hyperproof.io — dropped |
| Site Reliability Engineer (SRE) — Wiz | wiz.io careers URL returns 404 — dead |
| DevOps SRE – Senior or Lead — Southwest Power Pool `[ENERGY]` | Career site's job board is a JS-rendered Ultipro portal that returns no content to automated fetch, and no specific posting URL could be located — inconclusive, dropped (strong stack fit per search snippet — Terraform, Docker/K8s, Unix/Linux expert — worth a manual look) |
| Senior Site Reliability Engineer II — Juniper Square | No direct ATS URL locatable | 
| Senior Infrastructure & Security Engineer — Bluebird Technologies | Only sourced via WeWorkRemotely (bot-blocks automated fetch); no independent employer-side confirmation | 
| Senior SRE — Chipcolate | Small/unclear company, only sourced via WeWorkRemotely and a staffing-marketplace mirror (CloudDevs); low confidence, not pursued further |
| Platform Engineer IAM / SRE US Gov roles — Palantir `[ENERGY]` | Hybrid/on-prem, Washington DC-based — fails US-remote filter |
| Platform Engineer, Product Reliability — Kraken Technologies `[ENERGY]` | Location is Japan — fails US-remote filter |
| Senior SRE (x2) — Elastic; Staff/Senior SRE Databases — Grafana Labs (x2) | Confirmed non-US locations (Greece; Germany/Canada) — fails US-remote filter |
| Senior SRE (Cortex) — Palo Alto Networks | URL resolves to the generic PANW careers landing page, not the specific posting — dead/moved |

## Sources & method

- **Date run**: 2026-09-09
- **Sources queried**: `resources/sources.md` full source list — energy-sector employers, cloud-native tech employers, RemoteOK/WeWorkRemotely/Wellfound aggregators, LinkedIn (per workflow Step 2 ordering)
- **Filter criteria applied** (must pass all 3, per `resources/sources.md`): Terraform and/or Ansible explicitly named · SIEM/observability/telemetry angle named · US-remote eligible with no disqualifying location restriction
- **Validation method**: Greenhouse/Ashby/Lever JSON APIs where available, WebFetch direct otherwise, per workflow Step 3.5. RemoteOK, WeWorkRemotely, and Wellfound largely returned 403/410 to both WebFetch and (for RemoteOK) WebSearch tag-page queries.

## Notes for the workflow (Step 7 follow-ups)

- **RemoteOK yielded zero usable hits this run** — tag-page searches (`remoteok.com/remote-sre-jobs` etc.) returned only "hire a freelancer" pages, not real postings. Worth re-checking whether RemoteOK's site structure changed, or dropping it from the source list.
- **WeWorkRemotely and Wellfound both block WebFetch** (403/410) — collection had to rely on WebSearch snippets alone for these, which is why several "hits" from these sources couldn't be independently re-verified.
- **A high proportion of Greenhouse/Workday/Ashby job IDs surfaced by WebSearch are stale or wrong** even on well-known company boards (GitLab, Grafana Labs, Honeycomb, Wiz, Close, The Farmer's Dog all 404'd). Search engines appear to be indexing/caching removed postings faster than the collection step can catch. **Recommend**: for any employer with a Greenhouse/Ashby board, cross-check the job ID against that employer's full current listing (`/v1/boards/<token>/jobs` or the Ashby job-board list) rather than trusting the specific job ID from a search snippet — i.e., push more of Step 3.5's validation logic earlier, into Step 2 collection itself.
- **CrowdStrike's Workday tenant actively blocks direct job-ID fetch** (`403 permission denied` even via the documented `cxs` API pattern) — the workflow's Workday fallback instructions may need a caveat that some Workday tenants require a live browser session/cookie that curl/WebFetch cannot obtain.
- Given the extremely low yield, recommend a **fresh, larger-scope scan** (more companies, possibly loosening the "explicit Terraform/Ansible" wording slightly, e.g. accepting "Terraform or equivalent IaC" if the JD names a specific tool even if not exactly those two) before treating this as representative of the actual current market.
