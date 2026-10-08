---
title: "SPICED: A Synaptic Homeostasis-Inspired Framework for Unsupervised Continual EEG Decoding"
title_zh: SPICED：受突触稳态启发的无监督连续EEG解码框架
authors: "Yangxuan Zhou, Sha Zhao, Jiquan Wang, Haiteng Jiang, Shijian Li, Tao Li, Gang Pan"
date: 2025
publication_date: 2025
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf?id=qcdoHkkHcb"
tags: ["query:bci-da"]
score: 8.0
evidence: 无监督连续EEG解码处理个体间变异性
tldr: SPICED针对实际场景中新个体持续出现、个体间变异性大的无监督持续EEG解码问题，提出受突触稳态启发的神经形态框架。通过关键记忆重激活等三种生物启发机制实现动态扩展。实验证明该框架能有效适应新个体，为EEG解码的持续适应提供新思路。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
motivation: 现有EEG解码难以应对新个体持续出现的变异性。
method: 基于突触稳态机制，通过关键记忆重激活等生物机制实现动态扩展。
result: 实现无监督连续EEG解码，适应个体间差异。
conclusion: 为EEG解码提供持续适应新个体的方案。
---

## Abstract
Human brain achieves dynamic stability-plasticity balance through synaptic homeostasis, a self-regulatory mechanism that stabilizes critical memory traces while preserving optimal learning capacities. Inspired by this biological principle, we propose SPICED: a neuromorphic framework that integrates the synaptic homeostasis mechanism for unsupervised continual EEG decoding, particularly addressing practical scenarios where new individuals with inter-individual variability emerge continually. SPICED comprises a novel synaptic network that enables dynamic expansion during continual adaptation through three bio-inspired neural mechanisms: (1) critical memory reactivation, which mimics brain functional specificity, selectively activates task-relevant memories to facilitate adaptation; (2) synaptic consolidation, which strengthens these reactivated critical memory traces and enhances their replay prioritizations for further adaptations and (3) synaptic renormalization, which are periodically triggered to weaken global memory traces to preserve learning capacities. The interplay within synaptic homeostasis dynamically strengthens  task-discriminative memory traces and weakens detrimental memories. By integrating these mechanisms with continual learning system, SPICED preferentially replays task-discriminative memory traces that exhibit strong associations with newly emerging individuals, thereby achieving robust adaptations. Meanwhile, SPICED effectively mitigates catastrophic forgetting by suppressing the replay prioritization of detrimental memories during long-term continual learning. Validated on three EEG datasets, SPICED show its effectiveness. More importantly, SPICED bridges biological neural mechanisms and artificial intelligence through synaptic homeostasis, providing insights into the broader applicability of bio-inspired principles.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
无监督连续EEG解码处理个体间变异性。

### 2. 核心内容
SPICED针对实际场景中新个体持续出现、个体间变异性大的无监督持续EEG解码问题，提出受突触稳态启发的神经形态框架。通过关键记忆重激活等三种生物启发机制实现动态扩展。实验证明该框架能有效适应新个体，为EEG解码的持续适应提供新思路。

### 3. 对应检索需求
handling session-to-session variability in neural recordings。

### 4. 来源与原文
- Source：NeurIPS-2025-Accepted
- OpenReview：[https://openreview.net/forum?id=qcdoHkkHcb](https://openreview.net/forum?id=qcdoHkkHcb)
