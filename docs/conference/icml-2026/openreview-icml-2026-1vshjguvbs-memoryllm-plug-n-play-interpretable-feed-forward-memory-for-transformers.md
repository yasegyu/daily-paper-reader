---
title: "MemoryLLM: Plug-n-Play Interpretable Feed-Forward Memory for Transformers"
title_zh: MemoryLLM：面向Transformer的即插即用可解释前馈记忆
authors: "AJAY KUMAR JAISWAL, Lauren Hannah, Han-Byul Kim, Duc N.M Hoang, Arnav Kundu, Mehrdad Farajtabar, Minsik Cho"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/d38b16825bfe52e58e802a86f8852003ac917dae.pdf"
tags: ["query:agent-memory"]
score: 5.0
evidence: Transformer中可解释的前馈记忆机制
tldr: 理解Transformer组件运作对AI进展至关重要，本文聚焦前馈模块的可解释性难题。作者提出MemoryLLM，将前馈网络与自注意力解耦，使其可作为上下文无关的逐token神经检索记忆进行研究。方法通过仅用token嵌入单独训练前馈网络，实现记忆的预计算。该工作揭示输入token如何访问前馈参数中的记忆位置，为LLM记忆机制的可解释性提供新工具。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 前馈模块的可解释性不足，且其与自注意力耦合，难以单独研究其作为记忆的功能。
method: 提出MemoryLLM，将前馈网络与自注意力解耦，仅用token嵌入单独训练，使其成为上下文无关的检索记忆。
result: 分析显示不同下游任务对前馈记忆的依赖程度不同，且token以特定方式访问记忆位置。
conclusion: 该工作为理解LLM内部记忆机制提供了可解释的分析框架。
---

## Abstract
Understanding how transformer components operate in LLMs is important, as it is at the core of recent technological advances in artificial intelligence. In this work, we revisit the challenges associated with interpretability of feed-forward modules (FFNs) and propose MemoryLLM, which aims to decouple FFNs from self-attention and enables us to study the decoupled FFNs as context-free token-wise neural retrieval memory. In detail, we investigate how input tokens access memory locations within FFN parameters and the importance of FFN memory across different downstream tasks. MemoryLLM achieves context-free FFNs by training them in isolation from self-attention directly using the token embeddings. This approach allows FFNs to be pre-computed as token-wise lookups (ToLs), enabling on-demand transfer between VRAM and storage, additionally enhancing inference efficiency. We also introduce Flex-MemoryLLM, positioning it between a conventional transformer design and MemoryLLM. This architecture bridges the performance gap caused by training FFNs with context-free token-wise embeddings.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
Transformer中可解释的前馈记忆机制。

### 2. 核心内容
理解Transformer组件运作对AI进展至关重要，本文聚焦前馈模块的可解释性难题。作者提出MemoryLLM，将前馈网络与自注意力解耦，使其可作为上下文无关的逐token神经检索记忆进行研究。方法通过仅用token嵌入单独训练前馈网络，实现记忆的预计算。该工作揭示输入token如何访问前馈参数中的记忆位置，为LLM记忆机制的可解释性提供新工具。

### 3. 对应检索需求
Find top tier AI conference papers on memory architectures for autonomous agents and large language model agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=1vshJGUVBS](https://openreview.net/forum?id=1vshJGUVBS)
