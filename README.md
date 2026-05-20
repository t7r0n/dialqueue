# Dialqueue

A vertical, NAICS aware call prioritization engine that turns Throxy's human callers from "dial the next row" into a 3 7x higher connect/qualified meeting rate, with a short local demo of the rebuilt daily queue.

## Why This Exists

Throxy's entire moat is "we find the right human in a traditional industry that LinkedIn/Apollo can't surface." But the public artifact that proves this - an ICP to decision maker mapper for manufacturing/logistics/3PLs - does not exist. Today their AI Engineer role (YC) implies they're still doing this with internal Python + scraper duct tape. Meanwhile the cold calling team has a separate, unsolved problem: call list prioritization. They have ~10M emails sent and ~60 SDRs dialing daily (throxy.

## What It Builds

- Replays synthetic `throxy` and `entire` cases against the project's evidence rules.
- Scores `throxy_coverage`, `entire_risk`, and `right_precision` so regressions are visible in CSV and JSON.
- Plants `throxy drift` and `entire gap` failures as negative controls.
- Writes citation-locked decision claims; unsupported claims fail verification.
- Exports a review dashboard and demo pack for `dialqueue` without hosted services.

## Local Run

```bash
uv sync
uv run dialqueue all
uv run pytest -q
uv run ruff check .
```

## Outputs

- `outputs/analysis.json`
- `outputs/scenario_report.csv`
- `outputs/decision_report.md`
- `outputs/evidence_packet.md`
- `outputs/domain_rubric.json`
- `outputs/failure_matrix.md`
- `outputs/trace_graph.mmd`
- `outputs/dashboard.html`
- `outputs/demo_pack.zip`

## Sources

- https://throxy.com/resources/blog/ai-sdrs-are-killing-sales
- https://www.ycombinator.com/companies/throxy
- https://www.ycombinator.com/launches/NRm-throxy-book-meetings-without-the-busywork
- https://www.tryfondo.com/blog/throxy-launches
- https://gohub.vc/throxy-ai-sales-agents/
- https://gohub.vc/throxy-raises-6m-seed-round/
- https://www.linkedin.com/in/bmerey/
- https://arxiv.org/abs/1103.4601

## Boundary

This repository uses synthetic fixtures only. It has no credentials, no customer data, no outreach data, and no dependency on a hosted API.
