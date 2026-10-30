---
title: "Same Road, Different Day"
summary: "Year-over-year and repeatability analysis of road-survey runs, on a simulated five-year survey program over eastern Kentucky's real road network, every step scored against known truth."
weight: 5
---

**[Open the project →](https://ericallanwest.github.io/survey-runs/)** · [Repeatability lab](https://ericallanwest.github.io/survey-runs/lab/) · [Code](https://github.com/ericallanwest/survey-runs)

A pavement survey vehicle reads the road in 26.4-ft segments, each tagged with an odometer distance
and a GPS fix. Comparing surveys means lining up runs that never start in the same place, count the
same distance or follow the same GPS track, year against year and run against run. Real survey data
is proprietary, so this project simulates five years of surveys by two vehicles over the 1,861 miles
of US and KY routes in Kentucky's District 12, on the state's public road network, with a synthetic
friction-like index whose truth is known. Every step of the analysis is scored against it.

- **Matching:** each segment is placed on the linear referencing system by distance, bearing and the
  run's own context, with frozen GPS fixes bridged by odometer distance. 99.92% of 3.4 million
  segments land on the road actually driven, with a median measure error of 2 ft.
- **Year over year:** every year's readings on one 0.005-mi grid in both directions, with divided
  highways' far carriageways paired to the mainline. Resurfacing is flagged with 98.7% precision,
  and an odometer reading 0.5% short is caught from GPS alone.
- **Repeatability:** repeat runs are paired by odometer, GPS and LRS measure, then scored with BRSD
  and ICC. When two odometers disagree, pairing by odometer drifts up to 115 ft over a 3-mile site;
  pairing by position doesn't. A marimo notebook compiled to WebAssembly lets you change the GPS
  error, the odometer drift and the road's texture and watch it happen.
- **Background:** the methods mirror work I do on real survey data for state transportation
  agencies, rebuilt from scratch on public and simulated data.
