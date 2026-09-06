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

### 3. Domain
Live at **https://www.isikina.com/** — canonical tags, sitemap, robots.txt, and Open Graph tags all point here.

### 4. After that's live
- Submit the site to Google Search Console + Google Analytics (same steps as pngcasinoking.com).
- Every future push to the GitHub repo's `main` branch auto-redeploys — no manual redeploy step needed.

## Editing content later
The landing page's content is in `index.html` — bonus terms, WhatsApp link, FAQ text, and games list are all plain HTML you (or I) can edit directly. If Isikina's bonus terms or minimum deposit/withdrawal ever change, update them here to keep this page accurate.

## Blog
- `css/site.css` — shared styling for every page (landing page + blog), so new pages stay visually consistent without copy-pasting a big style block each time.
- `blog/index.html` — the blog listing page.
- `blog/<slug>.html` — one file per post.
- `keywords.csv` — upcoming keyword ideas for future posts (Isikina-brand and how-to-use angles, deliberately different from the generic PNG-casino terms pngcasinoking.com already targets, to avoid the two sites competing against each other in search).
- `used-keywords.md` — tracks which keywords are already live and where, so a future post doesn't duplicate one that already exists.

To add a new post: pick the next keyword from `keywords.csv`, write a new `blog/<slug>.html` (copy the structure of `blog/how-to-join-isikina-casino.html` — title/meta/OG tags, breadcrumb, TOC, FAQ with matching JSON-LD), add a card for it to `blog/index.html`, add its URL to `sitemap.xml`, and mark the keyword "Live" in `used-keywords.md`.
