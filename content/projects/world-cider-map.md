---
title: "World Cider Map"
summary: "3,054 cider producers across 62 countries, rebuilt from the dataset behind Cider Guide's map."
weight: 50
---

**[Open the map →](https://ericallanwest.github.io/ciderguide/)** · [Code](https://github.com/ericallanwest/ciderguide)

The directory of cidermakers I maintained at Cider Guide since the early 2010s, rebuilt as a
modern web map.

- **Data:** name, type and location for each producer, with coordinates verified through the
  Google Places API and links to their website and listings. The GeoJSON is open for reuse.
- **Pipeline:** a marimo notebook turns the raw spreadsheet into clean GeoJSON.
- **Map:** hand-built Leaflet page.
