# FLoRA Project Website

Minimal project page for **FLoRA — Multiple Task Realizations for Embodiment-Adaptive Robot Manipulation**.

Live page: https://nothingisavaliable.github.io/FloRA-website/

## RQ3: Embodiment-Adaptive Realization Selection

The homepage displays nine GIFs from `assets/gifs/`, with three examples per robot (Panda, Sawyer, UR5e). For each example the page preserves the two-stage evaluator data from `showcase_liquid.html`:

- **Stage 1: Collision Filtering** — all 27 candidates are shown with their retained/rejected status, and a retained count.
- **Stage 2: Tracking-Cost Ranking** — full table of the retained candidates (rank, implementation, position error, orientation error, and tracking cost) with the selected realization highlighted.

A compact two-stage summary appears below every GIF; click **View evaluation details** to expand both full datasets. The original m1–m27 realization names are accessible through **Realization labels (m1–m27)**.

## Planned RQ4: Dynamic Re-selection

RQ4 videos have **not yet been uploaded**. The planned layout is a 4-by-3 comparison: bowl displacements of 5, 10, and 15 cm, and task-object movement; methods CrossFormer, FLoRA-Fixed, and FLoRA-Reselect. The site does not show unverified placeholders as experimental results.

## Publishing

The site is a single static HTML file, published to GitHub Pages from the `main` branch using `.github/workflows/static.yml`.
