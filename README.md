# Ari Mix & Match

Mobile-first Mix & Match wardrobe web app for Ari Brand. Browse Tops, Pants, Socks, and Shoes in horizontally scrollable, scroll-snap rows; the item centered on screen becomes active and drives its size dropdown.

## Live demo

https://thanawut-p.github.io/ari-mix-match/

## Features

- Mobile-first layout, max-width 500px
- CSS scroll-snap carousels for Tops / Pants / Socks / Shoes
- Auto-detected active (centered) item via IntersectionObserver
- Per-row size dropdown driven by the active item's variants
- Sticky footer with two actions:
    - Try on in-store: posts the selected outfit to a Discord webhook
    - Buy online: opens a Shopify Cart Permalink with the four selected variant IDs

## Setup

1. Open `index.html` in a browser, or serve it via GitHub Pages (enabled on this repo).
2. Replace `DISCORD_WEBHOOK_URL` in the script with your real Discord webhook.
3. Replace the mock `PRODUCTS` data and variant IDs with real Shopify product/variant data.

## Tech

Plain HTML5, CSS3, and vanilla JavaScript. No build step, no dependencies.
