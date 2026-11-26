# Nova SaaS — Demo Deployment Guide

A public demo URL is required by the marketplace listing process described to the seller. This package contains the demo files but does not host them.

## Option: GitHub Pages

1. Sign in to GitHub and create a new **public** repository, for example `nova-saas-demo`.
2. Upload the contents of this `nova-saas` folder to the repository root. The `index.html` file must be at the root level (not buried inside another folder).
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then save.
6. Wait for the deployment to finish. GitHub will display the public demo URL in the Pages section.
7. Open the URL in a private/incognito browser window and test both languages, the navigation, pricing/FAQ anchors, mobile layout, contact link, and Back to top.
8. Paste the verified URL into the Zhaket product form.

## Before sharing the demo

- Keep only the demo website files in the public repository. Do not upload private credentials, account exports, or unrelated project files.
- The demo is a static front-end preview. It does not provide real login, payments, subscriptions, analytics, or server-side form processing.
- Keep the downloadable customer ZIP separate from any private development repository if it contains work-in-progress files.
- A public GitHub Pages demo exposes the files served by the site. It is a preview, not source-code protection. If the marketplace requires a different demo host or access mode, follow its current instructions.
