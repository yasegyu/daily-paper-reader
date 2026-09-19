---
title: "AOEB: Benchmarking Agent-Oriented Multimodal Embeddings"
title_zh: AOEB：面向智能体的多模态嵌入基准
authors: "Xin Zhang, Jiaxin Xu, mengjia zhou, Xinping Zhao, Yinghui Li, di yin, Xing Sun, Meishan Zhang, Baotian Hu, Wenjie Li, Min Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/6e1f3a3a7181ec86650fcfd44d05c06f76d98415.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 覆盖LLM智能体记忆检索能力的基准
tldr: 现有嵌入模型评测多聚焦通用场景，难以贴合智能体应用多样且演进的检索需求。作者提出面向智能体的嵌入基准AOEB，覆盖代码、工具、推理与记忆检索等五项关键能力，并支持多模态评测。该基准为评估智能体记忆检索等嵌入能力提供了统一标准，有助于推动智能体检索系统的发展，但对记忆架构本身贡献有限。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有嵌入评测聚焦通用场景，无法对齐智能体应用多样且不断演进的检索需求，尤其是记忆检索能力。
method: 提出面向智能体的嵌入基准AOEB，覆盖代码、工具、推理、记忆检索等五项任务能力，并提供多模态评测。
result: 该基准为评估智能体检索相关嵌入模型提供了统一评测套件，揭示了通用嵌入在智能体场景的不足。
conclusion: 强调需要专门面向智能体检索的评测标准，以支撑记忆检索等能力的可靠衡量。
---

## Abstract
LLM agents powered by retrieval and RAG are increasingly prevalent across research and applications. Embedding models play a critical role in these systems, particularly in embedding-based retrieval. However, current benchmarks for embeddings remain focused on general-purpose scenarios, which may fail to align well with the diverse and evolving needs of agentic applications. To close this gap, we introduce Agent-Oriented Embedding Benchmark (AOEB), a comprehensive evaluation suite dedicated to agent-centric retrieval for embedding models. AOEB is characterized by two key features: (1) Multi-Task, covering five essential capabilities for retrieval in LLM agents, including code, tool, reasoning, and memory retrieval; and (2) Multi-Modal, providing evaluation with both textual and visual data for each task category. We evaluate representative embedding models on AOEB and observe that they exhibit distinct strengths across different agent-oriented retrieval tasks. By curating AOEB, we aim to promote a move toward more practically oriented directions within the embedding community and foster further progress.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
覆盖LLM智能体记忆检索能力的基准。

### 2. 核心内容
现有嵌入模型评测多聚焦通用场景，难以贴合智能体应用多样且演进的检索需求。作者提出面向智能体的嵌入基准AOEB，覆盖代码、工具、推理与记忆检索等五项关键能力，并支持多模态评测。该基准为评估智能体记忆检索等嵌入能力提供了统一标准，有助于推动智能体检索系统的发展，但对记忆架构本身贡献有限。

### 3. 对应检索需求
Find top tier AI conference papers on memory architectures for autonomous agents and large language model agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=mNOx4mKh3F](https://openreview.net/forum?id=mNOx4mKh3F)
