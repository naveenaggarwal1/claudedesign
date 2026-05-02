# Underwater Datacenters

An animated 45-second explainer video built with [Claude Design](https://claude.ai/design), explaining how Israel is building underwater datacenters off the Mediterranean coast to cool the next wave of AI compute.

## How to view

Open **`Underwater Datacenters.html`** directly in any modern browser — no server, no build step, no dependencies to install. Everything is self-contained in the single HTML file.

## Controls

| Key | Action |
|-----|--------|
| `Space` | Play / Pause |
| `←` / `→` | Step back / forward 0.1s |
| `Shift + ←` / `Shift + →` | Step back / forward 1s |
| `0` or `Home` | Jump to beginning |

You can also click and drag the scrub bar at the bottom to jump to any moment.

## Scenes

| Time | Scene |
|------|-------|
| 0–5s | **Cold open** — title card with animated wave layers |
| 5–15s | **The Problem** — 945 TWh stat counter, datacenters heating up with thermal overlay |
| 15–30s | **The Solution** — sealed server capsule descending off Tel Aviv, seawater currents, fish, bubbles |
| 30–40s | **The Numbers** — three stat cards: 40% lower cooling costs, 0L freshwater, 8× closer to EU users |
| 40–45s | **Closing card** — "Israel's underwater datacenter race. Starts 2026." with logo placeholder |

## Visual style

- **Palette:** Mediterranean blue · sand beige · pure white · muted terracotta accent
- **Type:** Cormorant Garamond (serif titles) · IBM Plex Sans (body) · IBM Plex Mono (captions/stats)
- **Illustrations:** Thin-line SVG, 1.5–2px strokes throughout
- **Animation:** Smooth eased transitions, kinetic number counters, no hard cuts

## Tech stack

Pure HTML + CSS + JavaScript. Uses:
- [React 18](https://react.dev/) (UMD build, no bundler needed)
- [@babel/standalone](https://babeljs.io/docs/babel-standalone) for in-browser JSX compilation
- Google Fonts for Cormorant Garamond and IBM Plex families

## Customisation

To add your logo, replace the `[ logo ]` placeholder in the closing scene. Search for `[ logo ]` in the HTML and swap the dashed box div for an `<img>` tag pointing to your logo file.

---

*Generated with [Claude Design](https://claude.ai/design) · Implemented by Claude Code*
