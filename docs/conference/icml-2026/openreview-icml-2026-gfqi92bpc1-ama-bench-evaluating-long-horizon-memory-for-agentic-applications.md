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
evidence: 面向智能体长时程记忆的评测基准
tldr: 现有记忆评测多聚焦对话，无法刻画真实智能体由状态、动作、观测与工具输出构成的连续交互轨迹。本文提出AMA-Bench，结合真实应用中的智能体轨迹与专家标注问答，并用可扩展至任意长度的合成轨迹和规则问答补充。研究揭示当前模型在长时程智能体记忆上的不足，为智能体记忆架构提供了更贴近实际的评测标准。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有记忆基准多为对话式，无法反映真实智能体连续交互轨迹中的记忆需求。
method: 提出AMA-Bench，融合真实智能体轨迹与专家问答，并加入可扩展到任意长度的合成轨迹与规则问答。
result: 实验显示现有方法在长时程智能体记忆任务上表现存在明显不足。
conclusion: 该基准为评估智能体记忆能力提供了更贴近真实场景的标准化工具。
---

## Abstract
Large Language Models (LLMs) are increasingly used as autonomous agents in complex, long-horizon applications, where effective memory is critical for sustained performance. Yet existing memory benchmarks are largely dialogue-centric, while real agent memory consists of continuous agent-environment interaction trajectories composed of states, actions, observations, and tool outputs. To address this gap, we introduce **AMA-Bench** (**A**gent **M**emory with **A**ny length), a benchmark for evaluating long-horizon memory in realistic agentic settings. AMA-Bench combines real-world agent trajectories from representative applications with expert-curated QA, as well as synthetic trajectories that scale to arbitrary horizons with rule-based QA. Our study shows that existing memory systems underperform because they fail to capture causal and objective information and rely heavily on lossy similarity-based retrieval. We further propose **AMA-Agent**, a memory system based on causality-graph construction and tool-augmented retrieval. AMA-Agent achieves **57.22%** accuracy on AMA-Bench, outperforming the strongest baseline by **11.16%**. Resources are available at: [https://ama-bench.github.io/](https://ama-bench.github.io/).

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向智能体长时程记忆的评测基准。

### 2. 核心内容
现有记忆评测多聚焦对话，无法刻画真实智能体由状态、动作、观测与工具输出构成的连续交互轨迹。本文提出AMA-Bench，结合真实应用中的智能体轨迹与专家标注问答，并用可扩展至任意长度的合成轨迹和规则问答补充。研究揭示当前模型在长时程智能体记忆上的不足，为智能体记忆架构提供了更贴近实际的评测标准。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=GfQI92bpC1](https://openreview.net/forum?id=GfQI92bpC1)
