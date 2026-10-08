---
title: Self supervised learning for in vivo localization of microelectrode arrays using raw local field potential
title_zh: 基于原始局部场电位的微电极阵列在体定位的自监督学习
authors: "Tianxiao He, Malhar Patel, Chenyi Li, Anna Maslarova, Mihály Vöröslakos, Nalini Ramanathan, Wei-Lun Hung, Gyorgy Buzsaki, Erdem Varol"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=96liIPUPXG"
tags: ["query:bci-da"]
score: 7.0
evidence: 自监督Lfp2vec从局部场电位推断脑区以支持多天记录的稳定定位
tldr: 针对多天神经记录中脑区定位依赖外部解剖信息、无法实时反馈的问题，提出自监督学习框架Lfp2vec。该框架在原始局部场电位上继续训练音频预训练Transformer，可直接从神经信号推断解剖区域。实验表明该方法能够实现精确的在体定位，无需组织学或图谱。该工作为多天记录的稳定电极定位提供了实时方案，有利于长期稳定解码。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 多天记录中电极定位依赖图谱或事后组织学，精度和实时性不足。
method: 开发Lfp2vec，在原始局部场电位上对音频预训练Transformer进行自监督继续训练。
result: 实现了无需外部解剖信息的实时脑区推断，提高了多天记录定位一致性。
conclusion: 自监督学习从神经信号直接定位脑区，为长期稳定神经记录和解码提供基础支持。
---

## Abstract
Recent advances in large-scale neural recordings have enabled accurate decoding of behavior and cognitive states, yet decoding anatomical regions remains underexplored, despite being crucial for consistent targeting in multiday recordings and effective deep brain stimulation. Current approaches typically rely on external anatomical information, from atlas-based planning to post hoc histology, which are limited in precision, longitudinal applicability, and real-time feedback. In this work, we develop a self-supervised learning framework, Lfp2vec, to infer anatomical regions directly from the neural signal in vivo. We adapt an audio-pretrained transformer model by continuing self-supervised training on a large corpus of unlabeled local-field-potential (LFP) data, then fine-tuning for anatomical region decoding. Ablations show that combining out-of-domain initialization with in-domain self-supervision outperforms training from scratch. We demonstrate that our method  achieves strong zero-shot generalization across different labs and probe geometries, and outperforming state-of-the-art self-supervised models on electrophysiology data. The learned embeddings form anatomically coherent clusters and transfer effectively to downstream tasks like disease classification with minimal fine-tuning. Altogether, our approach enables zero-shot prediction of brain regions in novel subjects, demonstrates that LFP signals encode rich anatomical information, and establishes self-supervised learning on raw LFP as a foundation to learn representations that can be tuned for diverse neural decoding tasks. Code to reproduce our results is found in the github repository at https://github.com/tianxiao18/lfp2vec.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
自监督Lfp2vec从局部场电位推断脑区以支持多天记录的稳定定位。

### 2. 核心内容
针对多天神经记录中脑区定位依赖外部解剖信息、无法实时反馈的问题，提出自监督学习框架Lfp2vec。该框架在原始局部场电位上继续训练音频预训练Transformer，可直接从神经信号推断解剖区域。实验表明该方法能够实现精确的在体定位，无需组织学或图谱。该工作为多天记录的稳定电极定位提供了实时方案，有利于长期稳定解码。

### 3. 对应检索需求
Explore neuroscience literature on neural signal variability and long term stable decoding。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=96liIPUPXG](https://openreview.net/forum?id=96liIPUPXG)
