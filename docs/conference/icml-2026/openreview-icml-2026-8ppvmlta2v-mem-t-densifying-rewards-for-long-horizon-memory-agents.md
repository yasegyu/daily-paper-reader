---
title: "Mem-T: Densifying Rewards for Long-Horizon Memory Agents"
title_zh: Mem-T：为长程记忆智能体稠密化奖励
authors: "Yanwei Yue, Guibin Zhang, Boci Peng, Xuanbo Fan, Jiaxin Guo, Qiankun Li, Yan Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/50453717a0322909321c24d35a41152273110a8c.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 自主管理存储与多轮检索的记忆智能体
tldr: 记忆智能体自主管理记忆的处理、存储与检索，但现有训练中智能体需经历长程记忆操作才能获得稀疏延迟奖励，难以端到端优化记忆管理策略。作者提出Mem-T，通过连接轻量级层次化记忆数据库对流式输入进行动态更新与多轮检索。并设计MoT-GRPO训练方法稠密化奖励，从而有效训练长程记忆管理能力，推动自主记忆智能体的端到端优化。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 记忆智能体需经历长程记忆操作才获得稀疏延迟奖励，难以端到端优化其记忆管理策略。
method: 提出Mem-T自主记忆智能体，连接轻量级层次化记忆数据库进行动态更新与多轮检索，并用MoT-GRPO稠密化奖励训练。
result: 稠密奖励训练使智能体更有效地学习长程记忆管理，提升了自主记忆处理与检索的端到端表现。
conclusion: 表明通过奖励稠密化可训练长程自主记忆智能体，提升记忆管理策略的优化效果。
---

## Abstract
Memory agents, which depart from predefined memory-processing pipelines by endogenously managing the processing, storage, and retrieval of memories, have garnered increasing attention for their autonomy and adaptability. However, existing training paradigms remain constrained: agents often traverse long-horizon sequences of memory operations before receiving sparse and delayed rewards, which hinders truly end-to-end optimization of memory management policies. To address this limitation, we introduce Mem-T, an autonomous memory agent that interfaces with a lightweight hierarchical memory database to perform dynamic updates and multi-turn retrieval over streaming inputs. To effectively train long-horizon memory management capabilities, we further propose MoT-GRPO, a tree-guided reinforcement learning framework that transforms sparse terminal feedback into dense, step-wise supervision via memory operation tree backpropagation and hindsight credit assignment, thereby enabling the joint optimization of memory construction and retrieval.
Extensive experiments demonstrate that Mem-T is **(1) high-performing**, surpassing frameworks such as A-Mem and Mem0 by up to $14.94\\%$, and **(2) economical**, operating on a favorable accuracy-efficiency Pareto frontier and reducing inference tokens per query by $\sim24.45\\%$ relative to GAM without sacrificing performance.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
自主管理存储与多轮检索的记忆智能体。

### 2. 核心内容
记忆智能体自主管理记忆的处理、存储与检索，但现有训练中智能体需经历长程记忆操作才能获得稀疏延迟奖励，难以端到端优化记忆管理策略。作者提出Mem-T，通过连接轻量级层次化记忆数据库对流式输入进行动态更新与多轮检索。并设计MoT-GRPO训练方法稠密化奖励，从而有效训练长程记忆管理能力，推动自主记忆智能体的端到端优化。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=8ppVmLtA2V](https://openreview.net/forum?id=8ppVmLtA2V)
