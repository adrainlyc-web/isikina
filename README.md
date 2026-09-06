# Isikina Landing Page

A single-page marketing site for Isikina (WhatsApp-based 918Kaya deposit agent, Papua New Guinea). Plain static HTML/CSS, no build step, no framework — deploys directly to Vercel.

## What's in here
- `index.html` — the whole page (hero, how it works, bonuses, games, FAQ, WhatsApp CTAs)
- `images/` — the Isikina logo, favicon, and social-share image
- `robots.txt`, `sitemap.xml` — basic SEO plumbing
- `vercel.json` — tells Vercel this is a plain static site (no framework to detect)

## How to put this online (step by step)

### 1. Push this folder to GitHub
1. Go to [github.com/new](https://github.com/new), create a new **public** repository (e.g. `isikina-landing`). Don't add a README/gitignore — this folder already has one.
2. Come back here and tell me the repo URL — I'll push the code for you (I'll need a GitHub Personal Access Token from you at that point, same as we've done for pngcasinoking).

### 2. Import into Vercel
1. Go to [vercel.com/new](https://vercel.com/new).
2. Click **Import** next to the GitHub repo you just created.
3. Framework Preset: leave as **Other** (the `vercel.json` file already forces this).
4. Click **Deploy**. Vercel gives you a free `something.vercel.app` URL immediately.

### 3. Buy your domain later (through Vercel)
When you're ready:
1. In the Vercel project → **Settings → Domains**.
2. Type the domain you want (e.g. `isikina.com`) and follow the "Buy" flow — Vercel becomes the registrar, same as pngcasinoking.com.
3. Once bought, tell me the final domain and I'll update the placeholder `isikina.vercel.app` URLs in the code (canonical tag, sitemap, robots.txt, Open Graph tags) to match.

### 4. After that's live
- Submit the site to Google Search Console + Google Analytics (same steps as pngcasinoking.com).
- Every future push to the GitHub repo's `main` branch auto-redeploys — no manual redeploy step needed.

## Editing content later
Everything is in one file, `index.html` — bonus terms, WhatsApp link, FAQ text, and games list are all plain HTML you (or I) can edit directly. If Isikina's bonus terms or minimum deposit/withdrawal ever change, update them here to keep this page accurate.
