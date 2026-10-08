---
title: "PCRNet: Phase-aware Complex Refinement Network for EEG-based Auditory Attention Decoding"
title_zh: PCRNet：用于EEG听觉注意力解码的相位感知复数细化网络
authors: "Xiran Chen, Xiaoke Yang, Jian Zhou, Zhao Lv, Cunhang Fan"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/a7e7895f3a0e532a3ecb4ee5cd0cf84dbeefd93d.pdf"
tags: ["query:bci-da"]
score: 5.0
evidence: 基于EEG的听觉注意力解码神经模型
tldr: 针对现有EEG听觉注意力解码方法忽略相位信息导致鲁棒性不足的问题，本文提出相位感知复数细化网络PCRNet，通过时序上下文校准模块和双域集成模块利用相位引导区分结构化神经模式与随机噪声。实验表明，该方法在多说话人环境中能更准确地识别目标说话人，为神经操控听力设备提供了更鲁棒的解码模型。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有EEG听觉注意力解码方法忽略相位信息，导致抗噪能力差。
method: 提出相位感知复数细化网络，包含时序上下文校准和双域集成模块。
result: 在多说话人环境中实现更鲁棒的听觉注意力解码。
conclusion: 相位信息对EEG解码至关重要，PCRNet提升了解码性能。
---

## Abstract
Auditory attention decoding (AAD) based on Electroencephalography (EEG) aims to identify the attended speaker in multi-speaker environments. However, existing methods typically overlook the crucial phase information of EEG signals, which limits their ability to distinguish structured neural patterns from random noise in the frequency domain and hinders robust decoding. To address these issues, this paper proposes a Phase-aware Complex Refinement Network (PCRNet) for AAD, which consists of a Temporal Context Calibration (TCC) module and a Dual-Domain Integration (DDI) module. Specifically, the TCC module captures long-range temporal dependencies through multi-scale temporal attention mechanism, while the DDI module employs a phase-guided spectral filtering strategy to dynamically suppress noise-dominated frequencies and refine the real and imaginary components separately. This design enables effective phase recalibration and enhances the discriminability of target features in the complex domain. Experimental results on three public datasets demonstrate that PCRNet outperforms state-of-the-art (SOTA) methods, particularly under challenging ultra-short 0.1-second windows. Code is available at: https://github.com/SunshineGreeny/PCRNet.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
基于EEG的听觉注意力解码神经模型。

### 2. 核心内容
针对现有EEG听觉注意力解码方法忽略相位信息导致鲁棒性不足的问题，本文提出相位感知复数细化网络PCRNet，通过时序上下文校准模块和双域集成模块利用相位引导区分结构化神经模式与随机噪声。实验表明，该方法在多说话人环境中能更准确地识别目标说话人，为神经操控听力设备提供了更鲁棒的解码模型。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=89MeH5Ax8r](https://openreview.net/forum?id=89MeH5Ax8r)
