---
title: Real-Time Detection and Quantitative Analysis of Spurious Forgetting in Continual Learning
title_zh: 持续学习中虚假遗忘的实时检测与定量分析
authors: Weiwei Wang
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/7bd73f44601c1b012cf30ede77fd894cea2d7ea0.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 持续学习中虚假遗忘的定量分析
tldr: 灾难性遗忘是大模型持续学习的核心难题，近期研究指出性能下降可能源于任务对齐被破坏的虚假遗忘，而非真实知识丢失，但此前工作仅定性描述且依赖事后分析。本文提出浅层与深层对齐框架，首次定量刻画对齐深度，并实现虚假遗忘的实时检测与自动区分。结果揭示了现有对齐方法存在浅层对齐问题，为持续学习中的遗忘诊断与记忆管理提供了新工具。
source: ICML-2026-Rejected-Public
selection_source: conference_retrieval
motivation: 大模型持续学习中的性能下降可能来自虚假遗忘，但缺乏定量刻画与自动区分手段。
method: 提出浅层与深层对齐框架，定量刻画对齐深度并实时检测虚假遗忘。
result: 实验发现现有对齐方法存在浅层对齐问题，导致输出层遗忘。
conclusion: 为持续学习中的遗忘诊断与记忆保持提供了量化分析框架。
---

## Abstract
Catastrophic forgetting remains a fundamental challenge in continual learning for large language models. Recent work revealed that performance degradation may stem from spurious forgetting caused by task alignment disruption rather than true knowledge loss. However, this foundational work left critical gaps: it only qualitatively describes alignment, relies on post-hoc analysis, and lacks automatic distinction mechanisms.

Key Contribution: We extend the previous work by introducing the shallow versus deep alignment framework, which provides the first quantitative characterization of alignment depth. We identify that current task alignment approaches suffer from shallow alignment—alignment is maintained only over the first few output tokens (approximately 3-5), making models vulnerable to forgetting. This shallow alignment explains why spurious forgetting occurs, why it is reversible, and why fine-tuning attacks are effective.

In this paper, we propose a comprehensive framework that addresses all gaps in the previous work: (1) quantitative metrics (0-1 scale) to measure alignment depth across token positions, addressing the qualitative-only limitation; (2) real-time detection methods for identifying shallow alignment and spurious forgetting during training, enabling early intervention; (3) specialized analysis tools for alignment depth visualization and recovery prediction; and (4) adaptive mitigation strategies that automatically distinguish forgetting types and promote deep alignment. Extensive experiments on multiple datasets and model architectures (Qwen2.5-3B to Qwen2.5-32B) demonstrate 86.2-90.6% identification accuracy and show that promoting deep alignment improves robustness against forgetting by 3.3-7.1% over baselines, including the fixed freezing strategy in the previous work.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
持续学习中虚假遗忘的定量分析。

### 2. 核心内容
灾难性遗忘是大模型持续学习的核心难题，近期研究指出性能下降可能源于任务对齐被破坏的虚假遗忘，而非真实知识丢失，但此前工作仅定性描述且依赖事后分析。本文提出浅层与深层对齐框架，首次定量刻画对齐深度，并实现虚假遗忘的实时检测与自动区分。结果揭示了现有对齐方法存在浅层对齐问题，为持续学习中的遗忘诊断与记忆管理提供了新工具。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Rejected-Public
- OpenReview：[https://openreview.net/forum?id=zMxbdbk4fM](https://openreview.net/forum?id=zMxbdbk4fM)
