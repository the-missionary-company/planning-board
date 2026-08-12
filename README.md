# Kim planning board

Temporary interactive Thu–Fri planning UI for Liam/Sam Sung (Asia/Seoul).

Live URL (GitHub Pages): https://the-missionary-company.github.io/planning-board/

## Open

No build step. Open the file in a browser:

- Double-click `index.html`, or
- From a terminal: `xdg-open /workspace/planning-board/index.html` (Linux) / `open index.html` (macOS)
- Or serve locally if your browser blocks `file://` localStorage quirks:  
  `python3 -m http.server 8765 --directory /workspace/planning-board`  
  then visit `http://localhost:8765`

## Views

**Tasks** is the default landing view: full-width board grouped by area (Central Hub first), with per-group minutes, overall protect minutes, drag-to-reorder within a group, and click-through to the detail drawer.

**Calendar fit** keeps the 3-column layout (Big rocks | Thu/Fri calendar | Parking) for drag-into-slots, Suggest fit, and capacity checks.

## Features

- Dark single-file HTML + CSS + JS
- Two-view toggle in the header (Tasks default · Calendar fit)
- Drag work cards into free calendar slots (or parking)
- Fixed calendar blocks are not draggable (incl. Thu **CFT prep / family morning** 07:00–08:30 before clinic)
- **Suggest fit** packs `protect` items into earliest free slots (greedy) — Calendar fit view
- Persists to `localStorage` key `tmc-plan-board-v1` (same data model; Tasks order stored as `boardOrder`)
- Reset restores defaults

## Free windows (KST, evening end 21:00)

Thu morning is busy through clinic start: CFT + family/breakfast/Bible until ~08:30, then errands 08:30–11:15.

**Thu Aug 13:** 11:15–12:00 (45m), 14:00–16:00 (120m), 16:30–21:00 (270m) → **435m**  
**Fri Aug 14:** 08:30–12:00 (210m), 14:00–15:00 (60m), 19:00–21:00 (120m) → **390m**
