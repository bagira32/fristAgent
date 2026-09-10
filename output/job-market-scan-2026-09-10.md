# Job Market Scan — 2026-09-10

## Summary

- **First run under the updated filter criteria** (Seattle-area onsite/hybrid now qualifies without remote eligibility, per candidate's commute range).
- **~55 raw hits** collected across 3 source groups (18 energy, ~17 cloud-native/Seattle-majors, 20 LinkedIn — 8 of those Seattle-tagged).
- **3 roles survived filtering + live validation** — well short of the 10–15 target, but a real improvement over the 1-role yield on 2026-09-09. Per the workflow's rule, the shortfall is surfaced honestly rather than padded.
- **0 Seattle-area roles passed** despite real effort (Amazon, Boeing, Qualtrics, Microsoft, T-Mobile all checked): Amazon's Seattle security/IAM roles are live and security-relevant but don't name Terraform/Ansible; Boeing and Qualtrics postings were dead; Microsoft/T-Mobile had no locatable live direct-ATS URL. This looks like a real signal (big Seattle employers tend not to name specific IaC tools in JDs) rather than a validation artifact — worth revisiting with looser stack wording per the standing workflow note.
- **[ENERGY]**: 1 of 3. **[SEATTLE]**: 0 of 3.

## Top picks (3 of 3 — full shortlist)

- **Staff Security Engineer, Infrastructure Security** — GitLab
  Technical lead for infrastructure security on GitLab Dedicated for Government / FedRAMP — direct match for a DevSecOps/hardening background, and both Terraform and Ansible are explicitly named.
- **Site Reliability Engineer, Infrastructure Platforms — AMER** — GitLab
  Intermediate-to-Senior-Staff SRE role on infra platforms with explicit Terraform and observability ownership language.
- **Platform Engineer II** — Octopus Energy (Kraken Technologies) `[ENERGY]`
  Platform engineering at a grid-tech energy company with Terraform, observability, and Datadog explicitly named — strong SIEM/telemetry-pipeline overlap with the candidate's background.

## Full shortlist

- **Staff Security Engineer, Infrastructure Security** — GitLab
  - **Location**: US-remote
  - **Stack match**: Terraform ✅ · Ansible ✅ · SIEM/observability — security-tooling clause (FedRAMP, infrastructure security ownership) · Python — not confirmed
  - **Why it fits**: Infrastructure-security ownership + IaC tooling is a direct line to the candidate's multi-cloud hardening and DevSecOps background.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8769103002
  - **Source**: Greenhouse — GitLab careers
  - **Verified via**: Greenhouse JSON API — `api.greenhouse.io/v1/boards/gitlab/jobs/8769103002` (2026-09-10), title/location/content confirmed live

- **Site Reliability Engineer, Infrastructure Platforms — AMER (Intermediate to Senior Staff)** — GitLab
  - **Location**: US-remote (also open to Canada)
  - **Stack match**: Terraform ✅ · Ansible ❌ (not named) · SIEM/observability ✅ (observability ownership language) · Python — not confirmed
  - **Why it fits**: SRE ownership of infrastructure platforms with explicit Terraform and observability language matches the candidate's SRE/IaC profile.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8623389002
  - **Source**: Greenhouse — GitLab careers
  - **Verified via**: Greenhouse JSON API — `api.greenhouse.io/v1/boards/gitlab/jobs/8623389002` (2026-09-10), title/location/content confirmed live

- **Platform Engineer II** — Octopus Energy (Kraken Technologies) `[ENERGY]`
  - **Location**: US-remote
  - **Stack match**: Terraform ✅ · Ansible ❌ (not named) · SIEM/observability ✅ (observability, telemetry, Datadog explicitly named) · Python — not confirmed
  - **Why it fits**: Grid-tech energy platform engineering with Terraform + Datadog/telemetry ownership overlaps directly with the candidate's SIEM/log-pipeline and multi-cloud hardening background.
  - **Apply link**: https://jobs.lever.co/octoenergy/e2a5dba5-53ec-4623-8b25-85efcfed3d19
  - **Source**: Lever — Octopus Energy / Kraken Technologies careers
  - **Verified via**: Lever JSON API — `api.lever.co/v0/postings/octoenergy` (2026-09-10), posting present in current live array

## Roles found but dropped in validation (for the record)

| Role — Company | Reason dropped |
|---|---|
| 4× Leidos roles (Senior DevSecOps Engineer, Senior Multi-Cloud Engineer, Senior UNIX/Linux Sys Engineer, DevOps Engineer) — all Remote US, strong Terraform/Ansible stack signal per search snippet | `careers.leidos.com` returns 403 to automated fetch; Leidos doesn't run a public ATS API (not Greenhouse/Lever/Ashby/Workday) — no fallback available, inconclusive on both primary and fallback method |
| Staff SRE, Energy Software — Tesla Energy `[ENERGY]` | `tesla.com` returns 403 to automated fetch again (same as 2026-09-09 run); no ATS API fallback available |
| Senior DevOps Engineer — Schneider Electric `[ENERGY]` | `careers.se.com` returns 403; no ATS API fallback |
| Senior Site Reliability Engineer — Canonical | Confirmed live, fully remote — but neither Terraform nor Ansible named anywhere in the JD (repeat finding from 2026-09-09) — fails Linux+IaC filter |
| Systems Development Engineer, Foundational Security Services — Amazon `[SEATTLE]` | Confirmed live, Seattle WA — but neither Terraform nor Ansible named; role emphasizes IAM monitoring, not IaC tooling — fails Linux+IaC filter |
| Security Engineer, Platform Security — Amazon `[SEATTLE]` | Confirmed live, Seattle WA — same as above, no Terraform/Ansible named — fails Linux+IaC filter |
| Senior Site Reliability Engineer, Foundation — Qualtrics `[SEATTLE]` | Returns HTTP 410 Gone — dead |
| Senior Systems DevOps Developer — Boeing `[SEATTLE]` | Returns HTTP 404 — dead |
| DevOps Developer (Mid/Senior/Lead) — Boeing `[SEATTLE]` | Returns HTTP 404 — dead |
| Sr. Site Reliability Engineer - DBRE; SRE II - Observability — HashiCorp (x2) | Returned HTTP 429 "Vercel Security Checkpoint" on 2026-09-09; both now return HTTP 404 on direct re-check — dead/removed |
| Senior DevOps Engineer — Microsoft `[SEATTLE]`; Senior Full Stack DevOps Engineer — T-Mobile `[SEATTLE]` | No live direct-ATS URL locatable — Microsoft's careers site appears to have migrated ATS (old URLs 404/redirect to JS shell); T-Mobile posting looks ~1 year stale — inconclusive, dropped |
| Sr Engineer, SRE TechOps CICD (Remote); Sr. GovCloud Data Infrastructure Engineer (Remote) — CrowdStrike (x2) | Confirmed present in Workday's live listings-index search (title/location verified) but the JD body remains inaccessible — direct per-job fetch returns empty SPA render via WebFetch and `403 permission denied` via the documented Workday API fallback (same failure mode logged 2026-09-09) — live but stack-unconfirmed, dropped per the "don't treat 403 as pass" rule |
| Staff Software Engineer, Observability — Reddit | Confirmed live, Remote US, strong observability language (Grafana/Prometheus) — but neither Terraform nor Ansible named — fails Linux+IaC filter |
| Senior Site Reliability Engineer — Constellation Energy `[ENERGY]` | Workday tenant renders an empty SPA shell to WebFetch; no usable API fallback found this run — inconclusive |
| DevOps SRE - Senior or Lead (Remote Eligible) — Southwest Power Pool `[ENERGY]` | UltiPro job-board portal returns a browser-compatibility error page instead of content on direct fetch — dead/inaccessible via automation |
| Site Reliability Engineer — Twilio (Platform Engineering), Atlanta GA | No specific Greenhouse job ID locatable for this exact posting despite searching Twilio's live board — only unrelated/non-US postings found — inconclusive |
| Site Reliability Engineer — Lacework | No live ATS listing locatable under Lacework's name on Greenhouse/Lever — likely removed/renamed |
| Senior DevOps Engineer — Zendesk (US Remote) | No direct Greenhouse/Lever URL locatable despite searching — LinkedIn-only, unverifiable |
| Platform Engineer II — Octopus Energy, Houston TX `[ENERGY]` | Confirmed live via Lever API — but Houston is neither remote nor Seattle-area — fails geography filter |
| 3× Crusoe Energy roles, 5× Palantir roles (DC/NYC hybrid), 1× Hut 8 (Miami onsite) `[ENERGY]` | Confirmed live where checked — but none are remote or Seattle-area, and Hut 8 additionally lacks Terraform/Ansible/SIEM language |
| Cloud Platform Engineer — Epic; Senior SRE — Concentrix; DevOps Infra Engineer — Flexport; SRE — doxo (all `[SEATTLE]`, Bellevue/Seattle WA) | LinkedIn-only, no direct ATS URL found — unvalidated, dropped rather than shipped on a LinkedIn link |
| NS1, Lacework, Aha!, Platform Science, Formidable, ECO Tech, CyberCoders ×2 (remote-tagged) | LinkedIn-only with unconfirmed remote policy and/or no locatable direct ATS URL — dropped |
| F5 SRE Manager — Old Field, NY | Manager track, excluded per the "skip pure manager unless IC-track" nice-to-have |
| Sunrun, Enphase, Uplight, EVgo, David Energy, Arcadia, Tenable, F5 Networks (Seattle), Nordstrom, Shopify, GitHub, DuckDuckGo, Red Hat (Raleigh — not remote/Seattle), Palo Alto Networks Cortex (Santa Clara — not remote/Seattle) | Zero qualifying live hits after dead-link cross-check, or confirmed dead/removed job IDs — see Sources & method for the running "3-strikes" tally |

## Sources & method

- **Date run**: 2026-09-10
- **Sources queried**: `resources/sources.md` full list — energy-sector employers (including Southwest Power Pool, Leidos), cloud-native tech employers, Seattle-area majors added for this run (Amazon, Microsoft, F5, T-Mobile, Nordstrom), LinkedIn Jobs (remote query + new Seattle-area query)
- **Filter criteria applied**: Terraform and/or Ansible explicitly named · SIEM/observability/security-tooling angle named · US-remote eligible **or** onsite/hybrid in the Greater Seattle area (new as of 2026-09-10)
- **Validation method**: Greenhouse/Ashby/Lever JSON APIs where available, Workday listings-index search as a partial fallback, WebFetch direct otherwise, per workflow Step 3.5.

## Notes for the workflow (Step 7 follow-ups)

- **Leidos and Southwest Power Pool are not currently viable sources despite plausible-looking hits** — Leidos has no public ATS API and blocks WebFetch (403); SPP's UltiPro portal serves a browser-compatibility error page to automated fetch. Both were candidate additions from the 2026-09-09 run; recommend holding off on formally adding them to `sources.md` until a validation path exists, rather than promoting them on hit-count alone.
- **CrowdStrike's Workday tenant remains only partially checkable**: the listings-index search reliably confirms a job ID is live and returns its title/location, but the per-job detail endpoint still 403s and WebFetch still gets an empty SPA render — this is the second run in a row with this exact failure mode. If this profile is worth pursuing at CrowdStrike specifically, it likely needs a manual (human) check rather than further automation attempts.
- **HashiCorp's two postings flagged live-but-blocked on 2026-09-09 are confirmed dead now** — a useful data point that a 429/rate-limit response should not be assumed to mean "probably real," since both came back 404 a day later.
- **Seattle-area expansion needs a follow-up decision**: the big Seattle employers (Amazon, Microsoft) that would have the highest role volume tend not to name Terraform/Ansible specifically even in strong security/infra roles — internal tooling is common at that scale. Worth asking the candidate whether "IaC experience" language plus a named alternative tool (e.g. CloudFormation, Pulumi, Amazon's internal systems) should count for Seattle-area roles specifically, since the current filter may be systematically excluding a lot of realistic Seattle-area fits.
- Updated `resources/sources.md` 3-strikes tracking below.
