---
title: "Where Friction Matters"
summary: "Road geometry from public lidar along eastern Kentucky's state routes, checked against the state's own inventories and turned into a map of how much grip the road asks of a car."
weight: 6
---

**[Open the project →](https://ericallanwest.github.io/ky-road-geometry/)** · [Crest and sag explorer](https://ericallanwest.github.io/ky-road-geometry/explorer/) · [Code](https://github.com/ericallanwest/ky-road-geometry)

How much friction a road needs depends on its geometry: how sharp its curves are, how steep its
grades, how much its lanes bank, and how far ahead a driver can see. This project derives all of
it for the 2,060 miles of US and KY routes in Kentucky's District 12 from public data: the state's
road network and KyFromAbove's 2-ft lidar, read only along the roads. It checks the results against
the Kentucky Transportation Cabinet's own curve, grade and bridge inventories, then combines them
into friction demand: the share of a car's weight its tires must deliver at the speed the road is
likely driven.

- **Curves:** 96.5% of KYTC's 16,853 recorded curves found in the road's own geometry, with degrees
  of curve that match the inventory's without bias.
- **Grades:** 96% of recorded crests and sags read the right way. The inventory turns out to read
  about 0.9 percentage points steeper than the lidar, uphill and downhill alike.
- **Bridges:** bare-earth lidar has the bridges taken out, so they are found as dips in the road
  profile (97% of bridges 500 ft and longer) and decked over.
- **Demand:** braking and cornering combined on the friction circle, plus the friction it takes to
  stop within the sight distance a crest or sag leaves. Demand only: no pavement-supply data and
  no thresholds.
- **Crashes:** ten years of state police reports, placed on the network. From the least to the
  most demanding tenth of the road, roadway departures rise from 4 to 32 per 100 million
  vehicle-miles on wet pavement and from 9 to 49 on dry, while animal crashes, a placebo, fall.
- **Context:** the USDA's road ruggedness and rurality codes by census tract; the district holds
  39 of Kentucky's 71 tracts rated highly rugged along their roads.
- **Explorer:** shape a crest or a sag in the browser and run the project's own sight-distance
  code on it, checked against AASHTO's formulas.
