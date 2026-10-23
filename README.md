# TagLink – tag-centric change control (concept)

Single-file concept web app (`index.html`, no build). Open it in a browser.

Demonstrates: an equipment tag as the common reference across SmartPlant Foundation, Smart 3D, Smart Cloud, HxGN SDx2 and third-party tools; a controlled change (e.g. motor 250 → 315 kW) with discipline approvals; and an impact register that shows what propagates automatically versus what is flagged, needs engineer re-verification, or is not linked at all.

Key honesty rule built into the model: propagation depends on which apps are linked, attribute mappings and approval gates. Derived calcs are never auto-corrected.

Illustrative only. No real Hexagon APIs or data.

## Features
- Baseline → proposed diff per linked record, plus cost / schedule impact (illustrative rates)
- Configurable approval matrix (always / when impacted / never, plus % escalation rule)
- Isometric 3D view (baseline / proposed / overlay), per-role notification inbox, CSV/JSON tag import
- Dark and light hex-grid skins; BoM → requisition → PO procurement path with close-out task sign-off

## Architecture-aligned features
- Connected data architecture view (authoring → SDx exchange → data backbone → procurement / project / operations), click to link/unlink, packets animate on implementation
- Six lifecycle domains (design, technical, procurement, project, construction, asset) with new construction and maintenance records and a CMS integration
- Relationship graph (where-used cascade) and a pre-flight consistency check that gates implementation
- Lifecycle stage multiplies change cost and can force Construction approval
- Data exchange monitor, revision bumps, asset as-built history, handover readiness, project change register
