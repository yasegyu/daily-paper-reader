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
score: 6.0
evidence: 上下文持续学习中的泛化与遗忘理论分析
tldr: 针对现有上下文学习理论多局限于单任务、无法解释提示中含异构任务序列时模型是否隐式持续学习的问题，本文提出首个上下文持续学习理论框架，建模预训练Transformer通过共享注意力在单条提示内处理多顺序任务的过程，针对线性与掩码线性自注意力推导泛化与遗忘的误差表达式。该工作揭示了推理阶段隐式持续学习中的遗忘机制，为面向持续学习智能体的记忆管理与遗忘研究提供理论支撑。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有上下文学习理论多研究单任务，无法解释提示含异构任务序列时是否隐式持续学习。
method: 提出首个上下文持续学习理论框架，建模Transformer在单提示内处理多顺序任务并推导误差式。
result: 针对线性与掩码线性自注意力给出泛化与遗忘的误差表达式，揭示隐式持续学习机制。
conclusion: 为面向持续学习智能体的遗忘与记忆管理研究提供了理论基础。
---

## Abstract
In-context learning (ICL) derives its power from enabling Large Language Models to adapt to new tasks via prompt-based reasoning alone, entirely bypassing the need for parameter updates. Existing theories primarily study ICL in single-task settings, while real-world prompts often contain sequences of heterogeneous tasks, leaving a gap in understanding whether Large Language Models implicitly perform continual learning during inference. To bridge this gap, we propose the first theoretical framework for in-context continual learning, modeling how a pretrained Transformer processes multiple sequential tasks within a single prompt through shared attention mechanisms. Focusing on linear and masked linear self-attention, we derive error expressions for model predictions under sequential task prompts and analyze their generalization and forgetting behavior. Our results reveal that standard attention mechanisms inevitably induce inter-task interference by uniformly or causally aggregating historical contexts, leading to systematic bias. We further provide a bias–variance–interference decomposition of prediction error, characterizing when historical in-context information yields positive transfer or provable negative transfer. This analysis exposes fundamental limits of attention-based continual inference and offers theoretical explanations for order sensitivity and performance degradation in long prompts.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
上下文持续学习中的泛化与遗忘理论分析。

### 2. 核心内容
针对现有上下文学习理论多局限于单任务、无法解释提示中含异构任务序列时模型是否隐式持续学习的问题，本文提出首个上下文持续学习理论框架，建模预训练Transformer通过共享注意力在单条提示内处理多顺序任务的过程，针对线性与掩码线性自注意力推导泛化与遗忘的误差表达式。该工作揭示了推理阶段隐式持续学习中的遗忘机制，为面向持续学习智能体的记忆管理与遗忘研究提供理论支撑。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=68AMoK2YNk](https://openreview.net/forum?id=68AMoK2YNk)
