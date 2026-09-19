---
title: Benchmarking Agent Memory in Interdependent Multi-Session Agentic Tasks
title_zh: 在相互依赖的多会话智能体任务中评测智能体记忆
authors: "Zexue He, Yu Wang, Churan Zhi, Yuanzhe Hu, Tzu-Ping Chen, Lang Yin, Ze Chen, Tong Arthur Wu, Siru Ouyang, Zihan Wang, Jiaxin Pei, Julian McAuley, Yejin Choi, Alex Pentland"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/76c2c4e7ec8f3e47d153e7f82d46e02885c63b47.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 面向多会话智能体任务的智能体记忆基准
tldr: 现有智能体记忆评测往往将记忆与行动割裂：一类只测对话或文本回忆，无法反映记忆如何指导决策；另一类只测单会话任务，无需长期记忆。本文提出MemoryArena，一个统一的评测平台，在记忆-智能体-环境循环中评估多会话智能体记忆。该基准由人工构建，捕捉记忆获取与后续任务求解紧密耦合的真实设定。它为智能体记忆研究提供更贴近实际的标准评测。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有智能体记忆评测将记忆与行动割裂，无法反映记忆如何指导未来决策这一真实需求。
method: 提出MemoryArena统一评测平台，在记忆-智能体-环境循环中评估多会话任务下记忆与行动的耦合。
result: 该基准由人工构建，覆盖智能体在交互中获取记忆并用于后续任务求解的完整闭环。
conclusion: 该工作为智能体记忆提供了更贴近现实、兼顾记忆与行动的标准化评测方案。
---

## Abstract
Existing evaluations of agents with memory typically assess **memorization** and **action** in isolation. One class of benchmarks evaluates memorization by testing recall of past conversations or text but fails to capture how memory is used to guide future decisions. Another class focuses on agents acting in single-session tasks without the need for long-term memory. However, in realistic settings, memorization and action are tightly coupled: agents acquire memory while interacting with the environment, and subsequently rely on that memory to solve future tasks. To capture this setting, we introduce MemoryArena, a unified evaluation gym for benchmarking agent memory in multi-session Memory-Agent-Environment loops. The benchmark consists of human-crafted agentic tasks with explicitly interdependent subtasks, where agents must learn from earlier actions and feedback by distilling experiences into memory, and subsequently use that memory to guide later actions to solve the overall task. MEMORYARENA supports evaluation across web navigation, preference-constrained planning, progressive information search, and sequential formal reasoning, and reveals that agents with near-saturated performance on existing long-context memory benchmarks like LoCoMo perform poorly in our agentic setting, exposing a gap in current evaluations for agents with memory.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向多会话智能体任务的智能体记忆基准。

### 2. 核心内容
现有智能体记忆评测往往将记忆与行动割裂：一类只测对话或文本回忆，无法反映记忆如何指导决策；另一类只测单会话任务，无需长期记忆。本文提出MemoryArena，一个统一的评测平台，在记忆-智能体-环境循环中评估多会话智能体记忆。该基准由人工构建，捕捉记忆获取与后续任务求解紧密耦合的真实设定。它为智能体记忆研究提供更贴近实际的标准评测。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=JHYmxqS9Jv](https://openreview.net/forum?id=JHYmxqS9Jv)
