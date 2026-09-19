---
title: Pretrained Vision-Language-Action Models are Surprisingly Resistant to Forgetting in Continual Learning
title_zh: 预训练视觉-语言-动作模型在持续学习中出乎意料地抗遗忘
authors: "Huihan Liu, Changyeon Kim, Bo Liu, Minghuan Liu, Yuke Zhu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/f568ceca52aa63e540f2afda5a7a6cb3a2da988b.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 持续学习中经验回放的抗遗忘研究
tldr: 持续学习要求机器人在习得新技能时避免灾难性遗忘旧技能，但既有研究多针对从零训练的小型行为克隆策略，对大规模预训练VLA模型的行为尚不清楚。本文发现预训练VLA模型对遗忘具有显著鲁棒性，简单的经验回放即可在少量回放数据下实现近乎零遗忘，并分析其内在原因。该发现为持续学习智能体的记忆与遗忘管理提供新见解。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 持续学习中预训练VLA模型是否如小模型般易遗忘尚未被充分研究。
method: 系统对比预训练VLA与从零训练策略的持续学习表现，并测试经验回放效果。
result: 预训练VLA对遗忘高度鲁棒，简单经验回放在少量数据下近乎零遗忘。
conclusion: 为持续学习智能体的记忆与遗忘管理提供新认识。
---

## Abstract
Continual learning is a long-standing challenge in robot policy learning, where a policy must acquire new skills over time without catastrophically forgetting previously learned ones. While prior work has extensively studied continual learning in relatively small behavior cloning (BC) policy models trained from scratch, its behavior in modern large-scale pretrained Vision-Language-Action (VLA) models remains underexplored. In this work, we find that pretrained VLAs are remarkably resistant to forgetting compared with smaller policy models trained from scratch. Simple Experience Replay (ER) works surprisingly well on VLAs, sometimes achieving zero forgetting even with a small replay data size. Our analysis reveals that pretraining plays a critical role in downstream continual learning performance: large pretrained models mitigate forgetting with a small replay buffer size while maintaining strong forward learning capabilities. Furthermore, we find that VLAs can retain relevant knowledge from prior tasks despite performance degradation during learning new tasks. This knowledge retention enables rapid recovery of seemingly forgotten skills through finetuning. Together, these insights imply that large-scale pretraining fundamentally changes the dynamics of continual learning, enabling models to continually acquire new skills over time with simple replay.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
持续学习中经验回放的抗遗忘研究。

### 2. 核心内容
持续学习要求机器人在习得新技能时避免灾难性遗忘旧技能，但既有研究多针对从零训练的小型行为克隆策略，对大规模预训练VLA模型的行为尚不清楚。本文发现预训练VLA模型对遗忘具有显著鲁棒性，简单的经验回放即可在少量回放数据下实现近乎零遗忘，并分析其内在原因。该发现为持续学习智能体的记忆与遗忘管理提供新见解。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=VzdSHEab4G](https://openreview.net/forum?id=VzdSHEab4G)
