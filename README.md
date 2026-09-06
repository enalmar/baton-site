# Baton — website

Marketing site for [Baton](https://enalmar.github.io/baton-site/), a macOS menu
bar app that hands Magic peripherals between Macs.

Plain static HTML, no build step. Served by GitHub Pages from `main` at the
repository root.

## Editing

- `index.html` — the whole landing page.
- `assets/site.css` — one stylesheet, one type scale, one 4px spacing scale.
- `privacy/`, `support/`, `license/` — supporting pages.

Two things need filling in before selling:

1. **Checkout link.** In `index.html`, set `CHECKOUT_URL` (near the bottom) to
   the Polar checkout URL for the Baton product. Until then the buy button
   politely says checkout is not open yet instead of 404ing.
2. **Price.** Appears twice in `index.html`, both marked with a `PRICE` comment,
   and must match the price set in Polar.

## Local preview

```bash
python3 -m http.server 8899
```

Then open <http://127.0.0.1:8899/>.
