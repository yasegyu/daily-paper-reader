---
title: "Turning Back Without Forgetting: Selective Backward Refinement for Parameter-Efficient Continual Learning"
title_zh: 无遗忘地回望：面向参数高效持续学习的选择性反向精炼
authors: "Anushka Tiwari, Kaiyi Ji"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/cdf2fb7ed70ac5023ce5ed72e079ea70eaad5a02.pdf"
tags: ["query:agent-memory"]
score: 4.0
evidence: 持续学习中的反向知识迁移与缓解灾难性遗忘
tldr: 基于提示的参数高效持续学习虽能通过隔离任务提示缓解灾难性遗忘，却也阻碍了后续任务改进先前任务，反向知识迁移长期被忽视。本文提出无回放的SABER框架，利用基于提示梯度几何与损失分布相似度的任务相关性准则判断何时进行反向精炼，并通过限制更新方向保证精炼安全。该框架实现了受控的正向反向知识迁移，为持续学习中的知识保持与再利用提供了新方法。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 提示隔离虽缓解灾难性遗忘，却限制了后续任务对先前任务的反向知识迁移。
method: 提出无回放框架SABER，基于提示梯度几何与损失分布相似度判断并安全执行反向精炼。
result: 在参数高效持续学习设定下实现受控的反向知识迁移，提升知识再利用。
conclusion: 为持续学习中的遗忘缓解与知识迁移平衡提供了新的精炼框架。
---

## Abstract
While prompt-based parameter-efficient continual learning mitigates catastrophic forgetting by isolating task-specific prompts, this isolation also limits later tasks from improving earlier ones, leaving backward knowledge transfer underexplored. We address this limitation by proposing Selective bAckward refinement for positive Backward knowledge transfER (SABER), a replay-free framework that enables controlled backward transfer in prompt-based continual learning. SABER determines when backward refinement is beneficial using complementary task-correlation criteria based on prompt-gradient geometry and loss-distribution similarity, and how to perform refinement safely by restricting updates to non-interfering directions in the prompt parameter space. Extensive experiments across multiple continual learning benchmarks, and diverse pretrained backbones, including T5-Large, LLaMA, and Qwen, demonstrate that SABER consistently achieves positive backward transfer while maintaining strong overall average performance.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
持续学习中的反向知识迁移与缓解灾难性遗忘。

### 2. 核心内容
基于提示的参数高效持续学习虽能通过隔离任务提示缓解灾难性遗忘，却也阻碍了后续任务改进先前任务，反向知识迁移长期被忽视。本文提出无回放的SABER框架，利用基于提示梯度几何与损失分布相似度的任务相关性准则判断何时进行反向精炼，并通过限制更新方向保证精炼安全。该框架实现了受控的正向反向知识迁移，为持续学习中的知识保持与再利用提供了新方法。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=zD2ZhFSexc](https://openreview.net/forum?id=zD2ZhFSexc)
