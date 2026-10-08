---
title: "A Scalable, Causal, and Energy Efficient Framework for Neural Decoding with Spiking Neural Networks"
title_zh: 面向神经解码的可扩展因果高能效脉冲神经网络框架
authors: "Georgios Mentzelopoulos, Ioannis Asmanis, Konrad Kording, Eva L Dyer, Kostas Daniilidis, Flavia Vitale"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=oAbaGU9N1X"
tags: ["query:bci-da"]
score: 7.0
evidence: 面向BCI的因果高能效脉冲神经网络解码框架
tldr: 该论文针对现有BCI神经解码器要么因果但泛化差、要么非因果难以实时且功耗高的问题，提出基于脉冲神经网络的可扩展因果框架；实验表明该框架在保持因果性和实时性的同时具有高能效，为资源受限的脑机接口提供了可行的解码方案。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 现有学习型神经解码器难以兼顾因果性、泛化能力和实时低功耗需求。
method: 采用脉冲神经网络构建可扩展、因果且高能效的神经解码框架。
result: 该框架在实时性和能效上表现优异，同时保持解码精度。
conclusion: SNN解码器为脑机接口在资源受限设备上的实际部署提供了新途径。
---

## Abstract
Brain-computer interfaces (BCIs) promise to enable vital functions, such as speech and prosthetic control, for individuals with neuromotor impairments. Central to their success are neural decoders, models that map neural activity to intended behavior. Current learning-based decoding approaches fall into two classes: simple, causal models that lack generalization, or complex, non-causal models that generalize and scale offline but struggle in real-time settings. Both face a common challenge, their reliance on power-hungry artificial neural network backbones, which makes integration into real-world, resource-limited systems difficult. Spiking neural networks (SNNs) offer a promising alternative. Because they operate causally (i.e. only on present and past inputs) these models are suitable for real-time use, and their low energy demands make them ideal for battery-constrained environments. To this end, we introduce **Spikachu: a scalable, causal, and energy-efficient neural decoding framework based on SNNs**. Our approach processes binned spikes directly by projecting them into a shared latent space, where spiking modules, adapted to the timing of the input, extract relevant features; these latent representations are then integrated and decoded to generate behavioral predictions. We evaluate our approach on 113 recording sessions from 6 non-human primates, totaling 43 hours of recordings. Our method outperforms causal baselines when trained on single sessions using between 2.26× and 418.81× less energy. Furthermore, we demonstrate that scaling up training to multiple sessions and subjects improves performance and enables few-shot transfer to unseen sessions, subjects, and tasks. Overall, Spikachu introduces a scalable, online-compatible neural decoding framework based on SNNs, whose performance is competitive relative to state-of-the-art models while consuming orders of magnitude less energy.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向BCI的因果高能效脉冲神经网络解码框架。

### 2. 核心内容
该论文针对现有BCI神经解码器要么因果但泛化差、要么非因果难以实时且功耗高的问题，提出基于脉冲神经网络的可扩展因果框架；实验表明该框架在保持因果性和实时性的同时具有高能效，为资源受限的脑机接口提供了可行的解码方案。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=oAbaGU9N1X](https://openreview.net/forum?id=oAbaGU9N1X)
