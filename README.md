# Unicórnio da Rafaela

A unicorn game for a 5-year-old. It has two modes:

- **Colorir** — tap a color, then tap a part of the picture. Three pictures: rainbow, castle at night, party.
- **Quebra-cabeça** — drag the pieces onto the board. 4, 6, 9 or 12 pieces. The puzzle uses the child's own coloring.

The game is one HTML file with no build step. It works offline as a Progressive Web App (PWA).

## Play

Open the GitHub Pages URL: `https://<user>.github.io/unicornio-rafaela/`

## Install on a phone

- **Android (Chrome):** open the URL. Tap the menu (⋮). Tap **Add to Home screen** or **Install app**.
- **iPhone / iPad (Safari):** open the URL. Tap **Share**. Tap **Add to Home Screen**.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole game (HTML, CSS, JS) |
| `manifest.webmanifest` | App name, colors and icons for installation |
| `sw.js` | Service worker: offline cache |
| `icons/` | App icons (192, 512, maskable 512, Apple 180) |
| `.nojekyll` | Tells GitHub Pages to serve files as they are |

## Release an update

1. Change `index.html`.
2. Increase `VERSION` in `sw.js` (for example `v1` → `v2`).
3. Push to `main`. The phone gets the new version the next time the app opens online.

Drawings are saved in the browser storage of each device (`localStorage`).
