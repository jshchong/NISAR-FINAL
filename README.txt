NISAR Rice Globe (local version, full satellite imagery)

HOW TO RUN (Windows)
1. Unzip, then open PowerShell in this "globe" folder
   (Windows 11: right-click an empty spot in the folder > Open in Terminal).
2. Run:   python -m http.server        (or: py -m http.server)
3. Open http://localhost:8000 in Chrome or Edge. Keep the PowerShell window open.
   Do not double-click index.html - browsers block the data layers when opened as a file.

WHAT YOU SEE
- Layer 1: satellite globe (Esri World Imagery) with city/town labels.
- Layer 2: NISAR L-band rice growth stage for 14 ASEAN rice hubs (27 x 27 km each, 30 m pixels).
  Red = freshly planted, Orange = growing, Green = ready for harvest, Transparent = not rice / harvested / fallow.
- Timeline (bottom): steps through NISAR 12-day cycles (late Jun - early Nov 2026). Play/pause, prev/next, Latest.
  "Growth stage" mode = stage estimated using only images up to that date (from ~August).
  "Radar" mode = the raw false-colour radar image (R=HH, G=HV, B=HH).
- Confidence badge per region: whether its stage mix matches the local crop calendar.

CAVEATS
First estimates; not field-validated. Stage timing +/- 2-3 weeks. The rice test does not yet require a
flood signature, so some non-rice short-cycle crops may be included (esp. Isan, Ngawi).
NISAR data: NASA/JPL-Caltech, ISRO, ASF DAAC. Imagery: Esri, Maxar, Earthstar Geographics.
