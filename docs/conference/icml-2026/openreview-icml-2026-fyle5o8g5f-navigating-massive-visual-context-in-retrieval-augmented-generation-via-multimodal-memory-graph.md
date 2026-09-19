---
title: Navigating Massive Visual Context in Retrieval-Augmented Generation via Multimodal Memory Graph
title_zh: 通过多模态记忆图应对检索增强生成中的海量视觉上下文
authors: "Qiuchen Wang, Shihang Wang, Yu Zeng, Qiang Zhang, Fanrui Zhang, Zhuoning Guo, Bosi Zhang, Wenxuan Huang, Lin Chen, Zehui Chen, Pengjun Xie, Ruixue Ding"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/15bcadd889fea39eb43c9100ff8bf6e8f045eccf.pdf"
tags: ["query:agent-memory"]
score: 8.0
evidence: 用于智能体推理检索的多模态记忆图
tldr: 传统检索增强生成依赖线性交互历史，难以应对长上下文尤其是信息稀疏但token繁重的视觉数据。作者提出VimRAG框架，将智能体推理过程建模为动态有向无环图，把智能体状态与检索到的多模态证据组织为结构化记忆。该结构化记忆机制改善了跨文本、图像与视频的迭代推理与检索效率，为多模态智能体记忆检索提供了新思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 传统RAG依赖线性交互历史，难以处理迭代推理中信息稀疏却token繁重的长上下文多模态数据。
method: 提出VimRAG框架，将智能体推理过程建模为动态有向无环图，结构化组织智能体状态与检索到的多模态证据。
result: 该结构化记忆机制提升了跨文本、图像和视频的检索与迭代推理表现，缓解了长上下文处理难题。
conclusion: 说明用图结构记忆组织多模态证据可有效支撑智能体的长上下文检索增强推理。
---

## Abstract
Effectively retrieving, reasoning, and understanding multimodal information remains a critical challenge for agentic systems. Traditional Retrieval-augmented Generation (RAG) methods rely on linear interaction histories, which struggle to handle long-context tasks, especially those involving information-sparse yet token-heavy visual data in iterative reasoning scenarios. To bridge this gap, we introduce VimRAG, a framework tailored for multimodal Retrieval-augmented Reasoning across text, images, and videos. Inspired by our systematic study, we model the reasoning process as a dynamic directed acyclic graph that structures the agent states and retrieved multimodal evidence. Building upon this structured memory, we introduce a Graph-Modulated Visual Memory Encoding mechanism, with which the significance of memory nodes is evaluated via their topological position, allowing the model to dynamically allocate high-resolution tokens to pivotal evidence while compressing or discarding trivial clues. To implement this paradigm, we propose a Graph-Guided Policy Optimization strategy. This strategy disentangles step-wise validity from trajectory-level rewards by pruning memory nodes associated with redundant actions, thereby facilitating fine-grained credit assignment. Extensive experiments demonstrate that VimRAG consistently achieves state-of-the-art performance on diverse multimodal RAG benchmarks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
用于智能体推理检索的多模态记忆图。

### 2. 核心内容
传统检索增强生成依赖线性交互历史，难以应对长上下文尤其是信息稀疏但token繁重的视觉数据。作者提出VimRAG框架，将智能体推理过程建模为动态有向无环图，把智能体状态与检索到的多模态证据组织为结构化记忆。该结构化记忆机制改善了跨文本、图像与视频的迭代推理与检索效率，为多模态智能体记忆检索提供了新思路。

### 3. 对应检索需求
memory retrieval mechanisms for agent decision making。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=fylE5O8g5F](https://openreview.net/forum?id=fylE5O8g5F)
