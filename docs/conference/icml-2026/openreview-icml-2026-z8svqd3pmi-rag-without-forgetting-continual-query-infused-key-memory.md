---
title: "RAG without Forgetting: Continual Query-Infused Key Memory"
title_zh: 不遗忘的RAG：持续查询注入式键记忆
authors: "Yuntong Hu, Sha Li, Naren Ramakrishnan, Liang Zhao"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/014da7f78f2559372ce20ed814ed82657f6013d2.pdf"
tags: ["query:agent-memory"]
score: 7.0
evidence: RAG中不遗忘的持续演化检索记忆
tldr: 现有RAG的查询期适配（如查询扩展、迭代检索）是无状态的，每次查询重新计算并丢弃，无法累积学习且重复消耗推理成本。索引侧方法虽具持久性，却依赖离线预处理或弱对齐的启发式更新，导致语义漂移与噪声累积。本文提出Evolving Retrieval Memory（ERM），一个免训练框架，通过持续更新检索索引将瞬时收益转化为持久改进。该工作为RAG记忆的持续演化与遗忘抑制提供了新方法。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: RAG查询期适配无状态、无法累积学习，索引侧方法又易语义漂移与噪声累积。
method: 提出免训练的Evolving Retrieval Memory框架，通过持续更新检索索引持久化查询收益。
result: 将瞬时查询收益转化为持久检索改进，缓解语义漂移与重复推理开销。
conclusion: 为RAG系统的持续记忆演化与遗忘抑制提供免训练方案。
---

## Abstract
Retrieval-augmented generation (RAG) systems commonly improve robustness via query-time adaptations such as query expansion and iterative retrieval. While effective, these approaches are inherently stateless: adaptations are recomputed for each query and discarded thereafter, precluding cumulative learning and repeatedly incurring inference-time cost. Index-side approaches like key expansion introduce persistence but rely on offline preprocessing or heuristic updates that are weakly aligned with downstream task utility, leading to semantic drift and noise accumulation. We propose Evolving Retrieval Memory (ERM), a training-free framework that transforms transient query-time gains into persistent retrieval improvements. ERM updates the retrieval index through correctness-gated feedback, selectively attributes atomic expansion signals to the document keys they benefit, and progressively evolves keys via stable, norm-bounded updates. We show that query and key expansion are theoretically equivalent under standard similarity functions and prove convergence of ERM’s selective updates, amortizing optimal query expansion into a stable index with zero inference-time overhead. Experiments on BEIR and BRIGHT across 13 domains demonstrate consistent gains in retrieval and generation, particularly on reasoning-intensive tasks, at native retrieval speed.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
RAG中不遗忘的持续演化检索记忆。

### 2. 核心内容
现有RAG的查询期适配（如查询扩展、迭代检索）是无状态的，每次查询重新计算并丢弃，无法累积学习且重复消耗推理成本。索引侧方法虽具持久性，却依赖离线预处理或弱对齐的启发式更新，导致语义漂移与噪声累积。本文提出Evolving Retrieval Memory（ERM），一个免训练框架，通过持续更新检索索引将瞬时收益转化为持久改进。该工作为RAG记忆的持续演化与遗忘抑制提供了新方法。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=Z8svqD3pmI](https://openreview.net/forum?id=Z8svqD3pmI)
