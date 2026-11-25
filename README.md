# FLoRA Project Website

Minimal project page for **FLoRA — Multiple Task Realizations for Embodiment-Adaptive Robot Manipulation**.

Live page: https://nothingisavaliable.github.io/FloRA-website/

## RQ3: Embodiment-Adaptive Realization Selection

The homepage displays nine GIFs from `assets/gifs_0/`, with three examples per robot (Franka Panda, Sawyer, UR5e). Each example includes the two-stage evaluator results from `showcase_liquid.html`:

- **Stage 1: Collision Filtering** — all 27 candidate realizations are shown as retained/rejected; a retained count appears below each GIF.
- **Stage 2: Tracking-Cost Ranking** — the full retained-candidate ranking (rank, realization, position/orientation tracking error and cost), with the selected realization highlighted.

Click **View evaluation details** to expand the two stages. The separate **Realization labels (m1–m27)** control was removed from the public page.

## Additional RQ3: Comparative Rollouts

Seven GIFs in `assets/gifs_2/` are displayed in two distinct comparison groups before the original RQ3 selection gallery.

**Panda — Baseline Comparison**

| Method | GIF |
| --- | --- |
| A3: FLoRA | `Panda_A3_FLoRA.gif` |
| B3: CrossFormer | `Panda_B3_CrossFormer.gif` |
| C3: Implicit Global | `Panda_C3_Implicit_Global.gif` |
| D3: Vanilla DP3 | `Panda_D3_Vanilla_DP3.gif` |

**Sawyer — Evaluator Ablation**

| Variant | GIF |
| --- | --- |
| A3: FLoRA (two-stage evaluator) | `Sawyer_A3_FLoRA.gif` |
| E3: Stage-1 Only (collision filtering only) | `Sawyer_E3_Stage-1_Only.gif` |
| F3: Stage-2 Only (tracking-cost ranking only) | `Sawyer_F3_Stage-2_Only.gif` |

These are illustrative rollouts, not replacement measures for paper-level evaluation. GIFs retain their intrinsic aspect ratios and load lazily.

## RQ4: Dynamic Realization Re-selection

The homepage also displays 12 GIFs from `assets/gif_3/`. These updated GIFs begin shortly before the corresponding dynamic perturbation. In each scenario, animations appear side by side in the order **CrossFormer, FLoRA-Fixed, FLoRA-Reselect**.

| Perturbation | CrossFormer | FLoRA-Fixed | FLoRA-Reselect |
| --- | --- | --- | --- |
| Target Container +5 cm (X) | `XP5CM_crossformer.gif` | `XP5CM_flora-fixed.gif` | `XP5CM_flora-reselect.gif` |
| Target Container +10 cm (Y) | `YP10CM_crossformer.gif` | `YP10CM_flora-fixed.gif` | `YP10CM_flora-reselect.gif` |
| Target Container +15 cm (X) | `XP15CM_crossformer.gif` | `XP15CM_flora-fixed.gif` | `XP15CM_flora-reselect.gif` |
| O_task movement | `crossformer_obstacle_move.gif` | `flora-fixed_obstacle_move.gif` | `flora-reselect_obstacle_move.gif` |

All GIFs are displayed at their intrinsic aspect ratio with no fixed-height crop. RQ4 images are lazy-loaded to reduce initial bandwidth usage.

## Publishing

The site is static HTML and is published by GitHub Pages from `main` via `.github/workflows/static.yml`.

This public repository publishes the project website using GitHub Actions.
