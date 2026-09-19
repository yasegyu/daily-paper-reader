---
title: "Memora: A Harmonic Memory Representation Balancing Abstraction and Specificity"
title_zh: Memora：平衡抽象与具体的谐调记忆表示
authors: "Menglin Xia, Xuchao Zhang, Shantanu Dixit, Paramaguru Harimurugan, Rujia Wang, Victor Rühle, Robert Sim, Chetan Bansal, Saravan Rajmohan"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/0cb2d1b1e6a87f8e3c6fa7ef5facd8b3f2346657.pdf"
tags: ["query:agent-memory"]
score: 10.0
evidence: 平衡抽象与具体的智能体记忆表示与检索
tldr: 智能体记忆系统需容纳持续增长的信息并支持高效上下文感知检索，但抽象虽利于扩展却牺牲细节，影响推理。本文提出Memora谐调记忆表示，通过主抽象索引具体记忆值并整合相关更新，借助线索锚点扩展多角度检索访问并连接相关记忆。基于该结构设计激活式检索策略，在抽象与具体间取得平衡，为可扩展的智能体记忆架构提供新表示范式。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 智能体记忆需持续扩展并高效检索，但抽象化会牺牲推理所需的细粒度细节。
method: 提出Memora谐调记忆表示，用主抽象索引具体值并用线索锚点扩展检索连接。
result: 在抽象与具体之间取得结构平衡，支持高效上下文感知的记忆检索。
conclusion: 为可扩展的智能体记忆架构提供新的记忆表示与检索策略。
---

## Abstract
Agent memory systems must accommodate continuously growing information while supporting efficient, context-aware retrieval for downstream tasks. Abstraction is essential for scaling agent memory, yet it often comes at the cost of specificity, obscuring the fine-grained details required for effective reasoning. We introduce Memora, a harmonic memory representation that structurally balances abstraction and specificity. Memora organizes information via its *primary abstractions* that index concrete memory values and consolidate related updates into unified memory entries, while *cue anchors* expand retrieval access across diverse aspects of the memory and connect related memories. Building on this structure, we employ a retrieval policy that actively exploits these memory connections to retrieve relevant information beyond direct semantic similarity. Theoretically, we show that standard Retrieval-Augmented Generation (RAG) and Knowledge Graph (KG)-based memory systems emerge as special cases of our framework. Empirically, Memora establishes a new state-of-the-art on the LoCoMo and LongMemEval benchmarks, demonstrating better retrieval relevance and reasoning effectiveness as memory scales.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
平衡抽象与具体的智能体记忆表示与检索。

### 2. 核心内容
智能体记忆系统需容纳持续增长的信息并支持高效上下文感知检索，但抽象虽利于扩展却牺牲细节，影响推理。本文提出Memora谐调记忆表示，通过主抽象索引具体记忆值并整合相关更新，借助线索锚点扩展多角度检索访问并连接相关记忆。基于该结构设计激活式检索策略，在抽象与具体间取得平衡，为可扩展的智能体记忆架构提供新表示范式。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=zSrvkj0ers](https://openreview.net/forum?id=zSrvkj0ers)
