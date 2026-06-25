# Adept Style — Salon Website

Redesigned single-page website for **Adept Style Unisex Salon** (Dartford & Plumstead, London). Premium light theme, online-booking-first, with per-barber booking links, team, gallery, locations, hours and loyalty.

The site is a single self-contained `index.html` — all styles, fonts and scripts are inlined, so it works offline and needs **no build step**.

## Deploy to Vercel

**Option A — drag & drop**
1. Go to [vercel.com/new](https://vercel.com/new).
2. Drag this folder in (or import the GitHub repo below).
3. Framework preset: **Other**. Leave build & output settings empty.
4. Deploy. Vercel serves `index.html` as a static site.

**Option B — Vercel CLI**
```bash
npm i -g vercel
cd deploy
vercel        # preview
vercel --prod # production
```

## Push to GitHub

```bash
cd deploy
git init
git add .
git commit -m "Adept Style website redesign"
git branch -M main
git remote add origin https://github.com/<you>/adept-style.git
git push -u origin main
```

Then on Vercel: **New Project → Import Git Repository** and pick the repo. Every push to `main` auto-deploys.

## Local preview

Just open `index.html` in a browser, or:
```bash
npx serve .
```

## Files
- `index.html` — the entire website (self-contained)
- `vercel.json` — static hosting config + security headers
- `.gitignore`
- `README.md`

## Editing
`index.html` is a compiled bundle and not meant to be hand-edited. To make changes, update the source design and re-export.

## Notes
- Booking buttons link to the live booking pages on adeptstyle.co.uk.
- Photos are loaded from the salon's existing media. Swap in your own URLs to self-host them.

© 2014–2026 Adept Style Salon.
