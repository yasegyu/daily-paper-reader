---
title: "LRAgent: Efficient KV Cache Sharing for Multi-LoRA LLM Agents"
title_zh: LRAgent：面向多LoRA大模型智能体的高效KV缓存共享
authors: "Hyesung Jeon, Hyeongju Ha, Jae-Joon Kim"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/aad6d5a22a6ab8a9ad7c83d6bff25e05e9d49a41.pdf"
tags: ["query:agent-memory"]
score: 5.0
evidence: 在多LoRA智能体间共享KV缓存以减少冗余
tldr: 该文针对多LoRA多智能体系统中各智能体独立存储KV缓存导致的内存与算力开销问题，观察到智能体间缓存差异主要来自适配器输出，而共享骨干的激活高度相似。作者提出LRAgent，将缓存分解为共享基础分量与适配器分量以实现跨智能体复用。该方法为多智能体共享记忆与高效推理提供了系统级支持。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多LoRA智能体各自存储KV缓存，造成大量内存与计算冗余。
method: 提出LRAgent，将缓存分解为共享骨干分量与适配器输出分量以复用。
result: 利用骨干激活高度相似性实现跨智能体缓存共享，降低开销。
conclusion: 为多智能体系统的共享内存与高效服务提供实用方案。
---

## Abstract
Role specialization in multi-LLM agent systems is often realized via multi-LoRA, where agents share a pretrained backbone and differ only through lightweight adapters.
Despite sharing base model weights, each agent independently builds and stores its own KV cache for the same long, tool-augmented trajectories, incurring substantial memory and compute overhead.
Existing KV cache sharing methods largely overlook this multi-LoRA setting.
We observe that, across agents, cache differences are dominated by adapter outputs, while activations from the shared pretrained backbone remain highly similar.
Based on this observation, we propose LRAgent, a KV cache sharing framework for multi-LoRA agents that decomposes the cache into a shared base component from the pretrained weights and an adapter-dependent component from LoRA weights.
LRAgent reduces memory overhead by sharing the base component and storing the adapter component in its inherent low-rank form, and further reduces compute overhead, enabled by shared-$A$ multi-LoRA architectures, by also sharing the low-rank cache and avoiding redundant computations for contexts already processed by other agents.
To efficiently reconstruct adapter contributions at runtime, we introduce Flash-LoRA-Attention, a kernel that reorders attention computation to avoid materializing the low-rank cache to full dimension.
LRAgent achieves throughput and time-to-first-token latency close to fully shared caching, while preserving accuracy near the non-shared caching baseline across agentic question-answering benchmarks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
在多LoRA智能体间共享KV缓存以减少冗余。

### 2. 核心内容
该文针对多LoRA多智能体系统中各智能体独立存储KV缓存导致的内存与算力开销问题，观察到智能体间缓存差异主要来自适配器输出，而共享骨干的激活高度相似。作者提出LRAgent，将缓存分解为共享基础分量与适配器分量以实现跨智能体复用。该方法为多智能体共享记忆与高效推理提供了系统级支持。

### 3. 对应检索需求
shared memory and communication in multi-agent systems。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=ooRukY3zjQ](https://openreview.net/forum?id=ooRukY3zjQ)
