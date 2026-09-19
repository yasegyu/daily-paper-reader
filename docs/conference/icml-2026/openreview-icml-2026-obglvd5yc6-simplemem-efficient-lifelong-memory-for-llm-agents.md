---
title: "SimpleMem: Efficient Lifelong Memory for LLM Agents"
title_zh: SimpleMem：面向LLM智能体的高效终身记忆
authors: "Jiaqi Liu, Yaofeng Su, Peng Xia, Siwei Han, Zeyu Zheng, Cihang Xie, Mingyu Ding, Huaxiu Yao"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/af171ffc96696a3f1b46bc14d3e93f5a6ea2126c.pdf"
tags: ["query:agent-memory"]
score: 10.0
evidence: 面向LLM智能体的高效终身记忆框架
tldr: 针对LLM智能体长期交互中记忆冗余与token开销大的问题，本文提出SimpleMem高效记忆框架，基于语义无损压缩设计三阶段流水线：语义结构化压缩将非结构化交互蒸馏为紧凑多视图索引记忆单元，在线语义合成在会话内即时整合相关上下文。该框架在最大化信息密度与token利用率的同时降低历史管理的成本，为智能体终身记忆架构提供了可扩展方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有LLM智能体记忆要么被动扩展上下文导致冗余，要么迭代推理过滤噪声而token开销高。
method: 提出基于语义无损压缩的三阶段流水线，将交互蒸馏为多视图索引记忆单元并进行在线语义合成。
result: 在提升信息密度与token利用率的同时降低冗余，实现高效的终身记忆管理。
conclusion: 为LLM智能体提供可扩展的高效终身记忆架构，缓解长程交互中的记忆膨胀问题。
---

## Abstract
To support long-term interaction in complex environments, LLM agents require memory systems that manage historical experiences. Existing approaches either retain full interaction histories via passive context extension, leading to substantial redundancy, or rely on iterative reasoning to filter noise, incurring high token costs. To address this challenge, we introduce SimpleMem, an efficient memory framework based on semantic lossless compression. We propose a three-stage pipeline designed to maximize information density and token utilization: (1) Semantic Structured Compression, which distills unstructured interactions into compact, multi-view indexed memory units; (2) Online Semantic Synthesis, an intra-session process that instantly integrates related context into unified abstract representations to eliminate redundancy; and (3) Intent-Aware Retrieval Planning, which infers search intent to dynamically determine retrieval scope and construct precise context efficiently. Experiments on benchmark datasets show that our method consistently outperforms baseline approaches in accuracy, retrieval efficiency, and inference cost, achieving an average F1 improvement of 26.4% in LoCoMo while reducing inference-time token consumption by up to 30×, demonstrating a superior balance between performance and efficiency. Code is available at https://github.com/aiming-lab/SimpleMem.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向LLM智能体的高效终身记忆框架。

### 2. 核心内容
针对LLM智能体长期交互中记忆冗余与token开销大的问题，本文提出SimpleMem高效记忆框架，基于语义无损压缩设计三阶段流水线：语义结构化压缩将非结构化交互蒸馏为紧凑多视图索引记忆单元，在线语义合成在会话内即时整合相关上下文。该框架在最大化信息密度与token利用率的同时降低历史管理的成本，为智能体终身记忆架构提供了可扩展方案。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=oBgLvd5YC6](https://openreview.net/forum?id=oBgLvd5YC6)
