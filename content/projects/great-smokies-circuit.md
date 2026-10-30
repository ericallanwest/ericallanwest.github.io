---
title: "Great Smokies Circuit"
summary: "An itinerary planner for hiking every official trail in Great Smoky Mountains National Park as one continuous walk."
weight: 10
---

**[Launch the app →](https://ericallanwest.github.io/great-smokies-circuit/)** · [Code](https://github.com/ericallanwest/great-smokies-circuit)

An interactive map of pre-solved thru-hiking itineraries that cover every official trail in the
park as a single continuous walk. Choose a maximum hiking day and an open or closed circuit, then
step through the itinerary day by day: required mileage, backtracking, elevation gain, and the
route to that night's campsite or shelter.

- **Routing:** a rural windy postman solver assigns a traversal direction to every trail segment
  with OR-Tools CP-SAT, then splits the circuit into legal hiking days, with overnights only at
  backcountry campsites, shelters and campgrounds.
- **Elevation:** gain and loss come from USGS 3DEP 1-meter DEMs.
- **Background:** I completed every trail in the park myself (the 900 Miler Club, 2019–2022). The
  repository also collects the datasets, maps and known map-completion routes.
