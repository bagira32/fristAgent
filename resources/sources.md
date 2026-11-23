# Job Hunt Sources & Filter Criteria

Reusable seed list for the **Cloud / DevOps / SRE — US-Remote or Seattle-area**
market scan.
Last reviewed: 2026-11-23.

## Candidate profile (anchors the filter)

Linux Systems Engineer · multi-cloud hardening · Terraform / Ansible · Python ·
SIEM / log pipelines · global-scale observability · DevSecOps.

**Work eligibility: US citizen.** Citizenship-, Green-Card-, Public-Trust- or
clearance-gated roles are **eligible and must be shipped** like any other role
(tag them `[US-CITIZEN]` / `[CLEARANCE]`). Holds no active clearance today, so a
role requiring an *active* clearance at hire still ships, tagged
`[CLEARANCE-ACTIVE]` with a one-line note. Never drop or demote a role for
citizenship/clearance language. (Rule added 2026-10-26 — earlier runs wrongly
excluded these "without confirming eligibility.")

## Locked filter criteria

A role must hit **ALL three** must-haves to make a shortlist:

1. **Linux + IaC** — Terraform and/or Ansible explicitly named in the JD.
2. **Observability / SIEM / security angle** — SIEM, SOAR, detection engineering,
   log/telemetry pipelines, or strong observability ownership.
3. **US-remote eligible, OR onsite/hybrid in the Seattle area** — either open to
   US-based remote applicants (no state exclusion blocking the candidate's
   location), or based in the Greater Seattle area — Seattle, Bellevue, Redmond,
   Kirkland, Renton, Tacoma, Everett, or listed generically as "Seattle, WA" /
   "Puget Sound." The candidate can commute to onsite/hybrid roles in this area,
   so remote eligibility is not required for them. A city restriction *outside*
   this area (e.g. "must be in Austin") still disqualifies a role.

Nice-to-have (boost a match but not required):

- Python in the stack
- Senior / Staff IC ladder (skip pure manager unless IC-track)
- Energy-sector employer → tag `[ENERGY]`

## Source list

### Energy-sector employers (check career pages directly)

- Octopus Energy / Kraken Technologies — `octopus.energy/careers`, `kraken.tech/careers`.
  **Update 2026-11-16: 6th consecutive structural-zero run** (163 postings, still
  zero DevOps/SRE/Infra titles) — recommend moving to monthly rather than weekly
  checks.
- Tesla Energy — `tesla.com/careers` (403 at the site level 4 consecutive runs, not a proxy issue)
- Sunrun, Sunnova (Greenhouse token `sunnova`, confirmed 2026-10-05, thin board), Enphase — solar/storage
- ChargePoint, EVgo — EV charging
- Constellation, NextEra, Duke Energy, Exelon — US utilities
- Schneider Electric, Siemens Energy — grid/industrial
- Arcadia, David Energy — energy-data platforms. **Arcadia's Greenhouse board
  (`arcadiacareers`) is confirmed stale/deactivated** (404s, job links redirect to
  `?error=true`) as of 2026-10-05.
- Crusoe Energy (Ashby org slug `Crusoe`) — energy/compute crossover.
  **Correction 2026-10-05: Crusoe's board is NOT fully onsite-only** — it now
  includes Remote-US and Bellevue, WA postings alongside the SF/Denver/Dublin
  onsite roles; worth checking Bellevue/Remote-US postings specifically each
  run. **Correction 2026-11-09: the long-tracked Bellevue "Sr. Cloud Support
  Engineer - Weekend Shift" req is confirmed closed.** Replacement pick found
  (SF-primary / Bellevue-secondary OnSite — note Crusoe's qualifying pattern is
  consistently "SF primary + Bellevue as one of several secondary locations,"
  not Bellevue-primary): **Senior Staff Automation Engineer**
  (`ab5a5395-5480-4731-9053-3906b0f92f23`, Terraform+Ansible+AWX+osquery,
  dedicated config-management/observability charter — re-check each run, still
  live and shipped as a top pick 2026-11-23). The alternate pick **Senior
  Production Engineer, Storage** (`fb0c1911-c752-49df-84ef-4ff5309e8590`) is
  **confirmed DIED as of 2026-11-23** — absent from the current 316-job board
  entirely by both ID and title search; stop tracking it. A new weaker-fit
  alternative surfaced 2026-11-23: **Senior Software Engineer, Platform
  Networking** (`d0a11984-9ed0-42e1-99af-e63113b3681c`, Bellevue WA secondary
  location, Terraform/Ansible only a nice-to-have, network telemetry — gNMI/
  gRPC/NETCONF — rather than security/observability telemetry) — held back,
  worth re-evaluating only if the Automation Engineer pick ever dies.

**Dropped 2026-11-23**: **Hut 8** (Greenhouse token `hut8`) — confirmed **zero
technical roles for a 3rd consecutive check** (board remains 100% Miami, FL
legal/finance/data-center-build; the previously-tracked "Highrise AI" remote
SRE/Infra/NOC postings never reappeared after going to zero 2026-11-16).
Formally removed from active rotation per the 3-strikes convention — spot-check
only if a specific new lead resurfaces via aggregator/LinkedIn.
- Palantir (energy / Foundry) — `palantir.com/careers`, Lever slug `palantir`.
  **Formalized 2026-11-09 as a reliable recurring Seattle source** — req
  `c38bb622-6f8e-43a1-8ae7-32291da328a8` ("Senior Software Engineer, Substrate",
  Seattle WA hybrid, Terraform+Ansible+K8s/observability) has now qualified for
  2 consecutive runs. Re-check this ID each run.
- Leidos (Workday tenant `leidos`, site `External`, confirmed 2026-10-05) — large
  volume of DevOps/SRE/Linux-Administrator titles, but all tied to clearance-required
  onsite locations (Bethesda, Chantilly, Norfolk, Fort Meade, Annapolis Junction,
  plus AU/UK sites) so far — worth a dedicated remote-facet search next run.
  **Update 2026-11-09**: new qualifying fully-remote pick found — req `R-00196252`
  ("Senior DevOps Engineer", Remote/Teleworker US, Terraform+Ansible+CloudFormation+
  Splunk/Grafana/Prometheus) — requires an *active* DoD Secret/Top-Secret clearance
  at hire, tag `[CLEARANCE-ACTIVE]` `[US-CITIZEN]`. Re-check this ID each run
  alongside the onsite clearance-site titles (which remain excluded under filter 3
  — no remote option, not Seattle-area — regardless of citizenship eligibility).
  **Correction 2026-11-16: req `R-00196252` is confirmed CLOSED** (404 on direct
  fetch, absent from 5 searchText sweeps). No qualifying remote-US replacement
  found this run; closest candidate `R-00193640` ("Cloud Infrastructure Engineer",
  Remote US) fails the observability/SIEM filter and is junior-level (1–3 yrs)
  besides. **Leidos has zero qualifying roles this run** — needs a fresh full
  remote-facet sweep next run.
  **Update 2026-11-23 — Leidos recovery**: a fresh full remote-facet sweep (6
  searchText variants against the Remote-US facet) found **3 new qualifying
  remote-US roles**, Leidos's best showing in several runs: `R-00196293`
  ("Senior Network Support Engineer Remote", Terraform+Ansible+Elastic+Grafana —
  weakest of the 3, held back this run for shortlist redundancy), `R-00197465`
  ("Cryptography & Security Infrastructure Engineer – Mid-Level", Terraform+
  Ansible+SIEM, shipped), and `R-00197276` ("Orchestration Application
  Performance Engineer – Mid", Terraform+Ansible+SIEM+telemetry+Splunk+Elastic,
  strongest match, shipped as a top pick). All three require an **active** DoD
  Secret clearance plus US citizenship at hire — tag `[CLEARANCE-ACTIVE]`
  `[US-CITIZEN]`. Re-check all 3 IDs each run going forward (R-00196252/
  R-00193640 can stop being re-checked — both superseded/dead).

**Dropped 2026-10-05 per the "3+ consecutive runs with no qualifying source"
convention**: Uplight, AutoGrid, GridX — 4th consecutive run with zero resolvable
ATS via token-guessing or web search. Do not keep budgeting automated-search time
on these three; rely on manual/LinkedIn spot-checks only if revisited.

### Cloud-native tech employers (senior Linux/SRE remote-friendly)

- Observability / data: Datadog, Elastic, Grafana Labs, Honeycomb. **HashiCorp has
  no standalone careers board as of this run** — folded into IBM's careers/Workday
  system following the Feb 2025 acquisition; would need IBM's own Workday tenant to
  search specifically. **Chronosphere also has no standalone board** — folded into
  Palo Alto Networks post-acquisition; no PANW reqs tagged Chronosphere found yet.
- Infra / edge: Cloudflare, Fastly, GitLab, GitHub. **Fastly's long-standing TOP
  PICK req `8256238` ("Software Engineer, Platform Observability and
  Intelligence") is confirmed CLOSED as of 2026-11-23** (404, absent from the
  live 48-job board) — it had been the single strongest stack match found in
  this scan's history (Terraform+Ansible+Datadog+Grafana+OTel+Prometheus+
  Splunk). No replacement of similar quality found; its 6 remaining Terraform/
  observability-matching reqs are all city-specific-onsite or international —
  needs a fresh discovery pass if revisited. **GitLab now has a 2nd genuine
  recurring-watch pick** (`8623389002`, "SRE, Infrastructure Platforms — AMER",
  found 2026-11-23, held back as redundant with the long-tracked
  `8889193002`). **Cloudflare's `8263016` ("Senior Software Engineer –
  Kubernetes platform") now carries a Remote-US location option** (as of
  2026-11-23, previously Hybrid/Distributed-only) — upgrades it to
  filter-qualifying, though still held back as redundant with the shipped
  Cloudflare Storage Platform pick (`7629805`).
- Linux vendors: Red Hat (Workday tenant `redhat.wd5.myworkdayjobs.com`, site `Jobs`
  — **correction 2026-11-16: formalized recurring pick `R-060309-1` is now
  confirmed CLOSED** (absent from both an ID-specific search and a broad
  terraform/ansible sweep, 6 results, none matching). **Update 2026-11-23**: a
  fresh full-board sweep (9 searchText variants) found a genuine new
  nationwide-US-remote lead, `R-060248` ("Site Reliability Engineer," nominal
  office Raleigh but "telecommuting role to be performed anywhere in the
  U.S.," Ansible + Linux + Kubernetes + Python + generically-named
  observability) — held back this run for quality (no Terraform named,
  entry/mid-level ~2 yrs experience, below the candidate's senior profile) but
  worth tracking as Red Hat's clearest live lead in 2 runs; re-check each run.
  Separately, `R-060411` reappeared retitled `R-060411-2` ("Senior Architect,
  OpenShift Infrastructure – Active TS/SCI Clearance", Remote US CO) — still
  **no SIEM/observability term anywhere** in the JD, still fails filter 2, not
  shippable on the merits regardless of the now-explicit active-clearance
  requirement.), Canonical (Greenhouse
  token `canonical` — confirmed reachable 2026-10-05, the 2026-09-28
  "egress-blocked" note was session-specific, not a persistent block), SUSE
- Security: CrowdStrike (**correction 2026-10-26: its long-tracked "Principal Engineer – Network (Remote)" req `R30292` explicitly requires "US Citizenship or Green Card holder status" in the JD body** — this had been shipped on prior runs' shortlists without an eligibility flag; tag `[US-CITIZEN]` and ship it — candidate is a US citizen, see Candidate profile. **Update 2026-11-23**: the per-job Workday detail endpoint returned a clean HTTP 200 this run, no 403 flake — treat as a normal reliable Workday source going forward), Wiz (apply via Greenhouse URLs — see note below), Sysdig (**correction 2026-11-16: the long-tracked "Director of Security Engineering" req is no longer even on the board** — 34 reqs now, down from 38, title absent entirely — stop tracking it),
  Tenable, Palo Alto Networks (Cortex; Workday tenant/site confirmed 2026-10-05:
  `paloaltonetworks.wd5.myworkdayjobs.com`/`panwexternalcareers`). **Snyk's board
  moved off Greenhouse to Ashby** (confirmed 2026-10-12) — org slug `snyk`,
  `api.ashbyhq.com/posting-api/job-board/snyk`, 22 reqs, 0 qualifying yet. The
  old Greenhouse token (`api.greenhouse.io`/`boards-api.greenhouse.io`/
  `job-boards.greenhouse.io`) still 404s cleanly — query the Ashby endpoint
  going forward instead of re-deriving from scratch.
- Product cos with strong SRE culture: Stripe (apply via Greenhouse URLs — stripe.com's
  own domain is proxy-blocked in this environment, see note below), Shopify (still
  no discoverable public ATS token after repeated guesses), Reddit, DuckDuckGo

**Wiz has a 2nd distinct qualifying role type, found 2026-10-26:** beyond the recurring "Senior Partner Solutions Architect – GSI" (pre-sales, repeatedly cut for weak IC fit), Wiz's board also has `4711762006` ("Security Engineer, Product & Production Infrastructure", Remote-USA) — genuine hands-on DevSecOps engineering (Terraform/IaC + Python + detection-and-response), shipped this run. Re-check this ID each run alongside the pre-sales req.

**Wiz apply-link bug (found 2026-10-05):** Wiz's own `wiz.io` apply-page redirect
target has a live template bug — the URL contains a literal unsubstituted `:title`
placeholder (e.g. `wiz.io/careers/job/<id>/:title?gh_jid=<id>`) and is blocked by
this session's egress proxy besides. Use the Greenhouse-hosted URL instead
(`job-boards.greenhouse.io/wizinc/jobs/<id>`) as the apply link on reports — it
resolves reliably and is the de facto canonical apply URL until Wiz fixes it.

**Stripe apply note:** `stripe.com` is egress-blocked in this session's proxy, so its
own apply pages can't be fetched directly. The Greenhouse-hosted redirect URL
(`job-boards.greenhouse.io/stripe/jobs/<id>`) is confirmed live via the Greenhouse
JSON API and is what should ship as the apply link.

**Stripe's first-ever qualifying Seattle-area role, found 2026-10-26:** `8038771`
("Staff Software Engineer, Deployment Platform", Seattle, WA — Terraform +
observability). Stripe had never previously yielded a qualifying role in this
scan's history. Per the 2nd-appearance convention, not yet fully formalized as a
routine Seattle source — re-check this specific ID next run before treating Stripe
as a reliable recurring Seattle pick.

### Seattle-area major employers (onsite/hybrid OK per commute-range filter, added 2026-09-10)

- **Okta** (Greenhouse, board token `okta`, no company-prefix needed — 385 reqs) — **NEW formalized source, 2026-10-19.** Large Bellevue, WA hybrid hub with at least 5 SRE/reliability reqs naming Terraform and/or Ansible plus Splunk/Datadog/Grafana/Prometheus observability explicitly — the strongest new-source find in several runs. **`okta.com` itself is egress-blocked (DNS ENOTFOUND)** — the Greenhouse redirect target 404s on direct domain fetch, same failure pattern as Stripe/Fastly; use the Greenhouse-hosted URL (`job-boards.greenhouse.io/okta/jobs/<id>`) as the apply link, verified via the Greenhouse JSON API (`boards-api.greenhouse.io/v1/boards/okta/jobs/<id>?content=true`). **Recurring reliable pick to recheck each run**: req `7617976` ("Senior Database Reliability Engineer", Terraform+Ansible+Datadog+Grafana). Also worth rechecking: `8268917` (Senior SRE - EPG), `7317857` (Senior Manager, SRE - Infrastructure Platform — manager-tier). Most Okta Seattle-area postings list Bellevue alongside Chicago/NYC/SF/DC as interchangeable hybrid options — confirm Bellevue is actually in the location list before shipping. **Correction 2026-10-26: req `8160050` ("Staff Site Reliability Engineer - Kubernetes") is now confirmed CLOSED** — absent from the current Greenhouse listing after 2 consecutive runs as a tracked recurring pick; drop it from the recurring-pick list. **Correction 2026-11-02: req `7658254` ("Staff Site Reliability Engineer - Splunk") had its JD changed/retitled to "Splunk Infrastructure Engineer" and no longer names Terraform/Ansible — drop it from the recurring-pick list.** **Correction 2026-11-02: the "possible new lead" `8064877` ("Staff Site Reliability Engineer (FedRAMP)") flagged on 2026-10-26 is confirmed to NOT exist** (clean 404 against Okta's current board) — it was a stale aggregator-indexed ID; do not re-add without a fresh live sighting. **Added 2026-11-09: a 2nd distinct Seattle-area recurring pick confirmed** — req `8268917` ("Senior Site Reliability Engineer - EPG", Bellevue WA/San Francisco CA, Terraform+Datadog/Splunk/Grafana) was independently found by two separate collection passes this run, a strong signal of fit. Both this req and `7617976` (DBRE) carry a US-Person/FedRAMP citizenship requirement — tag both `[US-CITIZEN]` going forward (previously only noted on one). **Added 2026-11-23: a 3rd distinct Seattle-area recurring pick found** — req `8385706` ("Staff Site Reliability Engineer", Bellevue WA, Go/Python/Terraform, Grafana/Splunk/PagerDuty, FedRAMP/CrowdStrike Falcon — same team as `8268917`) — held back this run as redundant with the shipped EPG pick, but worth tracking as a 3rd Okta recurring-watch candidate going forward.

- **Zscaler** (Greenhouse, board token `zscaler`, 377 reqs) — **both long-tracked
  recurring picks are now dead, confirmed 2026-11-16**: req `5158936007`
  ("Production Engineer", the Bellevue/San Jose `[SEATTLE]` pick) is 404'd off
  the board entirely, and req `5029669007` ("Staff SRE Federal") is still live
  but its JD now requires strict Santa Clara, CA 3-day-onsite with no
  Bellevue/remote language — it no longer passes filter 3. **Zscaler has zero
  qualifying roles as of this run** — needs a fresh full-board Terraform/Ansible
  sweep next run rather than re-checking these two dead IDs.
  **Update 2026-11-23**: fresh full-board sweep done — 388 reqs, 25 raw hits, all
  held back (manager-tier "Manager – AI & Data Platform Engineering" `5268021007`;
  Federal/clearance SRE reqs restricted to Virginia/Maryland-remote or Santa
  Clara-onsite only; remaining reqs international or onsite-only). **Zscaler has
  shipped zero for a 2nd consecutive run** — structural pattern, not a
  validation gap.

- Amazon (AWS), Microsoft, F5 Networks, T-Mobile, Nordstrom Tech — high role volume but
  JDs at this scale often don't name specific IaC tools (internal tooling common).
  F5's Workday tenant is `ffive.wd5.myworkdayjobs.com`, site `f5jobs` — the
  previously-tracked role RP1038142 is **confirmed CLOSED as of 2026-10-12**
  (0 results on an ID-specific search, 404 on direct fetch). Its successor as
  the recurring reliable Seattle pick is **RP1038966** ("Site Reliability
  Engineer": Terraform + Prometheus/Grafana, Seattle hybrid) — re-check this ID
  each run. A separate new Seattle-hybrid req, RP1038431 ("Security Engineer -
  Incident response"), has a strong SIEM/CrowdStrike-EDR angle but explicitly
  lacks any Terraform/Ansible mention — worth re-checking in case the JD adds
  IaC language. Amazon and Microsoft's own
  career domains (`amazon.jobs`, `jobs.careers.microsoft.com`) are **still
  egress-blocked as of 2026-10-05** — NOT newly reachable, contrary to hope after
  the 2026-09-28 block; keep retrying each run. T-Mobile still 403s / stale
  search-indexed IDs with no public ATS API found. **Nordstrom Tech flagged for a
  deeper look next run**: 2026-10-05 search surfaced several plausible Seattle
  SRE/DevOps-titled roles (Senior Manager SRE, Senior Engineer 2 SRE, SRE-NOC,
  Engineering Manager DevOps) for the first time in 3+ runs, but all specific
  search-indexed job URLs were 404/stale and no live search API/feed was found to
  re-derive current IDs. **RESOLVED 2026-10-12**: `careers.nordstrom.com` is
  directly crawlable via WebFetch (HTTP 200, renders real listings) — no ATS
  API token found (not Greenhouse/Lever/Ashby/Workday despite `R-xxxxxx` req
  numbering); it's a custom-built careers site. Job permalinks follow the
  pattern `/{slug}/job/{32-char-hex-id}`. Yielded a qualifying hybrid-Seattle
  "Sr Engineering Manager – Network Infrastructure" role (Ansible/Terraform/
  NAPALM + Datadog/Splunk/New Relic). **Caveat**: the on-page keyword search
  box does not appear to filter results server-side (identical results
  returned across different queries) — prefer a fuller page-by-page crawl
  (site reports ~1,385 total jobs / 139 pages) if thoroughness is needed.
  Workiva (Workday tenant
  `workiva.wd1.myworkdayjobs.com`, site slug `careers` confirmed correct) remains
  unresolvable — its jobs-search POST endpoint has returned 422 on every payload
  variation tried across 2 consecutive runs now; the previously-seen reqs
  (R8280/R9272-3/R10266) could not be re-verified as a result.

### Newly formalized employers (2nd+ qualifying appearance, 2026-10-05)

- **SmarterDx** — Greenhouse token `smarterdx`. Strong SIEM/detection-engineering
  fit (runs Panther SIEM, AWS GuardDuty/Wiz investigation) — qualifying role found
  2026-10-05 after a stale-link false start on 2026-09-28.
- **Garner Health** — Greenhouse token `garnerhealth`. SRE/platform-engineering
  roles with Terraform + Datadog observability — 2 qualifying reqs found 2026-10-05
  (one carried over from a 2026-09-28 lead that wasn't validated at the time, now
  confirmed live and qualifying). **Correction 2026-11-16: the recurring "Senior
  SRE" pick is gone from the board** — only two thin-stack Security Engineer twins
  remain (`6238004004`, `6200743004`), both held back as borderline (Terraform +
  Wiz/Cyberhaven named but no SIEM/SOAR/detection-engineering term beyond generic
  "security monitoring"). Garner Health has no clearly qualifying role this run.
  **Update 2026-11-23**: a new replacement pick found — `6261236004`, Terraform +
  Grafana/OpenSearch — but its Greenhouse `title` field ("Senior Staff Site
  Reliability Engineer") doesn't match the JD body's opening line ("Senior Staff
  Platform Engineer"), a JD inconsistency worth confirming before shipping; held
  back for quality this run, worth re-checking next run. The two Security
  Engineer twins remain unchanged/held back.
- **Coalfire** — Lever slug `coalfire`. **NEW source, 2026-11-09.** FedRAMP/NIST
  800-53 compliance consultancy — recurring pick candidate `e2620778-f8e9-4b22-
  910e-ae0edfcc8238` ("Senior Site Reliability Engineer (FedRAMP)", Remote US,
  Terraform AND Ansible both named plus a dedicated SIEM/log-pipeline/observability
  specialty line). Note: a "Senior SIEM Engineer (ELK/Sentinel)" req that multiple
  aggregators still surface is confirmed dead/closed (Jun/Sep 2026) — don't chase
  that title, the live technical opening is the FedRAMP SRE req. Reconfirmed live
  again 2026-11-16.
- **TENEX.AI** — Ashby org slug `tenex` (not `tenexai`/`tenex-ai` as previously
  guessed in earlier runs — that's why the board was marked unresolvable before).
  **NEW source, 2026-11-16.** AI-native MDR (managed detection and response)
  provider; recurring candidate `fc7c5446-8d7d-4f8e-97fa-14a7e4ac3ad6` ("Staff
  Site Reliability Engineer", Remote USA, Terraform+SIEM+Datadog). Per-job Ashby
  detail endpoint 401s — use the list endpoint's `descriptionPlain` field instead.
- **DigiCert** — Greenhouse token `digicert`. **NEW source, 2026-11-16.**
  Recurring candidate `8885889002` ("Senior DevOps Engineer", US-Remote, Terraform
  AND Ansible both named plus Splunk) — strongest IaC-tool match found this run.
  `digicert.com` itself is egress-blocked; ship the Greenhouse-hosted URL
  (`job-boards.greenhouse.io/digicert/jobs/8885889002`) as the apply link.
- **Corelight** — Greenhouse token `corelight`. **NEW source, 2026-11-23**, found
  via a fresh discovery sweep. Network-detection/security company. Recurring
  candidate `8369707` ("Sr Software Engineer, Cloud Infrastructure/SRE", North
  America — role requires physical presence in the US — Terraform, Kubernetes,
  Prometheus, Grafana all named, FedRAMP-context federal cloud platform). JD
  requires US citizenship — tag `[US-CITIZEN]` — no active-clearance requirement
  found. Shipped as a top pick on first appearance; re-check each run.
- **DigitalOcean's ATS mystery resolved, 2026-11-23**: the correct Greenhouse
  token is `digitalocean98`, not a guessable plain `digitalocean` — explains 5+
  runs of "unresolvable ATS." Reviewed all 132 open reqs this run: zero SRE/
  DevOps/Platform-Engineer-titled roles currently (mostly product-security,
  physical/data-center-infra, and software-engineering titles; closest misses
  were "Senior Product Security Engineer" and "Cloud Operations Administrator -
  II," both Seattle, both naming zero Terraform/Ansible/SIEM keywords). Query
  `boards-api.greenhouse.io/v1/boards/digitalocean98/jobs` directly going
  forward instead of treating this as egress-blocked/unresolvable.

### Demoted to spot-check-only 2026-10-26 (5th consecutive non-qualifying run)

- **Paxos** — Ashby, org slug `paxos` (lowercase; `joinpaxos`/`paxosinc`/`paxostrust`
  all still 404). Per-job detail endpoint 401s for this org (list endpoint only).
  5 consecutive runs with zero qualifying roles (closest match each time has
  SIEM/EDR language but no Terraform/Ansible named) — demoted from active
  automated-query rotation per the 3-strikes convention. Spot-check only if
  revisited; do not budget full-board pulls each run.
- **BlackCloak** — Lever, slug `BlackCloak` (capitalized — case-sensitive, unusual
  for Lever). **Dropped from rotation entirely 2026-11-16** after an 8th
  consecutive run with zero DevOps/SRE/Cloud/Platform-titled reqs (board remains
  sales/CS/account-management only) — do not query automatically going forward;
  revisit only on a specific fresh lead.

### Promising unvalidated leads (need a 2nd look — both main domains egress-blocked 2026-10-05)

- **Aalyria** (space-comms startup) — "Staff Site Reliability Engineer – Spacetime,"
  Remote US, strong observability stack (Prometheus/Loki/Tempo/OTel, GCP, IaC/GitOps)
  but Terraform/Ansible not explicitly confirmed in the snippet seen. `aalyria.com`
  egress-blocked; no Greenhouse/Lever/Ashby board found under guessed slugs.
- **ScienceLogic** — reconfirmed dead a 2nd time, 2026-11-23: the Greenhouse
  token `sciencelogic` 404s at the board level AND for 4 separate job-ID guesses
  surfaced by a fresh WebSearch sweep. Essentially exhausted under the
  Greenhouse-guess approach — needs a wholly different ATS platform guess (not
  Greenhouse) or should be dropped as a lead.
- **Pondurance** — still unvalidatable, 2026-11-23: real ATS is JazzHR
  (`pondurance.applytojob.com`), still egress-blocked. A new strong-looking lead
  ("Senior Platform Engineer," Terraform + Linux + Datadog + GitHub Actions,
  Remote US) was found via WebSearch this run but could not be validated live —
  per the mandatory URL-validation rule, NOT shipped. Retry if the block lifts.
- **Blackpoint Cyber** (new lead, 2026-11-23) — aggregator sources point to
  multiple remote "Senior Site Reliability Engineer" reqs naming Terraform, but
  every link resolves to `jobs.accel.com` (a VC-portfolio jobs board, not
  Blackpoint's own ATS) — the real Greenhouse/Lever/Ashby/Workday token could
  not be found this run. Worth a dedicated from-scratch ATS lookup next run —
  plausible strong fit if resolved.
- **Netlify, Stacklok, Bugcrowd** — all re-investigated fresh 2026-11-23 and
  confirmed to have zero live SRE/DevOps-titled roles at all (not just egress or
  stale-link issues): Netlify (6 total reqs), Stacklok (2 total reqs), Bugcrowd
  (11 reqs, product/appsec only). The specific reqs multiple aggregators surface
  for all three are confirmed 404/gone. Deprioritize fully as leads.
- **"Remote" (remote.com)** (new lead chased and ruled out, 2026-11-23) — tried
  Greenhouse tokens `remotecom`, `remote`, `remote-com`, `theremotecompany`,
  `remotecompany`; none resolve to the actual company. `remote.com` itself is
  egress-blocked. Could not validate the "Senior/Staff SRE" leads search
  surfaced for this company.

### Aggregators / boards

- **LinkedIn Jobs** — query template:
  `("Senior" OR "Staff") ("SRE" OR "DevOps" OR "Cloud Engineer" OR "Platform Engineer" OR "Site Reliability") "remote" "United States"`
  Filters: Remote · United States · Experience: Senior+ · Date: past week.
  **2026-10-05 finding**: WebSearch returned zero direct `linkedin.com/jobs` URLs
  across 6 query variants this run (base + SIEM + Seattle + `inurl:` variants) — an
  apparent search-indexing gap for LinkedIn job pages in that session, not a
  query-wording problem. Worth trying a different query shape next run, or treating
  aggregator-sourced company names (Built In, etc.) as the de facto lead source when
  this recurs.

## Search query cheatsheet

For WebSearch / Google:

- `site:boards.greenhouse.io "Senior" ("SRE" OR "DevOps") remote terraform`
- `site:jobs.lever.co staff site reliability engineer remote terraform ansible`
- `site:ashbyhq.com senior platform engineer remote linux observability`
- `site:greenhouse.io energy senior devops terraform remote`
- `"hiring" "remote" "senior" ("SRE" OR "DevOps") "terraform" 2026`

## Maintenance notes

- Re-review this file quarterly — employers shut down hiring or change ATS hosts.
- If a company appears 3+ runs in a row with no qualifying role, drop it.
- Add new finds under the right section; keep alphabetical inside each group.

### From 2026-11-23 run

- **1 brand-new qualifying source**: Corelight (Greenhouse `corelight`, see Newly formalized section above) — found via a fresh discovery sweep, shipped as a top pick. **DigitalOcean's 5+ run ATS mystery is also resolved** (correct token `digitalocean98`), though it yielded 0 qualifying roles this run.
- **Leidos staged a strong recovery** from zero last run to 3 new qualifying remote-US roles (see Energy-sector note above) — its best showing in several runs, all requiring active DoD Secret clearance + US citizenship at hire.
- **Fastly's long-standing TOP PICK `8256238` is confirmed CLOSED** — the single strongest stack match found in this scan's history is gone, no replacement of similar quality found (see Infra/edge note above).
- **Hut8 formally dropped from rotation** (3rd consecutive confirmed-zero check) — see corrected entry above.
- **Crusoe's "Senior Production Engineer, Storage" pick confirmed dead**, replaced by a new weaker-fit alternative held back this run (see Energy-sector note above).
- **GitLab and Okta each surfaced a genuine 2nd/3rd recurring-watch pick** this run (`8623389002`, `8385706`) — both held back as redundant with already-shipped picks from the same employer, but worth tracking going forward. Cloudflare's `8263016` gained a Remote-US option, upgrading it to filter-qualifying (still held back as redundant).
- **Garner Health's replacement pick has a JD title/body inconsistency** flagged for next run's confirmation (see corrected entry above).
- **Nordstrom's on-page keyword search actually worked this run** (`/jobs?keyword=terraform`, a single targeted query rather than a full 139-page crawl) — found "Senior Identity Security Engineer" (`R-898894`, Seattle, Terraform explicit) but it's borderline on the observability/SIEM filter (ITDR/ITSM/KQL only, no named SIEM/SOAR tool) — held back, not shipped on a close call. Recommend adopting this lighter-weight keyword-search approach as the standard Nordstrom check going forward instead of the abandoned full-crawl approach.
- **Zscaler shipped zero for a 2nd consecutive run** (25 raw hits, all manager-tier/state-restricted-remote/onsite) — see corrected entry above.
- **Arcadia's Lever slug `arcadia` now resolves to a different, unrelated healthcare-data-analytics company** (arcadia.io) — the energy-sector Arcadia lead remains dead/unresolved; noted to prevent future false-positive confusion.
- **Octopus/Kraken's board reconfirmed alive via a quick existence check only** (not fully scanned, per the 2026-11-16 decision to move to monthly cadence) — next full check due roughly mid-December.
- **SmarterDx held back purely for shortlist-size curation** this run (an unusually strong week with 2 new-source finds + the Leidos recovery), not a quality or source issue — worth re-shipping next run.
- **New promising unresolved lead**: Blackpoint Cyber (Terraform-naming remote Senior SRE reqs via aggregator, real ATS token not found — see Promising unvalidated leads section above).
- **Netlify, Stacklok, Bugcrowd, ScienceLogic all confirmed fresh dead ends** this run (not just egress/unresolved) — can be deprioritized fully as leads.
- **New lead chased and ruled out**: "remote.com" (no resolvable ATS token found across 5 Greenhouse guesses, main domain still egress-blocked).
- **Tesla Energy**: 403 for a 10th+ consecutive run — strong case to finalize as a permanent skip rather than a weekly retry (not yet formally dropped).
- **Paxos**: 9th consecutive non-qualifying spot-check (closest miss: strong SIEM/detection-engineering language but zero Terraform/Ansible).
- **LinkedIn**: 0 direct `linkedin.com/jobs` URLs across 2 query variants — 9th+ consecutive structural indexing gap, unchanged.
- **Amazon/Microsoft/T-Mobile/Workiva**: egress/API issues persist a 9th consecutive run, no change.
- **CrowdStrike's per-job Workday detail endpoint returned a clean 200 this run** — no 403 flake, treat as a normal reliable source going forward.
- Reviewed 2026-11-16 → 2026-11-23.

### From 2026-11-16 run

- **2 brand-new qualifying sources**: TENEX.AI (Ashby `tenex`, see Newly formalized section above) and DigiCert (Greenhouse `digicert`, see Newly formalized section above) — both found via a fresh discovery sweep, both shipped as top picks.
- **Three previously-reliable sources went to zero this run**: Red Hat's formalized pick `R-060309-1` confirmed closed, Leidos's only remote pick `R-00196252` confirmed closed, and both of Zscaler's tracked picks dead/disqualified. See corrections above in each employer's entry. None of the three had a qualifying replacement found despite dedicated searches (Red Hat: broad terraform/ansible sweep; Leidos: 5 searchText variants; Zscaler: full-board check).
- **Hut8 and BlackCloak recommended for full removal** from the rotation (Hut8: 2nd consecutive check with zero technical roles; BlackCloak: 8th consecutive non-qualifying run, structurally sales/CS-only) — see corrections above.
- **Sysdig's long-tracked "Director of Security Engineering" is gone from the board entirely** — stop tracking.
- **Garner Health's recurring "Senior SRE" pick is gone**, replaced only by two thin-stack Security Engineer twins, both held back as borderline.
- **Palantir's Substrate req reconfirmed live for a 4th consecutive run** — remains the most reliable Seattle source alongside Okta (2 distinct Seattle picks shipped again this run).
- **New leads chased and ruled out this run**: ScienceLogic (Greenhouse token/job ID 404s, unresolvable), Pondurance (real ATS is JazzHR, egress-blocked, unverifiable) — see Promising unvalidated leads section above.
- **Octopus/Kraken**: 6th consecutive structural-zero run — recommend moving to monthly checks.
- **Amazon/Microsoft/T-Mobile/Workiva/Shopify/GitHub**: egress/API issues persist an 8th+ consecutive run, no change.
- **Paxos's per-job Ashby detail endpoint reverted to 401** — the 2026-11-09 "no longer 401s" note didn't hold; use the list endpoint instead going forward.
- Reviewed 2026-11-09 → 2026-11-16.

### From 2026-11-09 run

- **3 brand-new qualifying sources**: Red Hat (`R-060309-1`, see Linux vendors note above), Coalfire (`e2620778-...`, see Newly formalized note above), and Okta's 2nd distinct Seattle pick `8268917` (see Okta note above, independently found by two collection passes). Palo Alto Networks also broke its "CA-onsite/intl only" pattern with a new Remote-USA Terraform/Ansible+observability req (`JR-023885-1`, "Global Solutions Architect - AI and Automation") and Elastic surfaced its first-ever genuine US-remote Terraform/Ansible+SIEM reqs (`8325389`, `8352728`, "Consulting Architect" track) — both held back this run as Solutions-Architect/consulting-titled rather than hands-on IC, but worth tracking for a clearer IC-titled req next run.
- **Palantir formalized as a reliable recurring Seattle source** after req `c38bb622-...` ("Senior Software Engineer, Substrate") qualified for a 2nd consecutive run.
- **Crusoe Energy's long-tracked Bellevue weekend-shift req is confirmed closed** (consistent with the 2026-11-02 finding for the prior Leidos pick) — replaced by two new picks, see Energy-sector note above. Recovers this scan's `[ENERGY]` tag count from zero last run to 2.
- **Leidos's new fully-remote qualifying pick**: `R-00196252` ("Senior DevOps Engineer", Remote/Teleworker US) — requires an *active* clearance at hire, tag `[CLEARANCE-ACTIVE]`. See Energy-sector note above.
- **Cloudflare's `7992903` Seattle option is gone** (offices now Austin/Toronto only) — drop permanently as a Seattle pick. Also identified a recurring **false-positive pattern**: ~30 Cloudflare "Customer Engineer"/"Solutions Engineer" reqs share boilerplate JD language mentioning Terraform/Pulumi/observability verbatim — these are pre-sales roles, not engineering ICs; exclude on sight unless the surrounding JD is clearly infra/SRE.
- **Sysdig's "Director of Security Engineering" demoted from "held back, needs 2nd look" to a clean non-qualifier** — re-examined closely, it genuinely never names Terraform or Ansible (only unspecified "IaC"). Sysdig is cleanly 0/38 this run; stop carrying it as a borderline candidate.
- **Hut 8 demoted**: board has pivoted entirely to Miami-onsite data-center-build/legal/finance roles — the previously-tracked "Highrise AI" remote SRE/Infra/NOC postings are gone entirely. See Energy-sector note above.
- **Octopus Energy/Kraken**: 5th consecutive structural-zero run (166 postings, still all UK/EU customer-ops) — recommend demoting to quick-check-only.
- **Paxos and BlackCloak**: both now a 7th consecutive non-qualifying run. Paxos's per-job Ashby detail endpoint no longer 401s (worth re-checking if this access holds, 1 relevant posting found this run but fails the Terraform/Ansible test). **BlackCloak recommended for full removal from rotation** (demote from spot-check to drop — always sales/CS titles only, 7 consecutive runs).
- **Minor corrections confirmed this run**: Sunrun's Workday tenant/site (`sunrun.wd5.myworkdayjobs.com`/`Sunrun_Careers`) now correctly returns 251 reqs (was `total:0` in prior runs, likely a transient site-slug issue, now resolved — still 0 qualifying). ChargePoint's egress block has lifted (now 200/44 reqs, 0 qualifying) — drop the "historically egress-blocked" framing. Epic Games is reachable via its own Greenhouse board (`boards-api.greenhouse.io/v1/boards/epicgames/jobs`, 200 OK) — **not** via the Avature domain as previously noted (that note was stale/wrong); query Greenhouse directly going forward. No qualifying Epic Games role found.
- **New egress blocks found this run**: `apply.workable.com`/`jobs.workable.com` (blocks Stellar Cyber and any other Workable-hosted employer — a new, consequential block since Workable is a common ATS), `builtin.com` (blocks resolving aggregator apply-links back to source), Siemens Energy's `jobs.siemens-energy.com` (was previously reachable with Romania/India roles, now blocked), Schneider Electric's `careers.se.com` (escalated from a 302-redirect to a full CONNECT-tunnel block, now fully unreachable rather than just a dead-end redirect).
- **New leads chased and ruled out this run**: TENEX.AI (aggregator volume of ~85 claimed open roles but no verifiable Greenhouse/Lever/Ashby/Workday board found — needs a human to find the actual careers URL), Stellar Cyber (real ATS is Workable, newly egress-blocked, unverifiable), Arcadia (Greenhouse token still 404/stale, unresolvable), DigitalOcean (digitalocean.com/builtin.com/smartrecruiters.com all blocked, no Greenhouse/Lever token works, lead effectively stalled), Aalyria/Rippling (still egress-blocked), Qlik/Experian (ATS still unresolved/egress-blocked), Blumira (prior DevOps req confirmed closed, board down to 1 unrelated role — remove from promising leads).
- **LinkedIn**: 0 direct `linkedin.com/jobs` URLs across 4 query variants — 7th+ consecutive run with this structural indexing gap. Continuing to use aggregator-surfaced company names as a discovery layer (this is how Coalfire and Okta's EPG req were found this run), resolving every lead to the employer's own ATS before shipping.
- **Amazon/Microsoft/T-Mobile/Workiva**: egress/API issues persist a 7th consecutive run — well past the 3-strikes threshold, consider demoting to monthly rather than weekly checks.
- Reviewed 2026-11-02 → 2026-11-09.

### From 2026-11-02 run

- **Zero `[ENERGY]`-tagged roles survived this run** — a first in this scan's history. Both of the prior run's reliable energy picks died simultaneously: **Crusoe Energy's Bellevue req `43f1edf3-8459-4573-87db-9f00293e3118`** ("Sr. Cloud Support Engineer - Weekend Shift"), live for 4 consecutive runs, is now **confirmed CLOSED** (absent from the current 341-req Ashby board; per-job detail 401s). No qualifying Crusoe replacement found in its remaining Bellevue/Remote-US postings. **Leidos's `R-00192064`** ("Cloud Architect/Engineer", Remote US), the longest-tracked recurring energy-adjacent pick, is also **confirmed CLOSED** (0 results on exact-ID Workday search) — a dedicated remote-facet re-search (4 searchText variants, ~118 reqs reviewed, as requested after the 2026-10-26 run) found no qualifying Remote-US DevOps/SRE/Cloud replacement; the closest candidate, R-00194746 ("DevOps Platform Engineer/Linux Systems Administrator", Bethesda MD, Terraform+Ansible+Elastic), fails the location filter — it's majority-onsite with only "occasional opportunities for remote work," not genuinely remote-eligible or Seattle-area. Worth a dedicated look next run to see if this is a one-off dip or the start of a real energy-sector drought.
- **New qualifying find: Palantir's first-ever qualifying role** (Lever posting `c38bb622-6f8e-43a1-8ae7-32291da328a8`, "Senior Software Engineer, Substrate", Seattle WA hybrid — Terraform + Ansible + Kubernetes/observability + Linux/SRE experience). Breaks a 5-6 consecutive run losing streak for Palantir. Found via a full-board Lever pull filtered to Seattle-WA reqs, not search-indexed. **Needs a 2nd appearance before formalizing** as a reliable Seattle source.
- **Okta's recurring pick `7658254` is broken**: its JD was retitled from "Staff Site Reliability Engineer - Splunk" to **"Splunk Infrastructure Engineer"** and no longer names Terraform/Ansible anywhere — drop it from recurring-pick tracking. The other recurring Okta pick, `7617976` (Senior DBRE), is unaffected and remains a reliable [SEATTLE] pick.
- **Okta's "possible new lead" `8064877`** ("Staff SRE FedRAMP"), flagged unvalidated on 2026-10-26, is **confirmed to not exist** (clean 404 against Okta's current 388-req board) — it was a stale aggregator-indexed ID (still mirrored on Dice/BuiltInSeattle). Remove this lead; do not re-add without a fresh live sighting on Okta's own board.
- **Cloudflare's `7992903`** ("Senior Network Engineer", Seattle among 4 listed locations) passes all 3 locked filters but its JD states "Applications will be accepted until November 01, 2026" — that date has passed as of this run, so it's not genuinely appliable despite still returning from the live API. Not shipped this run; re-check next run in case it's relisted with a new deadline.
- **Stripe's one-time qualifying Seattle role `8038771`** is now a clean 404 — never received the 2nd appearance needed to formalize Stripe as a reliable Seattle source. Stripe remains unformalized.
- **New candidate source, not yet formalized: Sysdig** (Lever, slug `sysdig`) — "Director of Security Engineering" (Flexible-USA, Terraform + detection language) passes all 3 locked filters but is **manager-tier**, not IC-track — held back per the "skip pure manager unless IC-track" nice-to-have rather than shipped. Worth a 2nd-appearance check with the same seniority caveat; do not ship unless an IC-level Sysdig role surfaces instead.
- **Octopus Energy/Kraken**: 4th consecutive structural-zero run (168 postings, down slightly from 173, still zero DevOps/SRE/Infra-titled reqs) — recommend demoting to quick-check-only next run per the 3-strikes convention.
- **Paxos and BlackCloak**: both now a 6th consecutive non-qualifying run — stay demoted to spot-check-only, no change needed.
- **Tesla Energy**: 403 for an 8th+ consecutive run. **Workiva**: Workday jobs-search POST 422 for a 6th consecutive run. **Shopify**: no discoverable ATS board for a 6th+ consecutive run. **LinkedIn**: `site:linkedin.com/jobs` indexing gap persists for a 6th+ consecutive run. All four remain strong candidates for formal permanent-skip/demotion status if this continues.
- **New lead investigated and ruled out**: "Stacklok" (surfaced by a fresh web-search sweep for a Bellevue "Senior SRE" role) — its live Greenhouse board has only 2 reqs total, neither SRE/DevOps-titled. Not added as a source.
- Reviewed 2026-10-26 → 2026-11-02.

### From 2026-10-26 run

- **New qualifying finds**: GitLab `8889193002` ("Cloud Platform Engineer", Remote US/Canada — Terraform+Kubernetes+observability); Wiz's 2nd distinct role type `4711762006` (see Wiz note above); Stripe's first-ever qualifying Seattle role `8038771` (see Stripe note above, needs 2nd appearance to formalize); Cloudflare `7992903` ("Senior Network Engineer", Seattle WA among 4 listed locations, Ansible+observability) — cut in this run's curation for redundancy with the shortlisted Cloudflare Storage Platform role, but worth shipping next run if the shortlist has room. **Correction 2026-11-09: req `7992903`'s office list has changed to Austin, TX / Toronto, ON only — Seattle is gone. Drop permanently as a Seattle pick unless a Seattle-tagged req reappears.**
- **Corrections**: Okta req `8160050` confirmed CLOSED (see Okta note above). CrowdStrike's `R30292` noted as citizenship/Green-Card-gated (see CrowdStrike note above) — eligible for this candidate, ship with `[US-CITIZEN]` tag.
- **Paxos and BlackCloak formally demoted** to spot-check-only after a 5th consecutive non-qualifying run (see demoted section above) — first formal demotion since the 3-strikes convention was adopted.
- **Crusoe Energy's Bellevue req `43f1edf3-8459-4573-87db-9f00293e3118` confirmed live for a 4th consecutive run** and **F5's Seattle req `RP1038966` confirmed live for a 4th consecutive run** — both remain fully reliable recurring picks.
- **Leidos `R-00192064`** ("Cloud Architect/Engineer", Remote US) reconfirmed live with a strong Terraform+Ansible+Datadog stack match, but requires US citizenship + Public Trust clearance — eligible for this candidate (US citizen); ship with `[US-CITIZEN]` `[CLEARANCE]` tags.
- **Octopus Energy/Kraken**: 3rd consecutive run with zero DevOps/SRE/Infra-titled reqs (board now at 173 postings) — the structural non-technical-board read continues to hold; consider demoting to quick-check-only next run if a 4th consecutive zero occurs.
- **Palantir**: 5th+ consecutive non-qualifying run (309 postings via Lever, 2 Seattle-WA reqs checked, neither names Terraform/Ansible) — candidate for demotion if this continues.
- **Tesla Energy**: 403 for 7+ consecutive runs — recommend finalizing as a permanent skip rather than retrying each run.
- **Shopify**: 5th+ consecutive run with no discoverable Greenhouse/Lever/Ashby board — recommend formal permanent-skip status rather than re-guessing tokens.
- **Workiva**: Workday jobs-search POST still 422s on every payload tried — unresolved for a 5th consecutive run; candidate for demotion to spot-check-only.
- **LinkedIn's `site:linkedin.com/jobs` indexing gap persists for a 5th+ consecutive run** — reconfirmed structural WebSearch limitation, not a query-wording issue.
- **Nordstrom Tech**: site remains reachable (200) but the on-page keyword search still doesn't filter server-side (reconfirmed via a query-string test) and search-indexed job URLs continue to 404 — the full ~139-page crawl needed to reliably surface a current role keeps exceeding the weekly time budget; worth a dedicated one-off deep-crawl session outside the normal weekly run if this source is to stay worth checking.
- **Schneider Electric**: new failure mode — `careers.se.com` now 302-redirects to the plain `se.com` homepage instead of 403ing or timing out; still not a usable job-board lead.
- **Aalyria/Rippling, DigitalOcean, Epic Games, Qlik, Experian, SmartRecruiters** all egress-blocked again this run (4th+ consecutive for most) — no new ATS discovery possible until these domains become reachable.
- Reviewed 2026-10-19 → 2026-10-26.

### From 2026-10-19 run

- **Okta added as a NEW formalized source** — see Seattle-area section above. Biggest single-source find in several runs.
- **Red Hat's prior-run TOP PICK req R-059619 ("Senior Specialist Solution Architect", Raleigh) is now confirmed CLOSED** (0 results on ID-specific Workday search). No replacement Red Hat req found this run passing both locked filters — a new Remote-US-NY lead (R-059757-1, "Solution Architect") names Ansible but no observability/SIEM tool, so it doesn't qualify.
- **Crusoe Energy's Bellevue "Sr. Cloud Support Engineer - Weekend Shift" req (`43f1edf3-8459-4573-87db-9f00293e3118`) confirmed live for a 3rd consecutive run** — now a fully reliable recurring `[ENERGY][SEATTLE]` pick, same status tier as F5's Seattle req.
- **F5's Seattle req RP1038966 confirmed live for a 3rd consecutive run** — now a fully reliable recurring `[SEATTLE]` pick. RP1038431 ("Security Engineer - Incident response") also still live but still lacks any Terraform/Ansible mention.
- **Octopus Energy/Kraken's board grew to 171 postings (from 151) but has 0 DevOps/SRE/Infra-titled reqs for a 2nd consecutive run**, not just 0 qualifying — the pattern now looks structural (the board serves almost entirely UK/EU customer-ops/field-trades roles with a small US customer-support presence). Consider demoting to a quick-check-only source.
- **Hut8's board grew to 53 reqs with 7 new "Highrise AI" remote postings** (AI Infrastructure Operations Engineer, Network Engineer, NOC Engineer ×2, Principal AI Infrastructure/Network Engineer, Senior SRE) — a new technical-role wave worth a closer look next run, though this run's Senior SRE req named no Terraform/Ansible/observability tool.
- **Paxos and BlackCloak are both now at a 4th consecutive non-qualifying run** — recommend formal demotion from active automated-query rotation per the 3-strikes convention; spot-check only going forward rather than full board pulls.
- **Tesla Energy is now 403 for 6+ consecutive runs** — recommend formalizing as a permanent skip rather than retrying each run.
- **LinkedIn's `site:linkedin.com/jobs` indexing gap persists for a 4th+ consecutive run** — reconfirmed structural WebSearch limitation, not a query-wording issue. Treat LinkedIn as effectively unusable for direct job-URL discovery until this changes; aggregator-sourced company names remain the de facto lead source.
- **Workiva's Workday jobs-search POST still 422s on every payload tried** — unresolved for a 4th consecutive run.
- **Nordstrom Tech's site remains reachable (200) but all 3 search-indexed job URLs tried this run 404'd** — the dead-link pattern from 2026-09-21/09-28 persists despite the 2026-10-12 "directly crawlable" finding. A full page-by-page crawl (site reports ~1,385 jobs/139 pages) is needed to reliably surface a current qualifying role, which exceeded this run's time budget — flag for a dedicated deeper pass next run rather than relying on search-indexed IDs.
- **Aalyria/Rippling, DigitalOcean, Epic Games, Qlik, Experian, SmartRecruiters** all egress-blocked again this run (3rd+ consecutive for most) — no new ATS discovery possible until these domains become reachable from this environment.
- Reviewed 2026-10-12 → 2026-10-19.

### From 2026-10-12 run

- **Snyk's board moved off Greenhouse to Ashby** — org slug `snyk`
  (`api.ashbyhq.com/posting-api/job-board/snyk`, 22 reqs, 0 qualifying yet).
  The old Greenhouse token still 404s cleanly; this is a real migration, not
  an egress-block retry item.
- **Nordstrom Tech resolved as directly crawlable** at `careers.nordstrom.com`
  (no ATS API; custom site) — corrects the 2026-10-05 "all stale/404" finding.
  Yielded a qualifying hybrid-Seattle network-infrastructure management role.
  The on-page search box appears non-functional server-side — don't trust its
  filtering, prefer a fuller crawl.
- **F5's previously-tracked req RP1038142 is confirmed CLOSED.** New recurring
  Seattle pick: **RP1038966** ("Site Reliability Engineer", Terraform +
  Prometheus/Grafana). A second new Seattle-hybrid req, RP1038431 ("Security
  Engineer - Incident response"), has a strong SIEM/EDR angle but no
  Terraform/Ansible — re-check in case the JD adds IaC language.
- **Crusoe Energy's Bellevue "Sr. Cloud Support Engineer - Weekend Shift"**
  (job id `43f1edf3-8459-4573-87db-9f00293e3118`) is confirmed live for a
  **2nd consecutive run** — promote to a recurring reliable `[ENERGY][SEATTLE]`
  pick like F5's Seattle req; re-check this specific ID each run.
- **Aalyria's real ATS is Rippling** (`ats.rippling.com/aalyria-careers`), not
  Greenhouse/Lever/Ashby as previously guessed — but `ats.rippling.com` is
  itself newly egress-blocked this session, so the "Staff SRE – Spacetime"
  lead remains unvalidated.
- **DigitalOcean's ATS is definitively not Greenhouse, Lever, or Ashby**
  (clean 404 on all three for token `digitalocean`) — try Workday or
  SmartRecruiters next run instead of retrying these three. `digitalocean.com`
  itself remains egress-blocked.
- **Epic Games lead is weakening**: no live Bellevue/Seattle DevOps/SRE req
  found via search this run (only expired 2020-2021 listings), and its
  Avature domain now returns a 403 org-policy block — a harder failure mode
  than the prior run's DNS ENOTFOUND. Lower priority next run unless a fresh
  lead surfaces via a different channel.
- **Leidos now has reqs genuinely tagged "Remote, US"/"Remote/Teleworker US"**
  (not only clearance-onsite field sites as in prior runs) — but every one
  found so far (Cloud Architect/Engineer R-00192064, DevSecOps Engineer –
  Intelligent Platforms & Agents R-00192493) is still citizenship- or
  clearance-gated — which is fine: the candidate is a US citizen, so ship
  these with `[US-CITIZEN]`/`[CLEARANCE]` tags (only active-clearance-at-hire
  reqs get the `[CLEARANCE-ACTIVE]` note).
  Also noted: Workday's `searchText` does fuzzy/relevance matching here, not
  literal substring matching — always verify via the per-job detail endpoint.
- **Qlik and Experian**: both egress-blocked for a 2nd+ consecutive run now
  (`api.smartrecruiters.com` also blocked for Experian) — try an alternate
  ATS-platform guess (e.g. Workday) next run instead of re-hitting the same
  blocked domains.
- **Paxos and BlackCloak**: both now 3rd+ consecutive run with zero qualifying
  role — candidates for demotion from active automated-query rotation per the
  3-strikes convention; Paxos's per-job Ashby detail endpoint also 401s for
  this org (list endpoint only).
- **Octopus Energy/Kraken's Lever board continues shrinking** (174 → 160 → 151
  postings over the last 3 runs), with **zero DevOps/SRE/Infra-titled reqs at
  all** this run, not just zero qualifying.
- **Hut8's Greenhouse board (47 reqs) now has zero technical roles of any
  kind** (legal, electrical/mechanical systems only) — a steeper drop than
  prior runs' "field-ops, no match."
- **Tesla Energy now 403 for 5+ consecutive runs** — consider formalizing as
  a permanent skip rather than "try once" each run.
- **LinkedIn's `site:linkedin.com/jobs` indexing gap persists for a 3rd+
  consecutive run** — WebSearch does not appear to honor the `site:` operator
  for linkedin.com/jobs in this environment at all; treat as a structural
  tool limitation, not a query-wording problem.
- **Workiva's Workday jobs-search POST still 422s** on every payload shape
  tried (including empty `searchText` + `appliedFacets:{}`) — unresolved for
  a 3rd consecutive run.
- New egress blocks observed this run (beyond the standing list):
  `www.themuse.com`, `ats.rippling.com`, `jobs.spacetalent.org` (ENOTFOUND),
  `davidenergy.com` (newly probed, confirmed blocked). `epicgames.avature.net`
  moved from DNS ENOTFOUND to a 403 org-policy CONNECT block.
- Reviewed 2026-10-05 → 2026-10-12.

### From 2026-10-05 run

- **HashiCorp and Chronosphere both lost their standalone careers boards** to
  acquisitions — HashiCorp folded into IBM (Feb 2025 acquisition close), Chronosphere
  folded into Palo Alto Networks. Both now 404 cleanly on a bare Greenhouse token
  guess. Remove them as standalone sources; HashiCorp reqs would need IBM's own
  Workday tenant, Chronosphere reqs would need PANW's (now confirmed:
  `paloaltonetworks.wd5.myworkdayjobs.com`/`panwexternalcareers`) tenant searched
  for Chronosphere-tagged postings specifically.
- **Snyk's Greenhouse board is genuinely gone** (clean 404 on all 3 Greenhouse
  hosts for token `snyk`) — not an egress-block retry item anymore, a real
  disappearance. Needs a fresh from-scratch ATS lookup next run if revisited.
- **Crusoe Energy's board is no longer onsite-only** — now has 8 Remote-US postings
  and Bellevue, WA listings alongside the SF/Denver/Dublin onsite roles (yielded
  this run's one `[ENERGY]` match, a Bellevue cloud-support role). Reverses the
  2026-09-28 "entire board confirmed onsite-only" finding.
- **Octopus Energy/Kraken's prior qualifying Remote-USA Lever posting is gone** —
  board is down to 160 postings (from 174), zero US-remote DevOps/SRE/TechOps match
  this run. Keep checking; Lever boards turn over fast.
- **Zscaler req 5029669007** ("Staff SRE (Production Engineer) – Federal") now lists
  **Bellevue, WA** among its eligible offices (previously only San Jose was seen) and
  passes all 3 locked filters — but its JD explicitly requires **US citizenship**.
  Candidate is a US citizen, so this is eligible — ship it with a `[US-CITIZEN]`
  tag (2026-10-26 correction; earlier runs wrongly held it back).
- **Egress blocks newly observed this run**: `jobs.siemens-energy.com` (was
  reachable on 2026-09-28 with Romania/India roles found, now blocked), `www.evgo.com`
  / `careers.evgo.com` / `ev.careers`, `www.enphase.com`, `jobs.nexteraenergy.com`,
  `www.spp.org`, `recruiting.ultipro.com`, `www.aalyria.com`, `www.digitalocean.com`.
  Several of these (EVgo, Southwest Power Pool) had plausible aggregator-reported
  Terraform-named leads that could not be validated live as a direct result —
  dropped per the validation rule rather than shipped.
- **New failure mode, not a block**: `epicgames.avature.net` returned DNS
  `ENOTFOUND` this run, different from the prior egress-block finding — worth a
  different lookup approach (regional subdomain, alternate path) next run rather
  than assuming it's still a proxy block.
- **Jensen Hughes**: confirmed via full live board pull (168 reqs) to have zero
  SRE/DevOps/Platform/Cloud/Security-Engineer titles at all — it's a fire-protection
  engineering firm, wrong industry vertical structurally, not just a stale-link
  issue. Recommend not rechecking.
- **Bungie**: confirmed via live board pull to have only 2 open reqs total, neither
  technical — not a stale-ID issue, genuinely nothing here.
- Reviewed 2026-09-28 → 2026-10-05.

### From 2026-09-28 run

- **New confirmed ATS slugs/tenants this run** (previously unlisted or wrong):
  Wiz's Greenhouse board token is `wizinc`, not `wiz` (`wiz` 404s); also Wiz's
  own `absolute_url` field on wiz.io is malformed (literal `:title`
  placeholder) — always use the `boards.greenhouse.io/wizinc/jobs/<id>` form.
  Tenable's Greenhouse token is `tenableinc`. SUSE is on Workday, tenant
  `suse.wd3.myworkdayjobs.com`, site `Jobsatsuse` (26 reqs, thin on
  SRE/DevOps). DuckDuckGo is on Ashby, org slug `duck-duck-go` (hyphenated,
  only 10 reqs total). Hut8's ATS is Greenhouse, token `hut8` (43 reqs) — a
  prior Lever guess was wrong. Crusoe Energy is on Ashby, org slug `Crusoe`
  (350 reqs) — but the entire board is confirmed onsite-only (SF/Denver/
  Dublin), no remote/Seattle reqs exist structurally, future runs can
  deprioritize re-checking Crusoe for remote roles. Sysdig is on Lever, slug
  `sysdig` (28 reqs). Duke Energy's Workday tenant is
  `dukeenergy.wd1.myworkdayjobs.com`, site `Search`. Sunrun's correct Workday
  tenant is `sunrun.wd5.myworkdayjobs.com`, site `Sunrun_Careers` (a prior
  `wd1` guess was wrong host). Siemens Energy runs its own "Careers
  Marketplace" portal at `jobs.siemens-energy.com` (not Workday) — has
  Terraform/Ansible/Kubernetes DevOps roles but only in Romania/India so far,
  no US req found yet. Datadog (`datadog`), Grafana Labs (`grafanalabs`,
  skews EU/UK for SRE), Cloudflare (`cloudflare`), Fastly (`fastly`), Stripe
  (`stripe`), Reddit (`reddit`), Honeycomb (`honeycomb`) Greenhouse tokens
  all reconfirmed working with zero qualifying yield this run.
- **Workiva's Workday site slug is `careers` (lowercase)** —
  `workiva.wd1.myworkdayjobs.com/careers` — correcting prior runs' failed
  guesses of `External`/`Careers`/`workiva`/`Workiva`. Could not be exercised
  this run (Workday had a platform-wide maintenance outage across all
  tenants at validation time) — worth a fresh full-board pull next run now
  that the slug is confirmed. Leads seen: R8280 "Staff Site Reliability
  Engineer", R9272-3 "Staff Software Engineer - Site Reliability", R10266
  "Senior Software Engineer - Site Reliability" (USA-Remote).
- **LinkedIn-sourced job IDs had an unusually high dead-link rate this run**:
  5 distinct "new employer" leads found via LinkedIn/web search — Bungie
  (`boards.greenhouse.io/bungie/jobs/3460177`), SmarterDx, Zscaler ("Staff
  SRE - Federal"), Garner Health, and Attain — all 404'd against the
  employer's own current Greenhouse board when validated, despite fresh-
  looking search snippets. In 3 of the 5 cases (Zscaler, Garner Health,
  Attain) a similarly-titled role existed at a *different* job ID on the
  same board, but with worse geography (hybrid-only, non-Seattle) or a
  different seniority tier — so they still wouldn't have qualified even as
  substitutes. Treat LinkedIn-sourced job IDs as leads only, never as
  apply-ready, and always re-derive the current ID from the employer's own
  board rather than trusting the linked ID.
- **Bungie, SmarterDx, Garner Health, Attain, Zscaler**: not added to the
  formal source list yet (only 1 appearance each, and that appearance was a
  dead link) — worth a second look next run by pulling each company's full
  live Greenhouse board directly (tokens: `bungie`, `smarterdx`,
  `garnerhealth`, `attain`, `zscaler`) rather than trusting search-indexed
  job IDs again.
- **Session-level egress blocks observed this run** (may vary session to
  session — retry next run before assuming permanent): `icims.com` (blocked
  entirely — explains repeated Exelon/Constellation/NextEra iCIMS-guess
  failures), `careers.se.com` (Schneider Electric — now confirmed hard
  blocked, not intermittent), `canonical.com`, `jobs.experian.com` (and its
  suspected backend `api.smartrecruiters.com` also blocked at the proxy
  layer), `qlik.com`, `epicgames.avature.net`, `github.careers`, `snyk.io`,
  `www.t-mobile.com`, `www.amazon.jobs` (new block — wasn't blocked before,
  was previously just "no ATS found"), `jobs.careers.microsoft.com` (also a
  new block). Working fine this session: `jobs.paloaltonetworks.com`,
  `shopify.com` (though Shopify still has no discoverable JSON API).
- **GridX, AutoGrid, Arcadia**: 3rd consecutive run with zero resolvable ATS
  via token-guessing or web search — per the "3 runs no qualifying source"
  convention, recommend dropping automated-search budget on these three and
  relying on manual/LinkedIn spot-checks only going forward.
- **Palantir** (Lever, slug `palantir`): checked 6 current DevOps/SRE/
  InfoSec reqs this run — all hybrid DC/NY/Seattle-onsite/Palo-Alto, none
  remote, and none name Terraform/Ansible explicitly in the JD body. Same
  pattern as the 2026-09-21 run. Consider deprioritizing unless a remote or
  Seattle-based req appears.
- **Shopify, GitHub, Snyk**: no public Greenhouse/Lever/Ashby board found via
  token-guessing (all 404). Worth trying SmartRecruiters/Workable APIs next
  run, or treat like Amazon/Microsoft/Nordstrom as "no queryable ATS."
- Reviewed 2026-09-21 → 2026-09-28.

### From 2026-09-21 run

- **GitLab full-board re-check surfaced 2 additional qualifying roles missed by keyword/search-based collection**: a "Staff Corporate Security Engineer", "Senior Professional Services Technical Architect - Security", and "Staff Forward Deployed Engineer" all passed the three must-haves but weren't found by the earlier collection agents' targeted searches. **Recommend future runs always pull GitLab's full live Greenhouse board (`boards-api.greenhouse.io/v1/boards/gitlab/jobs?content=true`) and grep for Terraform/Ansible + observability/security keywords across every open req**, not just search-indexed or obviously-titled postings — GitLab is now 3 runs in a row as the single highest-yield source (6 of 11 shortlisted roles this run).
- **CrowdStrike's Workday site slug is `crowdstrikecareers`** (not bare `crowdstrike`, which 404s) — `crowdstrike.wd5.myworkdayjobs.com/wday/cxs/crowdstrike/crowdstrikecareers/...`. Found a 2nd strong, distinct CrowdStrike role this run beyond the usual SRE TechOps req: "Sr. Linux Systems Engineer – Object Storage (Remote)" (R29937) — an unusually direct title match to the candidate's own specialization. Worth searching this tenant's full job list each run, not just the previously-known req IDs.
- **F5's correct Workday tenant/site found**: `ffive.wd5.myworkdayjobs.com`, site `f5jobs` (prior runs' 422s were from guessing wrong site names like `f5` or `careers`). Yielded 3 Seattle-based security roles this run, none of which cleared both must-have filters, but the tenant is now directly queryable for future runs.
- **Exelon is on iCIMS, not Workday**: `careers-exeloncorp.icims.com`. This explains 2+ runs of 422 Unprocessable Entity from Workday tenant-name guessing for Exelon specifically. Constellation Energy and NextEra Energy's correct ATS platforms remain unconfirmed — try iCIMS-pattern lookups for them too next run before continuing to guess Workday tenants.
- **Splunk's career site now redirects to Cisco** (`splunk.com/en_us/careers/jobs/*.html` → 301 → `careers.cisco.com/global/en/splunk`, reflecting the Cisco acquisition), and `careers.cisco.com` is blocked by this session's network egress policy. Splunk is effectively unreachable until the block lifts or a Cisco-hosted ATS API is identified — do not keep budgeting search time on `splunk.com` URLs directly.
- **T-Mobile continues to return HTTP 403 to WebFetch with no public ATS API found**, 2nd run in a row it can't be validated despite the domain itself not being hard network-blocked. Deprioritize further manual chasing of T-Mobile search snippets unless a direct ATS is discovered.
- **New promising leads, not yet formalized (need a 2nd qualifying appearance)**: **Workiva** (Terraform/GCP/AWS stack per LinkedIn snippet for a "Staff Site Reliability Engineer" — Workday tenant `workiva.wd1.myworkdayjobs.com` confirmed to exist but the site slug wasn't resolvable this run and `workiva.com` is egress-blocked, so the correct slug couldn't be looked up); **Epic Games** `[SEATTLE]` (Bellevue, WA — Terraform/Ansible/Python/Go/Bash per LinkedIn snippet for a Sr./Senior DevOps Engineer role; actual ATS is Avature but no current job ID pinned yet — do not confuse with Epic Systems/careers.epic.com, a different company); **Qlik** and **Experian** (both egress-blocked this session with no ATS API alternative, but both had strong stack snippets — Qlik: Terraform/Crossplane/Ansible/Prometheus/OTel/Splunk; Experian: 3+ yrs Terraform).
- Home Depot's `careers.homedepot.com` was reachable this run (unlike the 2026-09-14 hard block) — confirmed its SIEM/EDR "Cybersecurity Engineer II" role is genuinely live, but it fails the Linux+IaC filter on the merits: zero mentions of Terraform or Ansible anywhere in the full JD despite the strong SIEM/EDR/Cortex/XSIAM language.
- Reviewed 2026-09-14 → 2026-09-21.

### From 2026-09-09 run

- **RemoteOK, WeWorkRemotely, and Wellfound removed from the source list.** RemoteOK returned zero usable postings (tag-page searches only surfaced "hire a freelancer" pages); WeWorkRemotely and Wellfound both block automated fetch (403/410), so collection could only rely on unverifiable WebSearch snippets for them. All three produced hits that repeatedly failed Step 3.5 validation. Revisit only if their fetch-blocking or listing quality changes.
- A high proportion of Greenhouse/Workday/Ashby job IDs surfaced by web search this run were stale (404 or removed) even on established boards (GitLab, Grafana Labs, Honeycomb, Wiz, Close, The Farmer's Dog) — validate job IDs against the employer's live ATS listing, not just the search snippet.
- Candidate additions surfaced this run (not yet added, need a second qualifying appearance first per the 3-strikes-you're-in convention): **Southwest Power Pool** `[ENERGY]` (grid/utility, strong Terraform/Linux stack fit, but posting could not be independently validated — JS-blocked career portal) and **Leidos** (gov/energy-adjacent DevOps).

### From 2026-09-14 run

- **Session network egress policy blocked ~10 major-employer domains entirely this run** (Home Depot, T-Mobile, Nordstrom, Palo Alto Networks, Splunk, Shopify, Tesla, Sunrun, Schneider Electric, Jobvite) — confirmed via both WebFetch and raw curl (`connect_rejected`, gateway 403 on CONNECT), not a dead-link condition. This forced several strong-looking candidates (notably Home Depot's SIEM/EDR Cybersecurity Engineer II and T-Mobile's Terraform/Ansible-named Software Reliability Engineer) to be dropped as unvalidatable rather than shipped unverified. This is environment-dependent and may not recur on future runs from a different session — re-attempt these sources next run before assuming they need removal.
- **Red Hat added as a confirmed-working source**: its Workday tenant (`redhat.wd5.myworkdayjobs.com`, site `Jobs`) is directly queryable and yielded a strong match this run (Terraform+Ansible+Splunk+observability). Search-indexed Red Hat job IDs were stale; query the Workday tenant search API directly instead.
- **CrowdStrike's Workday per-job detail endpoint is now working** (200, full JD body) for the two IDs re-tested this run, reversing the 403/empty-SPA finding from 2026-09-09/09-10. Treat CrowdStrike as a normal Workday source going forward rather than flagging it for manual review.
- **GitLab remains the highest-yield single source** — 3 of 7 shortlisted roles this run came from GitLab's Greenhouse board (`gitlab`), each with Terraform and/or Ansible plus observability language explicitly named.
- **Paxos's Greenhouse board no longer resolves under any guessed token** (`paxos`, `joinpaxos`, `paxosinc`, `paxostrust` all 404) — possible ATS migration; the specific Staff SRE posting found via LinkedIn/search could not be validated. Re-check next run before dropping as a candidate source.
- **Chainlink Labs' Ashby board is not resolvable via the public posting API** under any guessed org slug, and its hosted job page renders no extractable content via WebFetch (client-side SPA). No viable automated validation path found — do not add to the formal source list yet.
- **Utility-sector Workday tenants (Constellation Energy, NextEra Energy, Exelon) remain unresolved** — tenant-name guessing returned 422 Unprocessable Entity rather than confirming/denying. Needs the correct tenant slug (typically findable from the employer's own careers page) before these can be queried directly.
- Reviewed 2026-09-10 → 2026-09-14.

### From 2026-09-10 run

- **Filter criteria updated**: onsite/hybrid Seattle-area roles now qualify without remote eligibility (candidate can commute) — see Locked filter criteria above. 0 Seattle-area roles passed validation this run despite genuine effort (Amazon ×2 live but no Terraform/Ansible named; Boeing/Qualtrics dead; Microsoft/T-Mobile no locatable live URL) — this looks like a real pattern (big employers at this scale rarely name specific IaC tools) worth a follow-up decision on whether to loosen the IaC-tool wording for Seattle-area roles specifically.
- **Southwest Power Pool and Leidos both struck out again on validation** (2nd appearance for SPP, Leidos not previously formalized) — SPP's UltiPro portal serves a browser-incompatibility page instead of content to automated fetch, and Leidos's `careers.leidos.com` 403s with no public ATS API. Recommend NOT adding either to the formal source list — they surface plausible-looking hits repeatedly but have no viable automated validation path, which defeats the point of the source list.
- **HashiCorp's two postings** flagged live-but-rate-limited (429) on 2026-09-09 are now confirmed dead (404) — a data point that a 429 shouldn't be read as "probably real, just blocked."
- **CrowdStrike remains only partially checkable, 2nd run in a row**: Workday's listings-index search reliably confirms a job is live + its title, but the per-job detail endpoint 403s and WebFetch gets an empty SPA render every time. Automated stack-keyword validation isn't possible here without a different approach (e.g. a logged-in browser session) — flag for manual review if pursuing CrowdStrike specifically, rather than continuing to spend automation budget on it.
- Reviewed 2026-05-12 → 2026-09-10.
