---
title: A Generalist Intracortical Motor Decoder
title_zh: 通用皮层内运动解码器
authors: "Joel Ye, Fabio Rizzoglio, Xuan Ma, Adam Smoulder, Hongwei Mao, Gary H Blumenthal, William Hockeimer, Nicolas Guazzelli Kunigk, Dalton D. Moore, Patrick J. Marino, Raeed H. Chowdhury, J. Patrick Mayo, Aaron Batista, Steven Chase, Michael L Boninger, Charles M. Greenspon, Andrew B. Schwartz, Nicholas G. Hatsopoulos, Lee E. Miller, Kristofer Bouchard, Jennifer L Collinger, Leila Wehbe, Robert Gaunt"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=utXSSdD9mt"
tags: ["query:bci-da"]
score: 9.0
evidence: 通用皮层内运动解码器应对神经分布偏移
tldr: 针对皮层内运动解码模型通常局限于特定设置、难以泛化的问题，本文在2000小时的多受试者神经群体峰电活动与运动协变量数据上预训练自回归Transformer，构建通用运动解码器。该模型在8个下游解码任务上表现出色，并能泛化到多种神经分布偏移，包括可能的跨天变化。实验表明基础模型方法可提升脑机接口解码的鲁棒性和通用性，为长期稳定神经解码提供了新思路。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 皮层内运动解码通常受限于特定实验设置，难以泛化到多种任务和分布偏移。
method: 在2000小时的多猴/人神经群体峰电活动和运动数据上预训练自回归Transformer，构建通用解码器。
result: 该模型在8个下游解码任务上表现优异，并能泛化到多种神经分布偏移。
conclusion: 通用运动解码器展示了基础模型在脑机接口中的潜力，为跨天稳定解码提供了基础。
---

## Abstract
Mapping the relationship between neural activity and motor behavior is a central aim of sensorimotor neuroscience and neurotechnology. While most progress to this end has relied on restricting complexity, the advent of foundation models instead proposes integrating a breadth of data as an alternate avenue for broadly advancing downstream modeling. We quantify this premise for motor decoding from intracortical microelectrode data, pretraining an autoregressive Transformer on 2000 hours of neural population spiking activity paired with diverse motor covariates from over 30 monkeys and humans. The resulting model is broadly useful, benefiting decoding on 8 downstream decoding tasks and generalizing to a variety of neural distribution shifts. However, we also highlight that scaling autoregressive Transformers seems unlikely to resolve limitations stemming from sensor variability and output stereotypy in neural datasets.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
通用皮层内运动解码器应对神经分布偏移。

### 2. 核心内容
针对皮层内运动解码模型通常局限于特定设置、难以泛化的问题，本文在2000小时的多受试者神经群体峰电活动与运动协变量数据上预训练自回归Transformer，构建通用运动解码器。该模型在8个下游解码任务上表现出色，并能泛化到多种神经分布偏移，包括可能的跨天变化。实验表明基础模型方法可提升脑机接口解码的鲁棒性和通用性，为长期稳定神经解码提供了新思路。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=utXSSdD9mt](https://openreview.net/forum?id=utXSSdD9mt)
