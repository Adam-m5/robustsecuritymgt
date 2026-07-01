# Robust Security Management System - Cashbook & Financial System

Complete financial accountability for Robust Security — track inflows, outflows, staff payroll, site deployments and more in one secure platform.

## Live Demo

The application is live at: [https://robustsecuritymgtsystem.netlify.app/admin](https://robustsecuritymgtsystem.netlify.app/admin)

## Features

- Daily Cash Book & Receipts
- Bank Reconciliation & Wire Deposits
- Staff Payroll & Site Deployments
- Audit Trails & Accountability Forms

## Access

To access the system, please visit the admin login page and use your authorized credentials.

For any support or access issues, please contact:

- **Phone:** +256 750555114 / +256200920601 /+256783122579

## About

This system is developed for **Robust Security (U) Ltd** to manage and oversee all financial operations with complete transparency and accountability.

© 2026 Robust Security (U) Ltd

---

## Deployment / Static site in this repository

This repository also contains a pre-built static Single-Page Application (SPA) frontend that can be published to Netlify without adding build sources.

Location of the deploy-ready site in this repository:

- robust-security-mgmt-netlify-deploy (9)/
  - index.html (SPA entry that mounts into `#root`)
  - assets/ (compiled JS/CSS)
  - images/
  - favicon.png
  - _redirects
  - netlify.toml (if present inside the folder)

How to preview locally:

```bash
cd "robust-security-mgmt-netlify-deploy (9)"
python -m http.server 8000
# or
npx serve -s .
```

Quick Netlify publishing (no build):

A root-level `netlify.toml` is included to publish the existing static folder directly. This lets Netlify serve the pre-built files as-is without running a build step.

If you later add source files (for example, `src/` and `package.json` with a `build` script that outputs to `dist/`), update `netlify.toml` to run the build and publish the built output directory.

## Notes / Next steps

- The repository currently does not include original build sources (e.g., `src/`, `package.json`). Add them if you want to rebuild or edit the app.
- Consider renaming `robust-security-mgmt-netlify-deploy (9)` to a filesystem-friendly name (e.g., `site/` or `dist/`) to simplify tooling.
- I can help: (1) rename the deploy folder and update netlify.toml, or (2) add a minimal `package.json` and build script — tell me which you'd prefer.
