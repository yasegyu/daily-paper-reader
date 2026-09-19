---
title: "ParamMem: Augmenting Language Agents with Parametric Reflective Memory"
title_zh: ParamMem：以参数化反思记忆增强语言智能体
authors: "Tianjun Yao, Yongqiang Chen, Yujia Zheng, Pan Li, Zhiqiang Shen, Kun Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/a8f8d44c9fbeda54d0be37feb00e39fa531c146f.pdf"
tags: ["query:agent-memory"]
score: 8.0
evidence: 为语言智能体存储反思模式的参数化反思记忆模块
tldr: 针对语言智能体自反思常产生重复输出、限制推理性能的问题，本文发现反思多样性与任务成功率强正相关，提出ParamMem参数化记忆模块，将跨样本反思模式编码进模型参数，并通过温度控制采样生成多样化反思。基于该模块构建的ParamAgent反思式智能体框架进一步整合这些信号，显著提升推理表现，为智能体记忆增强提供了参数化存储与检索的新思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 语言智能体自反思易产生重复输出，限制推理性能，且缺乏多样反思信号。
method: 提出参数化记忆模块ParamMem，将跨样本反思模式编码进模型参数并温度采样生成多样反思。
result: 基于该模块的ParamAgent框架提升了反思多样性与任务成功率。
conclusion: 为语言智能体提供参数化记忆存储与检索机制，改善迭代推理的多样性。
---

## Abstract
Self-reflection enables language agents to iteratively refine solutions, yet often produces repetitive outputs that limit reasoning performance. Recent studies have attempted to address this limitation through various approaches, among which increasing reflective diversity has shown promise. Our empirical analysis reveals a strong positive correlation between reflective diversity and task success, further motivating the need for diverse reflection signals. We introduce `ParamMem`, a parametric memory module that encodes cross-sample reflection patterns into model parameters, enabling diverse reflection generation through temperature-controlled sampling. Building on this module, we propose ParamAgent, a reflection-based agent framework that integrates parametric memory with episodic and cross-sample memory. Extensive experiments on code generation, mathematical reasoning, and multi-hop question answering demonstrate consistent improvements over state-of-the-art baselines. Further analysis reveals that `ParamMem` is sample-efficient, enables weak-to-strong transfer across model scales, and supports self-improvement without reliance on stronger external model, highlighting the potential of `ParamMem` as an effective component for enhancing language agents.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
为语言智能体存储反思模式的参数化反思记忆模块。

### 2. 核心内容
针对语言智能体自反思常产生重复输出、限制推理性能的问题，本文发现反思多样性与任务成功率强正相关，提出ParamMem参数化记忆模块，将跨样本反思模式编码进模型参数，并通过温度控制采样生成多样化反思。基于该模块构建的ParamAgent反思式智能体框架进一步整合这些信号，显著提升推理表现，为智能体记忆增强提供了参数化存储与检索的新思路。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=tNosQdV9J1](https://openreview.net/forum?id=tNosQdV9J1)
