---
title: "MEIcoder: Decoding Visual Stimuli from Neural Activity by Leveraging Most Exciting Inputs"
title_zh: MEIcoder：利用最兴奋输入从神经活动解码视觉刺激
authors: "Jan Sobotka, Luca Baroni, Ján Antolík"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=V3WQoshcZe"
tags: ["query:bci-da"]
score: 6.0
evidence: 面向脑机接口的神经活动视觉刺激解码
tldr: 该论文针对神经解码中生物数据稀缺、深度学习解码困难的问题，提出MEIcoder方法，利用神经元特异的最兴奋输入、结构相似性损失和对抗训练；在灵长类初级视觉皮层单细胞活动上实现了最先进的视觉刺激重建，为脑机接口中的神经解码提供了有效方案。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 神经解码面临生物数据稀缺，高吞吐记录技术在灵长类或人类中难以应用。
method: 利用神经元最兴奋输入、结构相似性指标损失和对抗训练构建生物信息驱动的解码器。
result: MEIcoder在单细胞活动重建视觉刺激上达到最先进性能，优于现有方法。
conclusion: 该解码方法展示了利用生物先验提升神经解码的潜力，可促进脑机接口应用。
---

## Abstract
Decoding visual stimuli from neural population activity is crucial for understanding the brain and for applications in brain-machine interfaces. However, such biological data is often scarce, particularly in primates or humans, where high-throughput recording techniques, such as two-photon imaging, remain challenging or impossible to apply. This, in turn, poses a challenge for deep learning decoding techniques. To overcome this, we introduce MEIcoder, a biologically informed decoding method that leverages neuron-specific most exciting inputs (MEIs), a structural similarity index measure loss, and adversarial training. MEIcoder achieves state-of-the-art performance in reconstructing visual stimuli from single-cell activity in primary visual cortex (V1), especially excelling on small datasets with fewer recorded neurons. Using ablation studies, we demonstrate that MEIs are the main drivers of the performance, and in scaling experiments, we show that MEIcoder can reconstruct high-fidelity natural-looking images from as few as 1,000-2,500 neurons and less than 1,000 training data points. We also propose a unified benchmark with over 160,000 samples to foster future research. Our results demonstrate the feasibility of reliable decoding in early visual system and provide practical insights for neuroscience and neuroengineering applications.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向脑机接口的神经活动视觉刺激解码。

### 2. 核心内容
该论文针对神经解码中生物数据稀缺、深度学习解码困难的问题，提出MEIcoder方法，利用神经元特异的最兴奋输入、结构相似性损失和对抗训练；在灵长类初级视觉皮层单细胞活动上实现了最先进的视觉刺激重建，为脑机接口中的神经解码提供了有效方案。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=V3WQoshcZe](https://openreview.net/forum?id=V3WQoshcZe)
