---
title: Reinforcement Fine-Tuning Naturally Mitigates Forgetting in Continual Post-Training
title_zh: 强化微调自然缓解持续后训练中的遗忘
authors: "Song Lai, Haohan Zhao, Rong Feng, Changyi Ma, Wenzhuo Liu, Hongbo Zhao, Xi Lin, Dong Yi, Qingfu Zhang, Hongbin Liu, Gaofeng Meng, Fei Zhu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/6c4b92466c2b046fdf36d0e8cafa951c44496790.pdf"
tags: ["query:agent-memory"]
score: 4.0
evidence: 研究持续后训练中的遗忘与知识保持
tldr: 持续后训练能让基础模型适应不断变化的下游任务，但以往研究多聚焦数据回放等方法，学习范式本身对知识保持的作用仍不清楚。本文系统对比监督微调与强化微调两种后训练范式，以Qwen2.5-VL-7B-Instruct为基础在多个多模态任务上开展实验，考察二者对持续后训练中知识保持的影响。结果显示强化微调范式能够自然缓解遗忘，为持续学习智能体的记忆保持提供了新的范式视角。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 持续后训练中学习范式本身对知识保持的作用尚不明确，现有研究多关注数据回放等具体方法。
method: 对比监督微调与强化微调两种后训练范式，在多模态任务上考察其对持续后训练知识保持的影响。
result: 以Qwen2.5-VL-7B-Instruct为基础在多个多模态任务上实验，发现两种范式在遗忘程度上存在显著差异。
conclusion: 强化微调范式可自然缓解灾难性遗忘，为持续学习中的知识保持提供新思路。
---

## Abstract
Continual post-training (CPT) is a popular and effective technique for adapting foundation models like multimodal large language models to ever-evolving downstream tasks. While existing research primarily focuses on methods like data replay, model expansion, or parameter regularization, the fundamental role of the learning paradigm remains largely unexplored. This paper presents a comparative analysis of two core post-training paradigms: supervised fine-tuning (SFT) and reinforcement fine-tuning (RFT), investigating their respective impacts on knowledge retention during CPT. Our experiments are conducted across multiple multimodal tasks, utilizing Qwen2.5-VL-7B-Instruct as the base model. The investigation yields two significant findings: (1) When continuously learning on downstream tasks, SFT leads to catastrophic forgetting of previously learned tasks. In contrast, RFT inherently preserves prior knowledge and achieves performance comparable to multi-task training. (2) RFT successfully protects and even enhances the model's general knowledge on standard benchmarks, while SFT degrades general model capabilities severely. Further analysis reveals that this stability is not primarily due to explicit mechanisms like KL penalty or chain-of-thought reasoning. We investigate RFT's learning dynamics and find that its selective update mechanism inherently prevents interference with established knowledge. Based on this insight, we propose a rollout-based instance filtering algorithm (RIF-RFT) that enhances the training efficiency of RFT by focusing on learnable samples. Our comprehensive study demonstrates the superiority of RFT as a robust paradigm for continual post-training.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
研究持续后训练中的遗忘与知识保持。

### 2. 核心内容
持续后训练能让基础模型适应不断变化的下游任务，但以往研究多聚焦数据回放等方法，学习范式本身对知识保持的作用仍不清楚。本文系统对比监督微调与强化微调两种后训练范式，以Qwen2.5-VL-7B-Instruct为基础在多个多模态任务上开展实验，考察二者对持续后训练中知识保持的影响。结果显示强化微调范式能够自然缓解遗忘，为持续学习智能体的记忆保持提供了新的范式视角。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=nvnkuqWuu3](https://openreview.net/forum?id=nvnkuqWuu3)
