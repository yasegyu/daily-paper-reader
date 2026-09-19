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
evidence: 面向自演化大模型智能体的统一记忆提取与管理框架
tldr: 该文针对大模型智能体自演化记忆中提取与管理脱节的问题，指出既有方法多只优化记忆管理，而将记忆提取视为静态过程，导致智能体积累实例噪声而非稳健记忆。作者提出统一记忆提取与管理框架UMEM，联合优化同一模型同时完成经验提炼与记忆库更新，并引入语义邻域建模缓解过拟合。该方法提升了记忆的泛化能力，对智能体长期记忆架构具有重要意义。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有智能体记忆系统只优化管理而忽视提取，导致记忆泛化差、噪声多。
method: 提出UMEM联合优化提取与管理，并引入语义邻域建模抑制实例过拟合。
result: 使智能体同时提炼与维护记忆，获得更稳健可泛化的记忆。
conclusion: 统一提取与管理为自演化智能体记忆架构提供新范式。
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
面向自演化大模型智能体的统一记忆提取与管理框架。

### 2. 核心内容
该文针对大模型智能体自演化记忆中提取与管理脱节的问题，指出既有方法多只优化记忆管理，而将记忆提取视为静态过程，导致智能体积累实例噪声而非稳健记忆。作者提出统一记忆提取与管理框架UMEM，联合优化同一模型同时完成经验提炼与记忆库更新，并引入语义邻域建模缓解过拟合。该方法提升了记忆的泛化能力，对智能体长期记忆架构具有重要意义。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=BoiXvrwtdi](https://openreview.net/forum?id=BoiXvrwtdi)
