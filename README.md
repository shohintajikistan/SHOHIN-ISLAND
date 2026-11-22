# SHOHIN ISLAND

A mobile-first 3D tropical island exploration prototype built with Three.js.

## World target
- Planned total world area: **143,100 km²**
- The current playable prototype is the first local terrain region, approximately **5 km across**. The full world is not generated yet.
- The large world will need streamed terrain regions, saved world coordinates and biome transitions; it cannot be represented by one giant mesh.

## Current prototype
- Procedural mountainous tropical terrain
- Tropical palms, broadleaf forest, undergrowth, boulders and beaches
- River and waterfall scene elements
- Third-person explorer with touch joystick, swipe camera, jump and view toggle
- Instanced vegetation and capped device pixel ratio for mobile performance

## Run
Open `index.html` from GitHub Pages or a local static web server. Three.js is loaded from jsDelivr, so this version requires an internet connection.

## Publish with GitHub Pages
The workflow in `.github/workflows/pages.yml` deploys the site on pushes to `main`. In repository Settings → Pages, set the source to **GitHub Actions** if it is not already selected.

## Roadmap
1. Stream terrain in regions across the 143,100 km² world.
2. Improve terrain materials, realistic water and waterfall effects.
3. Add varied tropical tree and shrub assets, caves, wildlife and landmarks.
4. Add offline asset caching and an Android APK wrapper.
