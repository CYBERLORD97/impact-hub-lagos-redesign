# Impact Hub Lagos — Redesigned Homepage

A redesigned homepage for **Impact Hub Lagos** — the critical infrastructure for Nigeria's
innovation economy — rebuilt in the neo-brutalist design language of **CcHUB Design Lab**
(bright pastel pills, hard black borders, hard offset shadows, near-black hero stage),
while keeping Impact Hub Lagos's own brand, content and assets.

## Design system (adapted from CcHUB Design Lab)

- **Hero stage**: near-black (`#020202`) with real brand hero photo
- **Accents**: Impact Hub brand pastels — `#FFD546` yellow, `#F78A3C` orange, `#41BED0` teal, `#7EBB55` green, plus CcHUB pastels (`#E8C2E2`, `#FFDAC0`)
- **Shape language**: 999px pill buttons on 2px black borders, `0 6px 0 #000` hard offsets
- **Typography**: Poppins (local woff2, embedded at `assets/fonts/`)
- **Content**: real Impact Hub Lagos facts — spaces & ₦ pricing, programmes (SHEPitch, We Can Work Academy, Africa Climate Finance Day), 2020–2025 Impact Report, partner logos, 500k+ network figures

## Files

```
index.html        # the homepage (self-contained)
assets/
  fonts/          # Poppins woff2 (local)
  logos/          # IHL red/white logo (from the live site)
  images/         # hero, spaces, report cover, founder card
  partners/       # the 20 real partner logos
```

## Run locally

Any static server, e.g.:

```bash
npx serve impact-hub-lagos-redesign
# or  python3 -m http.server --directory impact-hub-lagos-redesign 8080
```

Open `index.html` directly in a browser — all assets are relative paths and there are no external dependencies.

## Deploy to GitHub Pages

1. Create a repo (e.g. `impact-hub-lagos-redesign`) and push this folder:

   ```bash
   cd impact-hub-lagos-redesign
   git init
   git add .
   git commit -m "Redesigned homepage — CcHUB design language"
   git remote add origin https://github.com/<you>/impact-hub-lagos-redesign.git
   git branch -M main
   git push -u origin main
   ```

2. In the repo settings → Pages → source: **Deploy from a branch → main / (root)**
3. Your site goes live at `https://<you>.github.io/impact-hub-lagos-redesign/`

## Notes

- Images/logos are the live Impact Hub Lagos site's own files (real photography and real partner logos).
- ₦ pricing is real, as published at lagos.impacthub.net. All prices exclude VAT.
- The newsletter form is front-end only (no backend).
