---
title: "Mind-Omni: A Unified Multi-Task Framework for Brain-Vision-Language Modeling via Discrete Diffusion"
title_zh: Mind-Omni：通过离散扩散实现大脑-视觉-语言统一多任务建模框架
authors: "Yizhuo Lu, Changde Du, Qingyu Shi, Hang Chen, Jie Peng, Liuyun Jiang, Shuangchen Zhao, Huiguang He"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/426378cbae09e997b188c2f3750124b7608a9421.pdf"
tags: ["query:bci-da"]
score: 5.0
evidence: 使用离散扩散和脑标记器实现BCI的统一多任务大脑编解码框架
tldr: 针对脑机接口领域单任务模型割裂、缺乏协同的问题，提出Mind-Omni统一框架。该框架通过离散扩散范式和新型脑标记器将异构连续脑信号转换为标准化离散令牌，统一七种编码与解码任务。实验表明多任务统一建模可以提升任务间的协同和整体性能。该工作为通用脑机接口解码提供了新的架构基础。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有BCI模型多为单任务专用，缺乏通用性，忽略任务间协同。
method: 提出Mind-Omni，利用离散扩散和脑标记器实现多模态令牌交互，统一七种编解码任务。
result: 多个编解码任务上展示了统一框架的可行性和性能提升。
conclusion: 统一多任务框架有望推动BCI模型从专用走向通用，增强多模态协同。
---

## Abstract
Modeling the interplay between external stimuli and internal neural representations is a pivotal research area for Brain-Computer Interfaces (BCIs). A major limitation of prior work is the prevailing paradigm of specialized, single-task models, which curtails versatility and neglects inter-task synergies. To address this, we propose Mind-Omni, the first versatile framework that unifies seven distinct encoding and decoding tasks through a discrete diffusion paradigm. At its core is a novel Brain Tokenizer that transforms heterogeneous, continuous brain signals into standardized, discrete tokens. This enables direct, token-level interactions for mutual understanding and generation between any two or more modalities within a shared semantic space. To unlock advanced reasoning capabilities, we further curate a specialized Brain Question Answering (BQA) instruction-tuning dataset. Our model not only establishes a new state-of-the-art among multi-task unified frameworks but also provides strong evidence for multi-task synergy. By demonstrating performance competitive with, and at times superior to, larger specialized models, our work offers a powerful new paradigm for neural modeling and paves the way for foundation models of neural activity.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
使用离散扩散和脑标记器实现BCI的统一多任务大脑编解码框架。

### 2. 核心内容
针对脑机接口领域单任务模型割裂、缺乏协同的问题，提出Mind-Omni统一框架。该框架通过离散扩散范式和新型脑标记器将异构连续脑信号转换为标准化离散令牌，统一七种编码与解码任务。实验表明多任务统一建模可以提升任务间的协同和整体性能。该工作为通用脑机接口解码提供了新的架构基础。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=3gCdh3u2GK](https://openreview.net/forum?id=3gCdh3u2GK)
