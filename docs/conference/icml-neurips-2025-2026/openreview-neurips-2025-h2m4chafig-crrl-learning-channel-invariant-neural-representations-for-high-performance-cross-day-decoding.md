---
title: "CRRL: Learning Channel-invariant Neural Representations for High-performance Cross-day Decoding"
title_zh: CRRL：学习通道不变神经表示以实现高性能跨天解码
authors: "Xianhan Tan, Binli Luo, Yu Qi, Yueming Wang"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=H2m4chAfig"
tags: ["query:bci-da"]
score: 10.0
evidence: 面向BCI跨天解码的通道不变表示
tldr: 针对脑机接口中因神经元死亡和电极偏移导致的跨天信号不稳定问题，本文提出CRRL方法，通过学习通道级不变神经表示来应对不同记录日间的通道差异。该方法包含通道重排模块以对齐通道层面的变异。实验表明CRRL在跨天解码任务上性能显著提升，为稳定BCI提供了新途径，相比仅对齐低维流形的方法更能应对显著漂移。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 跨天神经信号不稳定源于通道级变异，传统流形对齐难以处理。
method: 提出CRRL，学习通道级不变神经表示并重排通道。
result: 在跨天解码上实现高性能，优于低维流形对齐方法。
conclusion: 通道不变表示是解决BCI跨天稳定性的关键。
---

## Abstract
Brain-computer interfaces have shown great potential in motor and speech rehabilitation, but still suffer from low performance stability across days, mostly due to the instabilities in neural signals. These instabilities, partially caused by neuron deaths and electrode shifts, leading to channel-level variabilities among different recording days. Previous studies mostly focused on aligning multi-day neural signals of onto a low-dimensional latent manifold to reduce the variabilities, while faced with difficulties when neural signals exhibit significant drift. Here, we propose to learn a channel-level invariant neural representation to address the variabilities in channels across days. It contains a channel-rearrangement module to learn stable representations against electrode shifts, and a channel reconstruction module to handle the missing neurons. The proposed method achieved the state-of-the-art performance with cross-day decoding tasks over two months, on multiple benchmark BCI datasets. The proposed approach showed good generalization ability that can be incorporated to different neural networks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向BCI跨天解码的通道不变表示。

### 2. 核心内容
针对脑机接口中因神经元死亡和电极偏移导致的跨天信号不稳定问题，本文提出CRRL方法，通过学习通道级不变神经表示来应对不同记录日间的通道差异。该方法包含通道重排模块以对齐通道层面的变异。实验表明CRRL在跨天解码任务上性能显著提升，为稳定BCI提供了新途径，相比仅对齐低维流形的方法更能应对显著漂移。

### 3. 对应检索需求
brain-computer interface neural decoding across days。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=H2m4chAfig](https://openreview.net/forum?id=H2m4chAfig)
