# Kim planning board

Static swimlane Kanban planning board for The Missionary Company.

**Live:** https://the-missionary-company.github.io/planning-board/

## App (v3)
- Source of truth (full app): develop locally from full HTML; Pages serves a gzip base64 part loader
- Persistence key: `tmc-plan-board-v3` (merges seed defaults with local overrides by task id)
- Board default: topic swimlanes × status columns (Backlog → Done)
- Editable topic / epic / status (dropdown + drag); protect flag; LOE + decision memo

## Deploy shape
`index.html` is a tiny loader that fetches `parts/v3g0.b64` … `parts/v3g9.b64`, gunzips, and `document.write`s the real app.
