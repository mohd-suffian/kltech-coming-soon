# kltech-coming-soon

Placeholder page for kltech.my. Plain HTML + one CSS file. No JavaScript, no build step.

Files: index.html, assets/style.css, assets/fonts/, favicon.svg, CNAME (for GitHub Pages), .nojekyll.

## Option A: GitHub Pages (no server, works from a tablet)
1. GitHub > New repository > name `kltech-coming-soon`, Public (Pages on private repos needs a paid plan) > upload all files here (keep the folder structure; include `CNAME` and `.nojekyll`).
2. Repo > Settings > Pages > Source: "Deploy from a branch", Branch `main` / root > Save.
3. Same page > Custom domain: `kltech.my` > Save. Tick "Enforce HTTPS" once it becomes available (can take up to an hour after DNS works).
4. Hostinger DNS (change web records only, never MX/TXT/mail):
   - A @ -> 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153 (4 records, TTL 300)
   - delete AAAA @ (or use GitHub's IPv6 addresses from the docs)
   - CNAME www -> mohd-suffian.github.io (delete any existing www record first)
   - Confirm the IPs against GitHub's current docs before saving.

## Option B: Hetzner
Copy index.html, assets/ and favicon.svg into the `public/` folder of klt-website, then follow its README.
