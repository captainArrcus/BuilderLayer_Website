# BuilderLayer Website

Minimal bilingual landing page for BuilderLayer, ready for GitHub Pages.

## Included

- Single-page website in `index.html`
- German and English language switch (DE/EN)
- Color theme aligned with the BuilderLayer pitchdeck
- Optional canonical redirect from `*.github.io` to your own domain

## Run Locally

Open `index.html` in your browser.

## Deploy On GitHub Pages

1. Push this repository to GitHub.
2. Open `Settings -> Pages`.
3. Set `Build and deployment` to:
	- Source: `Deploy from a branch`
	- Branch: your main branch
	- Folder: `/ (root)`
4. Save and wait for deployment.

## Forward To Your Own Domain

Use one of these options:

1. Preferred: Custom domain directly in GitHub Pages
	- Add your domain in `Settings -> Pages -> Custom domain`
	- Configure DNS at your registrar:
	  - `CNAME` for `www` to `<your-user-or-org>.github.io`
	  - For root domain (`example.com`), use your provider's `ALIAS/ANAME` or GitHub Pages A records

2. Optional: Force redirect from `github.io` to your domain
	- In `index.html`, set `CANONICAL_HOST` in the script section to your domain
	- Example: `const CANONICAL_HOST = "www.builderlayer.com";`