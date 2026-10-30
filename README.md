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

The preview is marked `noindex`, so Google will not list it. Remove the `noindex` meta tag in
`index.html` and the `X-Robots-Tag` header in `render.yaml` at the real launch.

## Note on the assistant

On this site the chat assistant answers from its built-in answers and sends anything else to WhatsApp.
The extra AI answers only work in the Claude-hosted version.
