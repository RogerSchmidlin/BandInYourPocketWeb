# Band in your Pocket: website

Public static website for Band in your Pocket. Plain HTML and CSS, no JavaScript, no build step, no tracking, no external requests.

**For now it is a teaser.** It shows the name, "Coming to your pocket soon" and three animated phones (a player, a live jam and pads, all pulsing on the same beat). It deliberately says nothing about what the app does.

| File | What |
|---|---|
| `index.html` | The teaser page |
| `styles.css` | All styles and animations. Every pulse follows `--beat` (96 bpm); the phones scale with `--pw` |
| `favicon.svg` | Icon and logo mark |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |
| `CLAUDE.md` | Rules for Claude Code sessions in this repository (it never commits or pushes) |

## Where the content comes from

While this is a teaser, it contains no product information. When you decide to reveal more, the text comes only from product notes marked `publish: true` in the private repository (`BandInYourPocket/docs/product/`). Nothing from `docs/dev/` or `docs/business/` belongs here. See "The public website" in `docs/dev/ai-workflow.md`.

## Preview locally

Open `index.html` in a browser. Everything is relative, so it works straight from the folder. Visitors who turn on "reduce motion" in their system settings get a still version.

## Deploy

Any static host works. Two options:

- **Cloudflare Pages:** connect this repository, framework preset *None*, build command empty, output directory `/`.
- **GitHub Pages:** repository Settings → Pages → *Deploy from a branch* → `main`, folder `/ (root)`.
