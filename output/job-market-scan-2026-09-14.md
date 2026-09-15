# Job Market Scan — 2026-09-14

## Summary

- **~45 raw hits** collected across 3 source groups (7 energy, ~24 cloud-native/Seattle-majors incl. ad-hoc board scans, 14 LinkedIn).
- **7 roles survived filtering + live validation** — below the 10–15 target, but a real improvement over 2026-09-09 (1 role) and 2026-09-10 (3 roles). Per the workflow's rule, the shortfall is surfaced honestly rather than padded with unverified links.
- **Major new blocker this run**: this session's network egress policy hard-blocks an unusually large set of major-employer domains entirely (`careers.homedepot.com`, `careers.t-mobile.com`, `careers.nordstrom.com`, `jobs.paloaltonetworks.com`, `www.splunk.com`, `www.shopify.com`, `www.tesla.com`, `careers.sunrun.com`, `www.se.com`, `jobs.jobvite.com`) — confirmed via both WebFetch and raw curl (`connect_rejected`, gateway 403 on CONNECT). This is a session/environment restriction, not a dead-link finding, and it forced **7 otherwise-plausible candidates to be dropped as unvalidatable** rather than shipped unverified (Home Depot SIEM/EDR Cybersecurity Engineer II, T-Mobile Software Reliability Engineer, Nordstrom Senior Network Engineer, 3× Palo Alto Networks SRE roles, Splunk SRE FedRAMP, Shopify SRE, Tesla Energy, Sunrun, Schneider Electric, Uplight, EVgo ×2). See "Notes for the workflow" below — this needs a decision before next run.
- **[ENERGY]**: 1 of 7. **[SEATTLE]**: 0 of 7 (several Seattle-area candidates existed but sat on blocked domains — see above).
- Top recurring stack overlap: Terraform named in all 7; Ansible confirmed in 3 of 7; observability/security-tooling angle present in all 7.

## Top picks (4 of 7)

- **Sr Engineer, SRE TechOps CICD (Remote)** — CrowdStrike
  Strongest stack match in the batch — Terraform, Ansible, Chef, Puppet, Datadog, Splunk, and observability all explicitly named in the live JD. Direct hit on the candidate's Linux/IaC/telemetry-pipeline background.
- **OpenShift Infrastructure - Senior Consultant** — Red Hat
  Terraform, Ansible, Splunk, and security/observability language confirmed, plus deep RHEL/Linux bare-metal ownership — a near-exact match for the candidate's Linux Systems Engineer specialization.
- **Staff Infrastructure Security Engineer (USA)** — GitLab
  Terraform + Ansible confirmed; infrastructure-security ownership maps directly to the candidate's multi-cloud hardening/DevSecOps background. Repeat strong match from the 2026-09-10 run, still live.
- **Platform Engineer II** — Octopus Energy (Kraken Technologies) `[ENERGY]`
  Terraform, observability, and Datadog explicitly named at a grid-tech energy platform — strong SIEM/telemetry-pipeline overlap, and the only energy-sector role to survive this run's validation.

## Full shortlist

- **Sr Engineer, SRE TechOps CICD (Remote)** — CrowdStrike
  - **Location**: US-remote
  - **Stack match**: Terraform ✅ · Ansible ✅ · SIEM/observability ✅ (Datadog, Splunk, observability all named) · Python — not confirmed
  - **Why it fits**: CI/CD + SRE TechOps ownership with the full IaC/observability toolchain named is a direct line to the candidate's automated-infrastructure and telemetry-pipeline background.
  - **Apply link**: https://crowdstrike.wd5.myworkdayjobs.com/en-US/crowdstrikecareers/job/USA---Remote/Sr-Engineer--SRE-TechOps-CICD--Remote-_R29733
  - **Source**: Workday — CrowdStrike careers
  - **Verified via**: Workday JSON API — direct per-job fetch (`crowdstrike.wd5.myworkdayjobs.com/wday/cxs/.../job/.../_R29733`) (2026-09-14), title/location/full JD body confirmed live, Terraform/Ansible/observability/Splunk/Datadog/Chef/Puppet all present in body text

- **OpenShift Infrastructure - Senior Consultant** — Red Hat
  - **Location**: US-remote ("can be located anywhere in the U.S. within close proximity to an airport"; must reside in a state where Red Hat is registered to do business — no state exclusion identified that would block the candidate)
  - **Stack match**: Terraform ✅ · Ansible ✅ (strong proficiency required) · SIEM/observability ✅ (Splunk, logging, monitoring, security named) · Python — not confirmed
  - **Why it fits**: Bare-metal Linux (RHEL) provisioning, IaC (Terraform/Ansible), and infrastructure hardening/security language line up directly with the candidate's Linux Systems Engineer and multi-cloud hardening background.
  - **Apply link**: https://redhat.wd5.myworkdayjobs.com/Jobs/job/Remote-US-NC/OpenShift-Infrastructure---Senior-Consultant_R-052630
  - **Source**: Workday — Red Hat careers
  - **Verified via**: Workday JSON API — direct per-job fetch (`redhat.wd5.myworkdayjobs.com/wday/cxs/redhat/Jobs/job/...R-052630`) (2026-09-14), full JD body confirmed live, Terraform/Ansible/observability/Splunk/security all present in body text

- **Staff Infrastructure Security Engineer (USA)** — GitLab
  - **Location**: US-remote
  - **Stack match**: Terraform ✅ · Ansible ✅ · SIEM/observability — security-tooling clause (infrastructure security ownership) · Python — not confirmed
  - **Why it fits**: Infrastructure-security ownership + IaC tooling is a direct line to the candidate's multi-cloud hardening and DevSecOps background.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8769103002
  - **Source**: Greenhouse — GitLab careers
  - **Verified via**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/gitlab/jobs/8769103002` (2026-09-14), title/location/content confirmed live, Terraform + Ansible present in body text

- **Site Reliability Engineer, Infrastructure Platforms — AMER (Intermediate to Senior Staff)** — GitLab
  - **Location**: US-remote (also open to Canada)
  - **Stack match**: Terraform ✅ · Ansible ❌ (not named) · SIEM/observability ✅ (observability stack, metrics/logs/SLOs ownership) · Python — not confirmed
  - **Why it fits**: SRE ownership of infrastructure platforms with explicit Terraform and observability language matches the candidate's SRE/IaC profile.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8623389002
  - **Source**: Greenhouse — GitLab careers
  - **Verified via**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/gitlab/jobs/8623389002` (2026-09-14), re-confirmed live (also confirmed via WebFetch), Terraform + observability present in body text

- **Senior Platform Engineer, GitLab Orbit** — GitLab
  - **Location**: US-remote (also open to Canada)
  - **Stack match**: Terraform ✅ · Ansible ❌ (not named) · SIEM/observability ✅ (observability stack ownership) · Python — not confirmed
  - **Why it fits**: Platform engineering with named Terraform and observability ownership overlaps with the candidate's IaC/observability profile.
  - **Apply link**: https://job-boards.greenhouse.io/gitlab/jobs/8771527002
  - **Source**: Greenhouse — GitLab careers
  - **Verified via**: Greenhouse JSON API — `boards-api.greenhouse.io/v1/boards/gitlab/jobs/8771527002` (2026-09-14), title/location/content confirmed live, Terraform + observability present in body text

- **Platform Engineer II** — Octopus Energy (Kraken Technologies) `[ENERGY]`
  - **Location**: US-remote
  - **Stack match**: Terraform ✅ · Ansible ❌ (not named) · SIEM/observability ✅ (observability, Datadog explicitly named) · Python ✅
  - **Why it fits**: Grid-tech energy platform engineering with Terraform + Datadog/telemetry ownership overlaps directly with the candidate's SIEM/log-pipeline and multi-cloud hardening background.
  - **Apply link**: https://jobs.lever.co/octoenergy/e2a5dba5-53ec-4623-8b25-85efcfed3d19
  - **Source**: Lever — Octopus Energy / Kraken Technologies careers
  - **Verified via**: Lever JSON API — `api.lever.co/v0/postings/octoenergy` (2026-09-14), posting present in current live array, Terraform/observability/Datadog/Python confirmed in body text

- **Senior Engineer - Cloud (Sunnyvale, CA; US Remote)** — CrowdStrike
  - **Location**: Listed as Sunnyvale, CA with "US Remote" in the title; no explicit state-exclusion language found (weakest location confirmation of the seven — flagged for the candidate's own judgment)
  - **Stack match**: Terraform ✅ · Ansible ❌ (not named) · SIEM/observability — partial (security, telemetry, monitoring named; no SIEM/Splunk/Datadog specifically) · Python — not confirmed
  - **Why it fits**: Cloud infrastructure engineering with named Terraform and security/telemetry ownership; weaker fit than the other six but clears all three must-haves.
  - **Apply link**: https://crowdstrike.wd5.myworkdayjobs.com/en-US/crowdstrikecareers/job/USA---Sunnyvale-CA/Senior-Engineer---Cloud--Sunnyvale--CA--US-Remote-_R30109
  - **Source**: Workday — CrowdStrike careers
  - **Verified via**: Workday JSON API — direct per-job fetch (`crowdstrike.wd5.myworkdayjobs.com/wday/cxs/.../_R30109`) (2026-09-14), full JD body confirmed live, Terraform/security/telemetry/monitoring present in body text

## Roles found but dropped in validation (for the record)

| Role — Company | Reason dropped |
|---|---|
| Cybersecurity Engineer II \| SIEM and EDR (Remote) — Home Depot | Strong stack match per snippet (Ansible strongly preferred, Terraform, SIEM/EDR, Cortex XSIAM/Splunk/CrowdStrike) — but `careers.homedepot.com` is fully blocked by this session's network egress policy (`connect_rejected`, both WebFetch and curl); no ATS API fallback found. Inconclusive, not shipped. |
| Software Reliability Engineer — T-Mobile | Terraform/Ansible named per search snippet — but `careers.t-mobile.com` fully blocked by egress policy; no public ATS API. Inconclusive, not shipped. |
| Senior Network Engineer, Hybrid Seattle WA — Nordstrom `[SEATTLE]` | Python/Ansible/Terraform named per snippet — but `careers.nordstrom.com` fully blocked by egress policy; no public ATS API. Inconclusive, not shipped. |
| Senior Manager, SRE, Hybrid Seattle — Nordstrom `[SEATTLE]` | Same egress block as above; also manager-track, would have been excluded per the "skip pure manager" nice-to-have anyway. |
| Senior Site Reliability Engineer (Cortex); Senior Staff Site Reliability Engineer; Sr. Staff Engineer, Infrastructure Reliability (Chronosphere) — Palo Alto Networks (×3) | Cortex = strong SIEM/SOAR angle, Terraform named per snippets — but `jobs.paloaltonetworks.com` fully blocked by egress policy; no ATS API (custom platform). Inconclusive, not shipped. |
| Senior Site Reliability Engineer, FedRAMP Cloud Platform (Remote USA) — Splunk | Strong observability/SIEM-vendor fit — but `www.splunk.com` fully blocked by egress policy; no ATS API found. Inconclusive, not shipped. |
| Senior Site Reliability Engineer, Remote Americas (Hawaii) — Shopify | `www.shopify.com` fully blocked by egress policy; no ATS API found. Inconclusive, not shipped. |
| Staff Site Reliability Engineer, Energy Software — Tesla Energy `[ENERGY]` | `www.tesla.com` fully blocked by egress policy (3rd run in a row inaccessible — previously 403, now a hard connection-level block). No ATS API fallback. |
| Staff DevSecOps Engineer — Sunrun `[ENERGY]` | `careers.sunrun.com` fully blocked by egress policy. No ATS API fallback. |
| Expert/Senior Design Engineer, DevOps — Schneider Electric `[ENERGY]` | `www.se.com` fully blocked by egress policy. No ATS API fallback. |
| Senior Site Reliability Engineer — Uplight `[ENERGY]`; DevOps Engineer + Senior DevOps Engineer — EVgo `[ENERGY]` (×2) | All three hosted on `jobs.jobvite.com`, fully blocked by egress policy for both WebFetch and curl. No ATS API fallback. |
| Senior Site Reliability Engineer, Observability — Chainlink Labs | Ashby org slug for this employer could not be resolved via public API (tried `chainlink-labs`, `chainlink`, `chainlinklabs`, `Chainlink-Labs` — all 404) and the hosted `jobs.ashbyhq.com` job page rendered no extractable content via WebFetch (JS-rendered, empty). Inconclusive, dropped. |
| Staff Site Reliability Engineer, Platform Engineering — Paxos | Search-indexed Greenhouse ID (`joinpaxos/jobs/8289381002`) not present on any guessed board token (`paxos`, `joinpaxos`, `paxosinc`, `paxostrust` all 404) — board appears to no longer be public under Greenhouse. Dead/dropped. |
| Senior Site Reliability Engineer, Observability — Webflow | Search-indexed Greenhouse ID (`webflow/jobs/7909588`) confirmed absent from the current live board (24 jobs checked); no SRE/observability-titled role currently open in the US (only Argentina-remote infra/DevOps roles exist, which don't satisfy the US-remote criterion). Dead/dropped. |
| Sr. GovCloud Data Infrastructure Engineer (Remote) — CrowdStrike | Confirmed live via Workday API this run (per-job body now fetches successfully, unlike the 403/empty-SPA pattern from prior runs) — but no Terraform/Ansible named in the JD. Fails Linux+IaC filter. |
| Security Engineer (US Remote) — Stripe | Confirmed live via Greenhouse API — telemetry mentioned, but no Terraform/Ansible named. Fails Linux+IaC filter. |
| Staff Application Security Engineer — Datadog | Confirmed live via Greenhouse API — observability/detection/Datadog all named, but no Terraform/Ansible in JD; also remote eligibility limited to a specific list of East Coast states. Fails Linux+IaC filter. |
| AI Platform Engineer — Sysdig (×2, SF/Raleigh) | Confirmed live via Lever API — but role sits under Sales/Business Operations, no Terraform/Ansible named. Fails Linux+IaC filter. |
| Senior Systems Engineer — Cloudflare (Seattle hybrid) `[SEATTLE]` | Confirmed live via Greenhouse API — no Terraform/Ansible named. Fails Linux+IaC filter. |
| Senior Systems Engineer, IAM — Cloudflare (Austin hybrid) | Confirmed live, Terraform/observability present — but Austin-only, not remote and not Seattle-area. Fails geography filter. |
| Senior Site Reliability Engineer ×3, Site Reliability/Gitops Engineer ×2 — Canonical | Confirmed live (worldwide remote) — but consistent with prior runs, no Terraform/Ansible named anywhere. Fails Linux+IaC filter. |
| Cloud Security Engineer — Stripe (Seattle) `[SEATTLE]` | Confirmed live — Linux only, no Terraform/Ansible/SIEM named. Fails filters 1 & 2. |
| Senior Software Engineer II, LLM Observability — Honeycomb | Confirmed live — observability named but role is ML/SWE-flavored with no Terraform/Ansible. Fails Linux+IaC filter. |
| Senior Site Reliability Engineer, Ads — Reddit | Confirmed live via Greenhouse API, Remote US — but no Terraform/Ansible named. Fails Linux+IaC filter (consistent with 2026-09-10 finding). |
| Senior/Staff SRE — Semperis, Mozilla; Remote Sr/Principal DevOps-SRE — CyberCoders; Senior DevOps — Whip Media, Koverse, Formidable | LinkedIn-only, no direct ATS URL locatable this round — unvalidated, dropped rather than shipped on a LinkedIn link. |
| Senior Network Security Engineer — Home Depot | LinkedIn-only for this specific req; Home Depot's own career-page host is blocked anyway (see above) — dropped. |
| Senior Site Reliability Engineer (Bellevue, WA) — Bungie `[SEATTLE]` | LinkedIn-only; a live Greenhouse board exists for Bungie but the exact title/req could not be confidently matched this round — inconclusive, dropped. |
| DevOps Engineer — Arcadia; various — Hut8 (Greenhouse) | Search-indexed IDs confirmed dead (404 / board redirect, or absent from live board) at collection-time sanity check. |
| 3× Crusoe Energy roles | Two of five search-indexed IDs are live but retitled to onsite-only roles (SF, Dublin) with no Terraform/Ansible named; three others confirmed absent from the live Ashby board. All excluded. |
| Senior DevOps Architect – AWS — Sunnova; Senior Cloud Engineer – CI/CD — Duke Energy | Stale: neither role appears on the employer's live Greenhouse/Workday listing this run. |
| 5× Palantir roles (DC/NYC hybrid) | Confirmed live via Lever API — but hybrid DC/NYC only, not remote or Seattle-area. |
| Wiz, Fastly, Tenable, Grafana Labs, Elastic | Live SRE/security-engineer roles exist on these boards, but all are EU/UK/Australia/Israel-remote or non-US, not US-remote eligible. |
| GitHub, SUSE, Snyk, DuckDuckGo | No usable public ATS API found (Greenhouse/Lever/Ashby all 404 or placeholder-only for these orgs) and no qualifying role identified via other means this round. |
| Amazon, Microsoft, F5 Networks | No direct, current ATS URL with a specific job ID located this round (Amazon/Microsoft: no locatable direct link via search; F5: Workday tenant guesses returned 422). |
| Constellation Energy, NextEra Energy, Exelon | Workday tenant-name guesses did not resolve (422 Unprocessable Entity) — correct tenant slug not identified this round; revisit with a more targeted tenant-discovery approach next run. |

## Sources & method

- **Date run**: 2026-09-14
- **Sources queried**: `resources/sources.md` full list — energy-sector employers, cloud-native tech employers, Seattle-area majors (Amazon, Microsoft, F5, T-Mobile, Nordstrom), LinkedIn Jobs (remote + Seattle-area queries), plus ad-hoc direct Greenhouse/Lever/Ashby/Workday board scans for Datadog, GitHub, SUSE, Tenable, Snyk, Wiz, Sysdig, Fastly, Red Hat, Elastic, Grafana Labs, Stripe, Reddit, DuckDuckGo, Constellation/NextEra/Exelon (utility Workday tenants — not resolved this round)
- **Filter criteria applied**: Terraform and/or Ansible explicitly named · SIEM/observability/security-tooling angle named · US-remote eligible **or** onsite/hybrid in the Greater Seattle area
- **Validation method**: Greenhouse/Lever/Workday JSON APIs (worked reliably this run for all API-hosted candidates), WebFetch direct for non-API hosts where the domain was reachable (GitLab's Greenhouse page re-confirmed via WebFetch as a spot-check). A large set of custom-domain employer career sites were **entirely unreachable this run** due to a session-level network egress policy — see Summary and follow-ups.

## Notes for the workflow (Step 7 follow-ups)

- **Network egress policy is the dominant limiter this run, not dead links.** Roughly 10 otherwise-plausible candidates across multiple sectors (retail/security: Home Depot, T-Mobile, Nordstrom; security vendors: Palo Alto Networks, Splunk; e-commerce: Shopify; energy: Tesla, Sunrun, Schneider Electric, Uplight, EVgo via Jobvite) sat on domains this session's proxy rejects outright (`connect_rejected`, gateway 403 on CONNECT) for both WebFetch and curl — confirmed via `curl -sS $HTTPS_PROXY/__agentproxy/status`, which lists these as recent policy-denied relay failures, not transient errors. This is a materially different and larger-scale blocker than any prior run's per-host inconclusive findings (SPP, Leidos, CrowdStrike 403s). **Recommend flagging to whoever manages this environment's egress policy** — if these domains can be allowed, several strong candidates (esp. Home Depot's SIEM/EDR role and T-Mobile's Terraform/Ansible-named SRE role) would likely convert into validated shortlist entries next run.
- **GitLab remains the single most reliable source** — 3 of 7 shortlisted roles this run, all cleanly validated via Greenhouse API, with a consistent pattern of naming Terraform + observability across multiple open reqs. Worth keeping as a priority source.
- **CrowdStrike's Workday tenant is now fully checkable** — contrary to the 2026-09-09/09-10 finding that the per-job detail endpoint 403s, both `R29733` and `R30109` returned full JD bodies via direct per-job fetch this run (200, not 403). Recommend dropping the "CrowdStrike needs manual review" caveat from the workflow going forward and treating it as a normal Workday source.
- **Red Hat is a new strong source** — found via ad-hoc Workday tenant search (`redhat.wd5.myworkdayjobs.com`), not previously in `sources.md`'s explicit list beyond being named as a "Linux vendor." Recommend keeping Red Hat in the source list with a note to search its Workday tenant directly (`redhat`/`Jobs` site) rather than relying on stale search-indexed IDs (this run's search-indexed Red Hat ID, `R-055856`, was dead).
- **Chainlink Labs' Ashby board could not be resolved via public API** under any guessed org slug, and its hosted job page renders no extractable content via WebFetch — likely a fully client-side SPA. Not recommending for the source list until a working validation path is found.
- **Paxos and Webflow's specific SRE/observability postings are confirmed gone** — Paxos's Greenhouse board isn't resolvable under any guessed token at all (possible ATS migration), and Webflow's board is live but has no current US SRE/observability role. Worth a fresh look next run in case Paxos re-appears under a new board token.
- **Utility-sector Workday tenants (Constellation, NextEra, Exelon) still unresolved** — tenant-name guessing (`constellation`, `nexteraenergy`, `exeloncorp`, etc.) returned 422s rather than confirming or denying the role exists. This needs either a correct tenant slug (findable via one WebFetch to the employer's own careers page, if that domain isn't also blocked) or should be deprioritized if it keeps failing.
- Reviewed 2026-05-12 → 2026-09-14.
