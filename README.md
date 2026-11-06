# DEAD MISSIONS

**Version 0.0.2 — EARLY BUILD**

Dead Missions is a browser-first first-person mission game, built as a static Three.js site for desktop and mobile browsers.

## What's new in 0.0.2

- Larger first-person viewmodels for all five weapons, with visible uniform sleeves and gloved hands around the weapon grips.
- Improved layered sound effects for weapons, reloads, footsteps, aircraft and explosions.
- Radio voice callouts through the browser's built-in speech synthesis when supported. Audio effects are synthesized with Web Audio; no external API key is required.
- The training field and communications outpost have more structures, fences, roads, vehicles, lighting, crates, antennas and environmental detail.
- The first bombing sequence now pushes the viewpoint back, drops it toward the ground, and tilts the camera and weapon before the blackout transition.

## Missions

1. **Range Zero** — Complete the training drill with ten headshots. Aircraft pass overhead, bombs strike the range, and the player is knocked off their feet.
2. **Blackout Protocol** — Restore three communications relays, disable hostile drones, and reach the extraction beacon.

## Armory

- Primary: Vanguard AR, Striker SMG, Breach 12
- Secondary: M9 Sidearm, Sentinel .45

## Controls

| Action | Desktop | Touch |
|---|---|---|
| Move | W, A, S, D | Left movement pad |
| Aim | Mouse | Drag right side |
| Fire | Left click | FIRE |
| Reload | R | RLD |
| Switch weapon | 1 / 2 | SWAP |
| Interact | E | USE |
| Sprint | Shift | — |
| Pause | Escape | — |

## Run locally

Serve the repository root over HTTP, because the game uses JavaScript modules. For example, use the VS Code Live Server extension or `python -m http.server 8000`, then open `http://localhost:8000`.

## Deploy to GitHub Pages

The `.github/workflows/pages.yml` workflow deploys the static site when changes are pushed to `main`. Select **Settings → Pages → Build and deployment → GitHub Actions**.

For first-time Pages initialization, create a fine-grained token restricted to this repository with **Pages: Read and write** and **Administration: Read and write**, then add it as the Actions repository secret `PAGES_SETUP_TOKEN`. Once the Pages site exists, subsequent deployments use the workflow's normal `GITHUB_TOKEN`.

## Changelog

### 0.0.2 [EARLY BUILD]
- Held weapon models with visible hands and sleeves.
- Layered synthesized audio and browser TTS radio callouts.
- Bombing impact knockdown sequence.
- More detailed training range and communications outpost.

### 0.0.1 [EARLY BUILD]
- First browser-playable 3D build.
- Two campaign missions and mission unlock progression.
- Five selectable weapons.
- Desktop and touch controls, weapon swapping, firing and reload.
- In-game changelog and controls manual.

More missions coming soon.
