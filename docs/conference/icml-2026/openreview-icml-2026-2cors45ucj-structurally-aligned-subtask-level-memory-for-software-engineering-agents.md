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
evidence: 面向软件工程智能体的子任务级记忆存储与检索
tldr: 针对软件工程智能体记忆以整个问题解决实例为原子单位、存在粒度失配导致检索误导的问题，本文通过实证揭示相似表层描述的任务在特定阶段需要不同推理逻辑，提出结构对齐的子任务级记忆方法，将记忆的存储、检索与更新对齐到子任务粒度。该工作提升了长程推理中记忆检索的准确性，为智能体记忆架构的粒度设计提供了重要启示。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有软件工程智能体记忆以实例为原子粒度，存在粒度失配导致检索误导。
method: 提出结构对齐的子任务级记忆方法，使记忆存储、检索与更新对齐到子任务粒度。
result: 实证表明子任务级记忆能缓解相似描述任务的检索误导，提升长程推理准确性。
conclusion: 为智能体记忆架构的粒度对齐设计提供了重要方法与经验启示。
---

## Abstract
Large Language Models (LLMs) have demonstrated significant potential as autonomous software engineering (SWE) agents. Recent work has further explored augmenting these agents with memory mechanisms to support long-horizon reasoning. However, these approaches typically operate at a coarse instance granularity, treating the entire problem-solving episode as the atomic unit of storage and retrieval. We empirically demonstrate that instance-level memory suffers from a fundamental granularity mismatch, resulting in misguided retrieval when tasks with similar surface descriptions require distinct reasoning logic at specific stages. To address this, we propose Structurally Aligned Subtask-Level Memory, a method that aligns memory storage, retrieval, and updating with the agent’s functional decomposition. Extensive experiments on SWE-bench Verified demonstrate that our method consistently outperforms both vanilla agents and strong instance-level memory baselines across diverse backbones, improving mean Pass@1 over the vanilla agent by +4.7 pp on average (e.g., +6.8 pp on Gemini 2.5 Pro). Performance gains grow with more interaction steps, showing that leveraging past experience benefits long-horizon reasoning in complex software engineering tasks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向软件工程智能体的子任务级记忆存储与检索。

### 2. 核心内容
针对软件工程智能体记忆以整个问题解决实例为原子单位、存在粒度失配导致检索误导的问题，本文通过实证揭示相似表层描述的任务在特定阶段需要不同推理逻辑，提出结构对齐的子任务级记忆方法，将记忆的存储、检索与更新对齐到子任务粒度。该工作提升了长程推理中记忆检索的准确性，为智能体记忆架构的粒度设计提供了重要启示。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=2CoRS45Ucj](https://openreview.net/forum?id=2CoRS45Ucj)
