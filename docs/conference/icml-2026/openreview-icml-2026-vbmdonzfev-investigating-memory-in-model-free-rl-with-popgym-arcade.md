---
title: Investigating Memory in Model-Free RL with POPGym Arcade
title_zh: 用POPGym Arcade研究无模型强化学习中的记忆
authors: "Zekang Wang, Zhe He, Borong Zhang, Edan Toledo, Steven Morad"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/f0b8999c07b219f8508fb1c20522f47d297d93e3.pdf"
tags: ["query:agent-memory"]
score: 7.0
evidence: 分析强化学习智能体如何在部分可观测下利用记忆决策
tldr: 如何分析深度强化学习中的记忆机制尚缺乏系统工具，部分可观测下智能体如何利用记忆决策仍不清晰。本文提出POPGym Arcade，一组共享观测与动作空间、兼具完全与部分可观测变体的硬件加速环境，并提供分析工具。研究发现受控对比研究对公平比较是必要的，并揭示价值函数将信用摊到无关历史、以及分布外情境污染记忆的病理现象。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 部分可观测下深度强化学习智能体如何利用记忆决策缺乏系统分析工具与受控对比环境。
method: 提出POPGym Arcade环境集与配套分析工具，提供完全与部分可观测变体以开展可观测性反事实研究。
result: 研究发现价值函数会将信用摊到无关历史，且分布外情境会污染记忆并长期扰动策略。
conclusion: 该工作为理解智能体记忆机制与诊断记忆病理提供了可复用的实验平台与工具。
---

## Abstract
How should we analyze memory in deep RL? We introduce tools for analyzing policies under partial observability and revealing how agents use memory to make decisions. To utilize these tools, we present POPGym Arcade, a collection of Atari-inspired, hardware-accelerated environments sharing a single observation and action space. Each environment provides fully and partially observable variants, enabling counterfactual studies on observability. We find that controlled studies are necessary for fair comparisons and identify a pathology where value functions smear credit over irrelevant history. Using this pathology, we demonstrate how out-of-distribution scenarios can contaminate memory, perturbing the policy far into the future.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
分析强化学习智能体如何在部分可观测下利用记忆决策。

### 2. 核心内容
如何分析深度强化学习中的记忆机制尚缺乏系统工具，部分可观测下智能体如何利用记忆决策仍不清晰。本文提出POPGym Arcade，一组共享观测与动作空间、兼具完全与部分可观测变体的硬件加速环境，并提供分析工具。研究发现受控对比研究对公平比较是必要的，并揭示价值函数将信用摊到无关历史、以及分布外情境污染记忆的病理现象。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=vBMdonzFEV](https://openreview.net/forum?id=vBMdonzFEV)
