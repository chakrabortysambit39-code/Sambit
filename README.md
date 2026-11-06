# Lost World — The Forgotten Valley

A browser-based third-person 3D adventure built with Three.js. Explore a procedural valley, recover eight ancient crystals, fight forest creatures, defeat the guardian and restore the gate.

## Play

**Live game:** https://chakrabortysambit39-code.github.io/Sambit/

## Features

- Third-person explorer with hood, cloak, pack, boots and sword
- Procedural valley with forests, rocks, distant hills, flowers and trails
- Terrain-aware character, enemies, treasure and collectibles
- Day/night lighting, fog, fireflies and real-time shadows
- Eight crystals, treasure chests, berries, potions and coins
- Forest enemies, combat, health, stamina and guardian boss
- Quest journal, minimap, inventory, autosave and manual save
- Keyboard/mouse, touch controls and gamepad support
- Graphics presets, fullscreen and installable PWA shell

## Controls

| Action | Keyboard | Touch | Gamepad |
|---|---|---|---|
| Move | WASD / arrows | Left joystick | Left stick |
| Look | Mouse | Drag right side | Right stick |
| Sprint | Shift | Push joystick fully forward | L3 |
| Jump | Space | Jump button | A / Cross |
| Attack | F | Attack button | X / Square |
| Interact | E | Interact button | Y / Triangle |
| Use item | 1 | Use button | — |
| Pause | Esc | Settings | — |

## Run locally

Use a local static server because the game loads Three.js as an ES module:

```powershell
py -m http.server 8000
```

Open http://localhost:8000/docs/

## Publishing

GitHub Actions deploys the `docs/` folder to GitHub Pages whenever a change is pushed to `main`. The workflow can enable Pages automatically for this repository. After the first successful deployment, each release commit publishes automatically.

Three.js is loaded from jsDelivr, so the first launch requires an internet connection. The service worker caches the app shell for repeat visits; it does not bundle Three.js for fully offline play.
