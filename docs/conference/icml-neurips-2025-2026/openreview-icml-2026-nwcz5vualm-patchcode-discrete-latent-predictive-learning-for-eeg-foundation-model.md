---
title: "PATCHCODE: Discrete Latent Predictive Learning for EEG Foundation Model"
title_zh: PATCHCODE：用于脑电基础模型的离散潜在预测学习
authors: "KIEREN YU, Ziyang LIU, Chang Huang, Kaishun Wu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/da1db2af1fb17b9b75f284a3b9d2ffe9f19e5f35.pdf"
tags: ["query:bci-da"]
score: 6.0
evidence: 区域感知离散码作为稳定监督目标应对脑电跨个体差异
tldr: 针对脑电信号高频噪声大、跨个体差异强导致现有预训练目标不稳定的问题，提出区域感知离散预测学习框架。该方法在保持编码器输入连续的同时，引入区域感知离散码作为稳定监督目标，通过掩码预测训练编码器。实验表明该框架能学到更具迁移性和稳健性的脑电表征。该工作为脑电基础模型提供了新的预训练思路，有助于处理个体差异。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 脑电信号噪声高、个体差异大，传统重建式预训练易受随机波动干扰。
method: 提出PATCHCODE，采用区域感知离散码作为稳定监督目标进行掩码预测学习。
result: 预训练得到的表征在多个下游任务上表现出更好的迁移性和稳定性。
conclusion: 离散潜在预测学习能有效应对脑电的非平稳性，为脑电基础模型提供更强泛化能力。
---

## Abstract
EEG foundation models aim to learn transferable representations, yet EEG recordings are dominated by high-frequency noise and large cross-subject variability. Existing pretraining strategies such as masked autoencoding or autoregressive modeling often treat waveform reconstruction as the learning signal, making the objective sensitive to stochastic fluctuations rather than consistent neurophysiological structure. To address this overlap, we propose PATCHCODE, a region-aware discrete predictive learning framework that keeps the encoder input continuous while introducing region-aware discrete codes as stable supervision targets. We pretrain a masked predictive encoder on continuous EEG patches with dual-granularity learning: it predicts missing patch-level representations to preserve fine spatiotemporal structure, while aligning them to discretized code targets from a frozen tokenizer to anchor robust semantics. Extensive experiments across sixteen downstream datasets spanning emotion recognition, motor imagery, sleep staging, seizure detection, vigilance estimation, stress detection, and clinical diagnosis demonstrate that PATCHCODE achieves competitive performance compared to state-of-the-art baselines, with notable gains in data efficiency under limited labels. Our code is available at https://github.com/kierenyyu/Patchcode.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
区域感知离散码作为稳定监督目标应对脑电跨个体差异。

### 2. 核心内容
针对脑电信号高频噪声大、跨个体差异强导致现有预训练目标不稳定的问题，提出区域感知离散预测学习框架。该方法在保持编码器输入连续的同时，引入区域感知离散码作为稳定监督目标，通过掩码预测训练编码器。实验表明该框架能学到更具迁移性和稳健性的脑电表征。该工作为脑电基础模型提供了新的预训练思路，有助于处理个体差异。

### 3. 对应检索需求
domain adaptation techniques for brain signal decoding。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=NWcZ5vualM](https://openreview.net/forum?id=NWcZ5vualM)
