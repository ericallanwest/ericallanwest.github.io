---
title: "NBA League Pass Team Guide"
summary: "How much of each NBA team's season you can watch live on League Pass, and the ZIP codes where it's locally blacked out."
weight: 30
---

**[Open the guide →](https://ericallanwest.github.io/nba-league-pass/)** · [Code](https://github.com/ericallanwest/nba-league-pass)

For any team: its games on national TV, the ones League Pass blacks out everywhere, and a map of
the ZIP codes where League Pass blacks the team out locally. It succeeds an earlier Tableau Public
version.

- **Blackouts** for all 33,791 ZIP Code Tabulation Areas, from NBA.com's own lookup.
- **Drive times** from each ZIP to its nearest arenas, from the OpenRouteService Matrix API.
- **Population** from the Census Bureau's ACS 5-year estimates.
- **Pipeline:** GitHub Actions workflows refresh each dataset; the site is a static MapLibre page
  with no build step.
