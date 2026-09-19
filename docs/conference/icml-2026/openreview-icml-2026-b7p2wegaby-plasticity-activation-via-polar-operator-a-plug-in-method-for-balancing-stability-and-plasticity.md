---
title: "Plasticity Activation via Polar Operator: A Plug-in Method for Balancing Stability and Plasticity"
title_zh: 通过极算子激活可塑性：平衡稳定性与可塑性的插件方法
authors: "Guodong Zheng, Enneng Yang, Xiaoyan Wang, Yihan Chen, Feihong He, Quan Zheng, Peng Wang, Li Shen"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/dfb62414a6d304c72686326392b46ef5fa65831b.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 平衡遗忘与可塑性的持续学习插件
tldr: 持续学习要求模型在学习新任务的同时避免灾难性遗忘，但许多缓解遗忘的方法通过约束参数更新而牺牲了可塑性。作者重新审视典型持续学习方法的梯度奇异值谱，发现普遍存在奇异值塌缩，仅少数梯度方向驱动更新。为此提出极算子可塑性激活插件PAPO，在保留抑制遗忘的主方向同时激活被压制的方向以增强可塑性，实验证明其能兼顾稳定性与可塑性。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 持续学习需学习新知识又避免灾难性遗忘，但许多抗遗忘方法限制参数更新，削弱了模型可塑性。
method: 作者分析梯度奇异值谱，发现奇异值塌缩现象，提出PAPO插件，保留抗遗忘主方向同时激活被抑制方向以增强可塑性。
result: 实验表明该方法在缓解遗忘的同时提升可塑性。
conclusion: 为持续学习提供平衡稳定性与可塑性的通用插件。
---

## Abstract
Continual learning (CL) seeks models that acquire new knowledge while avoiding catastrophic forgetting. However, many methods that mitigate forgetting constrain parameter updates and thereby reduce model plasticity. We revisit the singular value spectrum of gradients in representative CL methods and show that they commonly exhibit singular value collapse, where only a small subset of gradient directions drive parameter updates. Motivated by this observation, we propose **P**lasticity **A**ctivation via **P**olar **O**perator (PAPO), a plug-in that preserves the dominant directions that mitigate forgetting while activating previously suppressed directions to enhance plasticity. Concretely, PAPO modifies the gradient $\mathbf{G}$ as
$\mathbf{G}\leftarrow \mathbf{G}+\lambda \cdot \operatorname{polar}(\mathbf{G})$,
which uniformly increases near-zero singular values without changing the singular vectors. To avoid the cost of explicit singular value decomposition, we approximate the polar factor using the iteration-dependent Polar Express scheme, which relies only on matrix multiplications and additions. In our empirical evaluation on both vision and language benchmarks, incorporating PAPO yields consistent improvements. In particular, on MiniImageNet, integrating PAPO into ER, MAS, GPM and TRGP produces substantial accuracy gains of $9.01\%$, $4.76\%$, $8.90\%$ and $9.19\%$, respectively.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
平衡遗忘与可塑性的持续学习插件。

### 2. 核心内容
持续学习要求模型在学习新任务的同时避免灾难性遗忘，但许多缓解遗忘的方法通过约束参数更新而牺牲了可塑性。作者重新审视典型持续学习方法的梯度奇异值谱，发现普遍存在奇异值塌缩，仅少数梯度方向驱动更新。为此提出极算子可塑性激活插件PAPO，在保留抑制遗忘的主方向同时激活被压制的方向以增强可塑性，实验证明其能兼顾稳定性与可塑性。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=b7P2WegaBY](https://openreview.net/forum?id=b7P2WegaBY)
