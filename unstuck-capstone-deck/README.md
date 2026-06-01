# Unstuck - Capstone slide deck (HTML)

**Live deck:** https://tericampbell.github.io/unstuck-capstone-deck/

Reveal.js deck for Product Faculty submission. Copy source: `../Unstuck_Capstone_Slides.md`. Video arc: `../Unstuck_Capstone_Video.md`.

## Local preview

```bash
cd unstuck-capstone-deck
npx --yes serve . -p 3456
```

Open http://localhost:3456. Use arrow keys or on-screen arrows to advance slides.

## Refresh screenshots from production

```bash
npm install playwright@1.49.1   # first time only
node scripts/capture-screenshots.mjs
```

Writes PNGs to `assets/screenshots/` from https://unstuck-app-flame.vercel.app/

## Publish to GitHub Pages (TeriCampbell.GitHub.io, same site as wireframe)

Deck lives in [TeriCampbell/TeriCampbell.GitHub.io](https://github.com/TeriCampbell/TeriCampbell.GitHub.io) as folder `unstuck-capstone-deck/` on branch `master`.

**After editing files in this folder**, copy into the Pages clone and push:

```bash
PAGES="/Users/tericampbell/Desktop/AI PM Capstone/TeriCampbell.GitHub.io"
DECK="/Users/tericampbell/Desktop/AI PM Capstone/unstuck-capstone-deck"

cp "$DECK/index.html" "$DECK/deck.css" "$PAGES/unstuck-capstone-deck/"
cp "$DECK/assets/screenshots/"*.png "$PAGES/unstuck-capstone-deck/assets/screenshots/"

cd "$PAGES"
git add unstuck-capstone-deck/
git commit -m "Update capstone deck"
git push origin master
```

Paste the live URL in the Google Doc PRD and slide 9 when you submit.

---

## Before you submit (reminders)

| When | Action |
|------|--------|
| Deck URL is live | Incognito + phone QA on the Pages link (not logged into GitHub). Confirm slides load and arrows work. |
| Deck content final | PDF backup: browser Print, save as `TeriCampbell_Unstuck_Capstone_Slides.pdf`. |
| Video uploaded | Edit `index.html` slide 9: replace video placeholder with your Vimeo link. |

---

## Edit tips

- **Copy / headlines:** `index.html` each `<section>`.
- **Styles:** `deck.css` (colors match app accent `#2d6a4f`).
- **New screenshot:** re-run capture script or replace PNG in `assets/screenshots/`.
