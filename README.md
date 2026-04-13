# TGMF: Taylor Gaussian Motion Field for Dynamic Head Avatars

<p align="center">
  <strong>Official project page and code hub for TGMF</strong><br/>
  A Taylor-based local motion field for dynamic Gaussian head avatars.
</p>

<p align="center">
  <a href="./index.html"><strong>Project Page</strong></a> ·
  <a href="./assets/output.mp4"><strong>Demo Video</strong></a> ·
  <a href="#citation"><strong>Citation</strong></a>
</p>

---

## Updates
- **[2026-04]** Initial GitHub showcase page is ready.
- **[Coming soon]** We will add demo videos for the remaining **8 subjects**.
- **[Planned]** More qualitative comparisons and subject-wise galleries.

---

## Overview
TGMF models dynamic head motion with a **second-order Taylor field** around a reference state.
Instead of treating Gaussian motion as a black-box frame-conditioned mapping, TGMF explicitly models **velocity** and **acceleration**, and refines motion through **bidirectional Gaussian--mesh optimization**.

This repository is organized for **project presentation first**:
- a lightweight **project page** for GitHub Pages,
- a playable **demo video**,
- clear **Do / Not Do** guidance,
- placeholders for the future **8-subject gallery**.

---

## Demo

### Main video
> GitHub Markdown does not reliably provide the best in-page video experience across all renderers.  
> For the full presentation with an embedded player, open the **Project Page**.

<p align="center">
  <a href="./index.html">
    <img src="./assets/poster.jpg" alt="TGMF demo poster" width="320"/>
  </a>
</p>

<p align="center">
  <a href="./assets/output.mp4">▶ Watch the demo video</a>
</p>

---

## Do / Not Do

### ✅ Do
- Show **smooth local motion** around a reference facial state.
- Highlight **mouth**, **eyelid**, and **hair-boundary** consistency.
- Present **novel-view synthesis** and **novel-expression/self-reenactment** results.
- Emphasize **temporal stability**, **reduced drift**, and **interpretable motion coefficients**.

### ❌ Not Do
- Do **not** describe TGMF as a universal solution for arbitrarily long or highly oscillatory motion.
- Do **not** oversell very high-frequency micro-motion fitting.
- Do **not** frame the Taylor field as a global video-time lookup table.
- Do **not** claim that the current page already contains all 9 subject videos.

---

## Subject Gallery Plan

| Subject | Status | Demo |
|---|---:|---|
| Subject 1 | Ready | `assets/output.mp4` |
| Subject 2 | Coming soon | — |
| Subject 3 | Coming soon | — |
| Subject 4 | Coming soon | — |
| Subject 5 | Coming soon | — |
| Subject 6 | Coming soon | — |
| Subject 7 | Coming soon | — |
| Subject 8 | Coming soon | — |
| Subject 9 | Coming soon | — |

---

## Recommended Repo Structure

```text
TGMF/
├── README.md
├── index.html
├── assets/
│   ├── output.mp4
│   └── poster.jpg
├── docs/                    # optional if you prefer GitHub Pages from /docs
├── configs/
├── scripts/
├── networks/
└── ...
```

---

## Suggested GitHub Pages Setup
1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Set the source to the repository **root** (or move `index.html` into `docs/` and choose `/docs`).
4. Your project page will then serve the embedded demo video directly.

---

## Acknowledgement
The project-page organization is intentionally inspired by the public presentation style often used in avatar repositories such as **MeGA**, while adapting the content to TGMF's motion-modeling focus.

---

## Citation
```bibtex
@article{wang2025tgmf,
  title   = {TGMF: Taylor Gaussian Motion Field for Dynamic Head Avatars},
  author  = {Wang, Xiangyang and Qiu, Yu and Tan, Xiao and Wang, Rui and Cheng, Erkang},
  journal = {arXiv preprint arXiv:XXXX.XXXXX},
  year    = {2025}
}
```

> Replace the arXiv identifier with the final one before release.
