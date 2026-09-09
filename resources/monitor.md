# Scan Telemetry Dashboard

Published Artifact URL: https://claude.ai/code/artifact/b2615fec-ddc3-4a80-a50a-22be2738b3f2

This dashboard reads the embedded run data inside its own HTML — it does not
live-read `logs/`. To reflect a new run, read every file under `logs/`, update
the `run-data` JSON array in the artifact's source (append the new run object),
and republish to the URL above (pass it as `url` to the Artifact tool) so the
link stays the same.

Source file for this artifact while it's being edited:
`logs/` (the JSON files themselves) — the artifact's own HTML lives wherever it
was last written locally before publish; if you don't have that local copy,
read the artifact back (`action: "read"`) before editing it further.
