---
title: Continual Learning through Control Minimization
title_zh: 通过控制最小化实现持续学习
authors: "Sander de Haan, Yassine Taoudi-Benchekroun, Pau Vilimelis Aceituno, Benjamin F Grewe"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/3313191f676007297de14b78bafe42ec4e8fd8c4.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 为对抗灾难性遗忘重构的持续学习
tldr: 灾难性遗忘是神经网络在顺序学习任务时面临的根本挑战。本文把持续学习重新表述为一个控制问题，让学习信号与保护信号在神经活动动力学中相互竞争，将正则惩罚转化为保护先前任务表示的保护信号，学习过程则通过最小化整合新任务所需的控制代价来进行。平衡时神经活动产生的权重更新可隐式编码完整的先验任务曲率，无需显式存储，实验验证该框架能恢复真实的先验信息，为持续学习提供了新视角。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 灾难性遗忘是神经网络顺序学习任务时的根本挑战。
method: 将持续学习重构为控制问题，把正则惩罚转化为保护先前任务表示的保护信号，通过最小化整合新任务所需的控制代价来学习。
result: 平衡时神经活动产生的权重更新隐式编码先前任务曲率，无需显式存储，实验验证其能恢复真实先验。
conclusion: 为持续学习提供无需曲率存储的新框架。
---

## Abstract
Catastrophic forgetting remains a fundamental challenge for neural networks when tasks are trained sequentially. In this work, we reformulate continual learning as a control problem where learning and preservation signals compete within neural activity dynamics. We convert regularization penalties into preservation signals that protect prior-task representations. Learning then proceeds by minimizing the control effort required to integrate new tasks while competing with the preservation of prior tasks. At equilibrium, the neural activities produce weight updates that implicitly encode the full prior-task curvature, a property we term the *continual-natural gradient*, requiring no explicit curvature storage. Experiments confirm that our learning framework recovers true prior-task curvature and enables task discrimination, outperforming existing methods on standard benchmarks without replay.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
为对抗灾难性遗忘重构的持续学习。

### 2. 核心内容
灾难性遗忘是神经网络在顺序学习任务时面临的根本挑战。本文把持续学习重新表述为一个控制问题，让学习信号与保护信号在神经活动动力学中相互竞争，将正则惩罚转化为保护先前任务表示的保护信号，学习过程则通过最小化整合新任务所需的控制代价来进行。平衡时神经活动产生的权重更新可隐式编码完整的先验任务曲率，无需显式存储，实验验证该框架能恢复真实的先验信息，为持续学习提供了新视角。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=ix1HdZkO8U](https://openreview.net/forum?id=ix1HdZkO8U)
