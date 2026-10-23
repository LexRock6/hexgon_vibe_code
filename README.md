# TagLink – tag-centric change control (concept)

Single-file concept web app (`index.html`, no build). Open it in a browser.

An equipment tag is the common reference across SmartPlant Foundation, Smart 3D, Smart Cloud, HxGN SDx2 and third-party / construction / maintenance systems. A controlled change (e.g. motor 250 → 315 kW) is approved by the affected disciplines, then propagated: mapped records auto-sync, everything else becomes a task. Nothing is claimed correct until an engineer signs off.

## Layout
- **Dashboard**: KPI tiles, my to-do (approve from here), impact mix, lifecycle stages, integration health, open change requests, consistency alerts, cost by tag, handover readiness, recent activity
- **Change control**: tags, raise single or **bundled multi-tag** change, approvals, consistency gate, close-out tasks with **engineer checklists** and sign-off notes
- **Impact analysis**: tag hub graph and cascade, baseline → proposed register, lifecycle domains, cost/schedule, 3D view
- **Integration**: architecture view, data exchange monitor, link/mapping toggles, approval matrix
- **Project & asset**: change register, procurement path, as-built history and handover readiness
- **Activity & data**: inbox, audit trail, **change-pack export (HTML/CSV)**, **auto-save + JSON backup/restore**, tag import

Illustrative only. No real Hexagon APIs, data or Ausenco process; rates and prices are made up.
