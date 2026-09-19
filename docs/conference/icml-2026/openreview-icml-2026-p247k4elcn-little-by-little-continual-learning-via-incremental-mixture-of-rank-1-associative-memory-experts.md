---
title: "Little By Little: Continual Learning via Incremental Mixture of Rank-1 Associative Memory Experts"
title_zh: 循序渐进：通过增量秩1联想记忆专家混合实现持续学习
authors: "Haodong Lu, Chongyang Zhao, Jason Xue, Lina Yao, Kristen Moore, Dong Gong"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/853cfbba8ece68c9715250dfc7d7e3ae6a79d777.pdf"
tags: ["query:agent-memory"]
score: 7.0
evidence: 通过秩1联想记忆专家缓解灾难性遗忘的持续学习
tldr: 大型预训练模型的持续学习需增量获取知识而不发生灾难性遗忘，但现有LoRA混合专家方法因专家粒度粗导致冗余、干扰与路由混乱。本文提出MoRAM（秩1联想记忆专家混合），基于权重矩阵即线性联想器的观点进行细粒度建模。该设计缓解专家重复与路由退化问题，从而减轻遗忘。该工作为持续学习中的记忆管理与遗忘抑制提供了新思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 持续学习中LoRA混合专家方法因专家粒度粗导致冗余、干扰与路由混乱并引发遗忘。
method: 提出MoRAM，将权重矩阵视为线性联想器，构建细粒度的秩1联想记忆专家混合。
result: 缓解专家重复、干扰与路由退化，从而减轻持续学习中的灾难性遗忘。
conclusion: 为持续学习智能体的记忆管理与遗忘抑制提供了细粒度专家方案。
---

## Abstract
Continual learning (CL) with large pre-trained models aims to incrementally acquire knowledge without catastrophic forgetting. Existing LoRA-based Mixture-of-Experts (MoE) methods expand capacity by adding isolated new experts while freezing old ones, but still suffer from redundancy, interference, routing ambiguity, and consequent forgetting. We investigate the issues stemming from coarse-grained expert granularity. Coarse-grained experts (e.g., high-rank LoRA) encode low-specialty information, leading to expert duplication/interference and routing degradation/confusion as experts accumulate. In this work, we propose MoRAM (Mixture of Rank-1 Associative Memory). Grounded in the view that weight matrices act as linear associative memories, MoRAM achieves CL as incremental expansion of reusable atomic rank-1 experts as memory. Each rank-1 adapter acts as a fine-grained MoE expert or an associative memory unit. By viewing rank-1 experts as key-value memory pairs, we eliminate explicit MoE-LoRA routers with self-activation, where each memory atom evaluates its relevance via its intrinsic key. The inference process thus becomes a content-addressable retrieval and recall over the incrementally accumulated memory of learning snapshots. Extensive experiments on CLIP and LLMs show that MoRAM significantly outperforms state-of-the-art methods, achieving a better plasticity–stability trade-off, stronger generalization, and reduced forgetting. Project page: https://artificer-ai-lab.github.io/MoRAM.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
通过秩1联想记忆专家缓解灾难性遗忘的持续学习。

### 2. 核心内容
大型预训练模型的持续学习需增量获取知识而不发生灾难性遗忘，但现有LoRA混合专家方法因专家粒度粗导致冗余、干扰与路由混乱。本文提出MoRAM（秩1联想记忆专家混合），基于权重矩阵即线性联想器的观点进行细粒度建模。该设计缓解专家重复与路由退化问题，从而减轻遗忘。该工作为持续学习中的记忆管理与遗忘抑制提供了新思路。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=P247k4ELcn](https://openreview.net/forum?id=P247k4ELcn)
