# Project structure

The project uses plain HTML, CSS, and JavaScript so it can be hosted on GitHub Pages or any static hosting service without a build process.

## Responsibilities

| File | Responsibility |
|---|---|
| `index.html` | Semantic page structure, store content, navigation, product grid container and cart drawer |
| `assets/css/main.css` | Brand tokens, layout, responsive breakpoints and interaction states |
| `assets/js/products.js` | Product names, descriptions, prices, categories and visual tokens |
| `assets/js/app.js` | Product rendering, filtering, cart persistence, drawer controls and service-worker registration |
| `manifest.webmanifest` | Mobile installation metadata and app theme |
| `sw.js` | Core-file caching for offline use |

## Data flow

1. `products.js` exposes the catalogue as `window.CIVILIZED_PRODUCTS`.
2. `app.js` reads the catalogue and renders product cards into `#products`.
3. Adding an item writes the cart to browser local storage.
4. Filters rerender the catalogue without changing the source data.

## Recommended next modules

When real commerce is added, create separate modules for authentication, inventory, checkout, orders and payment-provider integration. Do not place secret payment keys in browser JavaScript.

