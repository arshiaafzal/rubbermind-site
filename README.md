# rubbermind.ai

Landing page for Rubber Mind, served by GitHub Pages at https://rubbermind.ai.

Everything lives in `index.html` (styles and scripts are inline). The hero: `foreground.webp` is the woven rubber planet and the seated figure, cut out of the 6K artwork and graded to grayscale. Everything behind it (the rubber filament stream, galaxies made of rubber strands, loose strings, stars) is drawn live on a canvas in `index.html`.

Palette: black, white and grays only, plus the light blue of the scarf and faint ice-blue wave highlights.

Images: `logo.png` (256px badge), `logo-512.png` (hi-res), `favicon.png` / `favicon-32.png`, `apple-touch-icon.png`, `og.png` (social preview), all made from `pingo-source.png`.

## Edit and preview

```sh
git clone https://github.com/arshiaafzal/rubbermind-site.git
cd rubbermind-site
python3 -m http.server 8000   # open http://localhost:8000
```

## Deploy

Push to `main`. GitHub Pages redeploys automatically in about a minute.

```sh
git add -A && git commit -m "Update site" && git push
```

## Do not change

- `CNAME`: must contain `rubbermind.ai`, or the custom domain detaches.
- `.nojekyll`: serves files as-is.
- DNS lives in Squarespace (Domains → rubbermind.ai → DNS): four `A @` records to `185.199.108.153`–`185.199.111.153` and `CNAME www` → `arshiaafzal.github.io`.
