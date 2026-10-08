---
title: "ViEEG: Hierarchical Visual Neural Representation for EEG Brain Decoding"
title_zh: ViEEG：用于EEG脑解码的分层视觉神经表示
authors: "Minxu Liu, Donghai Guan, Chuhang Zheng, Chunwei Tian, Jie Wen, Qi Zhu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/6cc1ca714b70889700eadd325b51f651d9b8c40a.pdf"
tags: ["query:bci-da"]
score: 5.0
evidence: 从EEG进行分层视觉解码
tldr: ViEEG针对现有EEG视觉解码方法忽视大脑分层视觉处理的问题，提出神经启发框架，将视觉刺激分解为轮廓、前景物体和场景三个生物对齐组件，作为锚点进行分层表示。实验表明该框架提升EEG视觉解码性能，为脑机接口视觉解码提供新方法。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有EEG视觉解码忽视大脑分层视觉处理。
method: 将视觉刺激分解为轮廓、前景物体和场景，作为锚点进行分层表示。
result: 提升EEG视觉解码性能。
conclusion: 为EEG视觉解码提供神经启发框架。
---

## Abstract
Understanding and decoding brain activity into visual representations is a fundamental challenge at the intersection of neuroscience and artificial intelligence. While electroencephalogram (EEG) visual decoding has shown promise due to its non-invasive and low-cost nature, existing methods suffer from {Hierarchical Neural Encoding Neglect (HNEN)}, a critical limitation in which flat neural representations fail to model the brain’s hierarchical visual processing. Inspired by the hierarchical organization of visual cortex, we propose ViEEG, a neuro-inspired framework that addresses HNEN. ViEEG decomposes each visual stimulus into three biologically aligned components, namely contour, foreground object, and contextual scene, which serve as anchors for a three-stream EEG encoder. These EEG features are progressively integrated via cross-attention routing, simulating cortical information flow from low-level to high-level vision. We further adopt hierarchical contrastive learning for EEG-CLIP representation alignment, enabling zero-shot object recognition. Extensive experiments on THINGS-EEG dataset demonstrate that ViEEG significantly outperforms previous methods by a large margin in both subject-dependent and subject-independent settings. Results on THINGS-MEG dataset further confirm ViEEG's generalization to different neural modalities. ViEEG not only advances the performance frontier but also sets a new paradigm for EEG brain visual decoding. Our code is available at https://github.com/LauMason/ViEEG.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
从EEG进行分层视觉解码。

### 2. 核心内容
ViEEG针对现有EEG视觉解码方法忽视大脑分层视觉处理的问题，提出神经启发框架，将视觉刺激分解为轮廓、前景物体和场景三个生物对齐组件，作为锚点进行分层表示。实验表明该框架提升EEG视觉解码性能，为脑机接口视觉解码提供新方法。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=DkK7GUr8n3](https://openreview.net/forum?id=DkK7GUr8n3)
