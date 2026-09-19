---
title: Social Hippocampus Memory Learning
title_zh: 社会海马体记忆学习
authors: "Liping Yi, Zhiming Zhao, Kewen Zhu, Xiang Li, Zhiwei Shang, Qinghua Hu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/fc0da9f5a126e8760f247cd16891d1ffbecea71d.pdf"
tags: ["query:agent-memory"]
score: 7.0
evidence: 以记忆为中心、在异构智能体间共享记忆的社会学习框架
tldr: 针对异构联邦学习中共享模型参数或中间表示易泄露敏感信息且开销大的问题，本文受社会学习启发提出SoHip社会海马体记忆学习框架，让多个异构智能体通过共享抽象化的记忆而非参数进行协作学习。该框架以记忆共享为核心机制，在保护隐私、降低通信开销的同时实现知识交换，为多智能体系统中的共享记忆与协作通信提供了新的实现路径。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 异构联邦学习共享模型参数或中间表示易泄露隐私且通信开销大。
method: 提出SoHip以记忆为中心的社会机器学习框架，让异构智能体通过共享抽象记忆进行协作。
result: 在保护隐私、降低开销的同时实现异构智能体间的知识交换与协作。
conclusion: 为多智能体系统共享记忆与通信协作提供了新的记忆中心式范式。
---

## Abstract
Social learning highlights that learning agents improve not in isolation, but through interaction and structured knowledge exchange with others. When introduced into machine learning, this principle gives rise to social machine learning (SML), where multiple agents collaboratively learn by sharing abstracted knowledge. Federated learning (FL) provides a natural collaboration substrate for this paradigm, yet existing heterogeneous FL approaches often rely on sharing model parameters or intermediate representations, which may expose sensitive information and incur additional overhead.
In this work, we propose **SoHip** (**So**cial **Hip**pocampus Memory Learning), a memory-centric social machine learning framework that enables collaboration among heterogeneous agents via memory sharing rather than model sharing. SoHip abstracts each agent’s individual short-term memory from local representations, consolidates it into individual long-term memory through a hippocampus-inspired mechanism, and fuses it with collectively aggregated long-term memory to enhance local prediction. Throughout the process, raw data and local models remain on-device, while only lightweight memory are exchanged.
We provide theoretical analysis on convergence and privacy preservation properties. Experiments on two benchmark datasets with seven baselines demonstrate that SoHip consistently outperforms existing methods, achieving up to 8.78% accuracy improvements. The code of SoHip is available at https://github.com/LipingYi/SoHip.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
以记忆为中心、在异构智能体间共享记忆的社会学习框架。

### 2. 核心内容
针对异构联邦学习中共享模型参数或中间表示易泄露敏感信息且开销大的问题，本文受社会学习启发提出SoHip社会海马体记忆学习框架，让多个异构智能体通过共享抽象化的记忆而非参数进行协作学习。该框架以记忆共享为核心机制，在保护隐私、降低通信开销的同时实现知识交换，为多智能体系统中的共享记忆与协作通信提供了新的实现路径。

### 3. 对应检索需求
shared memory and communication in multi-agent systems。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=TxHOT32Maj](https://openreview.net/forum?id=TxHOT32Maj)
