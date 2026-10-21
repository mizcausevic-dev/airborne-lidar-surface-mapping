# Airborne Lidar Surface Mapping — Anatomy Motion Explainer

**About:** 34-second code-driven anatomy explainer of airborne lidar surface mapping: timed pulses, multiple returns, georeferencing, and ground classification with uncertainty.

**Topics:** `lidar` `earth-observation` `geospatial` `remote-sensing` `point-cloud` `motion-design` `canvas-animation` `georeferencing`

Live preview: GitHub Pages on the `pages` branch (root `index.html`).

## Run locally
Open `index.html` in a browser, or `python3 -m http.server 8000` then http://localhost:8000/?frame=420

## Timing (verified in code)
- 34 seconds, 30 fps, 1,020 frames indexed 0–1019
- 0–149 reveal scanner + positioning · 150–299 timed pulses · 300–509 returns · 510–749 georeference · 750–1019 classify ground with uncertainty

## Limits and safeguards
Conceptual schematic, not a certified design or operating procedure. Not every return is ground. Multiple returns and occlusion vary. No universal centimeter accuracy is claimed. Waveform and counts are qualitative/schematic. No dimensions, settings, efficiencies, or vendor internals are asserted.

Mechanism basis: USGS Mendenhall 20-43, fusing SAR and lidar (https://www.usgs.gov/centers/mendenhall-research-fellowship-program/20-43-fusing-synthetic-aperture-radar-and-lidar). Camera, palette, cutaways and timing are illustrative.

Note on naming: standing rule appends `-Cursor` before extensions. `index.html` is kept verbatim because GitHub Pages requires that exact filename at the site root. Supporting docs use the `-Cursor` suffix.
