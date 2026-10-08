---
title: "NeurIPS: Neuro-anatomical Inductive Priors for Sphere-based Brain Decoding"
title_zh: NeurIPS：基于球面脑解码的神经解剖学归纳先验
authors: "Sijin Yu, Zijiao Chen, Zhenyu Yang, Zihao Tan, Jiakun Xu, Zhongliang Liu, shengxian chen, WENXUAN WU, Xiangmin Xu, Xin Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/55dff9bcd050fbfbeccaf4d27c6325073bbfe34f.pdf"
tags: ["query:bci-da"]
score: 4.0
evidence: 基于解剖学归纳先验的fMRI脑解码
tldr: 针对现有fMRI解码器在性能和保真度之间的权衡问题，本文提出NeurIPS框架，将解剖变异从干扰转为预测先验。通过选择性ROI球形分词器和结构引导的专家混合，显式建模个体皮层解剖结构。在自然场景数据集上达到表面解码器的新state-of-the-art。该工作展示了神经解剖学先验对脑解码的增益。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有fMRI解码器面临效率与几何保真度的权衡，表面分词低效且未利用解剖预测信号。
method: 提出NeurIPS，结合选择性ROI球形分词器和结构引导的专家混合，建模个体皮层解剖。
result: 在自然场景数据集上取得表面解码器的新state-of-the-art性能。
conclusion: 将解剖变异转化为归纳先验可显著提升脑解码性能。
---

## Abstract
Current fMRI decoders face a performance-fidelity trade-off where efficient ID encoders outperform geometrically faithful surface-based models. We argue this is partly driven by inefficient surface tokenization and the failure to use anatomy as a predictive signal. We present **NeurIPS**, a framework that improves surface-based decoding by reframing anatomical variation from a nuisance to a powerful inductive prior. NeurIPS unites two innovations: a **Selective ROI Spherical Tokenizer (SRST)** for efficient geometric encoding, and a **Structure-Guided Mixture of Experts (SG-MoE)** that explicitly models individual anatomy using cortical features. On the Natural Scenes Dataset, NeurIPS establishes a new state-of-the-art for surface decoders and achieves performance comparable to strong 1D baselines. This is achieved with unprecedented efficiency, as the model converges dramatically faster (**10 vs. 600 epochs**). This efficiency enables rapid adaptation to new subjects using only **20\%** of data and ensures robust scalability as the training cohort is expanded. Ablations provide causal evidence that these gains are driven by the model's use of cortical features, not by memorizing subject IDs. By leveraging anatomical priors, NeurIPS provides a principled and scalable path toward robust, generalizable brain decoding.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
基于解剖学归纳先验的fMRI脑解码。

### 2. 核心内容
针对现有fMRI解码器在性能和保真度之间的权衡问题，本文提出NeurIPS框架，将解剖变异从干扰转为预测先验。通过选择性ROI球形分词器和结构引导的专家混合，显式建模个体皮层解剖结构。在自然场景数据集上达到表面解码器的新state-of-the-art。该工作展示了神经解剖学先验对脑解码的增益。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=gXTtBRI1yj](https://openreview.net/forum?id=gXTtBRI1yj)
