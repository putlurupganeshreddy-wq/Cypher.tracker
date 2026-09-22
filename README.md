# CYPHER — Student Attendance & Study Tracker

A single-page, mobile-first web app for tracking daily class attendance and nightly study sessions. No backend, no login — all data is stored locally in the browser via `localStorage`.

## Features

- Daily attendance tracking against a fixed Monday–Saturday timetable
- Subject-wise and total attendance percentages (Present ÷ Working Classes)
- Night study tracker for a single 8:00 PM – 10:00 PM session per day
- Monthly calendar with color-coded attendance status per day, editable for any past date
- Attendance goal setting with a "classes needed to reach goal" calculator
- Light/dark mode, subtle tap sounds, smooth animations
- Fully responsive — mobile-first, works on desktop too

## Running it

This is a single self-contained HTML file — no build step, no dependencies to install.

- **Locally:** just open `index.html` in a browser.
- **GitHub Pages:** push this repo, then go to **Settings → Pages**, set the source to the `main` branch (root), and GitHub will serve it at `https://<your-username>.github.io/<repo-name>/`.

## Installing it as an app

CYPHER is a PWA (Progressive Web App). Once it's live on GitHub Pages:

- **Android (Chrome):** open the site → menu (⋮) → "Add to Home screen" / "Install app"
- **iPhone (Safari):** open the site → Share icon → "Add to Home Screen"
- **Desktop (Chrome/Edge):** open the site → click the install icon in the address bar

It'll then open full-screen with its own icon, with no browser bar.

## Files

- `index.html` — the entire app (HTML, CSS, and JavaScript in one file)
- `manifest.json` — tells the browser CYPHER is installable (name, icons, colors)
- `service-worker.js` — makes the app installable and lets it load when offline
- `icon-192.png`, `icon-512.png`, `icon-180.png`, `icon-32.png` — app icons at various sizes
- `icon-192-maskable.png`, `icon-512-maskable.png` — padded versions of the icon used by Android's adaptive/maskable icon system, so the logo isn't cropped or scaled blurry on the home screen

All five files must sit in the same folder (repo root) for install to work — the paths inside `manifest.json` and `index.html` assume that.

## Data & privacy

All attendance and study data lives in the visitor's own browser `localStorage`. Nothing is sent to a server, and clearing browser data or using a different device/browser will reset the tracker.
