# SHOHIN ISLAND

A mobile-first 3D island exploration prototype built with Three.js.

## Current prototype
- Procedural island terrain representing a 5 km × 5 km world
- Forests, rocky ridges, beaches, river and waterfall elements
- Third-person explorer with touch joystick, swipe camera, jump and view toggle
- Performance-conscious instanced vegetation and capped device pixel ratio

## Run
Open `index.html` from GitHub Pages or a local static web server. Three.js is loaded from jsDelivr, so the first version requires an internet connection.

## Publish with GitHub Pages
The workflow in `.github/workflows/pages.yml` deploys the site on every push to `main`. In repository Settings → Pages, set the source to **GitHub Actions** if it is not already selected.

## Roadmap
1. Improve terrain materials and shoreline detail.
2. Replace procedural placeholders with optimized original 3D assets.
3. Add sound, wildlife, landmarks, caves and better water.
4. Add offline asset caching and an Android APK wrapper.
