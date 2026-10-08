---
title: Discretized Density-Guided Source-Free Domain Adaptation for Regression
title_zh: 离散密度引导的无源域自适应回归方法
authors: "Gezheng Xu, Qi CHEN, QIUHAO Zeng, Charles Ling, Boyu Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/4711a0d500c4098583974690eaf3d9d400616448.pdf"
tags: ["query:bci-da"]
score: 6.0
evidence: 面向回归的无源域自适应，利用离散密度信号，可用于连续脑解码标签
tldr: 针对无源域自适应用于连续回归任务时表示适应与伪标签精修困难的问题，提出基于离散密度引导的新算法。该方法利用实例相关的离散化密度监督信号，在不确定性感知范式下精修伪标签，同时促进表征紧凑。实验表明在多个回归基准上优于现有方法。该方法可作为脑解码中跨天连续标签适配的通用技术。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有无源域自适应多针对分类，回归任务因有序连续变量而面临独特挑战。
method: 提出离散密度引导的无源域自适应算法，利用离散密度监督信号精修伪标签。
result: 在多个回归基准上取得优于现有无源域自适应方法的性能。
conclusion: 该方法为连续标签场景下的分布偏移适应提供了有效工具，可迁移至脑解码等回归任务。
---

## Abstract
Source-Free Domain Adaptation (SFDA) enables model adaptation under distribution shifts without access to source data, providing a practical solution for privacy-sensitive applications and having shown substantial progress in classification. 
In contrast, regression involves ordered and continuous target variables, posing unique challenges for representation adaptation and pseudo-label refinement in the SFDA setting. 
To address this gap, we propose a novel algorithm for continuous label prediction in SFDA that leverages instance-dependent, discretized density–informed supervisory signals to refine pseudo-labels within an uncertainty-aware paradigm. 
By incorporating auxiliary discretized distribution learning, our method also promotes more compact and structured feature representations, mitigating the inherent difficulties of adapting regression models under distribution shift. 
We theoretically demonstrate that the resulting density structure is robust to potential perturbations, supporting reliable SFDA for regression. 
Extensive experiments across multiple benchmarks validate the effectiveness of the proposed approach.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向回归的无源域自适应，利用离散密度信号，可用于连续脑解码标签。

### 2. 核心内容
针对无源域自适应用于连续回归任务时表示适应与伪标签精修困难的问题，提出基于离散密度引导的新算法。该方法利用实例相关的离散化密度监督信号，在不确定性感知范式下精修伪标签，同时促进表征紧凑。实验表明在多个回归基准上优于现有方法。该方法可作为脑解码中跨天连续标签适配的通用技术。

### 3. 对应检索需求
domain adaptation techniques for brain signal decoding。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=UQLGAjV1cf](https://openreview.net/forum?id=UQLGAjV1cf)
