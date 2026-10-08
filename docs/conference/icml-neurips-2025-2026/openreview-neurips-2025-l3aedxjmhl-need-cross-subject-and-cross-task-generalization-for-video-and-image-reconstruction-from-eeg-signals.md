---
title: "NEED: Cross-Subject and Cross-Task Generalization for Video and Image Reconstruction from EEG Signals"
title_zh: NEED：基于脑电信号的视频与图像重建的跨被试与跨任务泛化
authors: "Shuai Huang, Huan Luo, Haodong Jing, Qixian Zhang, Litao Chang, Yating Feng, Xiao Lin, Chendong Qin, Han Chen, Shuwen Jia, Siyi Sun, Yongxiong Wang"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=L3aEdxJMHl"
tags: ["query:bci-da"]
score: 7.0
evidence: 个体适应模块归一化个体特异性模式以实现跨被试脑电视觉解码
tldr: 针对脑电视觉重建中跨被试泛化差和任务受限的问题，提出NEED框架。该框架通过个体适应模块在多数据集上预训练以归一化被试特异性模式，并解决空间分辨率限制等挑战。实验表明NEED首次实现零样本跨被试和跨任务的视频与图像重建。该工作为脑电解码中的个体差异适应提供了有效方法，与跨天会话适应具有共通性。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 脑电视觉重建模型在跨被试泛化上表现差，且局限于特定视觉任务。
method: 提出NEED，包含个体适应模块，在多脑电数据集上预训练以归一化个体差异。
result: 实现了零样本跨被试和跨任务的视频与图像重建，性能显著提升。
conclusion: 个体适应策略有效克服脑电个体差异，可推广至其他需要跨被试或跨会话适应的解码任务。
---

## Abstract
Translating brain activity into meaningful visual content has long been recognized as a fundamental challenge in neuroscience and brain-computer interface research. Recent advances in EEG-based neural decoding have shown promise, yet two critical limitations remain in this area: poor generalization across subjects and constraints to specific visual tasks. We introduce NEED, the first unified framework achieving zero-shot cross-subject and cross-task generalization for EEG-based visual reconstruction. Our approach addresses three fundamental challenges: (1) cross-subject variability through an Individual Adaptation Module pretrained on multiple EEG datasets to normalize subject-specific patterns, (2) limited spatial resolution and complex temporal dynamics via a dual-pathway architecture capturing both low-level visual dynamics and high-level semantics, and (3) task specificity constraints through a unified inference mechanism adaptable to different visual domains. For video reconstruction, NEED achieves better performance than existing methods. Importantly, Our model maintains 93.7% of within-subject classification performance and 92.4% of visual reconstruction quality when generalizing to unseen subjects, while achieving an SSIM of 0.352 when transferring directly to static image reconstruction without fine-tuning, demonstrating how neural decoding can move beyond subject and task boundaries toward truly generalizable brain-computer interfaces.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
个体适应模块归一化个体特异性模式以实现跨被试脑电视觉解码。

### 2. 核心内容
针对脑电视觉重建中跨被试泛化差和任务受限的问题，提出NEED框架。该框架通过个体适应模块在多数据集上预训练以归一化被试特异性模式，并解决空间分辨率限制等挑战。实验表明NEED首次实现零样本跨被试和跨任务的视频与图像重建。该工作为脑电解码中的个体差异适应提供了有效方法，与跨天会话适应具有共通性。

### 3. 对应检索需求
domain adaptation techniques for brain signal decoding。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=L3aEdxJMHl](https://openreview.net/forum?id=L3aEdxJMHl)
