---
title: "A-MemGuard: A Proactive Defense Framework For LLM-Based Agent Memory"
title_zh: A-MemGuard：面向大模型智能体记忆的主动防御框架
authors: "Qianshan Wei, Tengchao Yang, Yaochen Wang, Xinfeng Li, Lijun Li, Zhenfei Yin, Yi Zhan, Thorsten Holz, Zhiqiang Lin, XiaoFeng Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/8770b2c7271dfa6194d2e234a12ce022d1f95224.pdf"
tags: ["query:agent-memory"]
score: 8.0
evidence: 保护大模型智能体记忆免受注入攻击的防御框架
tldr: 大模型智能体依赖记忆从历史交互中学习，但这也带来安全风险：攻击者可向记忆注入看似无害的记录以操纵其未来行为。此类攻击的恶意效果仅在特定情境激活、难以孤立审计发现，且一旦触发会形成自我强化的错误循环。本文提出A-MemGuard主动防御框架，针对记忆注入的两大特性进行检测与防护，提升了智能体记忆架构的安全性。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 大模型智能体依赖记忆学习，但记忆注入攻击可在特定情境触发并形成自我强化的错误循环。
method: 提出主动防御框架A-MemGuard，针对注入记录的情境激活与自强化特性进行检测与拦截。
result: 该框架能识别孤立审计难以发现的恶意记忆，阻断错误累积与后续攻击门槛的降低。
conclusion: 该工作为智能体记忆架构的安全性提供了主动防护思路。
---

## Abstract
Large Language Model (LLM) agents use memory to learn from past interactions. However, this reliance on memory introduces a critical security risk: an adversary can inject seemingly harmless records into an agent's memory to manipulate its future behavior. This vulnerability is characterized by two core aspects: First, the malicious effect of injected records is only activated within a specific context, making them hard to detect when individual memory entries are audited in isolation. Second, once triggered, the manipulation can initiate a self-reinforcing error cycle: the corrupted outcome is stored as precedent, which not only amplifies the initial error but also progressively lowers the threshold for similar attacks in the future. To address these challenges, we introduce \emph{A-MemGuard} (\underline{A}gent-\underline{Mem}ory \underline{Guard}), the first defense framework for LLM agent memory. The core idea of our work is the insight that memory itself must become both \emph{self-checking} and \emph{self-correcting}. Without modifying the agent's core architecture, A-MemGuard combines two mechanisms: (1) \textbf{consensus-based validation}, which detects anomalies by comparing reasoning paths derived from multiple related memories and (2) a \textbf{dual-memory structure}, where detected failures are distilled into ``lessons'' stored separately and consulted before future actions, breaking error cycles and enabling adaptation.
Comprehensive evaluations on multiple benchmarks show that A-MemGuard effectively cuts attack success rates by over 95\% while incurring a minimal utility cost. This work shifts LLM memory security from static filtering to a proactive, experience-driven model where defenses strengthen over time.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
保护大模型智能体记忆免受注入攻击的防御框架。

### 2. 核心内容
大模型智能体依赖记忆从历史交互中学习，但这也带来安全风险：攻击者可向记忆注入看似无害的记录以操纵其未来行为。此类攻击的恶意效果仅在特定情境激活、难以孤立审计发现，且一旦触发会形成自我强化的错误循环。本文提出A-MemGuard主动防御框架，针对记忆注入的两大特性进行检测与防护，提升了智能体记忆架构的安全性。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=udqe7UZUZ6](https://openreview.net/forum?id=udqe7UZUZ6)
