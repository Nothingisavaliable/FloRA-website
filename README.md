# FLoRA Project Website

Minimal project page for **FLoRA — Multiple Task Realizations for Embodiment-Adaptive Robot Manipulation**.

Live page: https://nothingisavaliable.github.io/FloRA-website/

## RQ3: Embodiment-Adaptive Realization Selection

The homepage displays nine GIFs from `assets/gifs_0/`, with three examples per robot (Franka Panda, Sawyer, UR5e). Each example includes the two-stage evaluator results from `showcase_liquid.html`:

- **Stage 1: Collision Filtering** — all 27 candidate realizations are shown as retained/rejected; a retained count appears below each GIF.
- **Stage 2: Tracking-Cost Ranking** — the full retained-candidate ranking (rank, realization, position/orientation tracking error and cost), with the selected realization highlighted.

Click **View evaluation details** to expand the two stages. The separate **Realization labels (m1–m27)** control was removed from the public page.

## RQ4: Dynamic Realization Re-selection

The homepage also displays 12 GIFs from `assets/gifs_1/`. In each scenario, animations appear side by side in the order **CrossFormer, FLoRA-Fixed, FLoRA-Reselect**.

| Perturbation | CrossFormer | FLoRA-Fixed | FLoRA-Reselect |
| --- | --- | --- | --- |
| Bowl +5 cm (X) | `XP5CM_crossformer.gif` | `XP5CM_flora-fixed.gif` | `XP5CM_flora-reselect.gif` |
| Bowl +10 cm (Y) | `YP10CM_crossformer.gif` | `YP10CM_flora-fixed.gif` | `YP10CM_flora-reselect.gif` |
| Bowl +15 cm (X) | `XP15CM_crossformer.gif` | `XP15CM_flora-fixed.gif` | `XP15CM_flora-reselect.gif` |
| O_task movement | `crossformer_obstacle_move.gif` | `flora-fixed_obstacle_move.gif` | `flora-reselect_obstacle_move.gif` |

All GIFs are displayed at their intrinsic aspect ratio with no fixed-height crop. RQ4 images are lazy-loaded to reduce initial bandwidth usage.

## Publishing

The site is static HTML and is published by GitHub Pages from `main` via `.github/workflows/static.yml`.
