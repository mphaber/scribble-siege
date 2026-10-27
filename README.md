# Scribble Siege

A paper flick-combat game: flick your fighters across a sheet of notebook paper and blow up the enemy base. Space, Knights, and Tanks themes, 1P vs CPU or 2P pass-and-play.

Play: https://mphaber.github.io/scribble-siege/

This folder is the multi-file snapshot of the game, TEXT-ONLY edition: `index.html`, this README, and 55 JavaScript asset modules under `assets/`. Each module (`assets/<name>.js`) assigns one artwork image — the three board plates and every piece sprite — as a base64 data URI into `window.__SS_ASSETS`, keyed by the relative path the game code asks for; `index.html` loads the modules with ordinary script tags and its image loaders resolve through that map. The encoded bytes are exactly the game's WebP artwork, so the boards render identically. No binary files, no build step: serve or host the folder as-is.

Scribble Siege / Created by Matthew Haber / © 2026 Matthew Haber. All rights reserved.
