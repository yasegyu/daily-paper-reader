---
title: Learning Query-Aware Budget-Tier Routing for Runtime Agent Memory
title_zh: 面向运行时智能体记忆的查询感知预算分层路由学习
authors: "Haozhen Zhang, Haodong Yue, Tao Feng, Quanyu Long, Jianzhu Bao, Bowen Jin, Weizhi Zhang, Xiao Li, Jiaxuan You, Chengwei Qin, Wenya Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/6d34d163d6de7c6e7c44fb7d8ce6427a25700991.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 带预算分层路由的运行时智能体记忆框架
tldr: 现有LLM智能体记忆系统多依赖离线、与查询无关的构建方式，效率低且可能丢失查询关键信息。本文提出BudgetMem运行时记忆框架，将记忆处理拆分为多个模块，每个模块提供低中高三档预算，并用轻量路由器按查询动态选择预算层级。该设计在性能与成本之间实现显式可控的权衡，为跨上下文窗口的智能体记忆提供了更灵活的运行时方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有智能体记忆多为离线且与查询无关的构建方式，效率低且易丢弃关键信息。
method: 提出BudgetMem，把记忆处理组织为多模块三档预算，并用轻量路由器按查询进行预算分层路由。
result: 实现显式的查询感知性能与成本权衡控制，提升运行时记忆利用效率。
conclusion: 为跨上下文窗口的LLM智能体提供灵活可控的运行时记忆管理框架。
---

## Abstract
Memory is increasingly central to Large Language Model (LLM) agents operating beyond a single context window, yet most existing systems rely on offline, query-agnostic memory construction that can be inefficient and may discard query-critical information. Although runtime memory utilization is a natural alternative, prior work often incurs substantial overhead and offers limited explicit control over the performance-cost trade-off. In this work, we present **BudgetMem**, a runtime agent memory framework for explicit, query-aware performance–cost control. BudgetMem structures memory processing as a set of memory modules, each offered in three budget tiers (i.e., Low/Mid/High). A lightweight router performs budget-tier routing across modules to balance task performance and memory construction cost, which is implemented as a compact neural policy trained with reinforcement learning. Using BudgetMem as a unified testbed, we study three complementary strategies for realizing budget tiers: implementation (method complexity), reasoning (inference behavior), and capacity (module model size). Across LoCoMo, LongMemEval, and HotpotQA, BudgetMem surpasses strong baselines when performance is prioritized (i.e., high-budget setting), and delivers better accuracy–cost frontiers under tighter budgets. Moreover, our analysis disentangles the strengths and weaknesses of different tiering strategies, clarifying when each axis delivers the most favorable trade-offs under varying budget regimes. Code is available at https://github.com/ViktorAxelsen/BudgetMem

---

## 论文详细总结（自动生成）

### 1. 检索相关性
带预算分层路由的运行时智能体记忆框架。

### 2. 核心内容
现有LLM智能体记忆系统多依赖离线、与查询无关的构建方式，效率低且可能丢失查询关键信息。本文提出BudgetMem运行时记忆框架，将记忆处理拆分为多个模块，每个模块提供低中高三档预算，并用轻量路由器按查询动态选择预算层级。该设计在性能与成本之间实现显式可控的权衡，为跨上下文窗口的智能体记忆提供了更灵活的运行时方案。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=5G9puwbCsu](https://openreview.net/forum?id=5G9puwbCsu)
