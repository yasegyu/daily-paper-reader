---
title: Experience-Evolving Multi-Turn Tool-Use Agent with Hybrid Episodic–Procedural Memory
title_zh: 基于情节-程序混合记忆的经验演化多轮工具使用智能体
authors: "Sijia Li, Yuchen Huang, Zifan LIU, Zijian Li, Jingjing Fu, Lei Song, Jiang Bian, Jun Zhang, Rui Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/d7b1c92eae0525a01f32380127bad444afdeabf9.pdf"
tags: ["query:agent-memory"]
score: 10.0
evidence: 面向经验演化工具使用智能体的情节-程序混合记忆
tldr: 多轮智能体在意图展开与环境变化中面临不断迁移的决策情境，但现有经验复用方法受限：完整轨迹过于具体难以迁移，工具级复用又忽略上下文与环境。本文提出情节-程序混合记忆策略H-EPM，借鉴人类情节与程序记忆的整合，从累积轨迹构建工具图，以重复出现的工具依赖刻画程序性例程。该策略在推理与训练中自适应复用部分重叠的成功经验，实现多轮工具使用策略的经验演化。工作表明混合记忆能有效提升智能体的经验迁移能力。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多轮工具使用智能体面对不断变化的决策情境，完整轨迹难以迁移、工具级复用又忽略上下文。
method: 提出H-EPM混合情节-程序记忆，从轨迹构建工具图，捕捉工具依赖的程序性例程并自适应复用经验。
result: 在推理与训练中复用部分重叠的成功经验，实现多轮工具使用策略的经验演化。
conclusion: 表明情节与程序记忆的整合能提升智能体经验复用的迁移性与效率。
---

## Abstract
As intents unfold and environments change, multi-turn agents face continuously shifting decision contexts. Although reusing past experience is intuitively appealing, existing approaches remain limited: full trajectories are often too context-specific to transfer, while tool-level reuse ignores the context and environment. In this paper, we introduce a hybrid episodic–procedural memory strategy (H-EPM) that enables experience-evolution of multi-turn tool-use policies, by adaptively reusing partially overlapping successful experiences in both inference and training.
Inspired by human episodic–procedural integration, we build a tool graph from accumulated trajectories, where recurring tool-to-tool dependencies capture procedural routines and each edge is augmented with a compact episodic summaries of relevant context. At inference, the agent dynamically balances episodic recall for contextual reasoning and procedural execution for routine steps.
Beyond inference, H-EPM introduces a memory-guided reinforcement learning paradigm that directly addresses a core challenge in multi-turn agent RL: ineffective exploration over long trajectories. By biasing exploration toward historically successful tool transitions, H-EPM learns a stronger policy that generalizes during inference without relying on domain-specific experience collection. Experiments show that H-EPM consistently delivers substantial inference-time gains over strong baselines across multi-turn tool-use benchmarks, reaching up to 50%+. It also boosts RL policy performance, achieving up to 40%+ improvement on out-of-distribution tasks. Our code is available at https://github.com/LISijia-dev/H-EPM.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向经验演化工具使用智能体的情节-程序混合记忆。

### 2. 核心内容
多轮智能体在意图展开与环境变化中面临不断迁移的决策情境，但现有经验复用方法受限：完整轨迹过于具体难以迁移，工具级复用又忽略上下文与环境。本文提出情节-程序混合记忆策略H-EPM，借鉴人类情节与程序记忆的整合，从累积轨迹构建工具图，以重复出现的工具依赖刻画程序性例程。该策略在推理与训练中自适应复用部分重叠的成功经验，实现多轮工具使用策略的经验演化。工作表明混合记忆能有效提升智能体的经验迁移能力。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=PJ0GpmFYrR](https://openreview.net/forum?id=PJ0GpmFYrR)
