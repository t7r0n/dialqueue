# Failure Matrix: Dialqueue

| Scenario | Failure mode | Metric | Gate | Evidence |
| --- | --- | --- | --- | --- |
| throxy evidence replay | throxy_drift | throxy_coverage | block release until cited evidence is regenerated | ev_0000 |
| human operator packet | human_blindspot | human_latency | accept only if decision claims cite fixture evidence | ev_0007 |
| human operator packet | human_blindspot | human_latency | accept only if decision claims cite fixture evidence | ev_0011 |
| right regression harness | right_misroute | right_precision | open a regression issue with trace and benchmark delta | ev_0014 |
| entire boundary probe | entire_gap | entire_risk | route to reviewer with evidence packet | ev_0021 |
| right regression harness | right_misroute | right_precision | open a regression issue with trace and benchmark delta | ev_0022 |
| throxy evidence replay | throxy_drift | throxy_coverage | block release until cited evidence is regenerated | ev_0028 |
