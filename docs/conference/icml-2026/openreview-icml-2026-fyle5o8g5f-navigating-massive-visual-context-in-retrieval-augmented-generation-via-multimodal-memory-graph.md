---
title: Navigating Massive Visual Context in Retrieval-Augmented Generation via Multimodal Memory Graph
title_zh: 通过多模态记忆图导航检索增强生成中的海量视觉上下文
authors: "Qiuchen Wang, Shihang Wang, Yu Zeng, Qiang Zhang, Fanrui Zhang, Zhuoning Guo, Bosi Zhang, Wenxuan Huang, Lin Chen, Zehui Chen, Pengjun Xie, Ruixue Ding"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/15bcadd889fea39eb43c9100ff8bf6e8f045eccf.pdf"
tags: ["query:agent-memory"]
score: 7.0
evidence: 以多模态记忆图组织智能体状态与检索证据
tldr: 该文针对智能体系统在长上下文多模态推理中传统RAG依赖线性交互历史、难以处理信息稀疏却token密集的视觉数据的问题，提出VimRAG框架。它把推理过程建模为动态有向无环图，将智能体状态与检索到的多模态证据结构化为记忆，并在其上执行图式检索。该结构化记忆提升了跨文本图像视频的检索增强推理能力。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 传统RAG依赖线性历史，难以应对长程、token密集的多模态推理场景。
method: 提出VimRAG，将推理建模为动态有向无环图作为结构化记忆并图式检索。
result: 结构化多模态记忆提升了长上下文检索增强推理效果。
conclusion: 为交互式智能体的长程多模态记忆与检索提供图结构方案。
---

## Abstract
Effectively retrieving, reasoning, and understanding multimodal information remains a critical challenge for agentic systems. Traditional Retrieval-augmented Generation (RAG) methods rely on linear interaction histories, which struggle to handle long-context tasks, especially those involving information-sparse yet token-heavy visual data in iterative reasoning scenarios. To bridge this gap, we introduce VimRAG, a framework tailored for multimodal Retrieval-augmented Reasoning across text, images, and videos. Inspired by our systematic study, we model the reasoning process as a dynamic directed acyclic graph that structures the agent states and retrieved multimodal evidence. Building upon this structured memory, we introduce a Graph-Modulated Visual Memory Encoding mechanism, with which the significance of memory nodes is evaluated via their topological position, allowing the model to dynamically allocate high-resolution tokens to pivotal evidence while compressing or discarding trivial clues. To implement this paradigm, we propose a Graph-Guided Policy Optimization strategy. This strategy disentangles step-wise validity from trajectory-level rewards by pruning memory nodes associated with redundant actions, thereby facilitating fine-grained credit assignment. Extensive experiments demonstrate that VimRAG consistently achieves state-of-the-art performance on diverse multimodal RAG benchmarks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
以多模态记忆图组织智能体状态与检索证据。

### 2. 核心内容
该文针对智能体系统在长上下文多模态推理中传统RAG依赖线性交互历史、难以处理信息稀疏却token密集的视觉数据的问题，提出VimRAG框架。它把推理过程建模为动态有向无环图，将智能体状态与检索到的多模态证据结构化为记忆，并在其上执行图式检索。该结构化记忆提升了跨文本图像视频的检索增强推理能力。

### 3. 对应检索需求
Search for papers about long term memory, episodic memory, and memory retrieval in interactive agent systems.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=fylE5O8g5F](https://openreview.net/forum?id=fylE5O8g5F)
