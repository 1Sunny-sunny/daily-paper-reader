---
title: Multi-dataset Joint Pre-training of Emotional EEG Enables Generalizable Affective Computing
title_zh: 多数据集联合预训练情感脑电实现可泛化的情感计算
authors: "Qingzhu Zhang, Jiani Zhong, Li ZongSheng, Xinke Shen, Quanying Liu"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=xaxuzubN31"
tags: ["query:bci-da"]
score: 8.0
evidence: 跨数据集协方差对齐损失处理脑电分布偏移和个体差异用于情感识别
tldr: 针对现有通用脑电预训练模型在情感识别等复杂任务上因任务特征不匹配而泛化差的问题，提出面向任务的多数据集联合预训练框架。该方法引入跨数据集协方差对齐损失，对齐二阶统计特性，减轻数据集间分布偏移和个体差异。实验表明该框架在跨数据集情感识别上取得了更强的泛化能力，无需大量目标数据。该工作为脑电解码中的领域自适应提供了有效策略。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 现有通用脑电预训练模型与情感识别任务特征不匹配，跨数据集分布偏移和个体差异大。
method: 提出多数据集联合预训练框架，利用跨数据集协方差对齐损失对齐二阶统计特性。
result: 在跨数据集情感识别实验中，该方法显著提升了泛化性能，降低了对目标数据的依赖。
conclusion: 任务特定预训练结合协方差对齐是应对脑电分布偏移的有效途径，可推广至其他脑电解码任务。
---

## Abstract
Task-specific pre-training is essential when task representations diverge from generic pre-training features. Existing task-general pre-training EEG models struggle with complex tasks like emotion recognition due to mismatches between task-specific features and broad pre-training approaches. This work aims to develop a task-specific multi-dataset joint pre-training framework for cross-dataset emotion recognition, tackling problems of large inter-dataset distribution shifts, inconsistent emotion category definitions, and substantial inter-subject variability. We introduce a cross-dataset covariance alignment loss to align second-order statistical properties across datasets, enabling robust generalization without the need for extensive labels or per-subject calibration. To capture the long-term dependency and complex dynamics of EEG, we propose a hybrid encoder combining a Mamba-like linear attention channel encoder and a spatiotemporal dynamics model. Our method outperforms state-of-the-art large-scale EEG models by an average of 4.57% in AUROC for few-shot emotion recognition and 11.92% in accuracy for zero-shot generalization to a new dataset. Performance scales with the increase of datasets used in pre-training. Multi-dataset joint pre-training achieves a performance gain of 8.55\% over single-dataset training. This work provides a scalable framework for task-specific pre-training and highlights its benefit in generalizable affective computing. Our code is available at https://github.com/ncclab-sustech/mdJPT_nips2025.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
跨数据集协方差对齐损失处理脑电分布偏移和个体差异用于情感识别。

### 2. 核心内容
针对现有通用脑电预训练模型在情感识别等复杂任务上因任务特征不匹配而泛化差的问题，提出面向任务的多数据集联合预训练框架。该方法引入跨数据集协方差对齐损失，对齐二阶统计特性，减轻数据集间分布偏移和个体差异。实验表明该框架在跨数据集情感识别上取得了更强的泛化能力，无需大量目标数据。该工作为脑电解码中的领域自适应提供了有效策略。

### 3. 对应检索需求
domain adaptation techniques for brain signal decoding。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=xaxuzubN31](https://openreview.net/forum?id=xaxuzubN31)
