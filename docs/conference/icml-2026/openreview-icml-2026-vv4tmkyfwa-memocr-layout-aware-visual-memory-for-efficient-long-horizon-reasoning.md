---
title: "MemOCR: Layout-Aware Visual Memory for Efficient Long-Horizon Reasoning"
title_zh: MemOCR：面向高效长时程推理的版面感知视觉记忆
authors: "Yaorui Shi, Shugui Liu, Yu Yang, Wenyu Mao, Yuxin Chen, Qi GU, Hui Su, Xunliang Cai, Xiang Wang, An Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/76f14e73cf6aaf2154bb30987aedba5fe345728f.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 面向长时程智能体推理的版面感知视觉记忆
tldr: 长时程智能体推理需要把不断增长的交互历史压缩进有限上下文，但现有记忆系统多以文本序列化历史，token成本随长度线性增长，浪费在低价值细节上。为此，论文提出多模态记忆智能体MemOCR，通过视觉版面为记忆分配自适应信息密度。它维护结构化的富文本记忆（如标题、高亮）并渲染成图像，智能体查阅该图像访问记忆，视觉上突出关键证据并压缩次要细节。该工作为紧张上下文预算下的智能体记忆压缩提供了新思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 长时程推理需把增长的交互历史压入有限上下文，而文本式记忆token成本线性增长且浪费于低价值细节。
method: 提出多模态记忆智能体MemOCR，维护结构化富文本记忆并渲染为图像，用视觉版面自适应分配信息密度。
result: 在紧张上下文预算下提升长时程推理效率，视觉突出关键证据并压缩次要细节。
conclusion: 为智能体记忆压缩与检索提供基于视觉版面的新范式。
---

## Abstract
Long-horizon agentic reasoning necessitates effectively compressing growing interaction histories into a limited context window.
Most existing memory systems serialize history as text, where token-level cost is uniform and scales linearly with length, often spending scarce budget on low-value details.
To this end, we introduce **MemOCR**, a multimodal memory agent that improves long-horizon reasoning under tight context budgets by allocating memory space with adaptive information density through visual layout.
Concretely, MemOCR maintains a structured rich-text memory (e.g., headings, highlights) and renders it into an image that the agent consults for memory access, visually prioritizing crucial evidence while aggressively compressing auxiliary details.
To ensure robustness across varying memory budgets, we train MemOCR with reinforcement learning under budget-aware objectives that expose the agent to diverse compression levels.
Across long-context multi-hop and single-hop question-answering benchmarks, MemOCR outperforms strong text-based baselines and achieves more effective context utilization under extreme budgets.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向长时程智能体推理的版面感知视觉记忆。

### 2. 核心内容
长时程智能体推理需要把不断增长的交互历史压缩进有限上下文，但现有记忆系统多以文本序列化历史，token成本随长度线性增长，浪费在低价值细节上。为此，论文提出多模态记忆智能体MemOCR，通过视觉版面为记忆分配自适应信息密度。它维护结构化的富文本记忆（如标题、高亮）并渲染成图像，智能体查阅该图像访问记忆，视觉上突出关键证据并压缩次要细节。该工作为紧张上下文预算下的智能体记忆压缩提供了新思路。

### 3. 对应检索需求
Search for papers about long term memory, episodic memory, and memory retrieval in interactive agent systems.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=vv4TMkyfWA](https://openreview.net/forum?id=vv4TMkyfWA)
