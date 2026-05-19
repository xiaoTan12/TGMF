# TGMF: Taylor Gaussian Motion Field for Dynamic Head Avatars

**Submitted to IEEE Transactions on Multimedia**

Xiangyang Wang<sup>1</sup>, Yu Qiu<sup>1</sup>, Xiao Tan<sup>1</sup>, Rui Wang<sup>1,†</sup> Senior Member, IEEE, and Erkang Cheng<sup>2</sup>

<sup>1</sup> School of Communication and Information Engineering, Shanghai University, Shanghai 200444, China  
<sup>2</sup> Nullmax Co., Ltd., Shanghai, China  
<sup>†</sup> Corresponding author: Rui Wang

[![Paper](https://img.shields.io/badge/Paper-coming_soon-4c6ef5?style=for-the-badge)](#)
[![Code](https://img.shields.io/badge/Code-GitHub-black?style=for-the-badge)](https://github.com/xiaoTan12/TGMF)
[![Project Page](https://img.shields.io/badge/Project-Page-0f9d58?style=for-the-badge)](https://xiaotan12.github.io/TGMF/)

---

## Status

- [x] Project page is online.
- [x] Framework figure is available in this repository.
- [x] Demo video for the current subject is available.
- [ ] Paper PDF link will be added.
- [ ] Code release will be added.
- [ ] Demo videos for 8 additional subjects will be added.

## Framework

![TGMF framework](framework.png)

Overview of TGMF. The method models Gaussian motion with a second-order Taylor field and improves temporal consistency through bidirectional Gaussian--mesh optimization.

## Demo Video

[![Demo video poster](poster.jpg)](output.mp4)

Click the preview image to open the full-resolution demo video.

## Abstract

3D Gaussian Splatting has recently enabled high-quality head avatar reconstruction and animation. However, existing dynamic head-avatar methods usually rely on fixed Gaussian--mesh bindings or implicit deformation networks that do not explicitly model the geometric relationship between local Gaussian motion and global mesh deformation. As a result, they remain prone to local distortion, temporal blur, and drift under large expressions or rapid head motion.

This paper proposes Taylor Gaussian Motion Field (TGMF), a locally continuous dynamic field that parameterizes motion-related Gaussian attributes using a second-order Taylor formulation around a reference state. Rather than treating motion as a frame-conditioned black-box mapping, TGMF explicitly associates Gaussian evolution with interpretable velocity and acceleration coefficients, yielding a compact, differentiable, and physically meaningful representation of local dynamics.

To couple local Gaussian motion with global head geometry, we further introduce a unified affine motion formulation and a mesh-coupled optimization strategy that allows Gaussian trajectories to drive mesh deformation while using mesh reconstruction errors to refine the Gaussian motion field through bidirectional feedback. This design improves temporal consistency without sacrificing local flexibility in highly dynamic regions such as hair boundaries and facial contours.

Experiments on NeRSemble show that TGMF achieves stronger rendering fidelity than publicly reproducible baselines in both novel-view synthesis and self-reenactment, while producing smoother and more stable dynamic motion.

## Contact

For questions about this project, please contact Rui Wang or Xiao Tan through the affiliations and email addresses listed above.
