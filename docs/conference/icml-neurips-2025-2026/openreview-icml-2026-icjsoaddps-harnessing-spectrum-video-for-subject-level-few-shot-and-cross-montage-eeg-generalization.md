---
title: Harnessing Spectrum Video for Subject-Level Few-Shot and Cross-Montage EEG Generalization
title_zh: 利用频谱视频实现受试者级少样本和跨导联EEG泛化
authors: "Wei Wang, Fang He, Yifan Li, Wanying Qu, Yawei Li, Quanying Liu, Yanwei Fu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/7a479015e0343277f4642527062f8c58588e34f4.pdf"
tags: ["query:bci-da"]
score: 8.0
evidence: 频谱视频渲染实现少样本跨导联EEG泛化
tldr: 针对EEG模型受限于电极异质性和通道固定结构、难以跨受试者和导联泛化的问题，本文提出脑信号渲染方法，将原始信号转换为频谱视频张量，并利用VideoMAE进行自监督预训练以保留神经拓扑。通过受试者级少样本学习和跨导联微调，该方法能学习布局无关的鲁棒表示。实验表明其在跨受试者和跨导联任务上取得显著提升，为脑机接口的跨域适应提供了新路径。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有EEG模型受限于电极异质性和僵化的“通道优先”架构，难以跨受试者和导联泛化。
method: 提出脑信号渲染(BSR)方法，将EEG转换为频谱视频张量，利用VideoMAE自监督预训练，并进行少样本学习和跨导联微调。
result: 实验表明BSR能学习布局无关的时空表示，在跨受试者和跨导联设置下显著提升泛化性能。
conclusion: 该研究为EEG解码中的域适应和泛化提供了新方法，可扩展到跨会话脑机接口。
---

## Abstract
Existing EEG models are limited by electrode heterogeneity and rigid "channel-first" architectures that treat sensors as independent features. We propose Brain Signal Rendering (BSR), which reinterprets EEG as a physical projection of neural activity and transforms raw signals into structured spatiotemporal tensors (termed Spectrum Videos), enabling the transfer of rich priors from video foundation models. By utilizing VideoMAE for self-supervised pre-training, BSR learns robust, layout-agnostic spatiotemporal representations that preserve neural topology. We further employ subject-level few-shot learning and introduce cross-montage fine-tuning to rigorously evaluate generalization across subjects and electrode configurations. Experiments show that VideoMAE model integrated with the BSR framework significantly outperforms state-of-the-art spectrum based methods, providing a scalable and data-efficient foundation for generalizable EEG modeling. Our code is available at [https://github.com/yanweifu-sii/BSR-VideoMAE](https://github.com/yanweifu-sii/BSR-VideoMAE).

---

## 论文详细总结（自动生成）

### 1. 检索相关性
频谱视频渲染实现少样本跨导联EEG泛化。

### 2. 核心内容
针对EEG模型受限于电极异质性和通道固定结构、难以跨受试者和导联泛化的问题，本文提出脑信号渲染方法，将原始信号转换为频谱视频张量，并利用VideoMAE进行自监督预训练以保留神经拓扑。通过受试者级少样本学习和跨导联微调，该方法能学习布局无关的鲁棒表示。实验表明其在跨受试者和跨导联任务上取得显著提升，为脑机接口的跨域适应提供了新路径。

### 3. 对应检索需求
domain adaptation techniques for brain signal decoding。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=iCjSoADDPs](https://openreview.net/forum?id=iCjSoADDPs)
