---
title: "Memory is Reconstructed, Not Retrieved:  Graph Memory for LLM Agents"
title_zh: 记忆是被重建而非检索：面向LLM智能体的图记忆
authors: "Shuo Ji, Yibo Li, Bryan Hooi"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/287ef26120ae98620ee1b2cc5a8a704b47fceafa.pdf"
tags: ["query:agent-memory"]
score: 10.0
evidence: 面向LLM智能体推理的图记忆与主动重建
tldr: LLM智能体在长交互历史推理上仍显不足，现有记忆增强智能体依赖静态的先检索后推理范式，无法根据推理中发现的中间证据动态调整记忆访问。本文提出MRAgent，将记忆表示为线索-标签-内容图，并引入主动重建机制，把LLM推理直接融入记忆访问过程。该框架使智能体能迭代探索记忆，突破刚性流水线限制，提升长程推理能力。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有记忆增强智能体的先检索后推理范式过于刚性，无法根据推理中发现的中间证据动态调整记忆访问。
method: 提出MRAgent，将记忆组织为线索-标签-内容关联图，并用主动重建机制把LLM推理融入记忆访问。
result: 智能体可迭代探索记忆结构，动态重构所需记忆内容，改善长交互历史下的推理表现。
conclusion: 该工作主张记忆是重建而非检索，为智能体记忆访问范式提供新思路。
---

## Abstract
Despite recent progress, LLM agents still struggle with reasoning over long interaction histories. While current memory-augmented agents rely on a static ``retrieve-then-reason'' paradigm, this rigid pipeline design prevents them from dynamically adapting memory access to intermediate evidence discovered during inference. To bridge this gap, we propose MRAgent, a framework that combines an associative memory graph with an active reconstruction mechanism. We represent memory as a Cue–Tag–Content graph, where associative tags serve as semantic bridges connecting fine-grained cues to memory contents. Operating on this structure, our active reconstruction mechanism integrates LLM reasoning directly into memory access, allowing the agent to iteratively explore and prune retrieval paths based on accumulated evidence. This ensures that memory retrieval is dynamically adapted to the  reasoning context while avoiding combinatorial explosion caused by unconstrained expansion. Experiments on the LoCoMo benchmark  and LongMemEval benchmark  demonstrate significant improvements over strong baselines (up to $23\\%$), while substantially reducing retrieval cost, highlighting the effectiveness of active and associative reconstruction for long-horizon memory reasoning.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向LLM智能体推理的图记忆与主动重建。

### 2. 核心内容
LLM智能体在长交互历史推理上仍显不足，现有记忆增强智能体依赖静态的先检索后推理范式，无法根据推理中发现的中间证据动态调整记忆访问。本文提出MRAgent，将记忆表示为线索-标签-内容图，并引入主动重建机制，把LLM推理直接融入记忆访问过程。该框架使智能体能迭代探索记忆，突破刚性流水线限制，提升长程推理能力。

### 3. 对应检索需求
memory retrieval mechanisms for agent decision making。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=xRVWftS3ES](https://openreview.net/forum?id=xRVWftS3ES)
