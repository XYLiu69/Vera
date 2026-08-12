# Vera: Identity-Faithful Human Subject-to-Video Generation

[**arXiv**](https://arxiv.org/abs/2607.20247) | [**Project Page**](https://xyliu69.github.io/Vera/)

**Yulong Xu**<sup>1*</sup>, **Xinyue Liu**<sup>1,2*</sup>, **Shujuan Li**<sup>1,3</sup>, **Huafeng Shi**<sup>1</sup>, **Yan Zhou**<sup>1</sup>, **Jiwen Liu**<sup>1</sup>, **Xintao Wang**<sup>1</sup>, **Pengfei Wan**<sup>1</sup>, **Yu-Shen Liu**<sup>1</sup>, **Huaibo Huang**<sup>2†</sup>

(*Equal contribution, †Corresponding author)

<sup>1</sup>Kuaishou Technology, <sup>2</sup>Institute of Automation, Chinese Academy of Sciences, <sup>3</sup>Tsinghua University

## 📖 Introduction

**TL;DR:** Vera anchors each generated person to reference identity for faithful human video generation.

## 📖 Overview

Vera is a unified identity-faithful human subject-to-video generation framework for both single-person and multi-person scenarios. Unlike prior subject-to-video methods that mainly preserve coarse appearance, Vera focuses on fine-grained facial identity and maintains reliable identity–role–trajectory binding throughout generation. It is trained with a million-pair identity-aligned human image–video dataset and introduces Identity-Focal Masked Supervision (IFMS) to emphasize identity-critical facial regions, together with Reference-Aware Layer-wise Attention (RALA) to preserve stable reference anchors and selectively strengthen identity information at identity-sensitive layers. These designs enable Vera to generate natural, temporally coherent human videos while maintaining strong identity fidelity under pose, expression, viewpoint, motion, and interaction changes.

## 🌟 Citation

Please give us a star 🌟 and cite our paper if you find our work helpful.

```bibtex
@article{xu2026vera,
  title   = {Vera: Identity-Faithful Human Subject-to-Video Generation},
  author  = {Xu, Yulong and Liu, Xinyue and Li, Shujuan and Shi, Huafeng and Zhou, Yan and Liu, Jiwen and Wang, Xintao and Wan, Pengfei and Liu, Yu-Shen and Huang, Huaibo},
  journal = {arXiv preprint arXiv:2607.20247},
  year    = {2026}
}
```
