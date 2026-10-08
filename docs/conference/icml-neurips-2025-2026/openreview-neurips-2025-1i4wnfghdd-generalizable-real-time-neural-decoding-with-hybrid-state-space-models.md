---
title: "Generalizable, real-time neural decoding with hybrid state-space models"
title_zh: 基于混合状态空间模型的泛化实时神经解码
authors: "Avery Hee-Woon Ryoo, Nanda H Krishna, Ximeng Mao, Mehdi Azabou, Eva L Dyer, Matthew G Perich, Guillaume Lajoie"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=1i4wNFgHDd"
tags: ["query:bci-da"]
score: 9.0
evidence: 面向脑机接口的实时神经解码，具有对未见数据的泛化能力
tldr: 该论文针对脑机接口中神经解码模型难以同时满足泛化性与实时性约束的问题。提出POSSM混合架构，通过跨注意力进行脉冲标记化并结合循环状态空间层，以较低计算成本实现强泛化能力。在多个神经数据集上的实验结果验证了其优越性能，为实时脑机接口提供了实用方案。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 实时神经解码对脑机接口至关重要，但现有方法难以兼顾泛化性和低延迟。
method: 提出混合状态空间模型POSSM，结合脉冲标记化和跨注意力模块与循环结构。
result: 在多个神经数据集上取得优于现有方法的速度与泛化性能。
conclusion: 为实时且泛化的神经解码提供了高效可行的架构，适用于资源受限场景。
---

## Abstract
Real-time decoding of neural activity is central to neuroscience and neurotechnology applications, from closed-loop experiments to brain-computer interfaces, where models are subject to strict latency constraints. Traditional methods, including simple recurrent neural networks, are fast and lightweight but often struggle to generalize to unseen data. In contrast, recent Transformer-based approaches leverage large-scale pretraining for strong generalization performance, but typically have much larger computational requirements and are not always suitable for low-resource or real-time settings. To address these shortcomings, we present POSSM, a novel hybrid architecture that combines individual spike tokenization via a cross-attention module with a recurrent state-space model (SSM) backbone to enable (1) fast and causal online prediction on neural activity and (2) efficient generalization to new sessions, individuals, and tasks through multi-dataset pretraining. We evaluate POSSM's decoding performance and inference speed on intracortical decoding of monkey motor tasks, and show that it extends to clinical applications, namely handwriting and speech decoding in human subjects. Notably, we demonstrate that pretraining on monkey motor-cortical recordings improves decoding performance on the human handwriting task, highlighting the exciting potential for cross-species transfer. In all of these tasks, we find that POSSM achieves decoding accuracy comparable to state-of-the-art Transformers, at a fraction of the inference cost (up to 9x faster on GPU). These results suggest that hybrid SSMs are a promising approach to bridging the gap between accuracy, inference speed, and generalization when training neural decoders for real-time, closed-loop applications.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向脑机接口的实时神经解码，具有对未见数据的泛化能力。

### 2. 核心内容
该论文针对脑机接口中神经解码模型难以同时满足泛化性与实时性约束的问题。提出POSSM混合架构，通过跨注意力进行脉冲标记化并结合循环状态空间层，以较低计算成本实现强泛化能力。在多个神经数据集上的实验结果验证了其优越性能，为实时脑机接口提供了实用方案。

### 3. 对应检索需求
brain-computer interface neural decoding across days。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=1i4wNFgHDd](https://openreview.net/forum?id=1i4wNFgHDd)
