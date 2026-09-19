---
title: "ParamMem: Augmenting Language Agents with Parametric Reflective Memory"
title_zh: ParamMem：为语言智能体增强的参数化反思记忆
authors: "Tianjun Yao, Yongqiang Chen, Yujia Zheng, Pan Li, Zhiqiang Shen, Kun Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/a8f8d44c9fbeda54d0be37feb00e39fa531c146f.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 为语言智能体增强的参数化反思记忆模块
tldr: 自反思能让语言智能体迭代改进解，但常产生重复输出，限制推理性能，现有方法通过提升反思多样性来缓解。本文提出参数化记忆模块ParamMem，将跨样本的反思模式编码进模型参数，并通过温度控制采样生成多样化的反思信号。基于该模块构建的ParamAgent框架把反思记忆融入智能体推理流程。作者的分析显示反思多样性与任务成功率强正相关，表明参数化记忆是增强智能体经验利用的有效途径。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 语言智能体的自反思常产生重复输出，限制推理性能，而反思多样性与任务成功强相关。
method: 提出参数化记忆模块ParamMem，把跨样本反思模式编码进模型参数，用温度采样生成多样反思。
result: 基于该模块构建的ParamAgent框架通过提升反思多样性改善推理表现。
conclusion: 表明参数化记忆可作为智能体存储与复用经验的有效机制。
---

## Abstract
Self-reflection enables language agents to iteratively refine solutions, yet often produces repetitive outputs that limit reasoning performance. Recent studies have attempted to address this limitation through various approaches, among which increasing reflective diversity has shown promise. Our empirical analysis reveals a strong positive correlation between reflective diversity and task success, further motivating the need for diverse reflection signals. We introduce `ParamMem`, a parametric memory module that encodes cross-sample reflection patterns into model parameters, enabling diverse reflection generation through temperature-controlled sampling. Building on this module, we propose ParamAgent, a reflection-based agent framework that integrates parametric memory with episodic and cross-sample memory. Extensive experiments on code generation, mathematical reasoning, and multi-hop question answering demonstrate consistent improvements over state-of-the-art baselines. Further analysis reveals that `ParamMem` is sample-efficient, enables weak-to-strong transfer across model scales, and supports self-improvement without reliance on stronger external model, highlighting the potential of `ParamMem` as an effective component for enhancing language agents.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
为语言智能体增强的参数化反思记忆模块。

### 2. 核心内容
自反思能让语言智能体迭代改进解，但常产生重复输出，限制推理性能，现有方法通过提升反思多样性来缓解。本文提出参数化记忆模块ParamMem，将跨样本的反思模式编码进模型参数，并通过温度控制采样生成多样化的反思信号。基于该模块构建的ParamAgent框架把反思记忆融入智能体推理流程。作者的分析显示反思多样性与任务成功率强正相关，表明参数化记忆是增强智能体经验利用的有效途径。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=tNosQdV9J1](https://openreview.net/forum?id=tNosQdV9J1)
