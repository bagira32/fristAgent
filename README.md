# AI Agent Job Hunt Workspace

A Claude Code workspace for automated job hunting: searching job boards and employer
career pages, filtering listings against locked criteria, validating every apply link
is actually live, and producing a concise shortlist report.

## About

Built around a single candidate profile: a Linux Systems Engineer specialized in
multi-cloud hardening, Terraform/Ansible automation, and SIEM/telemetry pipelines
(SRE + DevSecOps background). See `CLAUDE.md` for the full profile and the rules
Claude follows in this workspace.

## Structure

```
CLAUDE.md         Project context, candidate profile, and agent rules
workflows/         Plain-English recipes the agent follows
  job-market-scan.md   Recurring Cloud/DevOps/SRE US-remote market scan
resources/         Reference docs and locked criteria
  sources.md           Filter criteria + seed list of employers/boards
  monitor.md            Link + update instructions for the telemetry dashboard
output/             Dated deliverables (one report per scan run)
logs/               Structured per-run telemetry (sites visited, API hits, token usage, timing)
```

## How it works

Running the `job-market-scan` workflow drives this sequence:

1. **Collect** — query employer career pages / ATS boards and aggregators listed in
   `resources/sources.md`, capturing raw hits without filtering.
2. **Filter** — keep only roles that hit all three locked must-haves: Linux + IaC
   (Terraform/Ansible named explicitly), an observability/SIEM/security angle, and
   US-remote eligibility.
3. **Validate** — every candidate apply URL is checked live (WebFetch, or the ATS's
   own JSON API for Lever/Greenhouse/Ashby/Workday) before it's allowed on the
   report. Dead, redirected, or aggregator-only links are dropped, not padded in.
4. **Rank & report** — top 10-15 roles, 3-5 flagged as top picks, written to
   `output/job-market-scan-YYYY-MM-DD.md` with sources cited.

`resources/sources.md` is a living document — employers or boards that go stale get
pruned, new finds get added, based on what each run turns up.

## Monitoring

Each run logs a structured JSON file to `logs/` — every site visited and ATS API
call made, its outcome, per-source-group coverage, timing, and token usage
(subagent totals are exact; main-thread usage is an estimate proxied from
tool-call volume, since no tool reports that from inside a session). A published
dashboard reads that data — see `resources/monitor.md` for the link and how to
update it after a new run.

## Status notes

- RemoteOK, WeWorkRemotely, and Wellfound were removed from the source list
  (2026-09-09): all three block automated fetch or return low-quality results, and
  hits sourced from them repeatedly failed URL validation. See `resources/sources.md`
  maintenance notes for details.
- URL validation is strict by design — a run can legitimately surface fewer than the
  10-15 target if most candidate links don't survive validation. The report says so
  honestly rather than shipping unverified links.
