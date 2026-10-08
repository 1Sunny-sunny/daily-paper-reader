---
title: "Neuro-KE: Scaling EEG Foundation Models via Label-Free Knowledge Integration"
title_zh: Neuro-KE：通过无标签知识集成扩展EEG基础模型
authors: "Hanrui Chen, Haotian Deng, Xiang Chen, Kexin Lou, Shinan Wang, Chen Wei, Quanying Liu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/77274615f21aaae77f95a71dbcedaa417155232c.pdf"
tags: ["query:bci-da"]
score: 5.0
evidence: 无标签整合信号处理知识用于EEG基础模型预训练
tldr: 该论文针对当前EEG基础模型忽视信号处理领域先验知识的问题，提出Neuro-KE框架，将时域、频域功率、频率结构和频率比四类特征以无标签方式集成到预训练中；实验表明该即插即用方法能增强EEG基础模型的泛化表示，对下游脑电解码任务有潜在提升。
source: ICML-2026-Rejected-Public
selection_source: conference_retrieval
motivation: 现有EEG基础模型主要依赖原始信号重建或稀缺标签，忽略了丰富的信号处理先验知识。
method: 提出无标签知识集成框架Neuro-KE，聚合时域、频域功率、频率结构和频率比特征用于预训练。
result: 实验显示Neuro-KE能即插即用地提升EEG基础模型的表示质量，有助于后续解码。
conclusion: 该框架为EEG基础模型融入领域知识提供了有效途径，可促进脑机接口解码任务。
---

## Abstract
Foundation Models for Electroencephalography (EEG) have shown promise in learning generalized representations from large-scale datasets.
However, current approaches primarily rely on raw signal reconstruction or scarce supervised labels, often neglecting the rich, domain-specific prior knowledge encapsulated in decades of signal processing research.
In this work, we introduce Neuro-KE (Neuro-Knowledge Engine), a plug-and-play, label-free framework designed to seamlessly integrate comprehensive signal characteristics into the pre-training of EEG foundation models.
Neuro-KE aggregates a 4-domain knowledge including Time Domain, Frequency Power, Frequency Structure, and Frequency Ratios features, distilling historical expertise into a unified knowledge base.
We demonstrate the versatility and effectiveness of Neuro-KE across three mainstream technical paradigms: Masked Modeling, Contrastive Learning, and EEG--Large Language Models.
Extensive experiments show that Neuro-KE significantly enhances model generalization and robustness, particularly in label-scarce downstream tasks, offering a rigorous pathway to embed domain-invariant signal dynamics into modern deep learning architectures.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
无标签整合信号处理知识用于EEG基础模型预训练。

### 2. 核心内容
该论文针对当前EEG基础模型忽视信号处理领域先验知识的问题，提出Neuro-KE框架，将时域、频域功率、频率结构和频率比四类特征以无标签方式集成到预训练中；实验表明该即插即用方法能增强EEG基础模型的泛化表示，对下游脑电解码任务有潜在提升。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：ICML-2026-Rejected-Public
- OpenReview：[https://openreview.net/forum?id=y7vaftM0NX](https://openreview.net/forum?id=y7vaftM0NX)
