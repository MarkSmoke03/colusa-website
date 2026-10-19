# Colusa Investments Ltd. — Website

Corporate website for **Colusa Investments Limited**, a 100% Zambian-owned industrial contractor based in Kitwe, Copperbelt Province.

All content is taken from the approved Company Profile (Final Profile). Compliance figures must only be changed against the source certificates.

## Stack
Plain static site — `index.html`, `assets/css/styles.css`, `assets/js/main.js`. No build step, so it loads fast on mobile networks and deploys anywhere.

## Run locally
```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## Deploy
Every push to `main` deploys to GitHub Pages via `.github/workflows/pages.yml`
(Settings → Pages → Source: **GitHub Actions**).

## Custom domain (once purchased)
1. Add a `CNAME` file in the repo root containing the domain, e.g. `colusainvestments.co.zm`.
2. At the domain registrar, point the domain to GitHub Pages (A records `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`; `www` CNAME → `marksmoke03.github.io`).
3. Settings → Pages → Custom domain → enable **Enforce HTTPS**.

## Content to update
- Compliance register: `#compliance` section in `index.html` — update validity dates on renewal.
- Photos: `assets/img/` (keep under ~300 KB each).
