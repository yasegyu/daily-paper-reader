---
title: "MemIncept: Steering LLM Agents via Cooperative Stealthy Memory Injections"
title_zh: MemIncept：通过协作式隐蔽记忆注入操控LLM智能体
authors: "Nan Yan, Qian Lou, Jiarong Xing"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/f617810031d03c65bd15ee7c09f86c69a681ae7a.pdf"
tags: ["query:agent-memory"]
score: 7.0
evidence: 针对LLM智能体长期记忆的记忆投毒攻击
tldr: 长期记忆赋予LLM智能体自适应推理能力，却也暴露了攻击面，攻击者可注入恶意记录以偏置智能体行为。现有攻击面临两难：有效注入往往明显恶意易被检测，而隐蔽注入效果有限。本文提出MemIncept，一种黑盒设置下仅用良性查询的记忆投毒攻击，通过双向进化策略优化协作查询集。该工作揭示了智能体记忆系统的安全脆弱性。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 长期记忆虽提升LLM智能体的自适应推理能力，却让攻击者可通过注入恶意记录偏置其行为。
method: 提出MemIncept记忆投毒攻击，用双向进化策略生成协同查询集，在黑盒下以良性查询实施注入。
result: 相比注入孤立记录的先前方法，协同查询集能更隐蔽且有效地改变智能体行为。
conclusion: 该研究揭示智能体长期记忆的安全风险，为记忆系统防御提供警示。
---

## Abstract
Long-term memory empowers LLM-based agents with adaptive reasoning but exposes a critical attack surface---adversaries can inject malicious records to bias agent behaviors. However, existing attacks face a dilemma: effective injections are often visibly malicious and easily detected, while stealthy, benign-looking injections are often less effective in altering agent behaviors. To address this, we propose MemIncept, a memory poisoning attack that can impact agents even in black-box settings using only benign-appearing queries. Unlike prior methods that inject isolated records, MemIncept generates a cooperative set of queries that work together to bias the agent.  It achieves this via a bidirectional evolutionary strategy that optimizes the query set from two ends. A forward pass ensures the queries collectively lead the agent to the target outcome, while a backward pass ensures they are semantically close to victim (benign) queries for reliable retrieval. This ``meet-in-the-middle'' approach creates injected records that are both easy to retrieve and effective at steering behavior. Through extensive experiments across diverse agents, we show that MemIncept significantly outperforms single-record attacks, achieving high success rates comparable to explicit attacks while remaining difficult to flag under automated filters or human inspection.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
针对LLM智能体长期记忆的记忆投毒攻击。

### 2. 核心内容
长期记忆赋予LLM智能体自适应推理能力，却也暴露了攻击面，攻击者可注入恶意记录以偏置智能体行为。现有攻击面临两难：有效注入往往明显恶意易被检测，而隐蔽注入效果有限。本文提出MemIncept，一种黑盒设置下仅用良性查询的记忆投毒攻击，通过双向进化策略优化协作查询集。该工作揭示了智能体记忆系统的安全脆弱性。

### 3. 对应检索需求
Find top tier AI conference papers on memory architectures for autonomous agents and large language model agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=1YNrlSSRsk](https://openreview.net/forum?id=1YNrlSSRsk)
