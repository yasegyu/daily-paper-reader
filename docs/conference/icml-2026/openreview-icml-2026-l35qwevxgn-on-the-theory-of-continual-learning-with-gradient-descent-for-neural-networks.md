---
title: On the Theory of Continual Learning with Gradient Descent for Neural Networks
title_zh: 论神经网络中基于梯度下降的持续学习理论
authors: "Hossein Taheri, Avishek Ghosh, Arya Mazumdar"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/fd3610d002a5b4ac50afa73945ce7902a9e6cb2b.pdf"
tags: ["query:agent-memory"]
score: 5.0
evidence: 梯度下降持续学习中的遗忘理论分析
tldr: 持续学习要求模型在适应新任务的同时不遗忘旧任务，但其内在机制仍不清晰。本文在可解析且具代表性的设定下研究其局限，分析单隐层二次神经网络在带高斯噪声的XOR簇数据序列上经梯度下降训练的动态。通过对训练损失梯度下降动态的紧致刻画，作者给出了训练时遗忘率关于迭代次数、样本量与任务数的显式界。该结果为理解持续学习与灾难性遗忘提供理论工具，但未涉及智能体记忆管理。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 持续学习希望模型适应新任务而不遗忘旧任务，但其内在机制与遗忘成因仍缺乏理论理解。
method: 在单隐层二次网络、XOR簇正交均值序列设定下，对梯度下降训练损失动态进行紧致刻画并推导遗忘率界。
result: 给出了训练时遗忘率关于迭代次数、样本规模和任务数量的显式上界。
conclusion: 为持续学习与灾难性遗忘提供理论刻画，但聚焦神经网络训练而非智能体记忆管理。
---

## Abstract
Continual learning, the ability of a model to adapt to an ongoing sequence of tasks without forgetting earlier ones, is a central goal of artificial intelligence. To better understand its underlying mechanisms, we study the limitations of continual learning in a tractable yet representative setting. Specifically, we analyze one-hidden-layer quadratic neural networks trained by gradient descent on a sequence of XOR-cluster datasets with Gaussian noise, where different tasks correspond to clusters with orthogonal means. Our analysis is based on a tight characterization of gradient descent dynamics for the training loss, which yields explicit bounds on the rate of train-time forgetting as functions of the number of iterations, sample size, number of tasks, and hidden-layer width. We then leverage an algorithmic stability framework to bound the generalization gap, leading to corresponding guarantees on test-time forgetting. Together, our results provide the first closed-form  guarantees for forgetting in continual learning with neural networks and show how key problem parameters jointly govern forgetting dynamics. Numerical experiments corroborate our theoretical results.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
梯度下降持续学习中的遗忘理论分析。

### 2. 核心内容
持续学习要求模型在适应新任务的同时不遗忘旧任务，但其内在机制仍不清晰。本文在可解析且具代表性的设定下研究其局限，分析单隐层二次神经网络在带高斯噪声的XOR簇数据序列上经梯度下降训练的动态。通过对训练损失梯度下降动态的紧致刻画，作者给出了训练时遗忘率关于迭代次数、样本量与任务数的显式界。该结果为理解持续学习与灾难性遗忘提供理论工具，但未涉及智能体记忆管理。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=l35QweVxgn](https://openreview.net/forum?id=l35QweVxgn)
