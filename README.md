# JEMD Digital Twin Research Dashboard

A polished, responsive portfolio demonstrator for a simulation-led industrial chimney design workflow. It maps the advertised KTP themes into an interactive digital-twin interface: parametric geometry, FEM evidence, Eurocode-oriented verification, DOE/AI optimisation, traceable run records, and stage-gate project control.

> **Important:** This is an independent portfolio demonstrator, not an official University of Derby, James Engineering, or JEMD product. All values are simulated and simplified. It is not suitable for engineering design, certification, or compliance decisions.

## Features

- Interactive chimney digital twin with wind-scenario control
- Stress/modal display modes and condition indicators
- FEM-to-analytical evidence chain and verification gate
- Eurocode-oriented design-check workflow
- Multi-objective optimisation and Pareto-candidate summary
- Traceable simulation run register with JSON export
- KTP stage-gate, KPI, validation, and delivery-control concepts
- Responsive dark industrial UI with no data API required
- GitHub Pages deployment workflow

## Technology

- React 19 + Vite
- lucide-react icons
- CSS/SVG visualisation, with no charting runtime
- GitHub Actions for Pages deployment

## Run locally

```bash
npm install
npm run dev
```

Open the local URL printed by Vite.

## Production check

```bash
npm run build
npm run preview
```

## Push to GitHub

```bash
git init
git add .
git commit -m "Add JEMD digital twin dashboard"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/jemd-digital-twin-dashboard.git
git push -u origin main
```

Then open **Settings → Pages → Build and deployment → Source** and choose **GitHub Actions**. The included workflow builds and deploys the site.

## Suggested interview walkthrough

1. Start with the evidence banner to establish engineering governance.
2. Change wind speed to show the live utilisation and risk response.
3. Explain the analytical-to-FEM-to-code verification chain.
4. Discuss DOE/RSM/ML as surrogate-assisted optimisation, never as a substitute for verification.
5. Export the run record to demonstrate traceability.
6. Close with the KTP stage-gate panel and knowledge-transfer plan.

## Proposed technical architecture

```text
Validated inputs → Parametric geometry → FEM solver adapter
                 → Analytical/code checks → Results schema
                 → DOE/RSM/ML optimiser → Decision-support UI
                 → versioned calculation record + audit trail
```

A production implementation should add authenticated APIs, a units library, schema validation, solver adapters, uncertainty quantification, test fixtures, role-based access, signed calculation records, materials databases, and independently verified Eurocode rules.

## References

- University of Derby vacancy 0280-26, FEM, Design & AI/ML Optimisation Engineer (KTP Associate)
- European Commission JRC Eurocodes portal, EN 1993 family
- BS EN 1993-3-2:2006, Towers, masts and chimneys — Chimneys

## Licence

MIT for the demonstrator source. Third-party marks and standards remain the property of their respective owners.
