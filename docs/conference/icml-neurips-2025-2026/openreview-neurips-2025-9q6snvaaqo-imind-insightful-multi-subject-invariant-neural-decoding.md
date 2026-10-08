---
title: "$i$MIND: Insightful Multi-subject Invariant Neural Decoding"
title_zh: iMIND：可解释的多被试不变性神经解码
authors: "Zixiang Yin, Jiarui Li, Zhengming Ding"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=9q6sNvAaqO"
tags: ["query:bci-da"]
score: 8.0
evidence: 多被试不变性神经解码双重框架
tldr: 针对视觉神经解码模型忽视底层神经表征、缺乏可解释性且跨被试差异处理不足的问题，本文提出iMIND模型，采用生物特征解码和语义解码的双重框架，以数据驱动方式提供神经可解释性。该方法旨在发现跨被试不变的神经表征，从而提升解码的泛化能力。实验结果表明其能有效区分个体并揭示共享语义编码，为多被试脑信号解码提供了域适应新思路。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 现有视觉解码模型忽视底层神经表征，依赖预训练先验，难以解释个体体素编码及跨被试差异。
method: 提出iMIND模型，采用双重解码框架（生物特征解码与语义解码），实现数据驱动的神经可解释性。
result: 该模型能揭示跨被试不变的神经表征，提升视觉信号解码的可解释性和泛化性。
conclusion: iMIND为多被试神经解码提供了可解释的不变性方法，可视为脑信号解码中的域适应途径。
---

## Abstract
Decoding visual signals holds an appealing potential to unravel the complexities of cognition and perception. While recent reconstruction tasks leverage powerful generative models to produce high-fidelity images from neural recordings, they often pay limited attention to the underlying neural representations and rely heavily on pretrained priors. As a result, they provide little insight into how individual voxels encode and differentiate semantic content or how these representations vary across subjects. To mitigate this gap, we present an $i$nsightful **M**ulti-subject **I**nvariant **N**eural **D**ecoding ($i$MIND) model, which employs a novel dual-decoding framework--both biometric and semantic decoding--to offer neural interpretability in a data-driven manner and deepen our understanding of brain-based visual functionalities. Our $i$MIND model operates through three core steps: establishing a shared neural representation space across subjects using a ViT-based masked autoencoder, disentangling neural features into complementary subject-specific and object-specific components, and performing dual decoding to support both biometric and semantic classification tasks. Experimental results demonstrate that $i$MIND achieves state-of-the-art decoding performance with minimal scalability limitations. Furthermore, $i$MIND empirically generates voxel-object activation fingerprints that reveal object-specific neural patterns and enable investigation of subject-specific variations in attention to identical stimuli. These findings provide a foundation for more interpretable and generalizable subject-invariant neural decoding, advancing our understanding of the voxel semantic selectivity as well as the neural vision processing dynamics.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
多被试不变性神经解码双重框架。

### 2. 核心内容
针对视觉神经解码模型忽视底层神经表征、缺乏可解释性且跨被试差异处理不足的问题，本文提出iMIND模型，采用生物特征解码和语义解码的双重框架，以数据驱动方式提供神经可解释性。该方法旨在发现跨被试不变的神经表征，从而提升解码的泛化能力。实验结果表明其能有效区分个体并揭示共享语义编码，为多被试脑信号解码提供了域适应新思路。

### 3. 对应检索需求
domain adaptation techniques for brain signal decoding。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=9q6sNvAaqO](https://openreview.net/forum?id=9q6sNvAaqO)
