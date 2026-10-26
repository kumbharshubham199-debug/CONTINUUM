# CONTINUUM — Coordinator Demo Guide

## One-sentence project description
CONTINUUM is a student-level manufacturing process management prototype that connects inventory, planning, production, quality, process inspection and dispatch, while retaining production-loss and machine-maintenance history.

## Approved six-module workflow
Inventory → Planning → Production → Quality → Process & Inspection → Dispatch

Maintenance is a supporting function inside Production, not a seventh main module.

## Suggested 5-minute demonstration
1. Sign in with a display name and choose a demonstration role.
2. Open Inventory and add a raw material with a quantity and minimum stock level. Use **+ Stock** and **Use** to demonstrate stock movement.
3. Open Planning and create a plan, for example Product A, planned quantity 500.
4. Open Production and record actual output 350. The app calculates 150 units of production loss.
5. Add a machine, then record a breakdown linked to the production run. Show the maintenance status and repair completion date. The production run and breakdown history remain saved after repair.
6. Add a Quality check with accepted/rejected quantities, then add a **Final inspection** stage with result **Passed**.
7. Open Dispatch. Only production runs with a Passed quality check and Passed final inspection are available. Dispatch quantity is checked against accepted quantities.
8. Open Settings & Data and export a JSON backup.

## Important technical statement
This is a browser-only academic prototype using HTML, CSS, vanilla JavaScript and localStorage. It has no backend or PostgreSQL. Its role picker is for classroom demonstration, not secure authentication. Data is stored in the current browser and is not automatically shared between computers. Export JSON backups regularly.

## Before the presentation
- Open `login.html` using VS Code Live Server or another local static server.
- Test the steps above once with fresh data.
- Export a backup if you want to preserve your demonstration records.
- Do not enter real company confidential information or real passwords.
