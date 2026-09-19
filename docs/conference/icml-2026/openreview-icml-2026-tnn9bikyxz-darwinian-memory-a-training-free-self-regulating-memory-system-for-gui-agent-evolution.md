---
title: "Darwinian Memory: A Training-Free Self-Regulating Memory System for GUI Agent Evolution"
title_zh: 达尔文记忆：面向GUI智能体演化的免训练自调节记忆系统
authors: "Hongze Mi, Yibo Feng, WenJie Lu, Song Cao, Jinyuan Li, Yanming Li, Xuelin Zhang, Haotian Luo, Songyang Peng, He Cui, Tengfei Tian, Jun Fang, Hua Chai, Naiqiang Tan"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/db9700e3ce01368639c8b929484815d1e360f418.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 面向GUI智能体演化的自调节记忆系统
tldr: 该文针对多模态GUI智能体在长程跨应用任务中上下文有限、既有记忆系统难以适应动态界面且易受陈旧经验污染的问题，提出达尔文记忆系统DMS。DMS将复杂轨迹分解并构建为遵循优胜劣汰法则的动态生态，让记忆在演化中自我调节。该训练无关架构缓解了幻觉并提升跨应用任务表现，为GUI智能体记忆管理提供新思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: GUI智能体受限于上下文窗口，静态记忆累积陈旧经验导致幻觉与粒度错配。
method: 提出DMS，将记忆构建为优胜劣汰的动态生态并分解复杂轨迹。
result: 通过自演化筛选记忆，缓解上下文污染并提升跨应用任务表现。
conclusion: 为动态环境下智能体记忆管理提供免训练自调节方案。
---

## Abstract
Multimodal Large Language Model (MLLM) agents facilitate Graphical User Interface (GUI) automation but struggle with long-horizon, cross-application tasks due to limited context windows. While memory systems provide a viable solution, existing paradigms struggle to adapt to dynamic GUI environments, suffering from a granularity mismatch between high-level intent and low-level execution, and context pollution where the static accumulation of outdated experiences drives agents into hallucination.  
  To address these bottlenecks, we propose the Darwinian Memory System (DMS), a self-evolving architecture that constructs memory as a dynamic ecosystem governed by the law of "survival of the fittest." DMS decomposes complex trajectories into independent, reusable units for compositional flexibility, and implements Utility-driven Natural Selection to track survival value, actively pruning suboptimal paths and inhibiting high-risk plans. This evolutionary pressure compels the agent to derive superior strategies. Extensive experiments on real-world multi-app benchmarks validate that DMS boosts general-purpose MLLMs without training costs or architectural overhead, achieving average gains of 18.0% in success rate and 33.9% in execution stability, while reducing task latency, establishing it as an effective self-evolving memory system for GUI tasks. The implementation is available at https://anonymous.4open.science/r/DMS-C48C.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向GUI智能体演化的自调节记忆系统。

### 2. 核心内容
该文针对多模态GUI智能体在长程跨应用任务中上下文有限、既有记忆系统难以适应动态界面且易受陈旧经验污染的问题，提出达尔文记忆系统DMS。DMS将复杂轨迹分解并构建为遵循优胜劣汰法则的动态生态，让记忆在演化中自我调节。该训练无关架构缓解了幻觉并提升跨应用任务表现，为GUI智能体记忆管理提供新思路。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=tNn9bikyXZ](https://openreview.net/forum?id=tNn9bikyXZ)
