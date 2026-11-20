# Band in your Pocket: website

Public static website for Band in your Pocket. Plain HTML and CSS, no build step, no tracking, no external requests.

| File | What |
|---|---|
| `index.html` | The one-page site: features, band sessions, how it works, roadmap |
| `styles.css` | All styles; light and dark mode follow the visitor's system setting |
| `favicon.svg` | Icon and logo mark |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |
| `CLAUDE.md` | Rules for Claude Code sessions in this repository (it never commits or pushes) |

## Where the content comes from

The text is derived from the product notes in the private repository (`BandInYourPocket/docs/product/`). Only notes marked `publish: true` may be used. Nothing from `docs/dev/` or `docs/business/` belongs here. When the product notes change, update this site in the same week; see "The public website" in `docs/dev/ai-workflow.md`.

## Preview locally

Open `index.html` in a browser. Everything is relative, so it works straight from the folder.

## Deploy

Any static host works. Two options:

- **Cloudflare Pages:** connect this repository, framework preset *None*, build command empty, output directory `/`.
- **GitHub Pages:** repository Settings → Pages → *Deploy from a branch* → `main`, folder `/ (root)`.

## Open items

- Newsletter sign-up: the "Follow along" section shows "coming soon" until a provider is chosen (see `docs/business/email-newsletter.md` in the private repository).
- Screenshots of the app, once there is one.
- Privacy page, once anything is collected.
