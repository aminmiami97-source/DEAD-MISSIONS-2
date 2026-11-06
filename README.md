# DEAD MISSIONS

**Version 0.0.1 — EARLY BUILD**

Dead Missions is a browser-first, first-person mission game. This early build is a static site powered by Three.js and can be hosted on GitHub Pages.

## Play

Open the deployed site in a modern desktop or mobile browser. The game loads Three.js from jsDelivr, so an internet connection is required.

### Controls

| Action | Desktop | Touch |
|---|---|---|
| Move | W, A, S, D | Left movement pad |
| Aim | Mouse | Drag right side |
| Fire | Left click | FIRE button |
| Reload | R | RLD |
| Switch weapon | 1 / 2 | SWAP |
| Interact | E | USE |
| Sprint | Shift | — |
| Pause | Escape | — |

## Missions

1. **Range Zero** — Complete the training drill with ten headshots. The exercise is interrupted by an unexpected aerial attack.
2. **Blackout Protocol** — Restore three communications relays, disable hostile drones, and reach the extraction beacon.

## Armory

- Primary: Vanguard AR, Striker SMG, Breach 12
- Secondary: M9 Sidearm, Sentinel .45

## Run locally

Because the game uses JavaScript modules, serve the repository root over HTTP rather than opening `index.html` directly. For example, use the VS Code Live Server extension or `python -m http.server 8000`, then open `http://localhost:8000`.

## Deploy to GitHub Pages

The `.github/workflows/pages.yml` workflow deploys the static site whenever changes are pushed to `main`. In repository settings, select **Settings → Pages → Build and deployment → GitHub Actions**.

## Changelog — 0.0.1 [EARLY BUILD]

- First browser-playable 3D build.
- Two campaign missions and mission unlock progression.
- Five selectable weapons with individual first-person models.
- PC and touch controls, weapon swapping, firing and reload.
- In-game field changelog and controls manual.
- More missions coming soon.

This is an early prototype. Gameplay, balance, visuals and device performance will continue to evolve.


### First-time Pages setup

If the first deployment fails because the Pages site does not exist yet, create a fine-grained personal access token restricted to this repository with **Pages: Read and write** and **Administration: Read and write** repository permissions. Add it under **Settings → Secrets and variables → Actions** as `PAGES_SETUP_TOKEN`, then re-run the deployment workflow. The setup token is used by `actions/configure-pages` only to create the Pages site; subsequent deployments can use the workflow's normal `GITHUB_TOKEN`.
