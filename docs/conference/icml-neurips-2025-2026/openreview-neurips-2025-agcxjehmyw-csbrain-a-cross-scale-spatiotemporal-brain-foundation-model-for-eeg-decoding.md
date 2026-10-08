---
title: "CSBrain: A Cross-scale Spatiotemporal Brain Foundation Model for EEG Decoding"
title_zh: CSBrain：面向EEG解码的跨尺度时空脑基础模型
authors: "Yuchen Zhou, Jiamin Wu, Zichen Ren, Zhouheng Yao, Weiheng Lu, Kunyu Peng, Qihao Zheng, Chunfeng Song, Wanli Ouyang, Chao Gou"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=agcXjEHmyW"
tags: ["query:bci-da"]
score: 6.0
evidence: 跨尺度时空脑基础模型用于EEG解码并面向脑机接口
tldr: 该论文指出当前EEG基础模型忽略神经活动的跨尺度时空结构，提出CSBrain模型，显式建模不同EEG任务模式的时空尺度；通过大规模预训练提升脑电解码性能，可应用于脑机接口、认知与情绪识别等，为通用脑解码提供了新基础模型。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 现有EEG基础模型沿用NLP/视觉的密集建模范式，忽略EEG固有的跨尺度时空特性。
method: 设计跨尺度时空脑基础模型CSBrain，显式建模不同时空尺度的EEG活动模式。
result: 在多个EEG解码任务上取得改进，展示了对脑机接口等应用的潜力。
conclusion: CSBrain为EEG解码提供了更符合神经活动本质的基础模型，推动通用脑信号处理。
---

## Abstract
Understanding and decoding human brain activity from electroencephalography (EEG) signals is a fundamental problem in neuroscience and artificial intelligence, with applications ranging from cognition and emotion recognition to clinical diagnosis and brain–computer interfaces. While recent EEG foundation models have made progress in generalized brain decoding by leveraging unified architectures and large-scale pretraining, they inherit a scale-agnostic dense modeling paradigm from NLP and vision. This design overlooks an intrinsic property of neural activity—cross-scale spatiotemporal structure. Different EEG task patterns span a broad range of temporal and spatial scales, from brief neural activations to slow-varying rhythms, and from localized cortical activations to large-scale distributed interactions. Ignoring this diversity may lead to suboptimal representations and weakened generalization ability. To address these limitations, we propose CSBrain, a Cross-scale Spatiotemporal Brain foundation model for generalized EEG decoding. CSBrain introduces two key components: (i) Cross-scale Spatiotemporal Tokenization (CST), which aggregates multi-scale features within localized temporal windows and anatomical brain regions into compact scale-aware token representations; and (ii) Structured Sparse Attention (SSA), which models cross-window and cross-region dependencies for diverse decoding tasks, further enriching scale diversities while eliminating the spurious dependencies. CST and SSA are alternately stacked to progressively integrate cross-scale spatiotemporal dependencies. Extensive experiments across 11 representative EEG tasks and 16 datasets demonstrate that CSBrain consistently outperforms both task-specific models and strong foundation baselines. These results establish cross-scale modeling as a key inductive bias for generalized EEG decoding and highlight CSBrain as a robust backbone for future brain–AI research.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
跨尺度时空脑基础模型用于EEG解码并面向脑机接口。

### 2. 核心内容
该论文指出当前EEG基础模型忽略神经活动的跨尺度时空结构，提出CSBrain模型，显式建模不同EEG任务模式的时空尺度；通过大规模预训练提升脑电解码性能，可应用于脑机接口、认知与情绪识别等，为通用脑解码提供了新基础模型。

### 3. 对应检索需求
neural decoding models for brain-computer interfaces。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=agcXjEHmyW](https://openreview.net/forum?id=agcXjEHmyW)
