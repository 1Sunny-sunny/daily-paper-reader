---
title: Time-Masked Transformers with Lightweight Test-Time Adaptation for Neural Speech Decoding
title_zh: 用于神经语音解码的具有轻量级测试时适应的时间掩码Transformer
authors: "Ebrahim Feghhi, Shreyas Kaasyap, Nima Ryan Hadidi, Jonathan Kao"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=0U7D9AFiZ0"
tags: ["query:bci-da"]
score: 8.0
evidence: 神经语音解码的测试时适应
tldr: "该工作针对现有语音神经假体解码精度高但计算成本大、缺乏实时性的问题，提出在训练时引入大量时间掩码（平均超过50%），并采用轻量级测试时适应。实验结果表明该方法在保持高精度的同时实现高效和实时神经语音解码，为实时语音神经假体提供新方案。"
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 现有语音神经假体解码精度高但计算成本大，缺乏实时性。
method: 训练时大量时间掩码，结合轻量级测试时适应。
result: 实现了准确、高效、实时的神经语音解码。
conclusion: 为实时神经语音解码提供新方法。
---

## Abstract
Speech neuroprostheses aim to restore communication for people with severe paralysis by decoding speech directly from neural activity. To accelerate algorithmic progress, a recent benchmark released intracranial recordings from a paralyzed participant attempting to speak, along with a baseline decoding algorithm. Prior work on the benchmark showed impressive accuracy gains. However, these gains increased computational costs and were not demonstrated in a real-time decoding setting. Here, we make three contributions that pave the way towards accurate, efficient, and real-time neural speech decoding. First, we incorporate large amounts of time-masking during training. On average, over $50\%$ of each trial is masked. Second, we replace the gated recurrent unit (GRU) architecture used in the baseline algorithm with a compact Transformer. The Transformer architecture uses $83\%$ fewer parameters, cuts peak GPU memory usage by $52\%$, and is significantly faster to calibrate relative to the GRU. Third, we design a lightweight variant of an existing test-time adaptation method developed for decoding handwriting from neural activity. Our variant adapts the model using multiple time-masked augmentations of a single trial and requires only one gradient step per trial. Together, these contributions reduce word error rate by over $20\%$ and effectively mitigate performance degradations across held-out days in a real-time decoding setting while substantially lowering computational costs.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
神经语音解码的测试时适应。

### 2. 核心内容
该工作针对现有语音神经假体解码精度高但计算成本大、缺乏实时性的问题，提出在训练时引入大量时间掩码（平均超过50%），并采用轻量级测试时适应。实验结果表明该方法在保持高精度的同时实现高效和实时神经语音解码，为实时语音神经假体提供新方案。

### 3. 对应检索需求
domain adaptation techniques for brain signal decoding。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=0U7D9AFiZ0](https://openreview.net/forum?id=0U7D9AFiZ0)
