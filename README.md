# Vespator Front campaign map (prototype)

This is a static GitHub Pages site. It currently supports draggable faction/player markers, editing marker name/symbol/color/notes, browser-local saving, and JSON export/import.

## Publish on GitHub Pages
1. Sign into GitHub and create a new repository (e.g. `vespator-campaign-map`). Public is simplest for Pages.
2. Upload `index.html`, `map.png`, and this README into the repository's root.
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**; select `main` and `/ (root)`, then Save.
5. GitHub will provide a Pages URL after it builds.

## Important: local save vs shared save
The prototype's current save is browser-local. To make it live/shared across all players, set up a Firebase Realtime Database and add the Firebase client integration. Don't share sensitive Firebase admin credentials; the website only needs the public web config and a carefully scoped database rule.

## Prototype controls
- **Add token**: create a marker
- Drag marker: reposition
- Click marker: edit marker details
- **Export save / Import save**: portable campaign backup

The map asset is `map.png`.
