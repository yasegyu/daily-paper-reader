---
title: "EvoCF: Multi-Agent Collaboration via Agentic Memory-Driven Evolutionary Counterfactual Planning"
title_zh: EvoCF：基于智能体记忆驱动进化反事实规划的多智能体协作
authors: "Haotian Chi, Zeyu Feng, Xingrui Yu, Linbo Luo, Yew-Soon Ong, Ivor Tsang, Hechang Chen, Yi Chang, Haiyan Yin"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/9fad72d7b7bbe2d670d065bff44b04133136bbb2.pdf"
tags: ["query:agent-memory"]
score: 8.0
evidence: 智能体记忆驱动的多智能体协作规划
tldr: 为多智能体具身系统规划协作策略是大模型规划器的核心挑战，它们常难以捕捉真实环境的物理与协调约束。本文提出EvoCF，一个智能体记忆驱动的进化反事实规划框架，通过符号约束归纳器从失败中提炼可复用规则形成进化规则库，并用进化式反事实规划生成器探索语义一致的规划变体。实验表明该方法能发现更优的多智能体协作策略，凸显了智能体记忆在协作规划中的作用。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 大模型规划器难以捕捉多智能体具身环境中的物理与协调约束。
method: 提出EvoCF，用符号约束归纳器构建进化规则库，并结合进化反事实规划生成器探索规划变体。
result: 实验表明该方法能发现改进的多智能体协作策略。
conclusion: 验证了智能体记忆驱动的规划框架在多智能体协作中的有效性。
---

## Abstract
Planning collaboration strategies for multi-agent embodied systems remains a core challenge for LLM-based planners, which often fail to capture the physical and coordination constraints of realworld environments. To address this, we present EvoCF, an agentic memory-driven evolutionary counterfactual planning framework for discovering improved multi-agent collaboration strategies through counterfactual plan generation and evaluation. First, we propose a symbolic constraint inductor that induces reusable symbolic constraints from failures, forming an evolving rule library. Then, we propose an evolutionary counterfactual plan generator that systematically explores semantically consistent plan variants through rule-conditioned mutations, enabling robust collaboration strategies beyond short-sighted one-shot LLM plans. Finally, we design an agentic memory-grounded evaluator that ranks candidate plans using retrieval-augmented evidence, producing interpretable, constraint-aware selections. Across multi-agent embodied simulation benchmarks, EvoCF consistently discovers more robust and executable plans compared to baseline approaches. Our results demonstrate that grounding multi-agent planning in agentic memory and counterfactual reasoning significantly enhances both effectiveness and robustness.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
智能体记忆驱动的多智能体协作规划。

### 2. 核心内容
为多智能体具身系统规划协作策略是大模型规划器的核心挑战，它们常难以捕捉真实环境的物理与协调约束。本文提出EvoCF，一个智能体记忆驱动的进化反事实规划框架，通过符号约束归纳器从失败中提炼可复用规则形成进化规则库，并用进化式反事实规划生成器探索语义一致的规划变体。实验表明该方法能发现更优的多智能体协作策略，凸显了智能体记忆在协作规划中的作用。

### 3. 对应检索需求
shared memory and communication in multi-agent systems。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=FsSirPJy9U](https://openreview.net/forum?id=FsSirPJy9U)
