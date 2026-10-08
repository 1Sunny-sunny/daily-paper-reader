---
title: Dynamical modeling of nonlinear latent factors in multiscale neural activity with real-time inference
title_zh: 多尺度神经活动非线性潜因子动力学建模与实时推理
authors: "Eray Erturk, Maryam M. Shanechi"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=jOHgjZaGqd"
tags: ["query:bci-da"]
score: 7.0
evidence: 从多尺度神经活动实时解码
tldr: 针对多模态神经信号（如尖峰和场电位）时间尺度不同、分布各异以及存在缺失的问题，本文提出一个学习框架，实现实时递归解码。该框架能同时处理多种神经模态，并在样本缺失情况下保持解码性能。实验表明其在神经科学应用中具有潜力，为需要实时解码的脑机接口提供了新方法。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 多模态神经数据具有不同时间尺度和概率分布，且可能存在缺失样本，现有非线性模型难以处理。
method: 开发一种学习框架，支持多模态神经活动的实时递归解码，并处理不同时间尺度和缺失样本。
result: 该框架可实现从尖峰和场电位等数据中实时解码目标变量，提高解码鲁棒性。
conclusion: 该方法为神经解码中的多模态融合和实时处理提供了新方案，适用于脑机接口应用。
---

## Abstract
Real-time decoding of target variables from multiple simultaneously recorded neural time-series modalities, such as discrete spiking activity and continuous field potentials, is important across various neuroscience applications. However, a major challenge for doing so is that different neural modalities can have different timescales (i.e., sampling rates) and different probabilistic distributions, or can even be missing at some time-steps. Existing nonlinear models of multimodal neural activity do not address different timescales or missing samples across modalities. Further, some of these models do not allow for real-time decoding. Here, we develop a learning framework that can enable real-time recursive decoding while nonlinearly aggregating information across multiple modalities with different timescales and distributions and with missing samples. This framework consists of 1) a multiscale encoder that nonlinearly aggregates information after learning within-modality dynamics to handle different timescales and missing samples in real time, 2) a multiscale dynamical backbone that extracts multimodal temporal dynamics and enables real-time recursive decoding, and 3) modality-specific decoders to account for different probabilistic distributions across modalities. In both simulations and three distinct multiscale brain datasets, we show that our model can aggregate information across modalities with different timescales and distributions and missing samples to improve real-time target decoding. Further, our method outperforms various linear and nonlinear multimodal benchmarks in doing so.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
从多尺度神经活动实时解码。

### 2. 核心内容
针对多模态神经信号（如尖峰和场电位）时间尺度不同、分布各异以及存在缺失的问题，本文提出一个学习框架，实现实时递归解码。该框架能同时处理多种神经模态，并在样本缺失情况下保持解码性能。实验表明其在神经科学应用中具有潜力，为需要实时解码的脑机接口提供了新方法。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=jOHgjZaGqd](https://openreview.net/forum?id=jOHgjZaGqd)
