# civilizED MEN

A responsive, installable clothing storefront created for the Indian menswear market.

## Features

- Responsive desktop and mobile layout
- Product category filters
- Shopping bag stored on the device
- Indian rupee pricing
- Progressive Web App manifest and offline cache
- Installable on Android, iPhone, and desktop

## Run locally

The website is static, so any local web server will work:

```bash
npx serve dist
```

Then open the local URL shown in the terminal.

## Project files

- `dist/index.html` — storefront layout, styling, products, and cart behavior
- `dist/manifest.webmanifest` — installable-app settings
- `dist/sw.js` — offline cache service worker
- `dist/icon.svg` — app and browser icon

## Deployment

Deploy the `dist` directory to GitHub Pages, Netlify, Cloudflare Pages, Vercel, or another static host.

Checkout is currently a demonstration placeholder. Connect Shopify, Razorpay, or another Indian payment provider before accepting orders.
