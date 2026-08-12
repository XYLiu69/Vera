# Vera: Identity-Faithful Human Subject-to-Video Generation

[**arXiv**](https://arxiv.org/abs/2607.20247) | [**Project Page**](https://xyliu69.github.io/Vera/)

**Yulong Xu**<sup>1*</sup>, **Xinyue Liu**<sup>1,2*</sup>, **Shujuan Li**<sup>1,3</sup>, **Huafeng Shi**<sup>1</sup>, **Yan Zhou**<sup>1</sup>, **Jiwen Liu**<sup>1</sup>, **Xintao Wang**<sup>1</sup>, **Pengfei Wan**<sup>1</sup>, **Yu-Shen Liu**<sup>1</sup>, **Huaibo Huang**<sup>2†</sup>

(*Equal contribution, †Corresponding author)

<sup>1</sup>Kuaishou Technology, <sup>2</sup>Institute of Automation, Chinese Academy of Sciences, <sup>3</sup>Tsinghua University

## 📖 Introduction

**TL;DR:** Vera anchors each generated person to reference identity for faithful human video generation.

## 📖 Overview

Vera is a unified human-centric subject-to-video framework for both single-person and multi-person generation. Existing S2V methods can preserve overall subject appearance while still allowing identity-critical human details to drift across frames, poses, and interactions. In multi-person scenes, this can further lead to subject confusion, attribute swapping, and excessive copying of appearance cues from the reference images. Vera addresses these issues with a million-pair identity-aligned human image-video dataset built through person-level cross-clip retrieval, together with two complementary designs. Identity-Focal Masked Supervision (IFMS) places stronger supervision on identity-relevant regions while reducing interference from irrelevant artifacts. Reference-Aware Layer-wise Attention (RALA) regulates how video tokens interact with reference identity cues in the DiT backbone, preserving stable identity anchors and improving identity readout across layers. Together, these designs improve human identity consistency, multi-person subject binding, and motion naturalness while reducing identity confusion and excessive reference-image copying.

## 📊 Dataset

We construct a large human identity dataset containing **1,001,891 aligned image and video pairs** for both single person and multi person subject to video generation. Rather than sampling reference frames directly from the target clip, we retrieve images of the same person from different clips. This provides explicit identity correspondence while naturally introducing variation in pose, expression, illumination, background, and motion context, which helps reduce shortcut copying. The resulting diverse reference sets support more reliable identity preservation and more accurate subject matching in multi person generation.

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
