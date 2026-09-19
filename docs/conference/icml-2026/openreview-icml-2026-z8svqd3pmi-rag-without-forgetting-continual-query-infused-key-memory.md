---
title: "RAG without Forgetting: Continual Query-Infused Key Memory"
title_zh: 不忘却的检索增强生成：持续查询注入的键记忆
authors: "Yuntong Hu, Sha Li, Naren Ramakrishnan, Liang Zhao"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/014da7f78f2559372ce20ed814ed82657f6013d2.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 跨查询持续演化且不遗忘的检索记忆
tldr: 检索增强生成常通过查询扩展与迭代检索提升鲁棒性，但这类查询时适配是无状态的，每次重算且随即丢弃，无法累积学习。索引侧方法虽有持久性，却依赖离线预处理或启发式更新，易产生语义漂移与噪声累积。本文提出演化检索记忆ERM，免训练地将查询时的瞬时收益转化为持久的检索改进，实现持续且不遗忘的检索记忆更新。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有查询时适配无状态、无法累积，索引侧更新又依赖离线或启发式处理，易致语义漂移。
method: 提出免训练框架ERM，将查询时的瞬时收益通过相关性更新转化为检索索引的持久改进。
result: ERM实现持续演化且不遗忘的检索记忆，在累积学习同时避免语义漂移与噪声堆积。
conclusion: 持久化检索记忆为RAG系统提供了可累积、抗遗忘的记忆管理方案。
---

## Abstract
Retrieval-augmented generation (RAG) systems commonly improve robustness via query-time adaptations such as query expansion and iterative retrieval. While effective, these approaches are inherently stateless: adaptations are recomputed for each query and discarded thereafter, precluding cumulative learning and repeatedly incurring inference-time cost. Index-side approaches like key expansion introduce persistence but rely on offline preprocessing or heuristic updates that are weakly aligned with downstream task utility, leading to semantic drift and noise accumulation. We propose Evolving Retrieval Memory (ERM), a training-free framework that transforms transient query-time gains into persistent retrieval improvements. ERM updates the retrieval index through correctness-gated feedback, selectively attributes atomic expansion signals to the document keys they benefit, and progressively evolves keys via stable, norm-bounded updates. We show that query and key expansion are theoretically equivalent under standard similarity functions and prove convergence of ERM’s selective updates, amortizing optimal query expansion into a stable index with zero inference-time overhead. Experiments on BEIR and BRIGHT across 13 domains demonstrate consistent gains in retrieval and generation, particularly on reasoning-intensive tasks, at native retrieval speed.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
跨查询持续演化且不遗忘的检索记忆。

### 2. 核心内容
检索增强生成常通过查询扩展与迭代检索提升鲁棒性，但这类查询时适配是无状态的，每次重算且随即丢弃，无法累积学习。索引侧方法虽有持久性，却依赖离线预处理或启发式更新，易产生语义漂移与噪声累积。本文提出演化检索记忆ERM，免训练地将查询时的瞬时收益转化为持久的检索改进，实现持续且不遗忘的检索记忆更新。

### 3. 对应检索需求
Search for papers about long term memory, episodic memory, and memory retrieval in interactive agent systems.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=Z8svqD3pmI](https://openreview.net/forum?id=Z8svqD3pmI)
