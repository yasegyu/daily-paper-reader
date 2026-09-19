---
title: "Beyond Buffer Limits: Energy-Based Data Reassembly for Continual Learning"
title_zh: 超越缓冲区限制：面向持续学习的能量式数据重组
authors: "Zhenyi Wang, Yixuan Sun, Yue Wang, Zhong Chen, Heng Huang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/49699383f12b96e34f33d266b684f927fb6cf712.pdf"
tags: ["query:agent-memory"]
score: 5.0
evidence: 基于记忆回放的持续学习抗遗忘方法
tldr: 针对记忆回放受限于缓冲区容量、每个样本仅代表单个实例的问题，本文提出数据重组范式，将当前任务数据切分为基本片段并通过能量模型动态重组为连贯回放样本。该方法显著提升记忆效率，在有限缓冲下缓解灾难性遗忘。其贡献在于为持续学习提供更高效的记忆管理机制，对智能体长期学习中的遗忘抑制具有借鉴意义。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 记忆回放方法受限于缓冲区容量，每个存储样本仅代表单个数据实例，导致抗遗忘效果受限。
method: 将当前任务训练数据切分为基本片段，通过能量模型动态重组为连贯的复合回放样本。
result: 在有限记忆容量下显著提升记忆效率，有效缓解灾难性遗忘。
conclusion: 为持续学习提供更高效的记忆管理范式，可支撑智能体的长期学习。
---

## Abstract
Continual learning (CL) aims to acquire new knowledge from a non-stationary data stream while retaining performance on previously learned tasks. Memory-based replay methods mitigate catastrophic forgetting by storing and revisiting past samples, but their effectiveness is fundamentally constrained by limited memory capacity, as each stored example represents only a single data instance. In this work, we propose data reassembly for CL, a new paradigm that significantly increases memory efficiency by reassembling composite replay samples from existing training data. Instead of storing raw training examples, we partition the current task training data into elementary patches and dynamically reassemble them into coherent replay instances through an energy-based optimization framework. The proposed objective jointly enforces semantic compatibility with target labels and global consistency among assembled patches. To make this optimization tractable, we derive an efficient variational inference algorithm that constructs a compact yet diverse set of reassembled samples for replay. Extensive theoretical analysis and experiments across multiple CL benchmarks demonstrate that data reassembly consistently outperforms existing memory-based approaches, achieving stronger retention of past knowledge while maintaining competitive computational efficiency.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
基于记忆回放的持续学习抗遗忘方法。

### 2. 核心内容
针对记忆回放受限于缓冲区容量、每个样本仅代表单个实例的问题，本文提出数据重组范式，将当前任务数据切分为基本片段并通过能量模型动态重组为连贯回放样本。该方法显著提升记忆效率，在有限缓冲下缓解灾难性遗忘。其贡献在于为持续学习提供更高效的记忆管理机制，对智能体长期学习中的遗忘抑制具有借鉴意义。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=cbicSAXMWQ](https://openreview.net/forum?id=cbicSAXMWQ)
