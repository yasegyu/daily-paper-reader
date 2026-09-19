---
title: "UMEM: Unified Memory Extraction and Management Framework for Generalizable Memory"
title_zh: UMEM：面向可泛化记忆的统一记忆提取与管理框架
authors: "Yongshi Ye, Hui Jiang, Feihu Jiang, Tian Lan, Yichao Du, Biao Fu, Xiaodong Shi, Qianghuai Jia, Longyue Wang, Weihua Luo"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/9bcba03fc57063491f6d3b408af5094d4d663f30.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 面向大模型智能体记忆的统一提取与管理框架
tldr: 自演化记忆被视为大模型智能体的可训练参数，其经验提取与记忆库更新需紧密协同。然而现有方法主要优化记忆管理，将提取视为静态过程，导致智能体积累大量实例特异噪声而非稳健记忆，泛化性差。本文提出统一记忆提取与管理框架UMEM，联合优化同一大模型同时进行记忆提取与管理，并引入语义邻域建模以缓解对特定实例的过拟合。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有智能体记忆方法只优化记忆管理、将提取视为静态，导致积累实例噪声且泛化性差。
method: 提出UMEM框架，联合优化大模型同时进行记忆提取与管理，并引入语义邻域建模抑制过拟合。
result: 联合优化与语义邻域建模使智能体获得更稳健、可泛化的记忆，减少实例特异噪声的累积。
conclusion: 统一提取与管理为智能体自演化记忆的可泛化性提供了有效方案。
---

## Abstract
Self-evolving memory serves as the trainable parameters for Large Language Models (LLMs)-based agents, where extraction (distilling insights from experience) and management (updating the memory bank) must be tightly coordinated. 
Existing methods predominantly optimize memory management while treating memory extraction as a static process, resulting in poor generalization, where agents accumulate instance-specific noise rather than robust memories.
To address this, we propose Unified Memory Extraction and Management (UMEM), a self-evolving agent framework that jointly optimizes a LLM to simultaneously extract and manage memories.
To mitigate overfitting to specific instances, we introduce Semantic Neighborhood Modeling and optimize the model with a neighborhood-level marginal utility reward via GRPO.
This approach ensures memory generalizability by evaluating memory utility across clusters of semantically related queries.
Extensive experiments across five benchmarks demonstrate that UMEM significantly outperforms highly competitive baselines, achieving up to 11.49 points improvement in multi-turn interactive tasks. Furthermore, UMEM maintains a stable improvement trend during continuous evolution.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向大模型智能体记忆的统一提取与管理框架。

### 2. 核心内容
自演化记忆被视为大模型智能体的可训练参数，其经验提取与记忆库更新需紧密协同。然而现有方法主要优化记忆管理，将提取视为静态过程，导致智能体积累大量实例特异噪声而非稳健记忆，泛化性差。本文提出统一记忆提取与管理框架UMEM，联合优化同一大模型同时进行记忆提取与管理，并引入语义邻域建模以缓解对特定实例的过拟合。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=BoiXvrwtdi](https://openreview.net/forum?id=BoiXvrwtdi)
