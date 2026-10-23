# TagLink – tag-centric change control (concept)

Single-file concept web app (`index.html`, no build). Open it in a browser.

An equipment tag is the common reference across SmartPlant Foundation, Smart 3D, Smart Cloud, HxGN SDx2 and third-party / construction / maintenance systems. A controlled change (e.g. motor 250 → 315 kW) is approved by the affected disciplines, then propagated: mapped records auto-sync, everything else becomes a task. Nothing is claimed correct until an engineer signs off.

## Portfolio → project
- **Portfolio home:** KPI tiles across all projects, searchable project tiles (name, code, commodity, location, lead, stage), health filter (At risk / Watch / On track), sort, cross-project "needs my attention" list, cost by project, recent activity, **+ New project**
- Six illustrative projects: Eskay Creek, Blackwater, North Island, Copper Ridge, Salar Norte, Mount Halcyon. Each has its own tags, integrations, approval matrix, changes, inbox and audit trail
- Selecting a project reveals its tabs

## Project tabs
- **Dashboard**, **Change control** (single or bundled multi-tag changes, approvals, consistency gate, close-out tasks), **Impact analysis**, **Integration**, **Project & asset**, **Activity & data**
- Close-out tasks use **discipline checklists with limits** (cable derating, voltage drop, clash clearance, crane utilisation…), a measured value checked against the limit, and a **required evidence reference** in the right format (calc revision, clash report ID, CMMS work order…)
- **Change pack** (HTML → print to PDF) opens with a **cover page**: document number, revision, impact summary and a **signature block per approving discipline**; plus CSV register export
- Auto-save in the browser, JSON backup/restore of the whole portfolio

Illustrative only. No real Hexagon APIs, data or Ausenco process; project names are examples, rates and prices are made up. Multi-user login, roles and shared data are intentionally not built (a hosted backend such as Supabase is the planned next step).
