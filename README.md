# movingOut

Simple static page listing furniture and home items for sale, meant to be
shared via a QR code posted on community bulletin boards.

- `index.html` — the full listing (photos, prices, dimensions, contact info)
- `flyer.html` — a one-page printable flyer with a large QR code that links
  to `index.html`
- `qr-code.svg` — the QR code image, pointing at
  `https://devvsurendra.github.io/movingOut/`

## Setup

1. In this repo's **Settings → Pages**, set the source to "Deploy from a
   branch", branch `main`, folder `/ (root)`. GitHub will publish the site
   at `https://devvsurendra.github.io/movingOut/`.
2. Fill in the real phone number, location/community name, and item photos
   in `index.html` (and `flyer.html` if you change the URL or contact
   details).
3. Open `flyer.html` in a browser and print it (Ctrl/Cmd+P) — the QR code
   links back to the full listing so buyers can see photos and prices
   before texting you.

If the site URL ever changes, regenerate `qr-code.svg` to match (e.g. with
the Python `qrcode` package) so the printed flyer keeps pointing to the
right place.
