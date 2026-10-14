# Datacom Field Kit — iOS web version (test)

The Datacom Field Kit as a hosted web app for iPhone: open the Pages URL in
Safari, then Share → Add to Home Screen. Runs fullscreen like an app.

This is a **separate project** from the Android app
(`WhiteFrostL33T/datacom-field-kit`) — separate versioning, separate builds.

## How it works

- `index.html` — the entire app (same single-file app as Android, plus iOS
  home-screen meta tags). All data lives in the browser on the device
  (localStorage) — no account, no cloud, works offline once loaded.
- `apple-touch-icon.png` — home-screen icon (keystone data jack).
- Backup: use the in-app Backup section — Export downloads a JSON file
  (lands in the Files app), Import reads one back via the file picker.

## Hosting

Served with GitHub Pages (Deploy from branch → `main`, root). Public URL:

https://whitefrostl33t.github.io/datacom-field-kit-ios/
