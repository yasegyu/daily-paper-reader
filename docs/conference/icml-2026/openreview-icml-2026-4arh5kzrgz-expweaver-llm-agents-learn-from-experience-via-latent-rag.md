---
title: "ExpWeaver: LLM Agents Learn from Experience via Latent RAG"
title_zh: ExpWeaver：大模型智能体通过潜在检索增强生成从经验中学习
authors: "Tao Feng, Tianyang Luo, Jingjun Xu, Zhigang Hua, Yan Xie, Shuang Yang, Ge Liu, Jiaxuan You"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/868299e3b83f82e8c4c8baa5f861219b70cb2ec8.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 大模型智能体通过潜在检索存储经验来学习
tldr: 现有基于经验的智能体方法局限于显式文本空间，通过语义相似度检索并拼接经验到上下文，导致大量token开销且检索与生成相互解耦。本文提出ExpWeaver，利用大模型自身隐状态编码经验，在解码每一步于潜在空间直接检索相关经验并融入生成，无需独立RAG模块。该方法降低了开销并提升了经验复用效率，为智能体经验学习提供了新架构。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有经验学习方法局限于显式文本空间，检索拼接带来高token开销且检索与生成解耦。
method: 提出ExpWeaver，用大模型隐状态编码经验，在潜在空间逐解码步检索并融合经验，无需独立RAG模块。
result: 该框架在降低token开销的同时实现检索与生成一体化，提升了智能体规划与推理的经验复用效果。
conclusion: 潜在空间经验检索为智能体记忆与经验学习提供了高效新范式。
---

## Abstract
Experience learning has achieved promising results in enhancing LLM agent planning and reasoning by integrating past interactions as reusable knowledge. However, existing methods remain confined to explicit text space—retrieving experiences via semantic similarity and concatenating them into the context window, leading to substantial token overhead and a decoupled architecture that separates retrieval from generation. To address these limitations, we propose ExpWeaver, a framework that enables LLM agents to learn from experience via latent retrieval-augmented generation, without requiring a separate RAG module. ExpWeaver encodes experiences using the LLM’s own hidden states, retrieves relevant experiences directly in latent space at each decoding step, and integrates them through cross-attention aggregation and gated residual mechanisms. The entire pipeline is optimized end-to-end with reinforcement learning, supporting both generative and ranking tasks. We evaluate ExpWeaver on 13 diverse tasks spanning question answering, reasoning, coding, scientific prediction, and recommendation. Results demonstrate that: (1) ExpWeaver achieves state-of-the-art on 12 out of 13 tasks, outperforming the strongest baseline by over 6.8%; (2) ExpWeaver maintains token efficiency comparable to non-retrieval baselines while text-based retrieval methods require 1.5–2× more tokens; and (3) ExpWeaver exhibits superior cross-domain generalization, outperforming the strongest baseline by 16.32% under zero-shot transfer and 15.21% under few-shot transfer. Our code for ExpWeaver is released at https://github.com/ulab-uiuc/ExpWeaver.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
大模型智能体通过潜在检索存储经验来学习。

### 2. 核心内容
现有基于经验的智能体方法局限于显式文本空间，通过语义相似度检索并拼接经验到上下文，导致大量token开销且检索与生成相互解耦。本文提出ExpWeaver，利用大模型自身隐状态编码经验，在解码每一步于潜在空间直接检索相关经验并融入生成，无需独立RAG模块。该方法降低了开销并提升了经验复用效率，为智能体经验学习提供了新架构。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=4ARH5kZrgz](https://openreview.net/forum?id=4ARH5kZrgz)
