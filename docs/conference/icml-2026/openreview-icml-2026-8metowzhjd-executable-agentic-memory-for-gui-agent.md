---
title: Executable Agentic Memory for GUI Agent
title_zh: 面向GUI智能体的可执行智能体记忆
authors: "Zerui Qin, Sheng Yue, Xingyuan Hua, Yongjian Fu, Ju Ren"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/2e90eea000fd7ad6bfc9e10d372a0038b88a0140.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 用于检索与执行规划的结构化智能体记忆
tldr: 现代GUI智能体依赖以模型为中心、逐步交互的范式，需在每个界面重新解释并决策，在长程任务中十分脆弱。本文提出可执行智能体记忆EAM，用结构化知识图谱将GUI规划从自由生成转变为稳健的检索与执行过程。方法包含状态感知DFS与动作组挖掘的记忆构建流水线，以及由轻量Q函数引导MCTS的值引导图搜索。该工作为长程GUI任务提供高效可靠的规划记忆。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: GUI智能体逐步交互范式需反复解释界面并决策，在长程任务中脆弱且低效。
method: 提出可执行智能体记忆EAM，用知识图谱压缩多步例程，并以Q函数引导MCTS进行值引导图搜索。
result: 该框架将规划转为检索与执行过程，理论上证明Q模型的偏差一致性并给出样本复杂度界。
conclusion: 该工作为GUI智能体提供了结构化、可复用的记忆规划方案。
---

## Abstract
Modern GUI agents typically rely on a model-centric and step-wise interaction paradigm, where LLMs must re-interpret the UI and re-decide actions at every screen, which is fragile in long-horizon tasks. In this paper, we propose Executable Agentic Memory (EAM), a structured Knowledge Graph (KG) that shifts GUI planning from free-form generation to a robust retrieval-and-execution process. Our approach includes a sample-efficient memory construction pipeline using state-aware DFS and action-group mining to compress multi-step routines. To ensure efficient planning, we introduce a value-guided graph search where a lightweight Q-function model steers Monte Carlo Tree Search (MCTS) over the KG. We theoretically establish bias-consistency for the Q-model and derive sample complexity bounds for path recovery. Empirically, EAM outperforms state-of-the-art baselines like UI-TARS-7B by up to $19.6\%$ on AndroidWorld, while reducing token costs $6\times$ relative to GPT-4o. With a $2.8$s average latency, EAM enables reliable, quick, and long-horizon GUI automation.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
用于检索与执行规划的结构化智能体记忆。

### 2. 核心内容
现代GUI智能体依赖以模型为中心、逐步交互的范式，需在每个界面重新解释并决策，在长程任务中十分脆弱。本文提出可执行智能体记忆EAM，用结构化知识图谱将GUI规划从自由生成转变为稳健的检索与执行过程。方法包含状态感知DFS与动作组挖掘的记忆构建流水线，以及由轻量Q函数引导MCTS的值引导图搜索。该工作为长程GUI任务提供高效可靠的规划记忆。

### 3. 对应检索需求
memory retrieval mechanisms for agent decision making。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=8metOwZHjD](https://openreview.net/forum?id=8metOwZHjD)
