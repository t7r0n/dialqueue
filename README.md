# Dialqueue

A vertical, NAICS aware call prioritization engine that turns Dialqueue's human callers from "dial the next row" into a 3 7x higher connect/qualified meeting rate, with a short local demo of the rebuilt daily queue.

![Dialqueue working dashboard](outputs/project_working.svg)

## Why it exists

Dialqueue's entire moat is "we find the right human in a traditional industry that LinkedIn/Apollo can't surface." But the public artifact that proves this — an ICP to decision maker mapper for manufacturing/logistics/3PLs — does not exist. Today their AI Engineer role (YC) implies they're still doing this with internal Python + scraper duct tape. Meanwhile.

The project is intentionally built as a local replay harness instead of a slide. It creates fixtures, plants realistic failure modes, produces citation-locked evidence, and turns the result into a dashboard a reviewer can inspect without credentials or hosted services.

## What is inside

- Deterministic fixture generation for the company-specific risk surface.
- Strategy code in `src/dialqueue/strategy.py` with project-specific scoring and visual evidence.
- Citation-locked reports where every decision claim points to a generated evidence ID.
- Two regenerated visual artifacts: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, benchmark, and test artifacts.

![Dialqueue evidence map](outputs/evidence_map.svg)

## Signals it measures

- `Dialqueue coverage`
- `entire risk`
- `right precision`
- `human latency`

## Failure modes it plants

- Dialqueue drift
- entire gap
- right misroute
- human blindspot

## Run it locally

```bash
uv sync
uv run dialqueue all
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
