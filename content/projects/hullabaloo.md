---
title: "Hullabaloo"
summary: "Route optimization for a 7-hour trail rogaine near Blacksburg, Virginia, solved to proven optimality."
weight: 20
---

**[View the project →](https://ericallanwest.github.io/hullabaloo/)** · [Code](https://github.com/ericallanwest/hullabaloo)

The Blacksburg Adventure Skills Hullabaloo is a timed rogaine on the Pandapas Pond / Poverty Creek
trail network. Competitors get 7 hours and score a point per trail completed and a point per
unique mile covered. Covering everything would take more than 10 hours, so the whole game is
deciding which miles to skip.

That makes it a **prize-collecting arc routing problem**: points sit on edges rather than nodes,
re-walking an edge earns nothing, and the tour must start and finish at the trailhead.

| Method | Score | Trails | Unique miles |
|---|---|---|---|
| Greedy nearest-trail baseline | 42.07 | 23 | 19.07 |
| ALNS heuristic (6 seeds × 500 iterations) | 47.60 | 26 | 21.60 |
| **MILP, proven optimal (HiGHS)** | **48.11** | **26** | **22.11** |

The mixed-integer program closes the gap to 0.00% in 45 seconds, 14% better than the greedy
baseline. The heuristic lands within 1.1% of the optimum and seeds the solver with a strong
starting route.
