---
title: Integrated Episodic and Semantic Memory via Modulating Transformer FeedForward Layers
title_zh: 通过调制Transformer前馈层整合情景记忆与语义记忆
authors: "Yiqun Yao, Xiang Li, Xin Jiang, Xuezhi Fang, Naitong Yu, Siwei Dong, Wenjia Ma, Jing Li, Aixin Sun, Yequan Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/96b3a6d551885bf0b3b28a9bf42fcea315a722aa.pdf"
tags: ["query:agent-memory"]
score: 8.0
evidence: 通过调制Transformer前馈层统一情景记忆与语义记忆
tldr: 针对Transformer中语义记忆隐含于前馈层、情景记忆依赖KV缓存且难以直接检索的问题，本文提出Hypermem，用超网络将上下文循环映射为前馈层参数的定向更新，使同一组参数兼具语义与情景记忆，并可在不显式访问KV缓存的情况下检索。作者以续写与随机访问联想记忆目标对超网络后训练，验证了统一记忆的可行性，为智能体情景记忆与长期记忆机制提供了新范式。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有模型语义记忆隐含于前馈层、情景记忆存于KV缓存，二者分离且情景记忆难以直接检索。
method: 提出Hypermem超网络，将上下文循环映射为前馈层参数的定向更新，实现统一记忆。
result: 以续写与随机访问联想记忆目标后训练，验证同一组参数兼具语义与情景记忆。
conclusion: 为智能体情景记忆与长期记忆机制提供了统一、可检索的新范式。
---

## Abstract
It is widely recognized that, after generative pre-training, Transformer FeedForward layers implicitly function as semantic memory, encoding linguistic and factual knowledge, while the contexts in key–value (KV) cache contain raw events, serving as the source of models' episodic memory. In this work, we show that a same group of Transformer FeedForward-layer parameters can both be semantic and episodic memory, which is retrievable without explicitly attending to the related KV cache. To realize this idea, we introduce Hypermem, a hypernetwork that recurrently maps contexts into targeted updates of FeedForward parameters. We post-train the hypernetwork using continuation and random-access associative memory objectives, eliminating the need for test-time training. Extensive experiments demonstrate that our approach outperforms related methods, including MemoryLLM and generative adapter, on memory retrieval, long-context question answering, and personalization benchmarks, establishing a new state of the art for hypernetwork-based memory mechanisms. Our results suggest that directly bridging data and parameters provides a viable direction for exploring next-generation foundation models with more flexible and persistent memory capabilities.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
通过调制Transformer前馈层统一情景记忆与语义记忆。

### 2. 核心内容
针对Transformer中语义记忆隐含于前馈层、情景记忆依赖KV缓存且难以直接检索的问题，本文提出Hypermem，用超网络将上下文循环映射为前馈层参数的定向更新，使同一组参数兼具语义与情景记忆，并可在不显式访问KV缓存的情况下检索。作者以续写与随机访问联想记忆目标对超网络后训练，验证了统一记忆的可行性，为智能体情景记忆与长期记忆机制提供了新范式。

### 3. 对应检索需求
Search for papers about long term memory, episodic memory, and memory retrieval in interactive agent systems.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=7D5WD70jKj](https://openreview.net/forum?id=7D5WD70jKj)
