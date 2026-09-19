---
title: "Textual Stochastic Gradient Descent: Discrete Optimization of External Memory for Reasoning Language Agents"
title_zh: 文本随机梯度下降：推理语言智能体外部记忆的离散优化
authors: "Jian Li, Hua Huang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/20d2cc89323456d72845cfab670731be07808850.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 为推理语言智能体优化外部经验记忆库
tldr: 针对RAG将记忆视为静态或仅追加语料、导致记忆饱和与噪声累积的问题，本文提出经验库优化框架，把智能体的外部记忆当作容量预算下的可学习参数，并设计文本随机梯度下降（TSGD）这一离散优化算法来精炼记忆。该工作使智能体无需参数重训即可从经验中持续学习，有效抑制冗余信息对性能的侵蚀，为记忆增强智能体提供了可管理的经验存储与更新机制。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: RAG把记忆当作静态或仅追加语料，导致噪声累积与记忆饱和，性能随时间退化。
method: 提出经验库优化框架，将外部记忆视为容量受限的可学习参数，并用文本随机梯度下降离散优化。
result: 在容量预算下有效精炼经验库，缓解记忆饱和，支持智能体持续从经验学习。
conclusion: 为记忆增强智能体提供可管理的经验存储与更新范式，无需参数重训即可持续学习。
---

## Abstract
While Large Language Models (LLMs) possess strong reasoning capabilities, enabling them to learn continuously from experience without parametric retraining remains an open challenge. Existing Retrieval-Augmented Generation (RAG) approaches typically treat memory as a static or append-only corpus, leading to "memory saturation," where accumulating noise and redundant information degrade performance over time. To address this, we propose an Experience Library Optimization framework that treats the agent's external memory, which we call the experience library, as a learnable parameter under an explicit capacity budget. We introduce Textual Stochastic Gradient Descent (TSGD), a discrete optimization algorithm that refines this library via failure-driven Add, Edit, and Delete operations. TSGD estimates "textual gradients" through self-reflection and uses a dual-verification mechanism to ensure generalization, which prevents overfitting to local errors. Empirical results on MATH and AIME benchmarks show that TSGD achieves state-of-the-art performance, improving accuracy by up to $18.7\%$ over zero-shot baselines and substantially outperforming static RAG, while keeping a compact memory footprint (compressing hundreds of experiences into $\approx 30$ high-utility rules).

---

## 论文详细总结（自动生成）

### 1. 检索相关性
为推理语言智能体优化外部经验记忆库。

### 2. 核心内容
针对RAG将记忆视为静态或仅追加语料、导致记忆饱和与噪声累积的问题，本文提出经验库优化框架，把智能体的外部记忆当作容量预算下的可学习参数，并设计文本随机梯度下降（TSGD）这一离散优化算法来精炼记忆。该工作使智能体无需参数重训即可从经验中持续学习，有效抑制冗余信息对性能的侵蚀，为记忆增强智能体提供了可管理的经验存储与更新机制。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=zVv11MhFLD](https://openreview.net/forum?id=zVv11MhFLD)
