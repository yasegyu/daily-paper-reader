---
title: Structurally Aligned Subtask-Level Memory for Software Engineering Agents
title_zh: 面向软件工程智能体的结构对齐子任务级记忆
authors: "Kangning Shen, Jingyuan Zhang, Chenxi Sun, Wencong Zeng, Yang Yue"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/3e2e8de22a1fb642ce3897235fef2bb6eef954c0.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 面向LLM软件智能体的子任务级记忆架构
tldr: LLM已展现作为自主软件工程智能体的潜力，近期工作为其引入记忆机制以支持长程推理，但这些方法通常在实例粒度上操作，把整个求解回合作为存储与检索的原子单元。作者实证表明实例级记忆存在根本性的粒度错配，当任务表面描述相似但在特定阶段需要不同推理逻辑时会导致误导性检索。为此提出结构对齐的子任务级记忆方法，将记忆的存储、检索与更新对齐到子任务粒度，从而缓解误导性检索问题。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: LLM作为软件工程智能体已展现潜力，但现有记忆机制多在整个问题求解回合的实例粒度上存储与检索，存在粒度错配。
method: 提出结构对齐的子任务级记忆方法，将记忆的存储、检索与更新对齐到子任务粒度。
result: 实验证明实例级记忆在表面描述相似但推理逻辑不同的任务上会导致误导性检索，子任务级对齐可缓解该问题。
conclusion: 为长程软件工程智能体提供更细粒度的记忆机制。
---

## Abstract
Large Language Models (LLMs) have demonstrated significant potential as autonomous software engineering (SWE) agents. Recent work has further explored augmenting these agents with memory mechanisms to support long-horizon reasoning. However, these approaches typically operate at a coarse instance granularity, treating the entire problem-solving episode as the atomic unit of storage and retrieval. We empirically demonstrate that instance-level memory suffers from a fundamental granularity mismatch, resulting in misguided retrieval when tasks with similar surface descriptions require distinct reasoning logic at specific stages. To address this, we propose Structurally Aligned Subtask-Level Memory, a method that aligns memory storage, retrieval, and updating with the agent’s functional decomposition. Extensive experiments on SWE-bench Verified demonstrate that our method consistently outperforms both vanilla agents and strong instance-level memory baselines across diverse backbones, improving mean Pass@1 over the vanilla agent by +4.7 pp on average (e.g., +6.8 pp on Gemini 2.5 Pro). Performance gains grow with more interaction steps, showing that leveraging past experience benefits long-horizon reasoning in complex software engineering tasks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向LLM软件智能体的子任务级记忆架构。

### 2. 核心内容
LLM已展现作为自主软件工程智能体的潜力，近期工作为其引入记忆机制以支持长程推理，但这些方法通常在实例粒度上操作，把整个求解回合作为存储与检索的原子单元。作者实证表明实例级记忆存在根本性的粒度错配，当任务表面描述相似但在特定阶段需要不同推理逻辑时会导致误导性检索。为此提出结构对齐的子任务级记忆方法，将记忆的存储、检索与更新对齐到子任务粒度，从而缓解误导性检索问题。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=2CoRS45Ucj](https://openreview.net/forum?id=2CoRS45Ucj)
