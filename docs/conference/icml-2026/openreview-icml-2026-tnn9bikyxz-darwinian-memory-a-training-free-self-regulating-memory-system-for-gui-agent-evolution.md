---
title: "Darwinian Memory: A Training-Free Self-Regulating Memory System for GUI Agent Evolution"
title_zh: 达尔文记忆：面向GUI智能体进化的免训练自调节记忆系统
authors: "Hongze Mi, Yibo Feng, WenJie Lu, Song Cao, Jinyuan Li, Yanming Li, Xuelin Zhang, Haotian Luo, Songyang Peng, He Cui, Tengfei Tian, Jun Fang, Hua Chai, Naiqiang Tan"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/db9700e3ce01368639c8b929484815d1e360f418.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 面向GUI智能体进化的自调节记忆系统
tldr: 多模态大模型智能体在长程跨应用GUI任务中受限于上下文窗口，现有记忆范式难以适应动态GUI环境，存在高层意图与底层执行粒度不匹配及上下文污染问题。本文提出达尔文记忆系统DMS，将记忆构建为遵循适者生存法则的动态生态系统，把复杂轨迹分解为可自适应演化的记忆单元。该架构无需训练即可自我调节，减少过时经验累积导致的幻觉，提升智能体长期演化能力。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有GUI智能体记忆范式难以适应动态环境，存在粒度不匹配与过时经验累积导致的上下文污染和幻觉。
method: 提出达尔文记忆系统DMS，将记忆构建为遵循适者生存法则的动态生态系统，对复杂轨迹分解与自演化管理。
result: 该系统免训练即可自调节，减少过时经验的静态累积，缓解智能体在长程任务中的幻觉。
conclusion: 该工作为动态环境下智能体记忆的自我调节与遗忘管理提供了新架构。
---

## Abstract
Multimodal Large Language Model (MLLM) agents facilitate Graphical User Interface (GUI) automation but struggle with long-horizon, cross-application tasks due to limited context windows. While memory systems provide a viable solution, existing paradigms struggle to adapt to dynamic GUI environments, suffering from a granularity mismatch between high-level intent and low-level execution, and context pollution where the static accumulation of outdated experiences drives agents into hallucination.  
  To address these bottlenecks, we propose the Darwinian Memory System (DMS), a self-evolving architecture that constructs memory as a dynamic ecosystem governed by the law of "survival of the fittest." DMS decomposes complex trajectories into independent, reusable units for compositional flexibility, and implements Utility-driven Natural Selection to track survival value, actively pruning suboptimal paths and inhibiting high-risk plans. This evolutionary pressure compels the agent to derive superior strategies. Extensive experiments on real-world multi-app benchmarks validate that DMS boosts general-purpose MLLMs without training costs or architectural overhead, achieving average gains of 18.0% in success rate and 33.9% in execution stability, while reducing task latency, establishing it as an effective self-evolving memory system for GUI tasks. The implementation is available at https://anonymous.4open.science/r/DMS-C48C.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向GUI智能体进化的自调节记忆系统。

### 2. 核心内容
多模态大模型智能体在长程跨应用GUI任务中受限于上下文窗口，现有记忆范式难以适应动态GUI环境，存在高层意图与底层执行粒度不匹配及上下文污染问题。本文提出达尔文记忆系统DMS，将记忆构建为遵循适者生存法则的动态生态系统，把复杂轨迹分解为可自适应演化的记忆单元。该架构无需训练即可自我调节，减少过时经验累积导致的幻觉，提升智能体长期演化能力。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=tNn9bikyXZ](https://openreview.net/forum?id=tNn9bikyXZ)
