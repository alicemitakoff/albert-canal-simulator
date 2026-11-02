# Albert Canal corridor

Digital twin of the 70 km Albert Canal corridor from Antwerp to BCTN Meerhout: live vessels from AIS, a forecast of each vessel's next hours with the best place to swap battery packs, and a play mode where up to four players take a vessel through the corridor.

Digital twin powered by NatPower Digital. Audience: CMA CGM.

- Map: summer 2024 orthophoto (Digitaal Vlaanderen, open data), Esri World Imagery when zoomed out, bridges, locks and moorings from OpenStreetMap, canal centreline from the AImovation survey.
- Live data: aisstream.io through the GitHub Action in `.github/workflows/live-ais.yml`, which keeps every position in `live/history/` on the `live-data` branch.
- Rebuild the corridor data: `python3 tools/corridor_osm.py`.
