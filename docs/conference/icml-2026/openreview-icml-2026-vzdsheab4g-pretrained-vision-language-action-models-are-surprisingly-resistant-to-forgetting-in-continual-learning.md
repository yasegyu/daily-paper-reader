---
title: Pretrained Vision-Language-Action Models are Surprisingly Resistant to Forgetting in Continual Learning
title_zh: 预训练视觉-语言-动作模型在持续学习中出人意料地抗遗忘
authors: "Huihan Liu, Changyeon Kim, Bo Liu, Minghuan Liu, Yuke Zhu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/f568ceca52aa63e540f2afda5a7a6cb3a2da988b.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 持续学习中的经验回放与抗遗忘
tldr: 持续学习是机器人策略学习的长期难题，需在习得新技能时避免灾难性遗忘，但以往研究多聚焦从零训练的小型行为克隆模型，对大规模预训练视觉-语言-动作模型的遗忘行为了解不足。本文发现预训练VLA模型对遗忘具有显著抵抗力，简单经验回放甚至能在小回放数据下实现零遗忘，并分析其背后原因。该结果为持续学习中的记忆回放策略提供了重要参考。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 大规模预训练VLA模型在持续学习中的遗忘行为尚未被充分研究。
method: 对比预训练VLA与从零训练模型，并测试简单经验回放策略的效果。
result: 发现VLA显著抗遗忘，小规模经验回放即可实现近乎零遗忘。
conclusion: 为机器人持续学习中的记忆回放策略提供了新见解。
---

## Abstract
Continual learning is a long-standing challenge in robot policy learning, where a policy must acquire new skills over time without catastrophically forgetting previously learned ones. While prior work has extensively studied continual learning in relatively small behavior cloning (BC) policy models trained from scratch, its behavior in modern large-scale pretrained Vision-Language-Action (VLA) models remains underexplored. In this work, we find that pretrained VLAs are remarkably resistant to forgetting compared with smaller policy models trained from scratch. Simple Experience Replay (ER) works surprisingly well on VLAs, sometimes achieving zero forgetting even with a small replay data size. Our analysis reveals that pretraining plays a critical role in downstream continual learning performance: large pretrained models mitigate forgetting with a small replay buffer size while maintaining strong forward learning capabilities. Furthermore, we find that VLAs can retain relevant knowledge from prior tasks despite performance degradation during learning new tasks. This knowledge retention enables rapid recovery of seemingly forgotten skills through finetuning. Together, these insights imply that large-scale pretraining fundamentally changes the dynamics of continual learning, enabling models to continually acquire new skills over time with simple replay.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
持续学习中的经验回放与抗遗忘。

### 2. 核心内容
持续学习是机器人策略学习的长期难题，需在习得新技能时避免灾难性遗忘，但以往研究多聚焦从零训练的小型行为克隆模型，对大规模预训练视觉-语言-动作模型的遗忘行为了解不足。本文发现预训练VLA模型对遗忘具有显著抵抗力，简单经验回放甚至能在小回放数据下实现零遗忘，并分析其背后原因。该结果为持续学习中的记忆回放策略提供了重要参考。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=VzdSHEab4G](https://openreview.net/forum?id=VzdSHEab4G)
