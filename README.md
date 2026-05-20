# Call Priority Lab

A vertical, NAICS-aware call prioritization engine that turns a raw account list into a ranked, evidence-backed daily queue.

![Call Priority Lab working dashboard](outputs/project_working.svg)

## Why it exists

Outbound teams in traditional industries often need to rank accounts and decision makers before a caller starts the day. The useful artifact is a local replay harness that can score source coverage, role fit, industry context, and queue priority without relying on private CRM data or hosted services.

The project is intentionally built as a local replay harness instead of a slide. It creates fixtures, plants realistic failure modes, produces citation-locked evidence, and turns the result into a dashboard a reviewer can inspect without credentials or hosted services.

## What is inside

- Deterministic fixture generation for the company-specific risk surface.
- Strategy code in `src/call_priority_lab/strategy.py` with project-specific scoring and visual evidence.
- Citation-locked reports where every decision claim points to a generated evidence ID.
- Two regenerated visual artifacts: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, benchmark, and test artifacts.

![Call Priority Lab evidence map](outputs/evidence_map.svg)

## Signals it measures

- `source coverage`
- `handoff risk`
- `role precision`
- `queue latency`

## Failure modes it plants

- source drift
- handoff gap
- role misroute
- queue blindspot

## Run it locally

```bash
uv sync
uv run call-priority-lab all
uv run pytest -q
uv run ruff check .
```

## Outputs worth opening

- `outputs/dashboard.html`
- `outputs/project_working.svg`
- `outputs/evidence_map.svg`
- `outputs/operator_brief.md`
- `outputs/decision_report.md`
- `outputs/strategy_model.json`
- `outputs/demo_pack.zip`

## Boundary

Everything runs locally against synthetic fixtures. There are no credentials, no customer records, no outreach files, and no hosted API dependency.
