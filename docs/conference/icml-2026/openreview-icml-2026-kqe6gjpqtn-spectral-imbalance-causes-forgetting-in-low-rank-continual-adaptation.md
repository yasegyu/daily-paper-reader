---
title: Spectral Imbalance Causes Forgetting in Low-Rank Continual Adaptation
title_zh: 谱不平衡导致低秩持续适配中的遗忘
authors: "Hao Gu, Mao-Lin Luo, Zi-Hao Zhou, Han-Chen Zhang, Min-Ling Zhang, Tong Wei"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/f53ed7c3d2434c97bc9e62ace5284761b332ecc7.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 从谱不平衡角度研究持续学习中的遗忘
tldr: 该文针对参数高效持续学习中的灾难性遗忘问题，指出低秩适配的奇异值谱高度不平衡，少数主导分量吸收大部分适配能量，从而更易破坏已学知识并受后续任务干扰。作者提出显式平衡各分量的解耦方法以自然保留旧知识。研究揭示了遗忘的结构性成因，为持续学习智能体的记忆保持提供了新视角。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有持续学习方法多关注避免干扰，却忽视何种更新属性可自然保留旧知识。
method: 从知识分解视角分析低秩适配的奇异值谱，并提出解耦以显式平衡各分量。
result: 发现谱不平衡与遗忘及后续干扰强相关，平衡后能更好保留历史知识。
conclusion: 为持续学习智能体的抗遗忘记忆机制提供了可迁移的结构性准则。
---

## Abstract
Parameter-efficient continual learning aims to adapt pre-trained models to sequential tasks without forgetting previously acquired knowledge. Most existing approaches treat continual learning as avoiding interference with past updates, rather than considering what properties make the current task-specific update naturally preserve previously acquired knowledge.
From a knowledge-decomposition perspective, we observe that low-rank adaptations exhibit highly imbalanced singular value spectra: a few dominant components absorb most of the adaptation energy, thereby (i) more likely to disrupt previously acquired knowledge and (ii) making the update more vulnerable to interference from subsequent tasks.
To enable explicit balance among components, we decouple the *magnitude* of the task update from its *directional structure* and formulate it as a constrained optimization problem on a restricted Stiefel manifold.
We address this problem using a projected first-order method compatible with standard deep-learning optimizers used in vision-language models.
Our method mitigates both backward and forward forgetting, consistently outperforming continual learning baselines. Source code is available in supplementary material.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
从谱不平衡角度研究持续学习中的遗忘。

### 2. 核心内容
该文针对参数高效持续学习中的灾难性遗忘问题，指出低秩适配的奇异值谱高度不平衡，少数主导分量吸收大部分适配能量，从而更易破坏已学知识并受后续任务干扰。作者提出显式平衡各分量的解耦方法以自然保留旧知识。研究揭示了遗忘的结构性成因，为持续学习智能体的记忆保持提供了新视角。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=kqE6GjpQTn](https://openreview.net/forum?id=kqE6GjpQTn)
