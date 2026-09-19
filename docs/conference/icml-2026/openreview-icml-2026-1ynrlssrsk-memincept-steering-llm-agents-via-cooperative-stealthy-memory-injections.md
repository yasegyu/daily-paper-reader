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
tldr: 长期记忆让LLM智能体具备自适应推理能力，但也带来了关键攻击面，攻击者可注入恶意记录来偏置智能体行为。现有攻击面临两难：有效注入往往明显恶意而容易被检测，隐蔽良性的注入又难以改变行为。MemIncept提出一种记忆投毒攻击，通过双向进化策略优化一组协作查询，即使仅有看似良性的查询也能在黑盒设定下协同偏置智能体，凸显了智能体记忆系统的安全隐患。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 长期记忆赋予LLM智能体自适应推理能力，但也暴露攻击面，攻击者可注入恶意记录以偏置智能体行为。
method: 提出记忆投毒攻击MemIncept，利用双向进化策略优化一组协作查询，仅用看似良性的查询即可在黑盒下注入并偏置智能体。
result: 该攻击在隐蔽性与有效性间取得平衡，能影响智能体行为。
conclusion: 揭示并利用LLM智能体长期记忆的安全脆弱性。
---

## Abstract
Long-term memory empowers LLM-based agents with adaptive reasoning but exposes a critical attack surface---adversaries can inject malicious records to bias agent behaviors. However, existing attacks face a dilemma: effective injections are often visibly malicious and easily detected, while stealthy, benign-looking injections are often less effective in altering agent behaviors. To address this, we propose MemIncept, a memory poisoning attack that can impact agents even in black-box settings using only benign-appearing queries. Unlike prior methods that inject isolated records, MemIncept generates a cooperative set of queries that work together to bias the agent.  It achieves this via a bidirectional evolutionary strategy that optimizes the query set from two ends. A forward pass ensures the queries collectively lead the agent to the target outcome, while a backward pass ensures they are semantically close to victim (benign) queries for reliable retrieval. This ``meet-in-the-middle'' approach creates injected records that are both easy to retrieve and effective at steering behavior. Through extensive experiments across diverse agents, we show that MemIncept significantly outperforms single-record attacks, achieving high success rates comparable to explicit attacks while remaining difficult to flag under automated filters or human inspection.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
针对LLM智能体长期记忆的记忆投毒攻击。

### 2. 核心内容
长期记忆让LLM智能体具备自适应推理能力，但也带来了关键攻击面，攻击者可注入恶意记录来偏置智能体行为。现有攻击面临两难：有效注入往往明显恶意而容易被检测，隐蔽良性的注入又难以改变行为。MemIncept提出一种记忆投毒攻击，通过双向进化策略优化一组协作查询，即使仅有看似良性的查询也能在黑盒设定下协同偏置智能体，凸显了智能体记忆系统的安全隐患。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=1YNrlSSRsk](https://openreview.net/forum?id=1YNrlSSRsk)
