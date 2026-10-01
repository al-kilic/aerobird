# AeroBird

Wildlife-strike risk forecasting for airports: by ring, by week and by phase of flight.

**Status: prototype.** Every figure on these pages is illustrative and generated for demonstration. Nothing here is a forecast or fit for operational use.

## What's in this repo

| Path | What it is |
|---|---|
| `waitlist/index.html` | Marketing site and waitlist, with a quick interactive risk board for one airport (LROP) |
| `waitlist/demo.html` | Demo console: overview, briefing, risk map, outlook, species, altitude, airside log, evidence |
| `waitlist/vercel.json` | Static hosting config (clean URLs) |

Both pages are single static HTML files with no build step and no dependencies beyond Google Fonts.

## Run locally

```bash
npx serve waitlist
```

Then open http://localhost:3000 and http://localhost:3000/demo.

## Deploy

Vercel project settings: **Root Directory** `waitlist`, **Framework Preset** Other, no build command, no output directory.

## Known gaps

- The waitlist form does not send anything yet.
- The demo model is illustrative: κ is uncalibrated and validation has not been run.
