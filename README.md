# gshitesh.github.io

Personal portfolio for **Sai Hitesh Gorantla** — Software Engineer specializing in developer platforms, backend systems, infrastructure automation, and CI/CD.

Single-page site. Pure HTML + CSS + a sprinkle of vanilla JS. **No build step, no dependencies.**

Live: [gshitesh.github.io](https://gshitesh.github.io/)

## Structure

- `index.html` — the entire site (styles and scripts inline). Sections:
  1. Hero + impact stats
  2. `#featured` — Featured Engineering Work (case studies)
  3. `#work` — Experience
  4. `#caps` — Capabilities
  5. `#archive` — Education & certifications
  6. `#contact` — Contact
- `Sai-Hitesh-Gorantla-Resume.pdf` — résumé served directly from the site (hero button + `⌘K` palette).
- `og.png` / `og.svg` — social share image (1200×630). `og.svg` is the editable source; `og.png` is what platforms render.
- `favicon.svg`, `404.html`, `robots.txt`, `sitemap.xml` — supporting assets and SEO.
- `.github/workflows/deploy.yml` — GitHub Pages deploy workflow.

## Local preview

Open `index.html` in any modern browser, or:

```sh
python -m http.server 8080
```

## Updating the résumé

Replace `Sai-Hitesh-Gorantla-Resume.pdf` with a new export (keep the same filename so the links stay valid).

## Regenerating the social image (`og.png`)

Edit the text in `og.svg`, then rasterize it to a 1200×630 PNG named `og.png` (e.g. via a headless browser or an SVG-to-PNG tool). Keep both in sync so link previews match the site.

## Deploy

The GitHub Actions workflow in `.github/workflows/deploy.yml` publishes to GitHub Pages on every push to `main`. Enable Pages with **Source: GitHub Actions** in repo settings.
