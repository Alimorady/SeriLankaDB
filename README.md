# Wee Oya Reservoir — Project Document & Study Map

Interactive, trilingual (فارسی / English / සිංහල) web map of the documents and studies
produced for the **Wee Oya Reservoir** project — a concrete arch dam on the Wee Oya river
(Kelani Ganga basin, Sri Lanka).

It visualises the three-stage consultant chain, the reports each company produced, their
dates, and how they relate to one another.

## Consultant chain

| Phase | Company | Period | Scope |
|---|---|---|---|
| 1 — Pre-Feasibility (DBIP) | Atkins Int'l + GreenTech | 2015–2019 | Whole Kelani basin risk assessment, TUFLOW/SWAT models |
| 2 — Feasibility | CECB (Sri Lanka) | 2019–2021 | Site-scale studies, Option 3 selected (FSL 129, 59.5 MCM, 5 MW) |
| 3 — Detailed Design | Mahab Ghodss (MGCE, Iran) | 2025–2026 | Dam break study, HEC-RAS 2D, EAP, tender documents |
| 4 — Construction | Contractor | Future | International competitive bidding |

## View locally

Open `index.html` in any modern browser. The page is fully self-contained
(one HTML file; the Sinhala font is loaded from Google Fonts when online).

## View online (GitHub Pages)

1. Push this repository to GitHub.
2. Settings → Pages → Branch: `main`, folder `/ (root)` → Save.
3. The site goes live at `https://<username>.github.io/<repo>/`.

## Update workflow (patch & push)

This site is updated layer by layer as the studies progress, using a
**patch-and-push** cycle:

1. A unified diff (`*.patch`) is prepared against the current `index.html`.
2. Apply it locally:
   ```bash
   git apply update.patch
   ```
3. Review, commit and push:
   ```bash
   git add -A
   git commit -m "Layer N: <description>"
   git push
   ```

## Status

- **Layer 1 (current):** Document inventory — companies, reports, dates, relationships.
- Next layers: deeper content extraction, data tables, maps, and study results.

---
*Prepared with Cowork · Mahab Ghodss Consulting Engineering — Detailed Design team.*
