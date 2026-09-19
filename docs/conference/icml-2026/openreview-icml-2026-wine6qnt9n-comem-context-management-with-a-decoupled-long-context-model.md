---
title: "CoMem: Context Management with A Decoupled Long-Context Model"
title_zh: CoMem：基于解耦长上下文模型的上下文管理
authors: "Yuwei Zhang, Chengyu Dong, Shuowei Jin, Changlong Yu, Hejie Cui, Hongye Jin, Xinyang Zhang, Hamed Bonab, Colin Lockard, Jianshu Chen, Zhenyu Shi, Jingbo Shang, Xian Li, Bing Yin"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/3e9e4ca03908c0899c354a7b64bb29b1550a6d28.pdf"
tags: ["query:agent-memory"]
score: 8.0
evidence: 面向长程智能体模型的解耦式记忆管理
tldr: 智能体模型通过迭代摘要历史交互来实现长程任务，但额外的摘要token带来显著解码开销，拖慢端到端响应。作者提出CoMem框架，将记忆管理从主智能体工作流中解耦，使二者并行执行，并提出k步异步流水线把摘要与推理重叠。配合奖励驱动训练策略保证异步下的鲁棒性，有效掩盖上下文处理延迟，为智能体记忆管理的效率问题提供了新方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 智能体通过迭代摘要历史交互解决长程任务，但额外摘要token带来显著解码开销，拖慢端到端响应延迟。
method: 提出CoMem框架，将记忆管理与主智能体工作流解耦，用k步异步流水线重叠摘要与推理，并配奖励驱动训练。
result: 该异步解耦方案有效掩盖上下文处理延迟，在保证鲁棒性的同时降低了长程任务的响应开销。
conclusion: 表明解耦并异步化记忆管理是提升智能体长程上下文处理效率的有效途径。
---

## Abstract
Context management enables agentic models to solve long-horizon tasks through iterative summarization of previous interaction histories.
However, this process typically incurs substantial decoding overhead for the extra summarization tokens, which significantly affect the end-to-end response latency at deployment.
In this paper, we introduce CoMem, a novel framework that decouples memory management from the primary agent workflow, enabling these processes to execute in parallel. We propose a $k$-step-off asynchronous pipeline that overlaps the memory model's summarization with the agent's inference, effectively masking the latency of context processing. To ensure robustness under this asynchronous setting, we introduce a reward-driven training strategy that aligns the memory model to capture sufficient statistics for the agent's decision-making. Theoretical analysis confirms that CoMem offers a superior efficiency-effectiveness trade-off compared to coupled architectures.
Our extensive experimental results on SWE-Bench-Verified show that CoMem provides 1.4x latency improvements upon vanilla long-context solutions while preserving most of the performance.
Furthermore, we demonstrate that these latency gains scale favorably with increased system throughput, offering a modular path forward for the independent optimization of agent reasoning and memory compression.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向长程智能体模型的解耦式记忆管理。

### 2. 核心内容
智能体模型通过迭代摘要历史交互来实现长程任务，但额外的摘要token带来显著解码开销，拖慢端到端响应。作者提出CoMem框架，将记忆管理从主智能体工作流中解耦，使二者并行执行，并提出k步异步流水线把摘要与推理重叠。配合奖励驱动训练策略保证异步下的鲁棒性，有效掩盖上下文处理延迟，为智能体记忆管理的效率问题提供了新方案。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=wInE6qnt9n](https://openreview.net/forum?id=wInE6qnt9n)
