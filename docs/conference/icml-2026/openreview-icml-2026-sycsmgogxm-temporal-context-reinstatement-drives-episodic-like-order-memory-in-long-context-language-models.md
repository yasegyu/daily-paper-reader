---
title: Temporal Context Reinstatement Drives Episodic-Like Order Memory in Long-Context Language Models
title_zh: 时间上下文重现驱动长上下文语言模型中的类情景顺序记忆
authors: "Mathis Pink, Vy A. Vo, Qinyuan Wu, Jianing Mu, Javier S. Turek, Uri Hasson, Kenneth A. Norman, Sebastian Michelmann, Alexander Huth, Mariya Toneva"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/ee942a26e9217a4f9faaf37d194b774c0ede18f1.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 长上下文语言模型中的类情景顺序记忆
tldr: 人类情景记忆能检索长时间跨度内的经历，但其计算机制因实验可及性有限而存争议。本文利用长上下文LLM探索这一机制，采用时间顺序记忆任务，并基于对整部长篇小说的记忆构建新数据集。实验显示模型表现出与人类一致的距离效应，随后作者应用长上下文机制可解释性方法分析其内部表征。该研究为情景记忆的计算机制提供了可检验的模型证据。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 人类情景记忆的计算机制因长期记忆实验可及性有限而存在争议，缺乏可操作的模型证据。
method: 利用长上下文LLM执行时间顺序记忆任务，并构建基于长篇小说的人类行为数据集进行机制可解释性分析。
result: 模型在任务上表现出与人类一致的距离效应，机制分析揭示了时间上下文重现的作用。
conclusion: 该研究说明长上下文LLM可作为研究情景记忆计算机制的有效平台。
---

## Abstract
Human episodic memory supports the retrieval of experiences that unfold over extended timescales, yet the computational mechanisms underlying this ability remain debated due to the limited mechanistic accessibility in long-term memory experiments in humans. Long-context LLMs may offer promising ways to reveal plausible computational mechanisms that drive this type of retrieval. Here, we investigate whether and how LLMs capture the core behavioral signatures of episodic memory via a temporal order memory task. Using a new dataset of human behavior based on memory of a full-length novel, we show that models exhibit the same characteristic distance effect observed in humans on this task. We next apply long-context mechanistic interpretability analyses to uncover how models solve this task, and find that model performance relies on a one-dimensional temporal code that is reinstated during retrieval by a single time-reinstatement attention head. These findings support temporal context reinstatement as an important mechanism for episodic-like temporal-order memory in LLMs, offering new insights into how temporal aspects of long-term episodic memory may be instantiated in both artificial and biological systems.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
长上下文语言模型中的类情景顺序记忆。

### 2. 核心内容
人类情景记忆能检索长时间跨度内的经历，但其计算机制因实验可及性有限而存争议。本文利用长上下文LLM探索这一机制，采用时间顺序记忆任务，并基于对整部长篇小说的记忆构建新数据集。实验显示模型表现出与人类一致的距离效应，随后作者应用长上下文机制可解释性方法分析其内部表征。该研究为情景记忆的计算机制提供了可检验的模型证据。

### 3. 对应检索需求
Search for papers about long term memory, episodic memory, and memory retrieval in interactive agent systems.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=sycSMgogxM](https://openreview.net/forum?id=sycSMgogxM)
