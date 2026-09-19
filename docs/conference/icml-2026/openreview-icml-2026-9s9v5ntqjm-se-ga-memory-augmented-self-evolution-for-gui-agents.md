---
title: "SE-GA: Memory-Augmented Self-Evolution for GUI Agents"
title_zh: SE-GA：面向GUI智能体的记忆增强自演化
authors: "Shilong Jin, Lanjun Wang, Zhuosheng Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/08ac4b5e4ff21fb40631ba5b306f6542c6784e16.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 具备情景与语义记忆检索的记忆增强自演化GUI智能体
tldr: 自主GUI智能体在多步任务中受限于上下文窗口和静态策略，难以适应动态环境。本文提出SE-GA自演化GUI智能体框架，将分层记忆结构与迭代自改进机制结合。核心的测试时记忆扩展（TTME）在推理时动态检索情景、语义与经验记忆以支持长期规划，记忆增强自演化（MASE）利用收集数据持续训练。该工作为交互式智能体的长期记忆与持续学习提供了完整方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 自主GUI智能体受限于上下文窗口与静态策略，难以应对多步任务与动态环境。
method: 提出SE-GA框架，结合分层记忆、测试时记忆扩展TTME与记忆增强自演化MASE训练流程。
result: 在推理时动态检索情景、语义与经验记忆以支持长期规划并持续提升策略。
conclusion: 为交互式GUI智能体提供长期记忆检索与持续学习的一体化框架。
---

## Abstract
Autonomous Graphical User Interface (GUI) agents often struggle with multi-step tasks due to constrained context windows and static policies that fail to adapt to dynamic environments. To address these limitations, this work proposes the Self-Evolving GUI Agent (SE-GA), a novel framework that integrates hierarchical memory structures with an iterative self-improvement mechanism.  At the core of our approach is Test-Time Memory Extension (TTME), which facilitates long-term planning by dynamically retrieving episodic, semantic, and experiential memories to provide salient contexts during inference. To ensure continuous learning, we introduce Memory-Augmented Self-Evolution (MASE), which is a training pipeline that adopts the data collected by TTME to stabilize and enhance the agent's foundational policy. Extensive evaluations across both offline and online benchmarks demonstrate SE-GA achieves state-of-the-art performance, reaching success rates of 89.0\% on ScreenSpot and 75.8\% on the challenging AndroidControl-High dataset. Furthermore, significant improvements on the AndroidWorld benchmark highlight the superior generalization to dynamic environments.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
具备情景与语义记忆检索的记忆增强自演化GUI智能体。

### 2. 核心内容
自主GUI智能体在多步任务中受限于上下文窗口和静态策略，难以适应动态环境。本文提出SE-GA自演化GUI智能体框架，将分层记忆结构与迭代自改进机制结合。核心的测试时记忆扩展（TTME）在推理时动态检索情景、语义与经验记忆以支持长期规划，记忆增强自演化（MASE）利用收集数据持续训练。该工作为交互式智能体的长期记忆与持续学习提供了完整方案。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=9S9V5ntQJM](https://openreview.net/forum?id=9S9V5ntQJM)
