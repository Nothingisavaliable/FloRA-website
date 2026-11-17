# FLoRA Project Website

Minimal project page for **FLoRA — Multiple Task Realizations for Embodiment-Adaptive Robot Manipulation**.

Live page: https://nothingisavaliable.github.io/FloRA-website/

## RQ3: Embodiment-Adaptive Realization Selection

The homepage currently displays nine recorded pouring GIFs, three per robot. Files are stored under `assets/gifs/`.

| Robot | Display order |
| --- | --- |
| Franka Panda | `Panda_m7_E_yp05_yawm20.gif`, `Panda_m16_E_yp05_yawm20.gif`, `Panda_m4_E_yp05_yawp20.gif` |
| Sawyer | `Sawyer_m1_f21_dx+0.03_dy-0.03_yaw+0.gif`, `Sawyer_m21_f36_supplement_dx+0.00_dy+0.00_yaw+5.gif`, `Sawyer_m2_f03_dx+0.00_dy-0.03_yaw+0.gif` |
| UR5e | `UR5e_m18_f26_dx+0.03_dy+0.03_yaw+10.gif`, `UR5e_m16_f06_dx+0.00_dy+0.03_yaw+0.gif`, `UR5e_m25_f25_dx+0.03_dy+0.03_yaw-10.gif` |

Each caption identifies the selected realization. The detailed evaluator candidate tables from the local `showcase_liquid.html` are intentionally omitted from the minimalist landing page.

## Planned RQ4: Dynamic Re-selection

RQ4 GIFs are **not yet included**. The planned layout is a 4-by-3 scenario/method comparison: bowl displacements of 5, 10, and 15 cm, plus task-object movement, with columns for CrossFormer, FLoRA-Fixed, and FLoRA-Reselect. Add these only after uploading the actual recordings; avoid presenting placeholders as experimental results.

## Publishing

The website is a static `index.html`, with no build dependencies. GitHub Pages publishes changes to `main` using `.github/workflows/static.yml`.
