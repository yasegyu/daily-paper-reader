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
score: 5.0
evidence: 持续学习中的灾难性遗忘
tldr: 针对神经网络顺序训练时的灾难性遗忘问题，本文将持续学习重构为控制问题，让学习信号与保持信号在神经活动动态中竞争。方法将正则惩罚转化为保护先验任务表征的保持信号，通过最小化整合新任务的控制代价来更新权重。实验表明该框架能恢复真实的先验任务曲率，无需显式存储曲率即可保护旧任务表征。其贡献在于提出continual-natural gradient概念，为持续学习中的遗忘抑制提供新的控制论视角。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 神经网络顺序训练时存在灾难性遗忘，需要在新任务学习与旧任务保持之间取得平衡。
method: 将持续学习重构为控制问题，把正则惩罚转化为保持信号，通过最小化整合新任务的控制代价来更新权重。
result: 实验证明该方法能恢复真实的先验任务曲率，无需显式存储曲率即可保护旧任务表征。
conclusion: 提出continual-natural gradient概念，为持续学习中的遗忘抑制提供了新的控制论视角。
---

## Abstract
Catastrophic forgetting remains a fundamental challenge for neural networks when tasks are trained sequentially. In this work, we reformulate continual learning as a control problem where learning and preservation signals compete within neural activity dynamics. We convert regularization penalties into preservation signals that protect prior-task representations. Learning then proceeds by minimizing the control effort required to integrate new tasks while competing with the preservation of prior tasks. At equilibrium, the neural activities produce weight updates that implicitly encode the full prior-task curvature, a property we term the *continual-natural gradient*, requiring no explicit curvature storage. Experiments confirm that our learning framework recovers true prior-task curvature and enables task discrimination, outperforming existing methods on standard benchmarks without replay.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
持续学习中的灾难性遗忘。

### 2. 核心内容
针对神经网络顺序训练时的灾难性遗忘问题，本文将持续学习重构为控制问题，让学习信号与保持信号在神经活动动态中竞争。方法将正则惩罚转化为保护先验任务表征的保持信号，通过最小化整合新任务的控制代价来更新权重。实验表明该框架能恢复真实的先验任务曲率，无需显式存储曲率即可保护旧任务表征。其贡献在于提出continual-natural gradient概念，为持续学习中的遗忘抑制提供新的控制论视角。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=ix1HdZkO8U](https://openreview.net/forum?id=ix1HdZkO8U)
