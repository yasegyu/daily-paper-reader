---
title: Understanding Generalization and Forgetting in In-Context Continual Learning
title_zh: 理解上下文持续学习中的泛化与遗忘
authors: "Guangyu Li, Meng Ding, Lijie Hu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/7914b433f7acc55d3895d99b12a0db34a3f38b4d.pdf"
tags: ["query:agent-memory"]
score: 5.0
evidence: 上下文持续学习中泛化与遗忘的理论框架
tldr: 该文针对上下文学习理论多局限于单任务、而真实提示常包含异质任务序列的问题，提出首个上下文持续学习理论框架。作者建模预训练Transformer通过共享注意力在单个提示内处理多个顺序任务的过程，针对线性与掩码线性自注意力推导误差表达式，刻画泛化与遗忘条件。该理论为理解智能体推理时的隐式持续学习与遗忘提供基础。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有上下文学习理论多针对单任务，缺乏对提示内多任务序列遗忘的分析。
method: 构建上下文持续学习理论框架，对线性自注意力推导误差表达式。
result: 刻画了Transformer在单提示内处理顺序任务时的泛化与遗忘条件。
conclusion: 为推理阶段的隐式持续学习与遗忘提供理论解释。
---

## Abstract
In-context learning (ICL) derives its power from enabling Large Language Models to adapt to new tasks via prompt-based reasoning alone, entirely bypassing the need for parameter updates. Existing theories primarily study ICL in single-task settings, while real-world prompts often contain sequences of heterogeneous tasks, leaving a gap in understanding whether Large Language Models implicitly perform continual learning during inference. To bridge this gap, we propose the first theoretical framework for in-context continual learning, modeling how a pretrained Transformer processes multiple sequential tasks within a single prompt through shared attention mechanisms. Focusing on linear and masked linear self-attention, we derive error expressions for model predictions under sequential task prompts and analyze their generalization and forgetting behavior. Our results reveal that standard attention mechanisms inevitably induce inter-task interference by uniformly or causally aggregating historical contexts, leading to systematic bias. We further provide a bias–variance–interference decomposition of prediction error, characterizing when historical in-context information yields positive transfer or provable negative transfer. This analysis exposes fundamental limits of attention-based continual inference and offers theoretical explanations for order sensitivity and performance degradation in long prompts.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
上下文持续学习中泛化与遗忘的理论框架。

### 2. 核心内容
该文针对上下文学习理论多局限于单任务、而真实提示常包含异质任务序列的问题，提出首个上下文持续学习理论框架。作者建模预训练Transformer通过共享注意力在单个提示内处理多个顺序任务的过程，针对线性与掩码线性自注意力推导误差表达式，刻画泛化与遗忘条件。该理论为理解智能体推理时的隐式持续学习与遗忘提供基础。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=68AMoK2YNk](https://openreview.net/forum?id=68AMoK2YNk)
