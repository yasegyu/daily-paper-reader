---
title: "Neuromem: A Granular Decomposition of the Streaming Lifecycle in External Memory for LLMs"
title_zh: Neuromem：LLM外部记忆流式生命周期的细粒度分解
authors: "Ruicheng Zhang, Xinyi Li, Tianyi Xu, Shuhao Zhang, Xiaofei Liao, Hai Jin"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/b220b1948f14ac0ed4397c5065686164ebfbf770.pdf"
tags: ["query:agent-memory"]
score: 8.0
evidence: 外部记忆的流式生命周期含巩固与检索
tldr: 现有对外部记忆模块的评估大多假设静态设定，即记忆离线构建并在固定状态下被查询，但现实中记忆是流式的，新事实持续到达，插入与检索交错进行。Neuromem提出一个可扩展测试平台，在插入与检索交错的协议下评测外部记忆，并将记忆生命周期细分为数据结构、归一化策略、巩固策略、查询方式等五个维度，从而揭示流式记忆在准确率与成本上的规律，为外部记忆研究提供细粒度评测基础。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有外部记忆模块评估多假设静态离线设定，而实际记忆是流式的，新事实不断到达且插入与检索交错。
method: 提出可扩展测试平台Neuromem，在插入-检索交错协议下评测外部记忆，并将记忆生命周期分解为数据结构、归一化、巩固策略、查询等维度。
result: 该平台揭示了流式记忆在准确率与成本上的生命周期规律。
conclusion: 为外部记忆模块提供细粒度、流式化的评测框架。
---

## Abstract
Most evaluations of External Memory Module assume a static setting: memory is built offline and queried at a fixed state. In practice, memory is streaming: new facts arrive continuously, insertions interleave with retrievals, and the memory state evolves while the model is serving queries. In this regime, accuracy and cost are governed by the full memory lifecycle, which encompasses the ingestion, maintenance, retrieval, and integration of information into generation. We present Neuromem, a scalable testbed that benchmarks External Memory Module under an interleaved insertion-and-retrieval protocol and decomposes its lifecycle into five dimensions including memory data structure, normalization strategy, consolidation policy, query formulation strategy, and context integration mechanism. Using three representative datasets LoCoMo, LONGMEMEVAL, and MemAgentBench, Neuromem evaluates interchangeable variants within a shared serving stack, reporting token-level F1 and insertion/retrieval latency.Overall, we observe that performance typically degrades as memory grows across rounds, and time-related queries remain the most challenging category. The memory data structure largely determines the attainable quality frontier, while aggressive compression and generative integration mechanisms mostly shift cost between insertion and retrieval with limited accuracy gain.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
外部记忆的流式生命周期含巩固与检索。

### 2. 核心内容
现有对外部记忆模块的评估大多假设静态设定，即记忆离线构建并在固定状态下被查询，但现实中记忆是流式的，新事实持续到达，插入与检索交错进行。Neuromem提出一个可扩展测试平台，在插入与检索交错的协议下评测外部记忆，并将记忆生命周期细分为数据结构、归一化策略、巩固策略、查询方式等五个维度，从而揭示流式记忆在准确率与成本上的规律，为外部记忆研究提供细粒度评测基础。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=mO7DgwFFVe](https://openreview.net/forum?id=mO7DgwFFVe)
