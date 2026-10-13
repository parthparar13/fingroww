# FinGrow PWA package

## Files
- `index.html`: FinGrow v3 adapted for PWA installation; includes progress export/import buttons.
- `manifest.json`: install name, theme, and icon settings.
- `sw.js`: caches the app shell for basic offline opening.
- `icon-192.png`, `icon-512.png`: app icons.

## Publish
Upload all five files to the root of a GitHub repository, enable GitHub Pages from `main` / root, then open the HTTPS URL in Chrome on Android and choose Install app / Add to Home screen.

## Progress preservation
1. Open the old FinGrow v3 file in the same browser where its progress is saved.
2. Tap `Export progress` and keep `FinGrow-progress-backup.json`.
3. After publishing and opening the PWA, tap `Import progress`, select that JSON file, and confirm.
4. The app reloads with the imported progress.

Browser file:// storage can behave differently across browsers and devices. Export progress from the same browser/profile where it was originally saved. Never clear the old browser data until you've confirmed the imported progress.
