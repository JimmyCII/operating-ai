# Operating AI — The Series (flipbook)

A self-hosted, page-flip flipbook of the four-part "Operating AI" series by Jim Cockerham.
Built from `Operating_AI_Series_Booklet_v2.pdf` (cover → contents → four articles, 17 pages).

**Live:** https://jimmycii.github.io/operating-ai/

## Contents
- `index.html` — the flipbook viewer (StPageFlip, vanilla JS)
- `pages/` — page images (`page-01.jpg` … `page-17.jpg`)
- `cover.jpg` — share-card thumbnail (page 1)
- `lib/page-flip.browser.js` — vendored flip library (no external CDN)
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Publish (one time)

1. On GitHub, create a new **public** repo named **`operating-ai`**.
2. From this folder, push it:
   ```bash
   git remote add origin https://github.com/jimmycii/operating-ai.git
   git branch -M main
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Source: Deploy from a branch → `main` / `root` → Save.**
4. Wait ~1 minute. Live at **https://jimmycii.github.io/operating-ai/**

> If you name the repo something other than `operating-ai`, update the three absolute
> `og:`/`twitter:` URLs in `index.html` (and the link above) to match the new path,
> so the Facebook/LinkedIn share card shows the right cover.

## Updating the book later
Replace the images in `pages/` (and `cover.jpg`), then `git commit` and `git push`.
