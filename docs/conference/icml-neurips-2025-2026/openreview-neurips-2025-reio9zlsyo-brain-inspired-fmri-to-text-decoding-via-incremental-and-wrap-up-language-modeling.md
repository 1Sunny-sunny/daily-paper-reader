---
title: Brain-Inspired fMRI-to-Text Decoding via Incremental and Wrap-Up Language Modeling
title_zh: 基于增量式与总结式语言建模的脑启发式fMRI文本解码
authors: "Wentao Lu, Dong Nie, Pengcheng Xue, Zheng Cui, Piji Li, Daoqiang Zhang, Xuyun Wen"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=REIo9ZLSYo"
tags: ["query:bci-da"]
score: 5.0
evidence: 用于脑机接口的fMRI到文本解码
tldr: 针对现有fMRI到文本解码中长序列导致的内存过载和语义漂移问题，本文提出脑启发的顺序解码框架，将长fMRI时间序列切分为连续片段并采用增量式语言建模。该方法模仿人类分段归纳认知策略，实验表明能有效提升开放词汇解码性能。该工作为脑机接口中的神经语言解码提供了新的序列处理思路。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 现有fMRI到文本解码一次性处理整个序列，长输入导致内存过载和语义漂移。
method: 提出将长fMRI序列分段，并采用增量式与总结式语言建模的脑启发框架。
result: 实验显示该方法能缓解长序列解码性能下降，提升开放词汇文本解码准确率。
conclusion: 该框架为脑机接口中的高效神经语言解码提供了新方法。
---

## Abstract
Decoding natural language text from non-invasive brain signals, such as functional magnetic resonance imaging (fMRI), remains a central challenge in brain-computer interface research. While recent advances in large language models (LLMs) have enabled open-vocabulary fMRI-to-text decoding, existing frameworks typically process the entire fMRI sequence in a single step, leading to performance degradation when handling long input sequences due to memory overload and semantic drift. To address this limitation, we propose a brain-inspired sequential fMRI-to-text decoding framework that mimics the human cognitive strategy of segmented and inductive language processing. Specifically, we divide long fMRI time series into consecutive segments aligned with optimal language comprehension length. Each segment is decoded incrementally, followed by a wrap-up mechanism that summarizes the semantic content and incorporates it as prior knowledge into subsequent decoding steps. This sequence-wise approach alleviates memory burden and ensures semantic continuity across segments. In addition, we introduce a text-guided masking strategy integrated with a masked autoencoder (MAE) framework for fMRI representation learning. This method leverages attention distributions over key semantic tokens to selectively mask the corresponding fMRI time points, and employs MAE to guide the model toward focusing on neural activity at semantically salient moments, thereby enhancing the capability of fMRI embeddings to represent textual information. Experimental results on the two datasets demonstrate that our method significantly outperforms state-of-the-art approaches, with performance gains increasing as decoding length grows.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
用于脑机接口的fMRI到文本解码。

### 2. 核心内容
针对现有fMRI到文本解码中长序列导致的内存过载和语义漂移问题，本文提出脑启发的顺序解码框架，将长fMRI时间序列切分为连续片段并采用增量式语言建模。该方法模仿人类分段归纳认知策略，实验表明能有效提升开放词汇解码性能。该工作为脑机接口中的神经语言解码提供了新的序列处理思路。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=REIo9ZLSYo](https://openreview.net/forum?id=REIo9ZLSYo)
