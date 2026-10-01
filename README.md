# AeroBird

Wildlife-strike risk forecasting for airports: by ring, by week and by phase of flight.

**© 2026 AeroBird. All rights reserved.** This repository is public for viewing only. No permission is granted to use, copy or redistribute any part of it. See [LICENSE](LICENSE).

**Status: prototype.** Every figure on these pages is illustrative and generated for demonstration. Nothing here is a forecast or fit for operational use.

## What's in this repo

| Path | What it is |
|---|---|
| `waitlist/index.html` | Marketing site and waitlist, with a quick interactive risk board for one airport (LROP) |
| `waitlist/demo.html` | Demo console: overview, briefing, risk map, outlook, species, altitude, airside log, evidence |
| `vercel.json` | Vercel config: serves `waitlist/` as static files with clean URLs |

Both pages are single static HTML files with no build step and no dependencies beyond Google Fonts.

## Run locally

```bash
npx serve waitlist
```

Then open http://localhost:3000 and http://localhost:3000/demo.

## Deploy

Connected to Vercel through GitHub: every push to `main` deploys to production, other branches get preview URLs. `vercel.json` points the output at `waitlist/`, so no build step or root-directory setting is needed.

## Known gaps

- The waitlist form does not send anything yet.
- The demo model is illustrative: κ is uncalibrated and validation has not been run.
