# Operator Brief: throxy

throxy gets a local, deterministic pressure test around throxy, entire, and right. The useful part is the repeatable evidence path from fixture to failure to operator action.

## Highest-leverage checks

- throxy evidence replay -> block release until cited evidence is regenerated (throxy_coverage, evidence ev_0132).
- human operator packet -> accept only if decision claims cite fixture evidence (entire_risk, evidence ev_0011).
- right regression harness -> open a regression issue with trace and benchmark delta (right_precision, evidence ev_0066).
- entire boundary probe -> route to reviewer with evidence packet (human_latency, evidence ev_0033).

## What makes this useful

The workflow is intentionally local and deterministic. A reviewer can run the same fixture set, inspect the evidence IDs, open the dashboard, and see exactly why a recommendation passed, went to review, or blocked.
