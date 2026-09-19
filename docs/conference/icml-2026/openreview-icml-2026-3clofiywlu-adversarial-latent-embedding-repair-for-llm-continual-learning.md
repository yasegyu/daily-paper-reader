---
title: Adversarial Latent Embedding Repair for LLM Continual Learning
title_zh: 面向LLM持续学习的对抗式潜在嵌入修复
authors: "Xilin Xia, Tong Xialiang, Jie Wang, Chi Ma, Shengxue Li, Yinqi Bai, Yuhang Jiang, Xing Li, Jianye HAO, Mingxuan Yuan, Feng Wu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/029da17b1af821f352ceb8e27573e1ae51a5e21f.pdf"
tags: ["query:agent-memory"]
score: 5.0
evidence: 面向LLM持续学习的免数据抗遗忘框架
tldr: LLM持续学习需在获取新技能时避免灾难性遗忘，但领域微调即便在窄更新下仍触发严重长尾遗忘，且预训练数据常不可得。本文提出ALER，一个免数据的持续学习框架，通过对抗搜索一小组潜在提示嵌入来最大化与冻结参考模型的logit差异，主动暴露高风险遗忘模式，再用在线蒸馏保留旧行为。该工作为LLM智能体的记忆保持与遗忘抑制提供新方法。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: LLM领域微调即便窄更新仍引发严重长尾遗忘，且预训练数据常不可访问。
method: 对抗搜索潜在提示嵌入以暴露遗忘模式，并对冻结参考模型进行在线蒸馏。
result: 在保留目标域适应性的同时有效抑制灾难性遗忘。
conclusion: 为LLM持续学习中的知识保持与遗忘抑制提供免数据方案。
---

## Abstract
Research on continual learning for LLMs seeks to acquire new skills without catastrophic forgetting of established prior knowledge.
However, domain-specific fine-tuning still triggers severe, long-tailed forgetting issues even under narrow updates, particularly when the pre-training data is inaccessible.
To tackle this challenge, we propose **ALER**, a data-free continual learning framework that adversarially searches for a small set of latent prompt embeddings to maximize logit divergence from a frozen reference model, proactively exposing high-risk forgetting modes at each step.
It then performs online distillation from the frozen reference using the discovered embeddings to retain prior behaviors while preserving target-domain adaptation.
We provide theoretical guarantees on the efficiency of our targeted repair, and extensive experiments demonstrate consistent improvements in the retention–adaptation frontier over representative baselines across $2$ domain-specific fine-tuning datasets and $6$ general-purpose benchmarks,
suggesting a more proactive approach for LLM continual learning.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向LLM持续学习的免数据抗遗忘框架。

### 2. 核心内容
LLM持续学习需在获取新技能时避免灾难性遗忘，但领域微调即便在窄更新下仍触发严重长尾遗忘，且预训练数据常不可得。本文提出ALER，一个免数据的持续学习框架，通过对抗搜索一小组潜在提示嵌入来最大化与冻结参考模型的logit差异，主动暴露高风险遗忘模式，再用在线蒸馏保留旧行为。该工作为LLM智能体的记忆保持与遗忘抑制提供新方法。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=3CLOFiyWLU](https://openreview.net/forum?id=3CLOFiyWLU)
