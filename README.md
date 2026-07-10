# Yudhistira Onggowarsito — Portfolio

A fast, responsive, single-page portfolio site. Pure HTML/CSS/JS — **no build step**, so it deploys to Vercel with zero configuration.

## Structure

```
portfolio/
├── index.html      # all page content
├── styles.css      # theme, layout, animations (light + dark)
├── main.js         # theme toggle, scroll reveal, project filters
├── favicon.svg     # gradient "YO" monogram
├── vercel.json     # security headers + clean URLs
└── Yudhistira_Onggowarsito_Resume.pdf   # ← replace this placeholder
```

## Deploy to Vercel

**Option A — drag & drop (fastest)**
1. Go to [vercel.com/new](https://vercel.com/new).
2. Drag this `portfolio` folder onto the page (or zip it and upload).
3. Framework preset: **Other**. Click **Deploy**. Done.

**Option B — Vercel CLI**
```bash
npm i -g vercel
cd portfolio
vercel          # preview deploy
vercel --prod   # production deploy
```

**Option C — Git + Vercel (recommended for updates)**
1. Push this folder to a GitHub repo.
2. In Vercel, **Add New → Project → Import** the repo.
3. Framework preset: **Other**, Root Directory: repo root. **Deploy.**
   Every future `git push` auto-deploys.

## Before you publish — quick checklist

- [ ] **Résumé:** replace `Yudhistira_Onggowarsito_Resume.pdf` with your real CV (keep the exact filename, or update the link in `index.html`).
- [ ] **LinkedIn:** the link points to `linkedin.com/in/yudhistira-onggowarsito` — update it in `index.html` (hero + contact) if your handle differs.
- [ ] **Custom domain (optional):** add one in Vercel → Project → Settings → Domains.

## Editing content

All projects live in `index.html` inside `<article class="card" data-cat="...">` blocks.
Set `data-cat="aiml"` or `data-cat="fullstack"` so the filter buttons work.

## Local preview

Just open `index.html` in a browser, or serve it:
```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```
