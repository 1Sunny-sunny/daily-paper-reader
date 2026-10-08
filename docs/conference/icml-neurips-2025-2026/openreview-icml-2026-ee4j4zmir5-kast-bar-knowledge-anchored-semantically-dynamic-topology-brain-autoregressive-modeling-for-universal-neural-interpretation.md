---
title: "KAST-BAR: Knowledge-Anchored Semantically-Dynamic Topology Brain Autoregressive Modeling for Universal Neural Interpretation"
title_zh: KAST-BAR：知识锚定的语义动态拓扑脑自回归模型用于通用神经解释
authors: "Haoning Wang, Wenchao Yang, Shuai Shen, Yang Li"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/007369c349d8375f649f19dc264fba83c9d92fe8.pdf"
tags: ["query:bci-da"]
score: 5.0
evidence: 用于通用神经解码的EEG基础模型
tldr: KAST-BAR针对EEG基础模型在复杂时空拓扑建模不足及模态差距问题，提出知识锚定的语义动态拓扑脑自回归模型。设计双流分层注意力编码器，动态对齐多级脑拓扑的生理表示与专家级语义空间。实现通用神经解码和解释，提升EEG解码的通用性。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有EEG基础模型难以建模复杂时空拓扑和模态差距。
method: 设计双流分层注意力编码器，动态对齐生理表示与专家语义空间。
result: 实现通用神经解码和解释。
conclusion: 提升EEG解码的通用性和语义对齐。
---

## Abstract
While EEG foundation models have shown significant potential in universal neural decoding across tasks, their advancement remains constrained by the inadequacy modeling of *complex spatiotemporal topology*, as well as the inherent *modality gap* between low-level physiological signals and high-level textual semantics.
    To address these challenges, we propose a **K**nowledge-**A**nchored **S**emantically-Dynamic **T**opology **B**rain **A**uto**r**egressive Model (KAST-BAR), which dynamically aligns physiological representations derived from multi-level brain topology with an expert-level semantic space. 
    Specifically, we design a Dual-Stream Hierarchical Attention (DSHA) encoder that accurately captures the brain's intrinsic non-Euclidean topology by modeling local temporal dynamics with global spatial contexts. 
    On this basis, a Knowledge-Anchored Semantic Profiler (KASP) is proposed to synthesize physically-grounded and instance-level textual profiles, which subsequently drive a Semantic Text-Aware Refiner (STAR) to dynamically reconstruct EEG representations using Latent Expert Queries. 
    By conducting large-scale pre-training on 21 diverse datasets to build a foundation model, KAST-BAR effectively integrates expert-level medical knowledge into EEG signal representations, consistently achieving state-of-the-art performance across six downstream tasks. Our code is available at https://github.com/KAST-BAR/KAST-BAR

---

## 论文详细总结（自动生成）

### 1. 检索相关性
用于通用神经解码的EEG基础模型。

### 2. 核心内容
KAST-BAR针对EEG基础模型在复杂时空拓扑建模不足及模态差距问题，提出知识锚定的语义动态拓扑脑自回归模型。设计双流分层注意力编码器，动态对齐多级脑拓扑的生理表示与专家级语义空间。实现通用神经解码和解释，提升EEG解码的通用性。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=Ee4j4zMir5](https://openreview.net/forum?id=Ee4j4zMir5)
