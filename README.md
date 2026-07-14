# movingOut

Simple static page listing furniture and home items for sale, meant to be
shared via a QR code posted on community bulletin boards.

- `index.html` — the full listing (prices, dimensions, contact info)
- `flyer.html` — a one-page printable flyer with a large QR code that links
  to `index.html`
- `qr-code.svg` — the QR code image, pointing at
  `https://devvsurendra.github.io/movingOut/`

GitHub Pages is already enabled (Settings → Pages, source: `main` branch,
`/` root), so the site is live at `https://devvsurendra.github.io/movingOut/`.

## Setup

1. Fill in the real phone number and location/community name in
   `index.html` and `flyer.html`.
2. To add real photos, replace an item's `<div class="item-photo">🛋️</div>`
   in `index.html` with `<img class="item-photo" src="photos/sofa.jpg">`
   (add your image files under a `photos/` folder).
3. Open `flyer.html` in a browser and print it (Ctrl/Cmd+P) — the QR code
   links back to the full listing so buyers can see prices and details
   before texting you.

If the site URL ever changes, regenerate `qr-code.svg` to match (e.g. with
the Python `qrcode` package) so the printed flyer keeps pointing to the
right place.
