---
title: "Learning to Remember, Learn, and Forget in Attention-Based Models"
title_zh: 在注意力模型中学习记忆、学习与遗忘
authors: "Djohan Bonnet, Jamie Lohoff, Jan Finkbeiner, Elidona Shiqerukaj, Emre Neftci"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/9a79a2a42eb0b1afe145d390252558fac533a76e.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 通过元可塑性在注意力中学习记忆与遗忘
tldr: Transformer的上下文学习被视为在线联想记忆，但在门控线性注意力中该记忆容量固定且易受干扰，尤其对长序列。本文将上下文学习视为需处理稳定性-可塑性困境的持续学习问题，提出Palimpsa自注意力模型，采用贝叶斯元可塑性，将每个注意力状态的可塑性绑定到由先验分布锚定的重要性状态。研究表明多种门控线性注意力模型可作为其特例涌现，为记忆的保持与遗忘管理提供统一视角。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 门控线性注意力中上下文学习记忆容量固定且易受干扰，长序列尤甚。
method: 提出Palimpsa，用贝叶斯元可塑性将注意力状态可塑性绑定到重要性状态。
result: 在稳定性-可塑性间取得平衡，多种门控线性注意力作为特例涌现。
conclusion: 为注意力记忆的保持与遗忘管理提供统一理论视角。
---

## Abstract
In-Context Learning (ICL) in transformers acts as an online associative memory and is believed to underpin their high performance on complex sequence processing tasks. 
However, in gated linear attention models, this memory has a fixed capacity and is prone to interference, especially for long sequences. 
We propose Palimpsa, a self-attention model that views ICL as a continual learning problem that must address a stability-plasticity dilemma. 
Palimpsa uses Bayesian metaplasticity, where the plasticity of each attention state is tied to an importance state grounded by a prior distribution that captures accumulated knowledge. 
We demonstrate that various gated linear attention models emerge as specific architecture choices and posterior approximations, and that Mamba2 is a special case of Palimpsa where forgetting dominates. 
This theoretical link enables the transformation of any non-metaplastic model into a metaplastic one, significantly expanding its memory capacity.
Our experiments show that Palimpsa consistently outperforms baselines on the Multi-Query Associative Recall (MQAR) benchmark and on Commonsense Reasoning tasks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
通过元可塑性在注意力中学习记忆与遗忘。

### 2. 核心内容
Transformer的上下文学习被视为在线联想记忆，但在门控线性注意力中该记忆容量固定且易受干扰，尤其对长序列。本文将上下文学习视为需处理稳定性-可塑性困境的持续学习问题，提出Palimpsa自注意力模型，采用贝叶斯元可塑性，将每个注意力状态的可塑性绑定到由先验分布锚定的重要性状态。研究表明多种门控线性注意力模型可作为其特例涌现，为记忆的保持与遗忘管理提供统一视角。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=wKMV7mXjUr](https://openreview.net/forum?id=wKMV7mXjUr)
