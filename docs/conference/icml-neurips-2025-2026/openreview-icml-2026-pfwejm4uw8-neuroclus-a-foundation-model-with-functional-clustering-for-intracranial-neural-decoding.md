---
title: "NeuroCLUS: A Foundation Model with Functional Clustering for Intracranial Neural Decoding"
title_zh: NeuroCLUS：具有功能聚类的颅内神经解码基础模型
authors: "Hui Zheng, Haiteng Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/9d418bbd5551f57401efb1ba8f497687a0e33525.pdf"
tags: ["query:bci-da"]
score: 6.0
evidence: 颅内神经解码的基础模型
tldr: NeuroCLUS针对现有颅内神经解码基础模型标记方案次优、未捕捉大脑功能模块化的问题，提出两阶段预训练框架：先通过功能上下文预测学习通道间功能上下文图，再引导软聚类表示。该方法学习到数据驱动的功能簇，提升了神经活动表示的泛化能力，为颅内神经解码提供了更符合大脑功能组织的基础模型。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有颅内神经解码基础模型采用次优标记方案，未能捕捉大脑功能模块化。
method: 提出两阶段预训练框架，先学习通道间功能上下文图，再引导软聚类表示。
result: 通过功能聚类建模提升了神经活动表示的泛化能力。
conclusion: 为颅内神经解码提供了更符合大脑功能组织的基础模型。
---

## Abstract
Foundation models for intracranial neural recordings aim to learn generalizable representations from large-scale unlabeled data. However, existing approaches rely on suboptimal tokenization schemes -- treating individual electrode channels as independent tokens or aggregating them into a single brain-wide representation -- which fail to capture the brain’s inherent functional modularity. We introduce NeuroCLUS, a foundation model that learns to represent neural activity through data-driven functional clusters. NeuroCLUS is built on a novel two-stage pre-training framework. First, a spatial-temporal model learns a functional context graph between channels via a functional context prediction task. Second, this graph guides a soft clustering of channels into a set of learnable prototype tokens, enabling the transformer backbone to process coherent functional units rather than raw channels. Evaluated across a diverse range of decoding paradigms -- including speech perception, speech production, and seizure detection -- NeuroCLUS consistently achieves state-of-the-art performance. The discovered functional clusters align with established neurophysiology and offer enhanced interpretability. Our work demonstrates that explicitly modeling functional neural groupings significantly improves the efficiency, generalization, and interpretability of foundation models for intracranial decoding.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
颅内神经解码的基础模型。

### 2. 核心内容
NeuroCLUS针对现有颅内神经解码基础模型标记方案次优、未捕捉大脑功能模块化的问题，提出两阶段预训练框架：先通过功能上下文预测学习通道间功能上下文图，再引导软聚类表示。该方法学习到数据驱动的功能簇，提升了神经活动表示的泛化能力，为颅内神经解码提供了更符合大脑功能组织的基础模型。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=pFweJM4Uw8](https://openreview.net/forum?id=pFweJM4Uw8)
