---
title: "AI Engram: In Search of Memory Traces in Artificial Intelligence"
title_zh: AI记忆印迹：在人工智能中寻找记忆痕迹
authors: "Jea Kwon, Dong-Kyum Kim, Jiwon Kim, Yonghyun Kim, Woong Kook, Meeyoung Cha"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/0f9a0557d49ba7165bc5060b9f2d89e480d4959c.pdf"
tags: ["query:agent-memory"]
score: 5.0
evidence: 神经网络中的记忆痕迹与擦除
tldr: 记忆形成是智能的基础，但深度神经网络是否像生物大脑那样保留可识别的记忆痕迹仍是未解问题。本文提出几何框架，将神经科学的特异性、再激活、充分性与必要性准则形式化为约束逆问题，推导出可从未缠结的全局参数中隔离单个记忆痕迹的闭式估计器。该解对应参数流形上的自然梯度更新，并支持通过线性算术组合或擦除任意记忆子集，为理解与操控人工网络记忆提供新工具。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 记忆形成是智能的基础，但深度神经网络是否保留类似生物记忆单元的可识别记忆痕迹仍是未解问题。
method: 提出几何框架，将神经科学的特异性、再激活、充分性与必要性准则形式化为约束逆问题，推导出闭式估计器以隔离单个记忆痕迹。
result: 该估计器与参数流形上的自然梯度更新对应，可对学得知识进行组合或擦除等外科手术式操作。
conclusion: 为理解与操控人工网络中的记忆痕迹提供统一框架。
---

## Abstract
Memory formation is fundamental to intelligence, yet whether deep neural networks preserve identifiable memory traces analogous to biological memory units remains an open question. This work introduces a geometric framework to identify such “AI engrams” by formalizing the neuroscientific criteria of specificity, reactivation, sufficiency, and necessity into a constrained inverse problem. We derive a closed-form estimator that isolates individual memory traces from globally entangled parameters, and show that this biologically-derived solution corresponds to a natural gradient update on the parameter manifold. AI engrams enable surgical manipulation of learned knowledge: any subset of memories can be composed or erased through linear arithmetic, without iterative optimization. Experiments ranging from simple MLPs to LLMs demonstrate the causal validity and substantial scalability of AI engrams. Together, these results bridge theories of biological memory and artificial representation learning and offer geometric insight into how deep networks simultaneously support functional specificity within distributed storage.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
神经网络中的记忆痕迹与擦除。

### 2. 核心内容
记忆形成是智能的基础，但深度神经网络是否像生物大脑那样保留可识别的记忆痕迹仍是未解问题。本文提出几何框架，将神经科学的特异性、再激活、充分性与必要性准则形式化为约束逆问题，推导出可从未缠结的全局参数中隔离单个记忆痕迹的闭式估计器。该解对应参数流形上的自然梯度更新，并支持通过线性算术组合或擦除任意记忆子集，为理解与操控人工网络记忆提供新工具。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=QZO3oby12w](https://openreview.net/forum?id=QZO3oby12w)
