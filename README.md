# Luna Vex

Model portfolio for Luna Vex — React single-page site with a purple/cyan
gradient identity.

Single file, no build step. React 18 + Babel standalone run straight from
CDN, so there is nothing to install and nothing to break.

## Stack

- **React 18** (UMD) — components and state
- **Babel standalone** — JSX transpiled in the browser
- **Playfair Display** — display serif
- **Bebas Neue** — heading accents
- **Inter** — body copy
- **Font Awesome 6.4** — icons
- **Tailwind CSS** (CDN) — layout

## Sections

1. **Hero** — mouse-tracked 3D tilt on the portrait, glowing gradient orbs
2. **About** — image grid with stat card, skill tags
3. **Stats** — `IntersectionObserver` number counters (150+ shoots, 50+ brands)
4. **Portfolio** — filterable grid (editorial / fashion / lifestyle) with lightbox modal
5. **Contact** — booking form with success state
6. **Footer**

## Features

- Animated gradient background + 20 floating particles
- Scroll-triggered reveal animations with staggered children
- Category filtering with active-state pills
- Lightbox modal with backdrop blur
- Sticky nav that solidifies on scroll, plus a mobile menu
- Booking form with in-button success confirmation
- All images served from Unsplash with verified-live URLs

## Image sourcing

All images are Unsplash URLs, each verified to return HTTP 200 before
deploy. The original design referenced `i.ibb.co` uploads that now 404 —
those were replaced with equivalent Unsplash photography.

## Deploy

Pushed to GitHub Pages on every commit to `main`. See
`.github/workflows/deploy.yml`.

## Local preview

Because it uses Babel standalone, opening `index.html` via a local server
works as-is:

```bash
python -m http.server 8080
# then open http://localhost:8080
```