# Project Context

This is my AI agent workspace. I use it for job hunting, search for jobs offerings, filter jobs base on specific criteria then generate a daily/weekly summary for jobs.

# About me

Linux Systems Engineer specialized in Linux systems and automated infrastructure. Expert in
hardening multi-cloud environments and engineering resilient telemetry pipelines using Python,
Terraform, and Ansible. Proven track record of deploying global-scale SIEM ecosystems and
transforming fragmented log data into actionable security intelligence through SRE and
DevSecOps principles.

# Rules

- Always ask clarifying questions before starting a complex task.
- Show your plan and steps before executing.
- Keep reports and summaries concise - bullet points are preferred.
- Save all output files to output directory.
- Cite sources when doing research.
- Every job apply URL that ships on a report must be validated live before delivery (WebFetch, with ATS JSON API fallback for Lever/Greenhouse/Ashby/Workday) - see the URL validation step in workflows/job-market-scan.md. Aggregator/mirror links and unverified search-snippet URLs never count.

# Project Structure

- workflows/ - Workflow instructions files (plain english recipes the agent follows). Currently: `job-market-scan.md`, the recurring Cloud/DevOps/SRE US-remote market scan.
- output/ - Finished deliverables (reports, drafts, analysis), one dated file per scan run.
- resources/ - Reference docs and templates. Currently: `sources.md`, the locked filter criteria and seed source list for the job scan.