---
title: "PlugMem: A Task-Agnostic Plugin Memory Module for LLM Agents"
title_zh: PlugMem：面向LLM智能体的任务无关插件式记忆模块
authors: "Ke Yang, Zixi Chen, Xuan He, Jize Jiang, Michel Galley, Chenglong Wang, Jianfeng Gao, Jiawei Han, ChengXiang Zhai"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/fa49d3fde622c96b3947888aa3f7e985709d9aba.pdf"
tags: ["query:agent-memory"]
score: 10.0
evidence: 面向LLM智能体的任务无关插件式记忆模块
tldr: 长期记忆对复杂环境中的LLM智能体至关重要，但现有设计要么任务特定难以迁移，要么任务无关却因检索原始经验而相关性低、上下文爆炸。本文提出PlugMem，一个可附加到任意LLM智能体的任务无关插件式记忆模块。受认知科学启发，它把情节记忆组织为紧凑可扩展、以知识为中心的记忆图，显式表示命题性与规范性知识。该表示支持高效检索并提升决策相关性，为通用智能体记忆提供了可迁移方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: LLM智能体的长期记忆设计要么任务特定难迁移，要么任务无关却因原始检索导致相关性低与上下文爆炸。
method: 提出PlugMem插件式记忆模块，把情节记忆组织为以知识为中心的紧凑记忆图，表示命题与规范性知识。
result: 可附加到任意LLM智能体而无需任务特定改造，提升记忆检索的相关性与效率。
conclusion: 为通用LLM智能体提供了可迁移、任务无关的长期记忆方案。
---

## Abstract
Long-term memory is essential for large language model (LLM) agents operating in complex environments, yet existing memory designs are either task-specific and non-transferable, or task-agnostic but less effective due to low task-relevance and context explosion from raw memory retrieval. We propose PlugMem, a task-agnostic plugin memory module that can be attached to arbitrary LLM agents without task-specific redesign. Motivated by the fact that decision-relevant information is concentrated as abstract knowledge rather than raw experience, we draw on cognitive science to structure episodic memories into a compact, extensible knowledge-centric memory graph that explicitly represents propositional and prescriptive knowledge. This representation enables efficient memory retrieval and reasoning over task-relevant knowledge, rather than verbose raw trajectories, and departs from other graph-based methods like GraphRAG by treating knowledge as the unit of memory access and organization instead of entities or text chunks. We evaluate PlugMem unchanged across three heterogeneous benchmarks (long-horizon conversational question answering, multi-hop knowledge retrieval, and web agent tasks). 
The results show that PlugMem consistently outperforms task-agnostic baselines and exceeds task-specific memory designs, while also achieving the highest information density under a unified information-theoretic analysis. Code and data are available at https://github.com/TIMAN-group/PlugMem.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向LLM智能体的任务无关插件式记忆模块。

### 2. 核心内容
长期记忆对复杂环境中的LLM智能体至关重要，但现有设计要么任务特定难以迁移，要么任务无关却因检索原始经验而相关性低、上下文爆炸。本文提出PlugMem，一个可附加到任意LLM智能体的任务无关插件式记忆模块。受认知科学启发，它把情节记忆组织为紧凑可扩展、以知识为中心的记忆图，显式表示命题性与规范性知识。该表示支持高效检索并提升决策相关性，为通用智能体记忆提供了可迁移方案。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=NWKaQIKoGp](https://openreview.net/forum?id=NWKaQIKoGp)
