# Shaligram website (preview)

Website for Shaligram, a bungalow project on Detroj Road, Kadi, Gujarat.
Hosted on Cloudflare Pages at www.cotshaligram.com (also builds on Render as a preview).

## What is in here

- `index.html`: the whole website (3D homes viewer, interior, walk-through, construction story, assistant)
- `img/`: architect renders, layout plan, photos
- `models/`: floor-plan textures used by the 3D viewer
- `_headers`: security and caching rules for Cloudflare Pages (the live host)
- `render.yaml`: the same rules for Render (the old preview host)

## How it is hosted

Cloudflare Pages serves these files as they are. Every push to the `main` branch redeploys the site automatically.

The live site at www.cotshaligram.com is open to search engines (`robots.txt`, `sitemap.xml`).
The `workers.dev` address and the old Render copy send `noindex`, so Google only lists the real domain.

## Note on the assistant

On this site the chat assistant answers from its built-in answers and sends anything else to WhatsApp.
The extra AI answers only work in the Claude-hosted version.
