---
title: "MEG-XL: Data-Efficient Brain-to-Text via Long-Context Pre-Training"
title_zh: MEG-XL：通过长上下文预训练实现数据高效的脑到文本解码
authors: "Dulhan Jayalath, Oiwi Parker Jones"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/e4c0407dac6d92faca863a0400ab8ea4f5e55408.pdf"
tags: ["query:bci-da"]
score: 6.0
evidence: 在长时MEG上下文上预训练提升跨被试脑到文本BCI解码泛化
tldr: 针对临床脑到文本接口患者训练数据有限的问题，提出使用长达2.5分钟的全脑磁图上下文进行预训练的MEG-XL模型。该模型通过长上下文捕获扩展神经上下文，在词解码任务上微调后仅用1小时数据即可匹配50小时监督训练的性能，并超越脑基础模型。实验表明长上下文预训练能大幅提升脑到文本解码的数据效率和跨被试泛化能力。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 临床脑到文本接口因瘫痪患者难以提供大量训练数据，现有预训练上下文过短。
method: 提出MEG-XL，使用2.5分钟长上下文MEG数据进行预训练，捕获扩展神经上下文。
result: 在词解码任务上，仅需1小时微调数据即可匹配监督训练50小时的性能，并优于脑基础模型。
conclusion: 长上下文预训练显著提升脑到文本解码的数据效率和泛化性，为临床BCI提供实用方案。
---

## Abstract
Clinical brain-to-text interfaces are designed for paralysed patients who cannot provide extensive training recordings. Pre-training improves data-efficient generalisation by learning statistical priors across subjects, but these priors critically depend on context. While natural speech might unfold gradually over minutes, most methods pre-train with only a few seconds of context. Thus, we propose *MEG-XL*, a model pre-trained with 2.5 minutes of MEG context per sample, 5-300× longer than prior work, and equivalent to 191k tokens, capturing extended neural context. Fine-tuning on the task of word decoding from brain data, MEG-XL matches supervised performance with a fraction of the data (e.g. 1hr vs 50hrs) and outperforms brain foundation models. We find that models pre-trained with longer contexts learn representations that transfer better to word decoding. Our results indicate that long-context pre-training helps exploit extended neural context that other methods unnecessarily discard.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
在长时MEG上下文上预训练提升跨被试脑到文本BCI解码泛化。

### 2. 核心内容
针对临床脑到文本接口患者训练数据有限的问题，提出使用长达2.5分钟的全脑磁图上下文进行预训练的MEG-XL模型。该模型通过长上下文捕获扩展神经上下文，在词解码任务上微调后仅用1小时数据即可匹配50小时监督训练的性能，并超越脑基础模型。实验表明长上下文预训练能大幅提升脑到文本解码的数据效率和跨被试泛化能力。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=cefix4VmhS](https://openreview.net/forum?id=cefix4VmhS)
