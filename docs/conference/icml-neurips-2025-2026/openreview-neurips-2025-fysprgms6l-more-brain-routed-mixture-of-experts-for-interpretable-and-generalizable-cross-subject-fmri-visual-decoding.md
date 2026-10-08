---
title: "MoRE-Brain: Routed Mixture of Experts for Interpretable and Generalizable Cross-Subject fMRI Visual Decoding"
title_zh: MoRE-Brain：用于可解释和泛化跨被试fMRI视觉解码的路由专家混合
authors: "YUXIANG WEI, Yanteng Zhang, Xi Xiao, Tianyang Wang, Xiao Wang, Vince Calhoun"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=fYSPRGmS6l"
tags: ["query:bci-da"]
score: 5.0
evidence: 跨被试fMRI视觉解码的专家混合
tldr: MoRE-Brain针对当前fMRI视觉解码忽视可解释性、跨被试泛化不足的问题，提出神经启发框架，采用分层专家混合架构，不同专家处理功能相关体素群。专家编码fMRI到冻结表示空间，实现高保真、可适应的视觉重建。该方法提升跨被试泛化能力和可解释性。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 现有fMRI视觉解码忽视可解释性，跨被试泛化不足。
method: 采用分层专家混合，专家处理功能相关体素组。
result: 实现高保真、可适应的视觉重建。
conclusion: 提供可解释且泛化的fMRI视觉解码。
---

## Abstract
Decoding visual experiences from fMRI offers a powerful avenue to understand human perception and develop advanced brain-computer interfaces. However, current progress often prioritizes maximizing reconstruction fidelity while overlooking interpretability, an essential aspect for deriving neuroscientific insight. To address this gap, we propose MoRE-Brain, a neuro-inspired framework designed for high-fidelity, adaptable, and interpretable visual reconstruction. MoRE-Brain uniquely employs a hierarchical Mixture-of-Experts architecture where distinct experts process fMRI signals from functionally related voxel groups, mimicking specialized brain networks. The experts are first trained to encode fMRI into the frozen CLIP space. A finetuned diffusion model then synthesizes images, guided by expert outputs through a novel dual-stage routing mechanism that dynamically weighs expert contributions across the diffusion process. MoRE-Brain offers three main advancements: First, it introduces a novel Mixture-of-Experts architecture grounded in brain network principles for neuro-decoding. Second, it achieves efficient cross-subject generalization by sharing core expert networks while adapting only subject-specific routers. Third, it provides enhanced mechanistic insight, as the explicit routing reveals precisely how different modeled brain regions shape the semantic and spatial attributes of the reconstructed image. Extensive experiments validate MoRE-Brain’s high reconstruction fidelity, with bottleneck analyses further demonstrating its effective utilization of fMRI signals, distinguishing genuine neural decoding from over-reliance on generative priors. Consequently, MoRE-Brain marks a substantial advance towards more generalizable and interpretable fMRI-based visual decoding.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
跨被试fMRI视觉解码的专家混合。

### 2. 核心内容
MoRE-Brain针对当前fMRI视觉解码忽视可解释性、跨被试泛化不足的问题，提出神经启发框架，采用分层专家混合架构，不同专家处理功能相关体素群。专家编码fMRI到冻结表示空间，实现高保真、可适应的视觉重建。该方法提升跨被试泛化能力和可解释性。

### 3. 对应检索需求
domain adaptation techniques for brain signal decoding。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=fYSPRGmS6l](https://openreview.net/forum?id=fYSPRGmS6l)
