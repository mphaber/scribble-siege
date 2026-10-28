# Scribble Siege

A paper flick-combat game: flick your fighters across a sheet of notebook paper and blow up the enemy base. Space, Knights, and Tanks themes, 1P vs CPU or 2P pass-and-play.

Play: https://mphaber.github.io/scribble-siege/

This folder is the multi-file snapshot of the game: `index.html`, this README, `site.webmanifest`, and 68 JavaScript asset modules under `assets/`. Each module (`assets/<name>.js`) assigns one artwork file — the three board plates, every piece sprite (including the two quarter faces), the entrance logo, and the two recorded crowd clips — as a base64 data URI into `window.__SS_ASSETS`, keyed by the relative path the game code asks for; `index.html` loads the modules with ordinary script tags and its image loaders resolve through that map. The encoded bytes are exactly the game's WebP artwork, so the boards render identically. No build step: serve or host the folder as-is.

The four PNGs at the root — `apple-touch-icon.png` (180×180), `icon-192.png`, `icon-512.png`, and `og-image.png` (1200×630) — are real binary files, not modules: they are the app icon and link-preview image (a ship circling a meteor, drawn on lined paper), and browsers and link crawlers fetch those URLs directly. `site.webmanifest` points at the two square icons.

Scribble Siege / Created by Matthew Haber / © 2026 Matthew Haber. All rights reserved.
