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
evidence: 为GUI智能体检索情景语义经验记忆的层次记忆
tldr: 自主GUI智能体因上下文窗口受限和策略静态，难以应对多步任务。作者提出自演化GUI智能体SE-GA，将层次化记忆结构与迭代自改进机制结合。其核心测试时记忆扩展TTME在推理时动态检索情景、语义与经验记忆，为长期规划提供显著上下文，并配记忆增强自演化训练管线持续学习。该方法提升了GUI智能体在动态环境中的多步任务表现。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 自主GUI智能体受限于上下文窗口和静态策略，难以适应动态环境中的多步任务。
method: 提出SE-GA框架，结合层次化记忆与迭代自改进，用测试时记忆扩展动态检索情景、语义和经验记忆，并配记忆增强自演化训练。
result: 该记忆增强机制为长期规划提供显著上下文并支持持续学习，提升了GUI智能体在多步任务中的表现。
conclusion: 表明层次化记忆检索结合自演化训练可有效增强GUI智能体的长程决策能力。
---

## Abstract
Autonomous Graphical User Interface (GUI) agents often struggle with multi-step tasks due to constrained context windows and static policies that fail to adapt to dynamic environments. To address these limitations, this work proposes the Self-Evolving GUI Agent (SE-GA), a novel framework that integrates hierarchical memory structures with an iterative self-improvement mechanism.  At the core of our approach is Test-Time Memory Extension (TTME), which facilitates long-term planning by dynamically retrieving episodic, semantic, and experiential memories to provide salient contexts during inference. To ensure continuous learning, we introduce Memory-Augmented Self-Evolution (MASE), which is a training pipeline that adopts the data collected by TTME to stabilize and enhance the agent's foundational policy. Extensive evaluations across both offline and online benchmarks demonstrate SE-GA achieves state-of-the-art performance, reaching success rates of 89.0\% on ScreenSpot and 75.8\% on the challenging AndroidControl-High dataset. Furthermore, significant improvements on the AndroidWorld benchmark highlight the superior generalization to dynamic environments.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
为GUI智能体检索情景语义经验记忆的层次记忆。

### 2. 核心内容
自主GUI智能体因上下文窗口受限和策略静态，难以应对多步任务。作者提出自演化GUI智能体SE-GA，将层次化记忆结构与迭代自改进机制结合。其核心测试时记忆扩展TTME在推理时动态检索情景、语义与经验记忆，为长期规划提供显著上下文，并配记忆增强自演化训练管线持续学习。该方法提升了GUI智能体在动态环境中的多步任务表现。

### 3. 对应检索需求
Search for papers about long term memory, episodic memory, and memory retrieval in interactive agent systems.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=9S9V5ntQJM](https://openreview.net/forum?id=9S9V5ntQJM)
