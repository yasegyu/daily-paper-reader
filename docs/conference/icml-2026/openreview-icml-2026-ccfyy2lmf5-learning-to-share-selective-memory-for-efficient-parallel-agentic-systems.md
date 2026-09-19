---
title: "Learning to Share: Selective Memory for Efficient Parallel Agentic Systems"
title_zh: 学会共享：面向高效并行智能体系统的选择性记忆
authors: "Joseph Fioresi, Parth Parag Kulkarni, Ashmal Vayani, Song Wang, Mubarak Shah"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/36afa45a025ea9f91750ce099712175131a4547b.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 面向并行智能体团队的习得共享记忆机制
tldr: 并行多智能体系统通过多团队探索提升鲁棒性，但团队间对相似子问题的独立推理造成大量重复计算与开销。本文提出Learning to Share（LTS），一种可学习的共享记忆机制，使并行智能体框架能够选择性地跨团队复用信息，同时控制上下文增长。该工作降低了并行执行成本，为多智能体系统的共享记忆与协作通信提供了新思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 并行多智能体团队独立推理相似子问题导致大量重复计算与高昂开销。
method: 提出Learning to Share可学习共享记忆机制，实现跨团队选择性信息复用并控制上下文增长。
result: 在保持鲁棒性与解质量的同时降低并行执行的重复计算成本。
conclusion: 为多智能体并行系统提供高效的共享记忆与协作通信机制。
---

## Abstract
Agentic systems solve complex tasks by coordinating multiple agents that iteratively reason, invoke tools, and exchange intermediate results. To improve robustness and solution quality, recent approaches deploy multiple agent teams running in parallel to explore diverse reasoning trajectories. However, parallel execution comes at a significant computational cost: when different teams independently reason about similar sub-problems or execute analogous steps, they repeatedly perform substantial overlapping computation. To address these limitations, in this paper, we propose Learning to Share (LTS), a learned shared-memory mechanism for parallel agentic frameworks that enables selective cross-team information reuse while controlling context growth. LTS introduces a global memory bank accessible to all teams and a lightweight controller that decides whether intermediate agent steps should be added to memory or not. The controller is trained using stepwise reinforcement learning with usage-aware credit assignment, allowing it to identify information that is globally useful across parallel executions. Experiments on the AssistantBench and GAIA benchmarks show that LTS significantly reduces overall runtime while matching or improving task performance compared to memory-free parallel baselines, demonstrating that learned memory admission is an effective strategy for improving the efficiency of parallel agentic systems.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向并行智能体团队的习得共享记忆机制。

### 2. 核心内容
并行多智能体系统通过多团队探索提升鲁棒性，但团队间对相似子问题的独立推理造成大量重复计算与开销。本文提出Learning to Share（LTS），一种可学习的共享记忆机制，使并行智能体框架能够选择性地跨团队复用信息，同时控制上下文增长。该工作降低了并行执行成本，为多智能体系统的共享记忆与协作通信提供了新思路。

### 3. 对应检索需求
shared memory and communication in multi-agent systems。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=cCFyY2LmF5](https://openreview.net/forum?id=cCFyY2LmF5)
