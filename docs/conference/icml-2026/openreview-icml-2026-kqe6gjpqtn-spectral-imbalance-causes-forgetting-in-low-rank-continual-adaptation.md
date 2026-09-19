---
title: Spectral Imbalance Causes Forgetting in Low-Rank Continual Adaptation
title_zh: 谱不平衡导致低秩持续适应中的遗忘
authors: "Hao Gu, Mao-Lin Luo, Zi-Hao Zhou, Han-Chen Zhang, Min-Ling Zhang, Tong Wei"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/f53ed7c3d2434c97bc9e62ace5284761b332ecc7.pdf"
tags: ["query:agent-memory"]
score: 4.0
evidence: 从谱不平衡角度分析持续适应中的遗忘
tldr: 参数高效持续学习需在适应新任务时避免遗忘旧知识，但现有方法多只关注避免干扰而非分析更新为何能保留知识。作者从知识分解视角发现低秩适应存在奇异值谱高度不平衡的问题，主导成分易破坏旧知识并受后续任务干扰。据此提出显式平衡各成分的方法以缓解遗忘。该研究为持续学习中的遗忘机制提供了理论解释，但与智能体记忆架构关联较弱。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有参数高效持续学习只关注避免干扰旧更新，未分析当前任务更新为何能自然保留既有知识。
method: 从知识分解角度发现低秩适应的奇异值谱高度不平衡，据此解耦并显式平衡各成分以缓解遗忘。
result: 分析表明主导成分易破坏旧知识并受后续任务干扰，平衡后能更好保留既有知识、减轻遗忘。
conclusion: 为持续学习中的遗忘成因提供了谱视角解释，并给出缓解遗忘的成分平衡策略。
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
从谱不平衡角度分析持续适应中的遗忘。

### 2. 核心内容
参数高效持续学习需在适应新任务时避免遗忘旧知识，但现有方法多只关注避免干扰而非分析更新为何能保留知识。作者从知识分解视角发现低秩适应存在奇异值谱高度不平衡的问题，主导成分易破坏旧知识并受后续任务干扰。据此提出显式平衡各成分的方法以缓解遗忘。该研究为持续学习中的遗忘机制提供了理论解释，但与智能体记忆架构关联较弱。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=kqE6GjpQTn](https://openreview.net/forum?id=kqE6GjpQTn)
