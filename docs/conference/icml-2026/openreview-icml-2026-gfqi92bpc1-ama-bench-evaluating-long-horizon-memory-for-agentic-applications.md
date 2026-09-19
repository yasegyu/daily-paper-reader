---
title: "AMA-Bench: Evaluating Long-Horizon Memory for Agentic Applications"
title_zh: AMA-Bench：面向智能体应用的长时程记忆评测
authors: "Yujie Zhao, Boqin Yuan, Junbo Huang, Haocheng Yuan, Zhongming Yu, Haozhou Xu, Lanxiang Hu, Abhilash Shankarampeta, Zimeng Huang, Wentao Ni, Yuandong Tian, Jishen Zhao"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/7ed1b741cbaf7f73630f6eb88e2ab8f95b67d86d.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 面向真实智能体应用的长时程记忆评测基准
tldr: 现有记忆基准多聚焦对话，而真实智能体记忆由状态、动作、观测与工具输出构成的连续交互轨迹组成。本文提出AMA-Bench，一个面向任意长度智能体记忆的评测基准，融合真实应用轨迹与专家标注问答，并提供可扩展至任意时程的合成轨迹与规则化问答。研究揭示当前记忆方法在长时程智能体场景下的不足，为智能体长期记忆研究提供标准化评测工具。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有记忆基准多为对话中心，无法反映由状态、动作、观测构成真实智能体交互轨迹。
method: 构建AMA-Bench基准，融合真实应用轨迹与专家问答，并用合成轨迹扩展时程。
result: 揭示现有记忆方法在真实长时程智能体场景中的能力差距。
conclusion: 为智能体长期记忆研究提供标准化、可扩展的评测基准。
---

## Abstract
Large Language Models (LLMs) are increasingly used as autonomous agents in complex, long-horizon applications, where effective memory is critical for sustained performance. Yet existing memory benchmarks are largely dialogue-centric, while real agent memory consists of continuous agent-environment interaction trajectories composed of states, actions, observations, and tool outputs. To address this gap, we introduce **AMA-Bench** (**A**gent **M**emory with **A**ny length), a benchmark for evaluating long-horizon memory in realistic agentic settings. AMA-Bench combines real-world agent trajectories from representative applications with expert-curated QA, as well as synthetic trajectories that scale to arbitrary horizons with rule-based QA. Our study shows that existing memory systems underperform because they fail to capture causal and objective information and rely heavily on lossy similarity-based retrieval. We further propose **AMA-Agent**, a memory system based on causality-graph construction and tool-augmented retrieval. AMA-Agent achieves **57.22%** accuracy on AMA-Bench, outperforming the strongest baseline by **11.16%**. Resources are available at: [https://ama-bench.github.io/](https://ama-bench.github.io/).

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向真实智能体应用的长时程记忆评测基准。

### 2. 核心内容
现有记忆基准多聚焦对话，而真实智能体记忆由状态、动作、观测与工具输出构成的连续交互轨迹组成。本文提出AMA-Bench，一个面向任意长度智能体记忆的评测基准，融合真实应用轨迹与专家标注问答，并提供可扩展至任意时程的合成轨迹与规则化问答。研究揭示当前记忆方法在长时程智能体场景下的不足，为智能体长期记忆研究提供标准化评测工具。

### 3. 对应检索需求
Search for papers about long term memory, episodic memory, and memory retrieval in interactive agent systems.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=GfQI92bpC1](https://openreview.net/forum?id=GfQI92bpC1)
