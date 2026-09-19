---
title: "Learning to Remember, Learn, and Forget in Attention-Based Models"
title_zh: 在基于注意力的模型中学习记忆、学习与遗忘
authors: "Djohan Bonnet, Jamie Lohoff, Jan Finkbeiner, Elidona Shiqerukaj, Emre Neftci"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/9a79a2a42eb0b1afe145d390252558fac533a76e.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 从持续学习视角研究记忆的记与忘
tldr: Transformer的上下文学习被视为一种在线联想记忆，但门控线性注意力模型中该记忆容量固定且易受长序列干扰。本文提出Palimpsa，将上下文学习视为需处理稳定性-可塑性困境的持续学习问题，用贝叶斯元可塑性将每个注意力状态的可塑性与其重要度绑定。研究表明多种门控线性注意力模型可作为其特例，为记忆的保留与遗忘提供了统一建模视角。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 门控线性注意力模型的上下文记忆容量固定，长序列下易受干扰。
method: 提出Palimpsa，用贝叶斯元可塑性将注意力状态可塑性绑定重要度，把ICL建模为持续学习。
result: 多种门控线性注意力模型被证明是该方法的具体架构特例与后验近似。
conclusion: 为注意力模型中的记忆保持与遗忘提供了统一的持续学习框架。
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
从持续学习视角研究记忆的记与忘。

### 2. 核心内容
Transformer的上下文学习被视为一种在线联想记忆，但门控线性注意力模型中该记忆容量固定且易受长序列干扰。本文提出Palimpsa，将上下文学习视为需处理稳定性-可塑性困境的持续学习问题，用贝叶斯元可塑性将每个注意力状态的可塑性与其重要度绑定。研究表明多种门控线性注意力模型可作为其特例，为记忆的保留与遗忘提供了统一建模视角。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=wKMV7mXjUr](https://openreview.net/forum?id=wKMV7mXjUr)
