# Unicórnio da Rafaela

A game for Rafaela and Giulia, in Portuguese (PT) and Swedish (SV). It works offline as a Progressive Web App (PWA).

Play: https://betokasa1982-del.github.io/unicornio-rafaela/

## Modes

| Mode | What the child does |
|---|---|
| **Colorir** | Pick one of 15 pictures (unicorns, geometric shapes, everyday objects). Tap a color, then tap an area (bucket), or draw freehand (brush). Pinch or use **+ / −** to zoom in on small details. |
| **Quebra-cabeça** | Any picture becomes a puzzle with 4, 6, 9, 12, 16, 20 or 24 pieces. The puzzle uses the child's own coloring. A star badge shows the biggest puzzle finished. |
| **Formas** | Drag each colored shape onto its outline. The game says the shape name. Levels with 3 to 12 shapes. |
| **Letras / Bokstäver** | Four exercises: trace the letters of a name, build a name from letter tiles, read a word and pick the picture, pick the first letter of a word. Word lists and letter names follow the selected language (Swedish includes Å, Ä, Ö). |
| **Matemática / Matte** | Count, add, subtract or mixed. Problems use pictures grouped in rows of 5. Levels: up to 5, 10 or 20. The game reads the problem aloud. |

The home screen selects the language (**PT** / **SV**) and who is playing (Rafaela or Giulia). The **Letras** screen has a **+** button to add other names (for example MAMÃE).

Voice: the game reads letters, words, numbers and shape names with the device's text-to-speech voice for the selected language (Portuguese (Brazil) or Swedish). Install the voice in the phone's text-to-speech settings if it is missing. The sound button on the home screen mutes sounds and voice.

## Fullscreen

- Installed app on Android: opens in fullscreen.
- In the browser: tap the fullscreen button (four corners) in the top bar.
- Turn the phone sideways for a bigger drawing area. The palette moves to the side.

## Install on a phone

- **Android (Chrome):** open the URL. Tap **⋮**. Tap **Install app**.
- **iPhone / iPad (Safari):** open the URL. Tap **Share**. Tap **Add to Home Screen**.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole game (HTML, CSS, JS) |
| `manifest.webmanifest` | App name, colors, icons, display mode |
| `sw.js` | Service worker: offline cache |
| `icons/` | App icons (192, 512, maskable 512, Apple 180) |
| `.nojekyll` | Tells GitHub Pages to serve files as they are |

## Release an update

1. Change `index.html`.
2. Increase `VERSION` in `sw.js` (for example `v4` → `v5`).
3. Push to `main`. The phone gets the new version the next time the app opens online.

Drawings, names and progress are saved in the browser storage of each device (`localStorage`).
