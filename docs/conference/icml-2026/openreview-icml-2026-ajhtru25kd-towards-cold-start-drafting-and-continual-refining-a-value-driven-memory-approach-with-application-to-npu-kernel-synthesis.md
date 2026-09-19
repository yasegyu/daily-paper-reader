---
title: "Towards Cold-Start Drafting and Continual Refining: A Value-Driven Memory Approach with Application to NPU Kernel Synthesis"
title_zh: 面向冷启动草拟与持续精炼：一种价值驱动记忆方法及其在NPU内核合成中的应用
authors: "Yujie Zheng, Zhuo Li, Shengtao Zhang, Jiaqian Wang, Junjie Sheng, Junchi Yan, Weinan Zhang, Ying Wen, Bo Tang, Muning Wen"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/22928270cbb3cec9d649ad5a1a9275e1c4403016.pdf"
tags: ["query:agent-memory"]
score: 6.0
evidence: 基于价值驱动记忆的自演化智能体框架用于持续精炼
tldr: 在NPU等数据稀缺的编程领域，大模型受数据墙限制难以进行内核合成，性能较CUDA等数据丰富平台大幅下降。本文提出EvoKernel，将合成过程建模为基于记忆的强化学习任务，通过价值驱动记忆机制实现从初始草稿到持续精炼的自演化智能体流程，无需昂贵微调即可突破冷启动瓶颈。该工作展示了记忆驱动智能体在领域编程中的迁移价值。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: NPU等数据稀缺编程领域存在数据墙，大模型内核合成遭遇冷启动与性能骤降问题。
method: 提出EvoKernel自演化智能体框架，将内核合成建模为基于记忆的强化学习任务，实现草拟到持续精炼。
result: 该框架无需昂贵微调即可缓解冷启动，通过记忆驱动持续精炼逐步提升内核合成质量。
conclusion: 价值驱动记忆为数据稀缺领域中的智能体自演化与持续改进提供了可行路径。
---

## Abstract
Deploying Large Language Models to data-scarce programming domains poses significant challenges, particularly for kernel synthesis on emerging Domain-Specific Architectures where a ``Data Wall'' limits available training data.
While models excel on data-rich platforms like CUDA, they suffer catastrophic performance drops on data-scarce ecosystems such as NPU programming.
To overcome this cold-start barrier without expensive fine-tuning, we introduce EvoKernel, a self-evolving agentic framework that automates the lifecycle of kernel synthesis from initial drafting to continual refining.
EvoKernel addresses this by formulating the synthesis process as a memory-based reinforcement learning task. Through a novel value-driven retrieval mechanism, it learns stage-specific Q-values that prioritize experiences based on their contribution to the current objective—whether bootstrapping a feasible draft or iteratively refining latency.
Furthermore, by enabling cross-task memory sharing, the agent generalizes insights from simple to complex operators.
By building an NPU variant of KernelBench and evaluating on it, EvoKernel improves frontier models' correctness from 11.0\% to 83.0\% and achieves a median speedup of 3.60$\times$ over initial drafts through iterative refinement. This demonstrates that value-driven experience accumulation allows general-purpose models to master the kernel synthesis task on niche hardware ecosystems.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
基于价值驱动记忆的自演化智能体框架用于持续精炼。

### 2. 核心内容
在NPU等数据稀缺的编程领域，大模型受数据墙限制难以进行内核合成，性能较CUDA等数据丰富平台大幅下降。本文提出EvoKernel，将合成过程建模为基于记忆的强化学习任务，通过价值驱动记忆机制实现从初始草稿到持续精炼的自演化智能体流程，无需昂贵微调即可突破冷启动瓶颈。该工作展示了记忆驱动智能体在领域编程中的迁移价值。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=ajHTru25Kd](https://openreview.net/forum?id=ajHTru25Kd)
