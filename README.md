# RSKA Notes v14 - internal testing build

Static web/PWA build for GitHub Pages. No Node.js or administrator installation is required.

## Files
- `index.html` - full RSKA Notes app, based on V13.15
- `manifest.webmanifest` - installable web-app metadata
- `sw.js` - basic offline shell caching
- `icon-192.png`, `icon-512.png` - app icons using the existing RSKA logo artwork - app icons

## Local test
Open `index.html` directly for basic testing. PWA installation/service-worker behaviour requires localhost or HTTPS, such as GitHub Pages.

## GitHub Pages
Publish all files at repository root and enable Pages using the `main` branch / root folder.

## Internal-testing note
Data, including photos, is stored locally in the browser/device by the current app. GitHub Pages hosts the application files; it does not provide a project database or automatically upload users' site records.
