# Luxro.Fashion — Baby & Kids Storefront

A responsive storefront built from the supplied product catalogue and product-photo ZIP. Includes category filtering, search, sorting, 85 product cards, a persistent shopping bag, WhatsApp enquiry checkout, mobile navigation, and Anime.js motion.

## Run locally

Because the catalogue is loaded from `products.json`, run this folder through a local web server rather than opening `index.html` directly.

**Python:**
```bash
python -m http.server 8000
```
Then open http://localhost:8000 in your browser from this folder.

Alternatively, open the folder in VS Code and use the Live Server extension.

## Before publishing

1. Open `app.js` and replace `91XXXXXXXXXX` in `WHATSAPP_NUMBER` with your WhatsApp number, digits only (country code included).
2. Replace “Luxro.Fashion” with your actual shop/brand name if different (in `index.html` and `app.js`).
3. The Excel sheet's website selling-price column is blank, and the prices shown in source images were marked for verification. The site therefore displays **Price on request** rather than assuming those are your retail prices.
4. Confirm product descriptions, stock, sizes, prices, delivery/return policies, and contact details before launch.

## Files
- `index.html` — page structure
- `style.css` — responsive styling and visual design
- `app.js` — interactions, bag, WhatsApp enquiry, Anime.js animations
- `products.json` — 85 catalogue entries
- `assets/products/` — original product images, keeping their original filenames

Anime.js is loaded from a CDN, so an internet connection is needed for the animations. Google Fonts are also loaded from a CDN; the page falls back to system fonts if unavailable.
