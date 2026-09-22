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

## Files

- `index.html` — the entire app (HTML, CSS, and JavaScript in one file)

## Data & privacy

All attendance and study data lives in the visitor's own browser `localStorage`. Nothing is sent to a server, and clearing browser data or using a different device/browser will reset the tracker.
