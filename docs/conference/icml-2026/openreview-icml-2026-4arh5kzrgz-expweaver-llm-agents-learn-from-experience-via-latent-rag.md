---
title: "ExpWeaver: LLM Agents Learn from Experience via Latent RAG"
title_zh: ExpWeaver：大模型智能体通过潜在RAG从经验中学习
authors: "Tao Feng, Tianyang Luo, Jingjun Xu, Zhigang Hua, Yan Xie, Shuang Yang, Ge Liu, Jiaxuan You"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/868299e3b83f82e8c4c8baa5f861219b70cb2ec8.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 大模型智能体通过潜在检索增强生成从经验中学习
tldr: 该文针对智能体经验学习中显式文本检索语义相似经验并拼接进上下文所带来的token开销大、检索与生成解耦的问题，提出ExpWeaver框架。它用大模型自身隐状态编码经验，在每个解码步于潜在空间直接检索相关经验并融合，无需独立RAG模块。该潜在记忆机制提升了智能体规划推理的经验复用效率。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有经验学习依赖显式文本检索与拼接，token开销大且检索生成解耦。
method: 提出ExpWeaver，用隐状态编码经验并在解码步于潜在空间检索融合。
result: 无需独立RAG模块即可高效复用过往经验提升规划推理。
conclusion: 为记忆增强智能体的经验存储与检索提供潜在空间新方案。
---

## Abstract
Experience learning has achieved promising results in enhancing LLM agent planning and reasoning by integrating past interactions as reusable knowledge. However, existing methods remain confined to explicit text space—retrieving experiences via semantic similarity and concatenating them into the context window, leading to substantial token overhead and a decoupled architecture that separates retrieval from generation. To address these limitations, we propose ExpWeaver, a framework that enables LLM agents to learn from experience via latent retrieval-augmented generation, without requiring a separate RAG module. ExpWeaver encodes experiences using the LLM’s own hidden states, retrieves relevant experiences directly in latent space at each decoding step, and integrates them through cross-attention aggregation and gated residual mechanisms. The entire pipeline is optimized end-to-end with reinforcement learning, supporting both generative and ranking tasks. We evaluate ExpWeaver on 13 diverse tasks spanning question answering, reasoning, coding, scientific prediction, and recommendation. Results demonstrate that: (1) ExpWeaver achieves state-of-the-art on 12 out of 13 tasks, outperforming the strongest baseline by over 6.8%; (2) ExpWeaver maintains token efficiency comparable to non-retrieval baselines while text-based retrieval methods require 1.5–2× more tokens; and (3) ExpWeaver exhibits superior cross-domain generalization, outperforming the strongest baseline by 16.32% under zero-shot transfer and 15.21% under few-shot transfer. Our code for ExpWeaver is released at https://github.com/ulab-uiuc/ExpWeaver.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
大模型智能体通过潜在检索增强生成从经验中学习。

### 2. 核心内容
该文针对智能体经验学习中显式文本检索语义相似经验并拼接进上下文所带来的token开销大、检索与生成解耦的问题，提出ExpWeaver框架。它用大模型自身隐状态编码经验，在每个解码步于潜在空间直接检索相关经验并融合，无需独立RAG模块。该潜在记忆机制提升了智能体规划推理的经验复用效率。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=4ARH5kZrgz](https://openreview.net/forum?id=4ARH5kZrgz)
