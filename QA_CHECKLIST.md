# CONTINUUM — Manual QA Checklist

Run these checks in a modern browser before presenting. The project is a classroom prototype, not a production ERP system.

- [ ] Login screen opens and enters the dashboard.
- [ ] Sidebar links open all six modules and Settings & Data.
- [ ] Add, edit, search and delete an inventory item.
- [ ] Add stock and use stock; stock cannot be reduced below zero.
- [ ] Create a production plan.
- [ ] Create a production run linked to the plan.
- [ ] Verify planned 500 and actual 350 gives loss 150.
- [ ] Verify actual output above plan does not create negative loss.
- [ ] Add a machine and record a breakdown linked to a production run.
- [ ] Mark the breakdown repaired and verify its historical record remains visible.
- [ ] Add a Passed quality check and a Passed Final inspection.
- [ ] Verify dispatch does not offer runs without both approvals.
- [ ] Verify dispatch quantity cannot exceed accepted approved quantity.
- [ ] Export JSON and check that a `.json` file downloads.
- [ ] Clear data only if appropriate, then import the exported JSON and confirm records return.
- [ ] Try importing invalid JSON; the app should show an error instead of replacing data.
- [ ] Refresh the browser and confirm localStorage records remain.
- [ ] Test at desktop and mobile width.

If a check fails, note the page and action. Do not claim the check passed until it has actually been run in a browser.
