# Decision Report: Dialqueue

A vertical, NAICS aware call prioritization engine that turns Throxy's human callers from "dial the next row" into a 3 7x higher connect/qualified meeting rate, with a short local demo of the rebuilt daily queue.

## Evidence-Grounded Findings

CLAIM: entire gap should `block release until replay is understood` because blocks=3 reviews=2 mean_severity=3.333. [EVID: ev_0011]
CLAIM: entire reviewer handoff should `block release until replay is understood` because blocks=2 reviews=4 mean_severity=2.583. [EVID: ev_0055]
CLAIM: human policy boundary should `block release until replay is understood` because blocks=2 reviews=3 mean_severity=1.708. [EVID: ev_0099]
CLAIM: right failure replay should `block release until replay is understood` because blocks=2 reviews=4 mean_severity=3.333. [EVID: ev_0044]
CLAIM: throxy drift should `block release until replay is understood` because blocks=2 reviews=3 mean_severity=2.5. [EVID: ev_0022]
CLAIM: throxy evidence recall should `block release until replay is understood` because blocks=3 reviews=3 mean_severity=1.875. [EVID: ev_0066]
