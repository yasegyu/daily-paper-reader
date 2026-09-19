---
title: Investigating Component Contributions in Multi-Agent ML Systems
title_zh: 多智能体机器学习系统中组件贡献的探究
authors: "Junsung Kim, Ilia Mireskandari, Seungwan Son, Yifan Zhou, Khizer Shahid, Dylan Yihan Dai"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/866ee982631523ab881bc1761fa3547bed3ed10e.pdf"
tags: ["query:agent-memory"]
score: 5.0
evidence: 在多智能体架构组件中消融记忆管理
tldr: 面向机器学习的自主智能体系统整合了多智能体分解、迭代精化、记忆管理与规划等多种技术，但难以判断哪些组件真正带来性能提升，且现有基准存在数据污染与过时基线问题。作者开展四千余次受控消融实验，并构建包含25个活跃竞赛的无污染动态基准K-live。结果系统性地厘清了记忆管理等组件对整体性能的贡献，为多智能体系统设计提供了可靠评估依据。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多智能体系统混合了记忆管理等多种组件，但难以判断哪些组件真正驱动性能。
method: 开展四千余次受控消融实验，并提出无数据污染的动态基准K-live。
result: 实验系统性地量化了记忆管理等各架构组件对性能的贡献。
conclusion: 为多智能体系统的组件设计与评估提供了可靠依据。
---

## Abstract
Autonomous agents for machine learning engineering have advanced rapidly, yet comparing their effectiveness remains difficult. Existing systems combine different techniques---multi-agent decomposition, iterative refinement, memory management, and planning---in varying configurations, making it unclear which components actually drive performance. Complicating evaluation, existing benchmarks rely on historical competitions whose data likely contaminates LLM training corpora and whose static baselines reflect outdated human performance. To address this, we conduct over 4,000 controlled experiments systematically ablating architectural components, alongside K-live, a new benchmark of 25 active competitions that provides a contamination-free, dynamic evaluation environment. Our findings challenge common design assumptions: iterative feedback contributes more than architectural complexity, and multi-agent coordination can hurt as often as it helps. These results provide concrete guidance for practitioners building ML engineering agents.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
在多智能体架构组件中消融记忆管理。

### 2. 核心内容
面向机器学习的自主智能体系统整合了多智能体分解、迭代精化、记忆管理与规划等多种技术，但难以判断哪些组件真正带来性能提升，且现有基准存在数据污染与过时基线问题。作者开展四千余次受控消融实验，并构建包含25个活跃竞赛的无污染动态基准K-live。结果系统性地厘清了记忆管理等组件对整体性能的贡献，为多智能体系统设计提供了可靠评估依据。

### 3. 对应检索需求
Find top tier AI conference papers on memory architectures for autonomous agents and large language model agents.

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=FOfvTwBGUX](https://openreview.net/forum?id=FOfvTwBGUX)
