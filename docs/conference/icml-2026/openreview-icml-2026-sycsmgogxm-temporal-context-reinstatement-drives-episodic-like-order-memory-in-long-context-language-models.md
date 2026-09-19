---
title: Temporal Context Reinstatement Drives Episodic-Like Order Memory in Long-Context Language Models
title_zh: 时序上下文重现驱动长上下文语言模型中的类情景顺序记忆
authors: "Mathis Pink, Vy A. Vo, Qinyuan Wu, Jianing Mu, Javier S. Turek, Uri Hasson, Kenneth A. Norman, Sebastian Michelmann, Alexander Huth, Mariya Toneva"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/ee942a26e9217a4f9faaf37d194b774c0ede18f1.pdf"
tags: ["query:agent-memory"]
score: 8.0
evidence: 长上下文语言模型中类情景记忆的时序机制
tldr: 人类情景记忆能检索跨越长时间跨度的经历，但其计算机制因长期记忆实验难以观测而存在争议。本文利用长上下文LLM开展时序顺序记忆任务，基于对整部长篇小说的记忆构建人类行为数据集。结果显示模型表现出与人类相同的距离效应，并通过长上下文机制分析揭示时序上下文重现的驱动作用。该工作为情景记忆的计算机制研究提供了可解释的模型视角。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 人类情景记忆的检索计算机制难以直接观测，长上下文语言模型提供了可分析的研究途径。
method: 构建基于整部长篇小说记忆的人类行为数据集，在LLM上进行时序顺序记忆任务与机制分析。
result: 模型呈现与人类一致的距离效应，机制分析显示时序上下文重现驱动该现象。
conclusion: 揭示长上下文语言模型中的类情景记忆机制，为记忆研究提供计算视角。
---

## Abstract
Human episodic memory supports the retrieval of experiences that unfold over extended timescales, yet the computational mechanisms underlying this ability remain debated due to the limited mechanistic accessibility in long-term memory experiments in humans. Long-context LLMs may offer promising ways to reveal plausible computational mechanisms that drive this type of retrieval. Here, we investigate whether and how LLMs capture the core behavioral signatures of episodic memory via a temporal order memory task. Using a new dataset of human behavior based on memory of a full-length novel, we show that models exhibit the same characteristic distance effect observed in humans on this task. We next apply long-context mechanistic interpretability analyses to uncover how models solve this task, and find that model performance relies on a one-dimensional temporal code that is reinstated during retrieval by a single time-reinstatement attention head. These findings support temporal context reinstatement as an important mechanism for episodic-like temporal-order memory in LLMs, offering new insights into how temporal aspects of long-term episodic memory may be instantiated in both artificial and biological systems.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
长上下文语言模型中类情景记忆的时序机制。

### 2. 核心内容
人类情景记忆能检索跨越长时间跨度的经历，但其计算机制因长期记忆实验难以观测而存在争议。本文利用长上下文LLM开展时序顺序记忆任务，基于对整部长篇小说的记忆构建人类行为数据集。结果显示模型表现出与人类相同的距离效应，并通过长上下文机制分析揭示时序上下文重现的驱动作用。该工作为情景记忆的计算机制研究提供了可解释的模型视角。

### 3. 对应检索需求
Search for papers about long term memory, episodic memory, and memory retrieval in interactive agent systems.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=sycSMgogxM](https://openreview.net/forum?id=sycSMgogxM)
