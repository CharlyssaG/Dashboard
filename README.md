# Headquarters

A personal emotion dashboard inspired by the *Inside Out* control panel — built around custom orb characters, a 1–10 intensity gauge, and a memory log.

## Run locally

Just open `index.html` in any browser. No build step, no dependencies.

```bash
# or serve it
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to Vercel

```bash
# install Vercel CLI once
npm i -g vercel

# from this folder
vercel
```

Or push to GitHub and import the repo at [vercel.com/new](https://vercel.com/new). Vercel auto-detects this as a static site and deploys.

## What's in here

- `index.html` — the entire app, single file. All 30 orb sticker images are embedded as base64 PNGs, so it works fully offline.
- `vercel.json` — minimal Vercel config.
- `.gitignore` — standard ignores.

## Editing

Open `index.html` in any editor. Emotions live in the `EMOTIONS` array. Family colors and status messages live in `FAM_STYLE` and `STATUS_LINES` near the top of the script.

## Notes

The dashboard does not currently persist data across sessions — each refresh starts a fresh log. If you want logs saved, we can add localStorage in a follow-up.
