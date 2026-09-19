---
title: "AOEB: Benchmarking Agent-Oriented Multimodal Embeddings"
title_zh: AOEB：面向智能体的多模态嵌入基准评测
authors: "Xin Zhang, Jiaxin Xu, mengjia zhou, Xinping Zhao, Yinghui Li, di yin, Xing Sun, Meishan Zhang, Baotian Hu, Wenjie Li, Min Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/6e1f3a3a7181ec86650fcfd44d05c06f76d98415.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 面向智能体嵌入检索（含记忆检索）的基准
tldr: 基于检索与RAG的LLM智能体日益普及，嵌入模型在检索中至关重要，但现有嵌入基准多面向通用场景，难以匹配智能体应用的多样化需求。本文提出Agent-Oriented Embedding Benchmark（AOEB），涵盖代码、工具、推理、记忆检索等五项智能体检索能力，并支持多模态评测。该基准为智能体记忆检索等场景的嵌入模型评估提供了针对性工具。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有嵌入基准面向通用场景，无法匹配LLM智能体多样化检索需求。
method: 提出AOEB基准，覆盖代码、工具、推理与记忆检索等五项能力并支持多模态评测。
result: 为智能体中心检索（含记忆检索）的嵌入模型提供系统化评测。
conclusion: 弥补通用嵌入基准与智能体检索需求之间的评估空白。
---

## Abstract
LLM agents powered by retrieval and RAG are increasingly prevalent across research and applications. Embedding models play a critical role in these systems, particularly in embedding-based retrieval. However, current benchmarks for embeddings remain focused on general-purpose scenarios, which may fail to align well with the diverse and evolving needs of agentic applications. To close this gap, we introduce Agent-Oriented Embedding Benchmark (AOEB), a comprehensive evaluation suite dedicated to agent-centric retrieval for embedding models. AOEB is characterized by two key features: (1) Multi-Task, covering five essential capabilities for retrieval in LLM agents, including code, tool, reasoning, and memory retrieval; and (2) Multi-Modal, providing evaluation with both textual and visual data for each task category. We evaluate representative embedding models on AOEB and observe that they exhibit distinct strengths across different agent-oriented retrieval tasks. By curating AOEB, we aim to promote a move toward more practically oriented directions within the embedding community and foster further progress.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向智能体嵌入检索（含记忆检索）的基准。

### 2. 核心内容
基于检索与RAG的LLM智能体日益普及，嵌入模型在检索中至关重要，但现有嵌入基准多面向通用场景，难以匹配智能体应用的多样化需求。本文提出Agent-Oriented Embedding Benchmark（AOEB），涵盖代码、工具、推理、记忆检索等五项智能体检索能力，并支持多模态评测。该基准为智能体记忆检索等场景的嵌入模型评估提供了针对性工具。

### 3. 对应检索需求
memory retrieval mechanisms for agent decision making。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=mNOx4mKh3F](https://openreview.net/forum?id=mNOx4mKh3F)
