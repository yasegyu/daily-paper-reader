---
title: "E-mem: Multi-Agent Based Episodic Context Reconstruction for LLM Agent Memory"
title_zh: E-mem：面向LLM智能体记忆的多智能体情节上下文重建
authors: "Kaixiang Wang, Yidan Lin, Zihan Wang, Bunyod Suvonov, Zhaojiacheng Zhou, Yuxiang Zheng, Jiaxi Cao, Zhiheng Dong, Chentao Wu, Jiong Lou, Jie LI"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/bd1b2b6e9e43b41af1dd5ece6e30eb30e09080b9.pdf"
tags: ["query:agent-memory"]
score: 10.0
evidence: 面向LLM智能体记忆的多智能体情节上下文重建
tldr: 现有LLM智能体记忆方法多将连续序列依赖压缩为嵌入或图等预定义结构，造成破坏性去语境化，损害深度推理所需的叙事完整性。为此，论文提出E-mem框架，受生物记忆印迹启发，从记忆预处理转向情节上下文重建，采用由多助手智能体构成的异构分层架构维护未压缩记忆内容。该工作旨在提升System 2式长程高精度推理中记忆的连贯性，为智能体记忆架构提供新范式。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 主流记忆预处理把连续序列压缩为嵌入或图结构，破坏语境，损害长程深度推理所需的逻辑完整性。
method: 提出E-mem，采用多助手智能体构成的异构分层架构，维护未压缩记忆并重建情节上下文而非预处理压缩。
result: 摘要未给出具体量化结果，但框架旨在维持长时程推理的叙事与逻辑完整性。
conclusion: 以情节上下文重建替代记忆预处理，为LLM智能体记忆架构提供生物启发的新思路。
---

## Abstract
The evolution of Large Language Model (LLM) agents towards System~2 reasoning, characterized by deliberative, high-precision problem-solving, necessitates maintaining rigorous logical integrity over extended horizons. However, prevalent memory preprocessing paradigms incur destructive de-contextualization. By compressing fluid sequential dependencies into pre-defined structures (e.g., embeddings or graphs), these methods sever the narrative integrity essential for deep reasoning. To address this, we propose E-mem, a framework shifting from Memory Preprocessing to Episodic Context Reconstruction inspired by biological engrams. E-mem employs a heterogeneous hierarchical architecture where multiple assistant agents maintain uncompressed memory contexts, while a central master agent orchestrates global planning. Unlike passive retrieval, our mechanism empowers assistants to locally reason within activated segments, extracting context-aware evidence before aggregation. Evaluations on the LoCoMo benchmark demonstrate that E-mem achieves over 54\% F1—surpassing the state-of-the-art GAM by 7.75\%—while reducing token cost by over 70\%. Our work is available on \url{https://anonymous.4open.science/r/E-mem-F6C3/}.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向LLM智能体记忆的多智能体情节上下文重建。

### 2. 核心内容
现有LLM智能体记忆方法多将连续序列依赖压缩为嵌入或图等预定义结构，造成破坏性去语境化，损害深度推理所需的叙事完整性。为此，论文提出E-mem框架，受生物记忆印迹启发，从记忆预处理转向情节上下文重建，采用由多助手智能体构成的异构分层架构维护未压缩记忆内容。该工作旨在提升System 2式长程高精度推理中记忆的连贯性，为智能体记忆架构提供新范式。

### 3. 对应检索需求
Search for papers about long term memory, episodic memory, and memory retrieval in interactive agent systems.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=FAjA0snAYq](https://openreview.net/forum?id=FAjA0snAYq)
