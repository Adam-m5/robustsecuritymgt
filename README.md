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

This repository contains a pre-built static Single-Page Application (SPA) frontend that can be published to Netlify without adding build sources.

Location of the deploy-ready site in this repository:

- `site/` (renamed from `robust-security-mgmt-netlify-deploy (9)` for cleaner filesystem paths)
  - index.html (SPA entry that mounts into `#root`)
  - assets/ (compiled JS/CSS)
  - images/
  - favicon.png
  - _redirects

How to preview locally:

```bash
cd site
python -m http.server 8000
# or
npx serve -s .
```

## Netlify deployment

A root-level `netlify.toml` has been configured to publish the `site/` directory directly. This lets Netlify serve the pre-built files as-is without a build step.

To deploy:

1. Connect this repository to Netlify (via Netlify dashboard).
2. Netlify will automatically use the configuration in `netlify.toml` and publish `site/`.
3. The `_redirects` file ensures client-side routing works (all paths rewrite to `/index.html`).

If you later add source files (for example, `src/` and `package.json` with a `build` script that outputs to `dist/`), update `netlify.toml` to run the build:

```toml
[build]
  command = "npm run build"
  publish = "dist"
```

## GitHub Pages deployment (optional)

You can also publish to GitHub Pages by enabling it in repository settings and selecting the `gh-pages` branch.

## Next steps

- Add development source files (e.g., `src/` folder and `package.json`) if you want to rebuild or edit the app.
- Create a CI/CD workflow to run builds and deploy previews on pull requests.
- Customize error pages or add middleware if using a full-stack setup later.
