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
score: 9.0
evidence: 面向LLM智能体的高效终身记忆框架
tldr: 面向复杂环境中LLM智能体的长期交互，现有记忆方法要么被动扩展上下文造成大量冗余，要么依赖迭代推理过滤噪声而消耗高昂token。SimpleMem提出基于语义无损压缩的三阶段记忆框架，通过语义结构化压缩把非结构化交互蒸馏为紧凑的多视图索引记忆单元，并借助在线语义合成在会话内即时整合相关上下文。该方法最大化信息密度与token利用率，为智能体提供高效的终身记忆能力。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: LLM智能体长期交互需管理历史经验，现有方法要么保留全部历史导致冗余，要么依赖迭代推理过滤噪声而开销高。
method: 提出基于语义无损压缩的三阶段记忆框架，将非结构化交互蒸馏为紧凑的多视图索引记忆单元，并在线进行语义合成。
result: 该流程提升信息密度与token利用率，在长期交互中兼顾效率与准确性。
conclusion: 为LLM智能体提供高效终身记忆方案。
---

## Abstract
To support long-term interaction in complex environments, LLM agents require memory systems that manage historical experiences. Existing approaches either retain full interaction histories via passive context extension, leading to substantial redundancy, or rely on iterative reasoning to filter noise, incurring high token costs. To address this challenge, we introduce SimpleMem, an efficient memory framework based on semantic lossless compression. We propose a three-stage pipeline designed to maximize information density and token utilization: (1) Semantic Structured Compression, which distills unstructured interactions into compact, multi-view indexed memory units; (2) Online Semantic Synthesis, an intra-session process that instantly integrates related context into unified abstract representations to eliminate redundancy; and (3) Intent-Aware Retrieval Planning, which infers search intent to dynamically determine retrieval scope and construct precise context efficiently. Experiments on benchmark datasets show that our method consistently outperforms baseline approaches in accuracy, retrieval efficiency, and inference cost, achieving an average F1 improvement of 26.4% in LoCoMo while reducing inference-time token consumption by up to 30×, demonstrating a superior balance between performance and efficiency. Code is available at https://github.com/aiming-lab/SimpleMem.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向LLM智能体的高效终身记忆框架。

### 2. 核心内容
面向复杂环境中LLM智能体的长期交互，现有记忆方法要么被动扩展上下文造成大量冗余，要么依赖迭代推理过滤噪声而消耗高昂token。SimpleMem提出基于语义无损压缩的三阶段记忆框架，通过语义结构化压缩把非结构化交互蒸馏为紧凑的多视图索引记忆单元，并借助在线语义合成在会话内即时整合相关上下文。该方法最大化信息密度与token利用率，为智能体提供高效的终身记忆能力。

### 3. 对应检索需求
Find top tier AI conference papers on memory architectures for autonomous agents and large language model agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=oBgLvd5YC6](https://openreview.net/forum?id=oBgLvd5YC6)
