---
title: "NeurIPT: Foundation Model for Neural Interfaces"
title_zh: NeurIPT：神经接口基础模型
authors: "Zitao Fang, CHENXUAN LI, Zhou Hongting, Shuyang Yu, Guodong DU, Ashwaq Qasem, Yang Lu, Jing Li, Junsong Zhang, Sim Kuan Goh"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=D4hcJPkJ3y"
tags: ["query:bci-da"]
score: 9.0
evidence: 面向多样EEG神经接口的基础模型，处理变异性
tldr: 针对EEG脑机接口中显著的受试者、任务和条件变异性及电极配置差异，本文提出NeurIPT基础模型，利用预训练Transformer同时捕获EEG信号中的同质和异质时空特性。该模型旨在为多样化的神经接口提供通用解码能力，减少对任务特定数据的依赖。实验显示其在多种EEG设置下具有潜力，为脑机接口神经解码的规模化与泛化开辟了新路径。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: EEG数据在受试者、任务和条件间变异性大，且电极配置多样，制约了基础模型在脑机接口中的应用。
method: 提出NeurIPT，一种基于预训练Transformer的EEG神经接口基础模型，捕捉脑电信号中的均匀与异质时空特征。
result: 该模型能适应多种EEG设置，有望提升跨受试者、跨任务的神经解码泛化能力。
conclusion: NeurIPT为脑机接口神经解码提供了可扩展的预训练基础模型，能应对实际EEG变异性挑战。
---

## Abstract
Electroencephalography (EEG) has wide-ranging applications, from clinical diagnosis to brain-computer interfaces (BCIs). With the increasing volume and variety of EEG data, there has been growing interest in establishing foundation models (FMs) to scale up and generalize neural decoding. Despite showing early potential, applying FMs to EEG remains challenging due to substantial inter-subject, inter-task, and inter-condition variability, as well as diverse electrode configurations across recording setups. To tackle these open challenges, we propose **NeurIPT**, a foundation model tailored for diverse EEG-based **Neur**al **I**nterfaces with a **P**re-trained **T**ransformer by capturing both homogeneous and heterogeneous spatio-temporal characteristics inherent in EEG signals. Temporally, we introduce Amplitude-Aware Masked Pretraining (AAMP), masking based on signal amplitude rather than random intervals, to learn robust representations across varying signal intensities beyond local interpolation. Moreover, this temporal representation is enhanced by a progressive Mixture-of-Experts (MoE) architecture, where specialized expert subnetworks are progressively introduced at deeper layers, adapting effectively to the diverse temporal characteristics of EEG signals. Spatially, NeurIPT leverages the 3D physical coordinates of electrodes, enabling effective transfer across varying EEG settings, and develops Intra-Inter Lobe Pooling (IILP) during fine-tuning to efficiently exploit regional brain features. Empirical evaluations across nine downstream BCI datasets, via fine-tuning and training from scratch, demonstrated NeurIPT consistently achieved state-of-the-art performance, highlighting its broad applicability and robust generalization. Our work pushes forward the state of FMs in EEG and offers insights into scalable and generalizable neural information processing systems.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向多样EEG神经接口的基础模型，处理变异性。

### 2. 核心内容
针对EEG脑机接口中显著的受试者、任务和条件变异性及电极配置差异，本文提出NeurIPT基础模型，利用预训练Transformer同时捕获EEG信号中的同质和异质时空特性。该模型旨在为多样化的神经接口提供通用解码能力，减少对任务特定数据的依赖。实验显示其在多种EEG设置下具有潜力，为脑机接口神经解码的规模化与泛化开辟了新路径。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=D4hcJPkJ3y](https://openreview.net/forum?id=D4hcJPkJ3y)
