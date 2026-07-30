# C40 Brew Guide

A mobile-first, unofficial Comandante C40 brewing helper. Installable to your phone's home screen as a standalone app (PWA) via GitHub Pages.

## Files
- `index.html` — the app
- `manifest.json` — makes the app installable ("Add to Home Screen")
- `sw.js` — service worker, caches the app so it opens instantly and works offline
- `icons/` — app icons (192px, 512px, maskable) + `apple-touch-icon.png` + `favicon.png`

## Publish with GitHub Pages
1. Create a new GitHub repository (public is fine; private also works with Pages on paid plans).
2. Upload all files in this folder — keep the `icons/` folder structure intact.
3. In GitHub: **Settings → Pages → Build and deployment → Deploy from a branch**.
4. Select `main` and `/ (root)`, then **Save**.
5. Wait ~1 minute, then your app is live at `https://<your-username>.github.io/<repo-name>/`.

## Add to your phone's home screen

**iOS (Safari):**
1. Open the GitHub Pages link in Safari.
2. Tap the **Share** icon (square with an arrow).
3. Tap **Add to Home Screen** → **Add**.
4. The app now opens full-screen, with its own icon, no browser bar.

**Android (Chrome):**
1. Open the link in Chrome.
2. Tap the **⋮** menu → **Add to Home screen** (Chrome may also show an automatic "Install app" prompt).
3. Confirm — it installs like a native app.

## Updating the app later
Just edit `index.html` (or other files) in the GitHub repo and push/commit — GitHub Pages redeploys automatically within a minute or two. Because of the service worker cache, you (and anyone who installed it) may need to fully close and reopen the app once for the update to show up.

## Recommendation model
Official Comandante guidance is used where the company publishes explicit ranges:
- Espresso: 7–13 Standard clicks
- Bialetti/stovetop: 14–20
- Pour-over filter: 18–35
- French press/cupping: 25–35
- AeroPress: Comandante explicitly says this depends on recipe

Other method defaults and roast shifts are intentionally conservative heuristic starting points and are labelled as such in the UI. Red Clix values are 2× Standard clicks, following Comandante's guidance that Red Clix inserts an additional step between Standard clicks.

This project is unofficial and not affiliated with Comandante.
