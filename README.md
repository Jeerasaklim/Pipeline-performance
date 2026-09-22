# Pipeline Performance Tracking — static frontend

Public static frontend served by GitHub Pages. It is **auth-gated**: all data
loads from a Google Apps Script Web App backend **only after Google sign-in
(@cjmart.co.th)**; the backend verifies the Google token server-side.

## Files
- `index.html` — redirect to `live_dashboard.html`
- `live_dashboard.html` — main dashboard (loads live data via GAS after login)
- `CJX_Map_Prototype.html` — Site Management map, embedded by the dashboard via iframe

No business data is baked into these files (site details, notes, PIC and cost
were removed at build time). This repo contains **static frontend only** — no
build scripts, no Apps Script (`.gs`), no source modules, no data files.
