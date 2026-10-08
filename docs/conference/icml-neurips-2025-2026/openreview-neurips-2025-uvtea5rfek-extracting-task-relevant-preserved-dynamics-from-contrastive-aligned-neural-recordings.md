---
title: Extracting task-relevant preserved dynamics from contrastive aligned neural recordings
title_zh: 从对比对齐神经记录中提取任务相关的保持动力学
authors: "Yiqi Jiang, Kaiwen Sheng, Yujia Gao, E. Kelly Buchanan, Yu Shikano, Seung Je Woo, Yixiu Zhao, Tony Hyun Kim, Fatih Dinc, Scott Linderman, Mark Schnitzer"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=uvTea5Rfek"
tags: ["query:bci-da"]
score: 9.0
evidence: 从跨天和跨受试者的神经记录中提取保持动力学
tldr: 针对高维神经群体活动在跨会话记录中因神经元群体变化而难以对齐的问题，本文提出CANDY端到端框架，通过对比学习对齐神经记录与行为数据，提取跨天和跨受试者保持的低维任务相关动力学。该方法连续建模行为，避免了离散化破坏连续性的问题。实验表明CANDY能有效提取保持动力学，为长期稳定神经解码提供表征基础。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 神经记录在跨会话中神经元群体变化，难以提取保持动力学。
method: 提出CANDY框架，利用对比学习对齐神经与行为数据。
result: 成功提取跨天保持的任务相关低维动力学。
conclusion: CANDY为长期神经解码提供了稳定表征方法。
---

## Abstract
Recent work indicates that low-dimensional dynamics of neural and behavioral data are often preserved across days and subjects. However, extracting these preserved dynamics remains challenging: high-dimensional neural population activity and the recorded neuron populations vary across recording sessions. While existing modeling tools can improve alignment between neural and behavioral data, they often operate on a per-subject basis or discretize behavior into categories, disrupting its natural continuity and failing to capture the underlying dynamics. We introduce $\underline{\text{C}}$ontrastive $\underline{\text{A}}$ligned $\underline{\text{N}}$eural $\underline{\text{D}}$$\underline{\text{Y}}$namics (CANDY), an end‑to‑end framework that aligns neural and behavioral data using rank-based contrastive learning, adapted for continuous behavioral variables, to project neural activity from different sessions onto a shared low-dimensional embedding space. CANDY fits a shared linear dynamical system to the aligned embeddings, enabling an interpretable model of the conserved temporal structure in the latent space. We validate CANDY on synthetic and real-world datasets spanning multiple species, behaviors, and recording modalities. Our results show that CANDY is able to learn aligned latent embeddings and preserved dynamics across neural recording sessions and subjects, and it achieves improved cross-session behavior decoding performance. We further show that the latent linear dynamical system generalizes to new sessions and subjects, achieving comparable or even superior behavior decoding performance to models trained from scratch. These advances enable robust cross‑session behavioral decoding and offer a path towards identifying shared neural dynamics that underlie behavior across individuals and recording conditions. The code and two-photon imaging data of striatal neural activity that we acquired here are available at https://github.com/schnitzer-lab/CANDY-public.git.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
从跨天和跨受试者的神经记录中提取保持动力学。

### 2. 核心内容
针对高维神经群体活动在跨会话记录中因神经元群体变化而难以对齐的问题，本文提出CANDY端到端框架，通过对比学习对齐神经记录与行为数据，提取跨天和跨受试者保持的低维任务相关动力学。该方法连续建模行为，避免了离散化破坏连续性的问题。实验表明CANDY能有效提取保持动力学，为长期稳定神经解码提供表征基础。

### 3. 对应检索需求
Explore neuroscience literature on neural signal variability and long term stable decoding。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=uvTea5Rfek](https://openreview.net/forum?id=uvTea5Rfek)
