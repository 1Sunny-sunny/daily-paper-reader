---
title: "SPINT: Spatial Permutation-Invariant Neural Transformer for Consistent Intracortical Motor Decoding"
title_zh: SPINT：用于稳定皮层内运动解码的空间置换不变神经变换器
authors: "Trung Le, Hao Fang, Jingyuan Li, Tung Nguyen, Lu Mi, Amy L Orsborn, Uygar Sümbül, Eli Shlizerman"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=XjayhGBraW"
tags: ["query:bci-da"]
score: 10.0
evidence: 解决皮层内脑机接口的非平稳性与跨会话解码
tldr: 针对长期皮层内脑机接口部署中神经记录非平稳、记录群体组成和调谐特性跨会话变化的问题，本文提出SPINT，一种空间置换不变的神经变换器。该方法无需固定神经身份、无需测试时标签或参数更新即可跨会话泛化。实验表明其在跨会话运动解码中实现一致稳定性能。该工作为脑机接口跨天稳定解码提供了新范式。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 现有方法依赖固定神经身份和测试时更新，难以应对神经记录的非平稳性和跨会话变化。
method: 提出空间置换不变的神经变换器SPINT，消除对固定电极身份的依赖，实现跨会话泛化。
result: 实验显示SPINT在不更新参数的情况下实现跨会话一致的皮层内运动解码性能。
conclusion: SPINT为长期脑机接口的稳定解码提供了无需对齐的新方案。
---

## Abstract
Intracortical Brain-Computer Interfaces (iBCI) decode behavior from neural population activity to restore motor functions and communication abilities in individuals with motor impairments. A central challenge for long-term iBCI deployment is the nonstationarity of neural recordings, where the composition and tuning profiles of the recorded populations are unstable across recording sessions. Existing approaches attempt to address this issue by explicit alignment techniques; however, they rely on fixed neural identities and require test-time labels or parameter updates, limiting their generalization across sessions and imposing additional computational burden during deployment. In this work, we address the problem of cross-session nonstationarity in long-term iBCI systems and introduce SPINT - a Spatial Permutation-Invariant Neural Transformer framework for behavioral decoding that operates directly on unordered sets of neural units. Central to our approach is a novel context-dependent positional embedding scheme that dynamically infers unit-specific identities, enabling flexible generalization across recording sessions. SPINT supports inference on variable-size populations and allows few-shot, gradient-free adaptation using a small amount of unlabeled data from the test session. We evaluate SPINT on three multi-session datasets from the FALCON Benchmark, covering continuous motor decoding tasks in human and non-human primates. SPINT demonstrates robust cross-session generalization, outperforming existing zero-shot and few-shot unsupervised baselines while eliminating the need for test-time alignment and fine-tuning. Our work contributes an initial step toward a robust and scalable neural decoding framework for long-term iBCI applications.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
解决皮层内脑机接口的非平稳性与跨会话解码。

### 2. 核心内容
针对长期皮层内脑机接口部署中神经记录非平稳、记录群体组成和调谐特性跨会话变化的问题，本文提出SPINT，一种空间置换不变的神经变换器。该方法无需固定神经身份、无需测试时标签或参数更新即可跨会话泛化。实验表明其在跨会话运动解码中实现一致稳定性能。该工作为脑机接口跨天稳定解码提供了新范式。

### 3. 对应检索需求
brain-computer interface neural decoding across days。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=XjayhGBraW](https://openreview.net/forum?id=XjayhGBraW)
