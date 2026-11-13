# FLoRA Project Website

A minimal research project page for **FLoRA — Multiple Task Realizations for Embodiment-Adaptive Robot Manipulation**.

Live page: https://nothingisavaliable.github.io/FloRA-website/

## Add pouring demonstrations

The page displays three GIFs. Upload your own robot rollout recordings into the existing `assets` directory using these exact paths:

| File | Caption |
| --- | --- |
| `assets/panda.gif` | Franka Panda |
| `assets/ur5e.gif` | UR5e |
| `assets/sawyer.gif` | Sawyer |

Until each GIF is uploaded, the corresponding tile shows “Coming soon”. Actual experiment GIFs replace the placeholders automatically after a commit to `main`.

Tips: export consistent 4:3 GIFs if possible, keep camera framing and playback speed comparable, and compress large animations to reduce loading time. If you use a different filename or file format, update its `src` in `index.html`.

## Publishing and editing

This is a dependency-free HTML/CSS page served by GitHub Pages. The workflow at `.github/workflows/static.yml` deploys changes from `main`. To edit the page, update `index.html`; no build setup is required.
