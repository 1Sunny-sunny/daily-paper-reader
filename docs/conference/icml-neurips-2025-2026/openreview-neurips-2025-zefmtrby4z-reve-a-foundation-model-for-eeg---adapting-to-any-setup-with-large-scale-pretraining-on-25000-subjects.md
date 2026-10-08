---
title: "REVE: A Foundation Model for EEG - Adapting to Any Setup with Large-Scale Pretraining on 25,000 Subjects"
title_zh: REVE：基于25000名被试大规模预训练的能适应任何设置的脑电基础模型
authors: "Yassine El Ouahidi, Jonathan Lys, Philipp Thölke, Nicolas Farrugia, Bastien Pasdeloup, Vincent Gripon, Karim Jerbi, Giulia Lioi"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=ZeFMtRBy4Z"
tags: ["query:bci-da"]
score: 6.0
evidence: 4D位置编码实现跨不同脑电协议、设备和电极配置的泛化
tldr: 针对公开脑电数据集在协议、设备、电极配置上的高度异质性导致现有基础模型泛化受限的问题，提出REVE模型。该模型引入新颖的4D位置编码方案，并在25000名被试的大规模数据上预训练，显式适配不同脑电设置。实验表明REVE在线性探测下显著优于受限于单一设置的前模型。该工作为跨设置脑电解码提供了通用基础模型。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 公开脑电数据集存在协议、设备、电极配置差异，现有基础模型难以跨设置泛化。
method: 提出REVE模型，设计4D位置编码并在大规模多源数据上预训练以适应任意设置。
result: 线性探测评估显示REVE在不同脑电设置上均取得优于现有模型的性能。
conclusion: 大规模预训练结合4D位置编码有效解决了脑电异质性问题，为通用脑电解码提供基础。
---

## Abstract
Foundation models have transformed AI by reducing reliance on task-specific data through large-scale pretraining. While successful in language and vision, their adoption in EEG has lagged due to the heterogeneity of public datasets, which are collected under varying protocols, devices, and electrode configurations. Existing EEG foundation models struggle to generalize across these variations, often restricting pretraining to a single setup, resulting in suboptimal performance, in particular under linear probing.
We present REVE (Representation for EEG with Versatile Embeddings), a pretrained model explicitly designed to generalize across diverse EEG signals. REVE introduces a novel 4D positional encoding scheme that enables it to process signals of arbitrary length and electrode arrangement. Using a masked autoencoding objective, we pretrain REVE on over 60,000 hours of EEG data from 92 datasets spanning 25,000 subjects, representing the largest EEG pretraining effort to date.
REVE achieves state-of-the-art results on 10 downstream EEG tasks, including motor imagery classification, seizure detection, sleep staging, cognitive load estimation, and emotion recognition. With little to no fine-tuning, it demonstrates strong generalization, and nuanced spatio-temporal modeling. We release code, pretrained weights, and tutorials to support standardized EEG research and accelerate progress in clinical neuroscience.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
4D位置编码实现跨不同脑电协议、设备和电极配置的泛化。

### 2. 核心内容
针对公开脑电数据集在协议、设备、电极配置上的高度异质性导致现有基础模型泛化受限的问题，提出REVE模型。该模型引入新颖的4D位置编码方案，并在25000名被试的大规模数据上预训练，显式适配不同脑电设置。实验表明REVE在线性探测下显著优于受限于单一设置的前模型。该工作为跨设置脑电解码提供了通用基础模型。

### 3. 对应检索需求
domain adaptation techniques for brain signal decoding。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=ZeFMtRBy4Z](https://openreview.net/forum?id=ZeFMtRBy4Z)
