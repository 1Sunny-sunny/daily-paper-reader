---
title: "ZEBRA: Towards Zero-Shot Cross-Subject Generalization for Universal Brain Visual Decoding"
title_zh: ZEBRA：面向通用脑视觉解码的零样本跨被试泛化
authors: "Haonan Wang, Jingyu Lu, Hongrui Li, Xiaomeng Li"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=CDQ0MI4rLw"
tags: ["query:bci-da"]
score: 7.0
evidence: 对抗解耦被试相关和语义相关成分实现零样本跨被试脑解码
tldr: 该论文针对现有脑视觉解码方法依赖被试特定模型或微调、难以扩展的问题，提出ZEBRA框架，利用对抗训练将fMRI表示显式解耦为被试相关和语义相关成分，实现零样本跨被试泛化；实验表明该方法无需任何被试适应即可重建视觉体验，为通用脑解码和领域自适应提供了新思路。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 现有脑视觉解码方法依赖被试特定模型或微调，限制可扩展性和实际应用。
method: 提出ZEBRA框架，利用对抗训练将fMRI表示分解为被试相关和语义相关成分，实现零样本跨被试泛化。
result: 实验显示ZEBRA无需被试特定适应即可重建视觉体验，达到通用解码效果。
conclusion: 该方法为脑解码中的跨被试域自适应提供了有效方案，推动通用脑机接口研究。
---

## Abstract
Recent advances in neural decoding have enabled the reconstruction of visual experiences from brain activity, positioning fMRI-to-image reconstruction as a promising bridge between neuroscience and computer vision. However, current methods predominantly rely on subject-speciﬁc models or require subject-speciﬁc ﬁne-tuning, limiting their scalability and real-world applicability. In this work, we introduce ZEBRA, the ﬁrst zero-shot brain visual decoding framework that eliminates the need for subject-speciﬁc adaptation. Z EBRA is built on the key insight that fMRI representations can be decomposed into subject-related and semantic-related components. By leveraging adversarial training, our method explicitly disentangles these components to isolate subject-invariant, semantic-speciﬁc representations. This disentanglement allows ZEBRA to generalize to unseen subjects without any additional fMRI data or retraining. Extensive experiments show that ZEBRA signiﬁcantly outperforms zero-shot baselines and achieves performance comparable to fully ﬁnetuned models on several metrics. Our work represents a scalable and practical step toward universal neural decoding. Code and model weights are available at: https://github.com/xmed-lab/ZEBRA.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
对抗解耦被试相关和语义相关成分实现零样本跨被试脑解码。

### 2. 核心内容
该论文针对现有脑视觉解码方法依赖被试特定模型或微调、难以扩展的问题，提出ZEBRA框架，利用对抗训练将fMRI表示显式解耦为被试相关和语义相关成分，实现零样本跨被试泛化；实验表明该方法无需任何被试适应即可重建视觉体验，为通用脑解码和领域自适应提供了新思路。

### 3. 对应检索需求
domain adaptation techniques for brain signal decoding。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=CDQ0MI4rLw](https://openreview.net/forum?id=CDQ0MI4rLw)
