# FLoRA Project Website

Minimal academic project page for **FLoRA — Multiple Task Realizations for Embodiment-Adaptive Robot Manipulation**.

## Website
https://nothingisavaliable.github.io/FloRA-website/

The site is a dependency-free HTML/CSS page, hosted through GitHub Pages.

## Add your research figures

Upload the following files using the same names and paths:

| File | Website location | Recommended content |
| --- | --- | --- |
| `assets/framework.png` | Framework | Architecture overview figure, exported from your paper |
| `assets/panda.gif` | Franka Panda | Real recorded robot/simulation rollout |
| `assets/ur5e.gif` | UR5e | Real recorded rollout of dynamic re-selection |
| `assets/sawyer.gif` | Sawyer | Real recorded robot/simulation rollout |

Create an `assets` folder in the repository (GitHub's file upload accepts files into this folder).
As soon as the images are committed to `main`, the page shows them automatically, and GitHub Pages redeploys.

For static images instead of GIFs, update the corresponding `src` values in `index.html` (e.g. `assets/panda.png`).
No experiments are claimed on the site until the actual figures are uploaded.

## Publishing

The repository has a GitHub Actions Static HTML workflow in `.github/workflows/static.yml`. Commits to `main` trigger redeployment.

## Editing

The site is a single `index.html` file. Update headings and descriptions directly there; no build tools are required.
