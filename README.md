# movingOut

Simple static page listing furniture and home items for sale, meant to be
shared via a QR code posted on community bulletin boards.

- `index.html` — the full listing (photos, prices, dimensions, contact info)
- `flyer.html` — a one-page printable flyer with a large QR code that links
  to `index.html`
- `qr-code.svg` — the QR code image, pointing at
  `https://devvsurendra.github.io/movingOut/`
- `photos/` — item photos referenced by `index.html`

GitHub Pages is already enabled (Settings → Pages, source: `main` branch,
`/` root), so the site is live at `https://devvsurendra.github.io/movingOut/`.

## Setup

1. Fill in the real phone number and location/community name in
   `index.html` and `flyer.html`.
2. To add or swap a photo, drop a new file in `photos/` and update the
   matching `<img src="photos/...">` in `index.html`.
3. Open `flyer.html` in a browser and print it (Ctrl/Cmd+P) — the QR code
   links back to the full listing so buyers can see photos and prices
   before texting you.

If the site URL ever changes, regenerate `qr-code.svg` to match (e.g. with
the Python `qrcode` package) so the printed flyer keeps pointing to the
right place.
