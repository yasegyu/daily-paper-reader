---
title: "Beyond Buffer Limits: Energy-Based Data Reassembly for Continual Learning"
title_zh: 超越缓冲区限制：面向持续学习的基于能量的数据重组
authors: "Zhenyi Wang, Yixuan Sun, Yue Wang, Zhong Chen, Heng Huang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/49699383f12b96e34f33d266b684f927fb6cf712.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 面向持续学习的高效记忆重放数据重组方法
tldr: 持续学习需在非平稳数据流上获取新知识并保持旧任务性能，基于记忆重放的方法虽能缓解灾难性遗忘，却受限于有限记忆容量，因为每个存储样本只代表单个数据实例。本文提出面向持续学习的数据重组范式，不再存储原始样本，而是把当前任务数据划分为基本片段，并通过基于能量的方法动态重组为连贯的重放实例。该方法显著提升记忆效率，突破重放缓冲区容量限制。其为持续学习中的记忆管理与遗忘缓解提供了新途径。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 基于重放的持续学习受限于记忆容量，每个存储样本仅代表单个数据实例，效率低下。
method: 提出数据重组范式，把任务数据切分为基本片段，并用基于能量的方法动态重组为连贯重放样本。
result: 显著提升记忆效率，突破重放缓冲区的容量限制并缓解灾难性遗忘。
conclusion: 为持续学习中的记忆管理与遗忘缓解提供了更高效率的重放途径。
---

## Abstract
Continual learning (CL) aims to acquire new knowledge from a non-stationary data stream while retaining performance on previously learned tasks. Memory-based replay methods mitigate catastrophic forgetting by storing and revisiting past samples, but their effectiveness is fundamentally constrained by limited memory capacity, as each stored example represents only a single data instance. In this work, we propose data reassembly for CL, a new paradigm that significantly increases memory efficiency by reassembling composite replay samples from existing training data. Instead of storing raw training examples, we partition the current task training data into elementary patches and dynamically reassemble them into coherent replay instances through an energy-based optimization framework. The proposed objective jointly enforces semantic compatibility with target labels and global consistency among assembled patches. To make this optimization tractable, we derive an efficient variational inference algorithm that constructs a compact yet diverse set of reassembled samples for replay. Extensive theoretical analysis and experiments across multiple CL benchmarks demonstrate that data reassembly consistently outperforms existing memory-based approaches, achieving stronger retention of past knowledge while maintaining competitive computational efficiency.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向持续学习的高效记忆重放数据重组方法。

### 2. 核心内容
持续学习需在非平稳数据流上获取新知识并保持旧任务性能，基于记忆重放的方法虽能缓解灾难性遗忘，却受限于有限记忆容量，因为每个存储样本只代表单个数据实例。本文提出面向持续学习的数据重组范式，不再存储原始样本，而是把当前任务数据划分为基本片段，并通过基于能量的方法动态重组为连贯的重放实例。该方法显著提升记忆效率，突破重放缓冲区容量限制。其为持续学习中的记忆管理与遗忘缓解提供了新途径。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=cbicSAXMWQ](https://openreview.net/forum?id=cbicSAXMWQ)
