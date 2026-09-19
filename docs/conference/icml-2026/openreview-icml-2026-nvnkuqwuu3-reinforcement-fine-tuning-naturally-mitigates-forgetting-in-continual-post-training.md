---
title: Reinforcement Fine-Tuning Naturally Mitigates Forgetting in Continual Post-Training
title_zh: 强化微调天然缓解持续后训练中的遗忘
authors: "Song Lai, Haohan Zhao, Rong Feng, Changyi Ma, Wenzhuo Liu, Hongbo Zhao, Xi Lin, Dong Yi, Qingfu Zhang, Hongbin Liu, Gaofeng Meng, Fei Zhu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/6c4b92466c2b046fdf36d0e8cafa951c44496790.pdf"
tags: ["query:agent-memory"]
score: 5.0
evidence: 比较SFT与RFT在持续后训练中的知识保持与遗忘
tldr: 针对持续后训练中遗忘问题、现有方法多聚焦数据回放与参数正则而忽视学习范式作用的问题，本文对监督微调与强化微调两种范式进行对比分析，在多模态任务上以Qwen2.5-VL-7B-Instruct为基座开展实验。研究发现强化微调能天然缓解持续后训练中的遗忘，更好保持已有知识，为持续学习智能体的记忆保持与遗忘缓解提供了新的范式视角。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 持续后训练存在遗忘问题，现有研究多聚焦数据回放与参数正则，忽视学习范式的作用。
method: 对比监督微调与强化微调两种范式，在多模态任务上以Qwen2.5-VL为基座分析知识保持。
result: 发现强化微调能天然缓解持续后训练中的遗忘，更好地保持已有知识。
conclusion: 为持续学习智能体的遗忘缓解与记忆保持提供了学习范式层面的新视角。
---

## Abstract
Continual post-training (CPT) is a popular and effective technique for adapting foundation models like multimodal large language models to ever-evolving downstream tasks. While existing research primarily focuses on methods like data replay, model expansion, or parameter regularization, the fundamental role of the learning paradigm remains largely unexplored. This paper presents a comparative analysis of two core post-training paradigms: supervised fine-tuning (SFT) and reinforcement fine-tuning (RFT), investigating their respective impacts on knowledge retention during CPT. Our experiments are conducted across multiple multimodal tasks, utilizing Qwen2.5-VL-7B-Instruct as the base model. The investigation yields two significant findings: (1) When continuously learning on downstream tasks, SFT leads to catastrophic forgetting of previously learned tasks. In contrast, RFT inherently preserves prior knowledge and achieves performance comparable to multi-task training. (2) RFT successfully protects and even enhances the model's general knowledge on standard benchmarks, while SFT degrades general model capabilities severely. Further analysis reveals that this stability is not primarily due to explicit mechanisms like KL penalty or chain-of-thought reasoning. We investigate RFT's learning dynamics and find that its selective update mechanism inherently prevents interference with established knowledge. Based on this insight, we propose a rollout-based instance filtering algorithm (RIF-RFT) that enhances the training efficiency of RFT by focusing on learnable samples. Our comprehensive study demonstrates the superiority of RFT as a robust paradigm for continual post-training.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
比较SFT与RFT在持续后训练中的知识保持与遗忘。

### 2. 核心内容
针对持续后训练中遗忘问题、现有方法多聚焦数据回放与参数正则而忽视学习范式作用的问题，本文对监督微调与强化微调两种范式进行对比分析，在多模态任务上以Qwen2.5-VL-7B-Instruct为基座开展实验。研究发现强化微调能天然缓解持续后训练中的遗忘，更好保持已有知识，为持续学习智能体的记忆保持与遗忘缓解提供了新的范式视角。

### 3. 对应检索需求
Identify research on memory consolidation, forgetting, and memory management for continual learning agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=nvnkuqWuu3](https://openreview.net/forum?id=nvnkuqWuu3)
