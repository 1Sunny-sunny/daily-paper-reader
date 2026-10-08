---
title: "S$^2$M-Former: Spiking Symmetric Mixing Branchformer for Brain Auditory Attention Detection"
title_zh: S²M-Former：用于大脑听觉注意力检测的脉冲对称混合分支former
authors: "Jiaqi Wang, Zhengyu Ma, Xiongri Shen, Chenlin Zhou, Leilei Zhao, Han Zhang, Yi Zhong, Siqi Cai, Zhenxi Song, Zhiguo Zhang"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=WtMuGdHvh6"
tags: ["query:bci-da"]
score: 5.0
evidence: 基于EEG的听觉注意力检测脉冲神经网络
tldr: 针对EEG听觉注意力检测中缺乏能充分利用互补特征且能效高的框架问题，本文提出脉冲对称混合框架S²M-Former，采用并行空间和频率分支的镜像对称结构，利用生物启发的令牌-通道混合器在脉冲驱动下进行特征融合。实验表明该方法在能效约束下提升了解码性能，为神经操控听力设备提供了高效方案。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 现有EEG听觉注意力检测缺乏能效与特征融合兼顾的方法。
method: 设计脉冲对称混合分支former，并行处理空间与频率信息。
result: 在能效约束下实现高精度听觉注意力解码。
conclusion: 脉冲混合框架为低功耗BCI提供了新思路。
---

## Abstract
Auditory attention detection (AAD) aims to decode listeners' focus in complex auditory environments from electroencephalography (EEG) recordings, which is crucial for developing neuro-steered hearing devices.  Despite recent advancements, EEG-based AAD remains hindered by the absence of synergistic frameworks that can fully leverage complementary EEG features under energy-efficiency constraints. We propose ***S$^2$M-Former***, a novel ***s***piking ***s***ymmetric ***m***ixing framework to address this limitation through two key innovations:  i)   Presenting a spike-driven symmetric architecture composed of parallel spatial and frequency branches with mirrored modular design, leveraging biologically plausible token-channel mixers to enhance complementary learning across branches; ii) Introducing lightweight 1D token sequences to replace conventional 3D operations, reducing parameters by 14.7$\times$. The brain-inspired spiking architecture further reduces power consumption, achieving a 5.8$\times$ energy reduction compared to recent ANN methods, while also surpassing existing SNN baselines in terms of parameter efficiency and performance. Comprehensive experiments on three AAD benchmarks (KUL, DTU and AV-GC-AAD) across three settings (within-trial, cross-trial and cross-subject) demonstrate that S$^2$M-Former achieves comparable state-of-the-art (SOTA) decoding accuracy, making it a promising low-power, high-performance solution for AAD tasks. Code is available at https://github.com/JackieWang9811/S2M-Former.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
基于EEG的听觉注意力检测脉冲神经网络。

### 2. 核心内容
针对EEG听觉注意力检测中缺乏能充分利用互补特征且能效高的框架问题，本文提出脉冲对称混合框架S²M-Former，采用并行空间和频率分支的镜像对称结构，利用生物启发的令牌-通道混合器在脉冲驱动下进行特征融合。实验表明该方法在能效约束下提升了解码性能，为神经操控听力设备提供了高效方案。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=WtMuGdHvh6](https://openreview.net/forum?id=WtMuGdHvh6)
