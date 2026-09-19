---
title: "Mem-T: Densifying Rewards for Long-Horizon Memory Agents"
title_zh: Mem-T：为长时序记忆智能体稠密化奖励
authors: "Yanwei Yue, Guibin Zhang, Boci Peng, Xuanbo Fan, Jiaxin Guo, Qiankun Li, Yan Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/50453717a0322909321c24d35a41152273110a8c.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 具备动态更新与多轮检索的自主记忆智能体
tldr: 现有记忆智能体在长时序记忆操作中常面临奖励稀疏且延迟的问题，难以端到端优化记忆管理策略。本文提出Mem-T，一个自主记忆智能体，接入轻量分层记忆数据库，对流转输入进行动态更新与多轮检索。为训练长时序记忆能力，作者提出MoT-GRPO奖励稠密化方法。该工作提升了记忆管理策略的可训练性，为自主记忆智能体提供了新范式。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 记忆智能体在长时序操作中奖励稀疏且延迟，阻碍记忆管理策略的端到端优化。
method: 提出Mem-T自主记忆智能体，结合分层记忆数据库与MoT-GRPO奖励稠密化训练方法。
result: 实现对流转输入的动态更新与多轮检索，并有效训练长时序记忆管理能力。
conclusion: 为自主记忆智能体的记忆存储与检索管理提供了可端到端优化的新方案。
---

## Abstract
Memory agents, which depart from predefined memory-processing pipelines by endogenously managing the processing, storage, and retrieval of memories, have garnered increasing attention for their autonomy and adaptability. However, existing training paradigms remain constrained: agents often traverse long-horizon sequences of memory operations before receiving sparse and delayed rewards, which hinders truly end-to-end optimization of memory management policies. To address this limitation, we introduce Mem-T, an autonomous memory agent that interfaces with a lightweight hierarchical memory database to perform dynamic updates and multi-turn retrieval over streaming inputs. To effectively train long-horizon memory management capabilities, we further propose MoT-GRPO, a tree-guided reinforcement learning framework that transforms sparse terminal feedback into dense, step-wise supervision via memory operation tree backpropagation and hindsight credit assignment, thereby enabling the joint optimization of memory construction and retrieval.
Extensive experiments demonstrate that Mem-T is **(1) high-performing**, surpassing frameworks such as A-Mem and Mem0 by up to $14.94\\%$, and **(2) economical**, operating on a favorable accuracy-efficiency Pareto frontier and reducing inference tokens per query by $\sim24.45\\%$ relative to GAM without sacrificing performance.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
具备动态更新与多轮检索的自主记忆智能体。

### 2. 核心内容
现有记忆智能体在长时序记忆操作中常面临奖励稀疏且延迟的问题，难以端到端优化记忆管理策略。本文提出Mem-T，一个自主记忆智能体，接入轻量分层记忆数据库，对流转输入进行动态更新与多轮检索。为训练长时序记忆能力，作者提出MoT-GRPO奖励稠密化方法。该工作提升了记忆管理策略的可训练性，为自主记忆智能体提供了新范式。

### 3. 对应检索需求
memory-augmented agent models that store and retrieve experience。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=8ppVmLtA2V](https://openreview.net/forum?id=8ppVmLtA2V)
