# Lost World — Three.js browser prototype

A small third-person exploration game built with Three.js and hosted with GitHub Pages.

## Play locally

Open `docs/index.html` through a local web server (recommended because it uses JavaScript modules). For example, with Python installed:

```powershell
py -m http.server 8000
```

Then open http://localhost:8000/docs/

## Controls

- **W / A / S / D** or arrow keys — move
- **Mouse** — look around (click the game to capture the mouse)
- **Shift** — sprint
- **Space** — jump
- **Esc** — release the mouse

## Goal

Explore the valley and collect all 8 glowing ancient crystals.

## Publish with GitHub Pages

1. Open the repository **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **GitHub Actions**.
3. Open the **Actions** tab and wait for **Deploy Lost World to GitHub Pages** to finish.
4. Your game will be published at:
   https://chakrabortysambit39-code.github.io/Sambit/

The first deployment may take a few minutes. Three.js is loaded from jsDelivr, so the browser needs an internet connection.

## Next development steps

- Replace the procedural explorer with the Ranger GLTF model.
- Add character animations and improved terrain.
- Add sound, landmarks, quests and save progress.
