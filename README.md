# [Portfolio](https://hakierka.github.io)

Live site: [hakierka.github.io](https://hakierka.github.io)

| Dark | Light |
| --- | --- |
| ![Portfolio in dark theme, hero and highlights](docs/screenshot-dark.png) | ![Portfolio in light theme, hero and highlights](docs/screenshot-light.png) |

## What it is

A single-page portfolio with a retro pixel look: silver desktop windows, an arcade-style hero and a dino on the ground. It lists articles, docs, demos, videos and events. One HTML file, no build step.

## Features

- **Dark and light theme:** follows the system setting automatically. A toggle remembers your choice in `localStorage`. Without JavaScript, the system theme still applies through CSS.
- **Retro pixel look:** Silver window bars and bevelled buttons, a halftone grey background, pixel sprites in `assets/`. JetBrains Mono and Silkscreen, self-hosted.
- **Accessible:** skip link, visible focus, keyboard navigation, `prefers-reduced-motion` respected, readable at 360px wide. Body text meets WCAG AA contrast in both themes. The big name in the hero is a graphic title from my LinkedIn cover and has lower contrast (about 2:1).
- **Fast and private:** one HTML file, no build, no framework, no external requests, no tracking. About 255 KB in total (HTML, fonts, avatar and sprites).

## Run locally

```bash
git clone https://github.com/hakierka/hakierka.github.io.git
cd hakierka.github.io
python3 -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000).

Or: `npx serve`.

Opening `index.html` from disk also works.

## Project structure

```
index.html
avatar.png
fonts/
assets/
docs/
```

`assets/` holds pixel sprites: dino, clouds, ground. The cacti are drawn as inline SVG in `index.html`.

## Palette

| Name | Hex | Where used |
| --- | --- | --- |
| `--bg` | `#d9d9d9` | Light page background |
| `--bg` | `#1b1b1b` | Dark page background |
| `--silver` | `#c0c0c0` | Window bars and bevelled buttons |
| `--lemon` | `#ffee32` | Headings and links in dark mode; accents |
| `--gold` | `#ffd100` | Hard shadows in dark mode |
| `--shadow` | `#000` | Light theme: outlines and hard shadows; dark theme uses `#ffd100` |
| `--ink` | `#e6e6e6` | Body text in dark mode |
| `--ink` | `#141414` | Body text in light mode |
| `--panel` | `#262626` | Panels in dark mode |
| `--panel` | `#ececec` | Panels in light mode |

## Credits and license

- Fonts (JetBrains Mono, Silkscreen): [SIL Open Font License 1.1](fonts/OFL.txt)
- Code: MIT
- Text, photos and avatar: all rights reserved
