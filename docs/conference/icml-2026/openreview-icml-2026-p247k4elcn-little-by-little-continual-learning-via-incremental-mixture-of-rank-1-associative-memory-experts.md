---
title: "Little By Little: Continual Learning via Incremental Mixture of Rank-1 Associative Memory Experts"
title_zh: 积少成多：基于增量式秩一联想记忆专家的持续学习
authors: "Haodong Lu, Chongyang Zhao, Jason Xue, Lina Yao, Kristen Moore, Dong Gong"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/853cfbba8ece68c9715250dfc7d7e3ae6a79d777.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 用于持续学习抗遗忘的联想记忆专家
tldr: 大型预训练模型的持续学习需增量获取知识而不遗忘旧任务，现有基于LoRA的专家混合方法存在冗余、干扰与路由歧义等问题。本文从专家粒度出发，提出MoRAM，即秩一联想记忆专家混合，将权重矩阵视为线性联想记忆以提升专家特化程度。该方法缓解专家重复与路由退化，从而抑制持续学习中的遗忘。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有LoRA专家混合方法因专家粒度粗导致冗余、干扰、路由歧义，进而引发持续学习中的遗忘。
method: 提出MoRAM，将权重矩阵视为线性联想记忆，采用增量式秩一联想记忆专家实现细粒度专家特化。
result: 通过提升专家特化与路由质量，MoRAM缓解专家重复与干扰，改善持续学习性能。
conclusion: 该工作表明细粒度联想记忆专家是抑制持续学习遗忘的有效方向。
---

## Abstract
Continual learning (CL) with large pre-trained models aims to incrementally acquire knowledge without catastrophic forgetting. Existing LoRA-based Mixture-of-Experts (MoE) methods expand capacity by adding isolated new experts while freezing old ones, but still suffer from redundancy, interference, routing ambiguity, and consequent forgetting. We investigate the issues stemming from coarse-grained expert granularity. Coarse-grained experts (e.g., high-rank LoRA) encode low-specialty information, leading to expert duplication/interference and routing degradation/confusion as experts accumulate. In this work, we propose MoRAM (Mixture of Rank-1 Associative Memory). Grounded in the view that weight matrices act as linear associative memories, MoRAM achieves CL as incremental expansion of reusable atomic rank-1 experts as memory. Each rank-1 adapter acts as a fine-grained MoE expert or an associative memory unit. By viewing rank-1 experts as key-value memory pairs, we eliminate explicit MoE-LoRA routers with self-activation, where each memory atom evaluates its relevance via its intrinsic key. The inference process thus becomes a content-addressable retrieval and recall over the incrementally accumulated memory of learning snapshots. Extensive experiments on CLIP and LLMs show that MoRAM significantly outperforms state-of-the-art methods, achieving a better plasticity–stability trade-off, stronger generalization, and reduced forgetting. Project page: https://artificer-ai-lab.github.io/MoRAM.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
用于持续学习抗遗忘的联想记忆专家。

### 2. 核心内容
大型预训练模型的持续学习需增量获取知识而不遗忘旧任务，现有基于LoRA的专家混合方法存在冗余、干扰与路由歧义等问题。本文从专家粒度出发，提出MoRAM，即秩一联想记忆专家混合，将权重矩阵视为线性联想记忆以提升专家特化程度。该方法缓解专家重复与路由退化，从而抑制持续学习中的遗忘。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=P247k4ELcn](https://openreview.net/forum?id=P247k4ELcn)
