---
title: "Turning Back Without Forgetting: Selective Backward Refinement for Parameter-Efficient Continual Learning"
title_zh: 不忘却地回望：面向参数高效持续学习的选择性反向精炼
authors: "Anushka Tiwari, Kaiyi Ji"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/cdf2fb7ed70ac5023ce5ed72e079ea70eaad5a02.pdf"
tags: ["query:agent-memory"]
score: 5.0
evidence: 无回放的持续学习框架在不忘却前提下控制反向迁移
tldr: 基于提示的参数高效持续学习虽通过隔离任务提示缓解灾难性遗忘，但这种隔离也限制了后续任务改进早期任务，反向知识迁移研究不足。本文提出SABER，一种无回放框架，利用提示梯度几何与损失分布相似性判断反向精炼的时机，并通过限制更新方向安全执行精炼。该方法在不引起遗忘的前提下实现了受控的正向反向迁移。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 提示隔离虽缓解灾难性遗忘，却限制后续任务改进早期任务，反向知识迁移未被充分探索。
method: 提出无回放框架SABER，用提示梯度几何与损失分布相似性判断精炼时机并限制更新方向以安全精炼。
result: 该方法在避免灾难性遗忘的同时实现受控的反向知识迁移，改善早期任务的性能。
conclusion: 选择性反向精炼为持续学习中的知识迁移与记忆保持提供了新思路。
---

## Abstract
While prompt-based parameter-efficient continual learning mitigates catastrophic forgetting by isolating task-specific prompts, this isolation also limits later tasks from improving earlier ones, leaving backward knowledge transfer underexplored. We address this limitation by proposing Selective bAckward refinement for positive Backward knowledge transfER (SABER), a replay-free framework that enables controlled backward transfer in prompt-based continual learning. SABER determines when backward refinement is beneficial using complementary task-correlation criteria based on prompt-gradient geometry and loss-distribution similarity, and how to perform refinement safely by restricting updates to non-interfering directions in the prompt parameter space. Extensive experiments across multiple continual learning benchmarks, and diverse pretrained backbones, including T5-Large, LLaMA, and Qwen, demonstrate that SABER consistently achieves positive backward transfer while maintaining strong overall average performance.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
无回放的持续学习框架在不忘却前提下控制反向迁移。

### 2. 核心内容
基于提示的参数高效持续学习虽通过隔离任务提示缓解灾难性遗忘，但这种隔离也限制了后续任务改进早期任务，反向知识迁移研究不足。本文提出SABER，一种无回放框架，利用提示梯度几何与损失分布相似性判断反向精炼的时机，并通过限制更新方向安全执行精炼。该方法在不引起遗忘的前提下实现了受控的正向反向迁移。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=zD2ZhFSexc](https://openreview.net/forum?id=zD2ZhFSexc)
