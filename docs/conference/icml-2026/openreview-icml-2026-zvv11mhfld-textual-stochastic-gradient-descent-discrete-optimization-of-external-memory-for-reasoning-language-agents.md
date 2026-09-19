---
title: "Textual Stochastic Gradient Descent: Discrete Optimization of External Memory for Reasoning Language Agents"
title_zh: 文本随机梯度下降：面向推理语言智能体外部记忆的离散优化
authors: "Jian Li, Hua Huang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/20d2cc89323456d72845cfab670731be07808850.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 优化语言智能体存储经验的外部记忆
tldr: 大模型虽具强推理能力，但要从经验中持续学习而不做参数重训仍是难题，现有检索增强生成把记忆当作静态或仅追加的语料，导致噪声与冗余累积的记忆饱和。本文提出经验库优化框架，将智能体的外部记忆视为容量预算下的可学习参数，并设计文本随机梯度下降进行离散优化。实验表明该方法能有效管理记忆、缓解饱和并提升推理智能体的持续表现。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有RAG把智能体记忆视为静态或仅追加语料，导致记忆饱和与性能退化。
method: 提出经验库优化框架，把外部记忆当作可学习参数，并用文本随机梯度下降进行离散优化。
result: 实验表明该方法能缓解记忆饱和并提升智能体持续推理表现。
conclusion: 为语言智能体外部记忆的优化管理提供了新思路。
---

## Abstract
While Large Language Models (LLMs) possess strong reasoning capabilities, enabling them to learn continuously from experience without parametric retraining remains an open challenge. Existing Retrieval-Augmented Generation (RAG) approaches typically treat memory as a static or append-only corpus, leading to "memory saturation," where accumulating noise and redundant information degrade performance over time. To address this, we propose an Experience Library Optimization framework that treats the agent's external memory, which we call the experience library, as a learnable parameter under an explicit capacity budget. We introduce Textual Stochastic Gradient Descent (TSGD), a discrete optimization algorithm that refines this library via failure-driven Add, Edit, and Delete operations. TSGD estimates "textual gradients" through self-reflection and uses a dual-verification mechanism to ensure generalization, which prevents overfitting to local errors. Empirical results on MATH and AIME benchmarks show that TSGD achieves state-of-the-art performance, improving accuracy by up to $18.7\%$ over zero-shot baselines and substantially outperforming static RAG, while keeping a compact memory footprint (compressing hundreds of experiences into $\approx 30$ high-utility rules).

---

## 论文详细总结（自动生成）

### 1. 检索相关性
优化语言智能体存储经验的外部记忆。

### 2. 核心内容
大模型虽具强推理能力，但要从经验中持续学习而不做参数重训仍是难题，现有检索增强生成把记忆当作静态或仅追加的语料，导致噪声与冗余累积的记忆饱和。本文提出经验库优化框架，将智能体的外部记忆视为容量预算下的可学习参数，并设计文本随机梯度下降进行离散优化。实验表明该方法能有效管理记忆、缓解饱和并提升推理智能体的持续表现。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=zVv11MhFLD](https://openreview.net/forum?id=zVv11MhFLD)
