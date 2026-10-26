# CONTINUUM — Integrated Manufacturing Process Management System

**Academic prototype built using HTML, CSS and vanilla JavaScript.**

## Pages
- `login.html` — demo entry screen (no real passwords)
- `index.html` — dashboard with saved-data metrics and recent activity
- `inventory.html` — raw materials, minimum stock, add/use stock, search and records
- `planning.html` — production plans and material-availability indicator
- `production.html` — production runs, planned vs actual output, calculated loss, machines and maintenance history
- `quality.html` — inspected, accepted and rejected quantities, defect reasons and quality status
- `inspection.html` — process stages, inspection result and final approval
- `dispatch.html` — dispatch only from runs with passed quality and passed final inspection
- `settings.html` — JSON export/import, demo role selection, data summary and clear-data action
- `style.css` — shared responsive design
- `app.js` — shared navigation, forms, calculations, localStorage and validated JSON import/export
- `COORDINATOR_DEMO_GUIDE.md` — suggested presentation flow
- `QA_CHECKLIST.md` — manual testing checklist

## Run locally
1. Extract this ZIP.
2. Open the extracted folder in VS Code.
3. Use VS Code Live Server if available, then open `login.html` in your browser.
4. Enter a display name and choose a demo role.
5. Create records in each module. Use Settings & Data to export a JSON backup.

Opening the HTML file directly in a modern browser may also work, but a local static server is recommended for a consistent demo.

## Approved workflow
Inventory → Planning → Production → Quality → Process & Inspection → Dispatch.

Maintenance is a supporting function inside Production, not a seventh main module.

## Data and security limitations
- No Python, PostgreSQL, Node.js, React, TypeScript or backend is used by this prototype.
- Records are stored in the current browser's `localStorage`; they are not shared across devices.
- The role picker is only for classroom demonstration. It is not secure authentication or server-side role enforcement.
- Do not store real passwords or confidential company data.
- Clearing browser storage can erase records. Export JSON backups regularly.
- This is an academic prototype, not a production-ready ERP system.

## Before presenting
Follow `COORDINATOR_DEMO_GUIDE.md` and work through `QA_CHECKLIST.md`. Only mark a test as passed after testing it in the browser.
