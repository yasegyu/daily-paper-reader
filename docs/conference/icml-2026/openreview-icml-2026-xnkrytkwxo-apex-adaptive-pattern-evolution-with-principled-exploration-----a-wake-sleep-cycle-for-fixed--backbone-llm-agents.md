---
title: "APEX: Adaptive Pattern Evolution with Principled Exploration --- A Wake-Sleep Cycle for Fixed--Backbone LLM Agents"
title_zh: APEX：面向固定主干LLM智能体的自适应模式演化与有原则探索——一种唤醒-睡眠循环
authors: "Yuxuan Fu, Xiaoyu Tan, Teqi Hao, Xihe Qiu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/4bee1c0a0333e253793bdae055c57c5d26aa4d6d.pdf"
tags: ["query:agent-memory"]
score: 8.0
evidence: 为LLM智能体整合经验池的演化记忆机制
tldr: 上下文强化学习（ICRL）无需更新参数即可让冻结LLM适配新领域，但现有方法在积累速度与检索效率间难以兼顾，常形成无结构记忆池与静态示例选择。本文提出APEX框架，将ICRL重构为固定主干LLM智能体的唤醒-睡眠循环。在睡眠阶段引入演化记忆机制，通过拓扑算子结构化精炼经验池并蒸馏泛化模式。该工作为智能体的经验记忆整合与高效检索提供了新范式。
source: ICML-2026-Rejected-Public
selection_source: conference_retrieval
motivation: ICRL在积累速度与检索效率间难兼顾，常产生无结构记忆池与次优静态示例选择。
method: 提出APEX框架，将ICRL重构为唤醒-睡眠循环，睡眠阶段用演化记忆机制精炼经验池。
result: 通过拓扑算子结构化整合经验并蒸馏泛化模式，提升记忆检索与利用效率。
conclusion: 为固定主干LLM智能体的经验记忆整合与演化提供新范式。
---

## Abstract
In-Context Reinforcement Learning (ICRL) has emerged as a promising paradigm for adapting frozen Large Language Models (LLMs) to specialized domains without parameter updates. However, existing methods trade off accumulation speed with retrieval efficiency, typically resulting in unstructured memory pools and suboptimal, static example selection. In this work, we propose **APEX** (Adaptive Pattern Evolution with **Principled** Exploration), a framework that reimagines ICRL as a **Wake-Sleep cycle** for fixed-backbone LLM agents. On the consolidation front (“Sleep”), we introduce an Evolutionary Memory Mechanism that structurally refines the experience pool through topological operators, distilling generalized patterns from raw trajectories rather than merely accumulating them. On the inference front (“Wake”), we formulate prompt selection as a Neural Contextual Bandit problem. By leveraging a non-linear reward predictor with **theoretically grounded exploration** derived from NeuralUCB, APEX adaptively constructs high-confidence context sets tailored to query hardness. Empirically, we show that this adaptive cycle boosts mathematical reasoning performance on benchmarks like AIME, allowing frozen agents to significantly outperform both static retrieval baselines and computationally expensive fine-tuned models. Code will be released upon acceptance.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
为LLM智能体整合经验池的演化记忆机制。

### 2. 核心内容
上下文强化学习（ICRL）无需更新参数即可让冻结LLM适配新领域，但现有方法在积累速度与检索效率间难以兼顾，常形成无结构记忆池与静态示例选择。本文提出APEX框架，将ICRL重构为固定主干LLM智能体的唤醒-睡眠循环。在睡眠阶段引入演化记忆机制，通过拓扑算子结构化精炼经验池并蒸馏泛化模式。该工作为智能体的经验记忆整合与高效检索提供了新范式。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Rejected-Public
- OpenReview：[https://openreview.net/forum?id=xnKrytKWxo](https://openreview.net/forum?id=xnKrytKWxo)
