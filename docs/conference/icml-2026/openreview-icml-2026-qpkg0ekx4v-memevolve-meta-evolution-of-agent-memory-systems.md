---
title: "MemEvolve: Meta-Evolution of Agent Memory Systems"
title_zh: MemEvolve：智能体记忆系统的元演化
authors: "Guibin Zhang, Haotian Ren, Chong Zhan, Junhao Wang, He Zhu, Wangchunshu Zhou, Shuicheng YAN"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/1e41a1afd50901e4fabd439045aa390f5d0448f8.pdf"
tags: ["query:agent-memory"]
score: 10.0
evidence: 联合演化智能体记忆架构与经验的元演化
tldr: 自演化记忆系统正重塑LLM智能体的演化范式，但以往多依赖人工设计的记忆架构存储轨迹、蒸馏经验与合成工具，其记忆系统本身是静态的，无法针对多样任务进行元适配。作者提出MemEvolve元演化框架，联合演化智能体的经验知识与记忆架构。该方法使智能体系统不仅能积累经验，还能自适应调整记忆结构，为智能体记忆架构的自动化演进开辟了新方向。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 以往智能体记忆多依赖人工设计的静态架构，虽支持智能体演化，却无法针对多样任务对记忆架构本身进行元适配。
method: 提出MemEvolve元演化框架，联合演化智能体的经验知识与记忆架构，使二者协同自适应调整。
result: 该框架让智能体不仅积累经验，还能自适应地重构记忆结构，提升了跨多样任务情境的适应能力。
conclusion: 表明记忆架构可与经验协同元演化，突破静态人工记忆系统的局限。
---

## Abstract
Self-evolving memory systems are rapidly reshaping the evolutionary paradigm of large language model (LLM)-based agents. Prior work has predominantly relied on manually engineered memory architectures to store trajectories, distill experience, and synthesize reusable tools, enabling agents to evolve on the fly within environment interactions. However, this paradigm is fundamentally constrained by the \textit{staticity} of the memory system itself: while memory facilitates agent-level evolving, the underlying memory architecture cannot be meta-adapted to diverse task contexts. To address this gap, we propose MemEvolve, a meta-evolutionary framework that jointly evolves agents’ experiential knowledge and their memory architecture, allowing agent systems not only to accumulate experience but also to progressively refine how they learn from it. To ground MemEvolve in prior work and promote openness in future self-evolving systems, we introduce EvolveLab, a unified memory codebase that distills twelve representative memory systems into a modular design space (\textit{encode}, \textit{store}, \textit{retrieve}, \textit{manage}), providing a standardized implementation substrate and a fair experimental arena. Extensive evaluations on four challenging agentic benchmarks show that MemEvolve delivers (i) substantial performance gains, improving frameworks such as SmolAgent and Flash-Searcher by up to $17.06\%$, and (ii) strong cross-task and cross-LLM generalization, yielding memory architectures that transfer effectively across diverse benchmarks and backbones.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
联合演化智能体记忆架构与经验的元演化。

### 2. 核心内容
自演化记忆系统正重塑LLM智能体的演化范式，但以往多依赖人工设计的记忆架构存储轨迹、蒸馏经验与合成工具，其记忆系统本身是静态的，无法针对多样任务进行元适配。作者提出MemEvolve元演化框架，联合演化智能体的经验知识与记忆架构。该方法使智能体系统不仅能积累经验，还能自适应调整记忆结构，为智能体记忆架构的自动化演进开辟了新方向。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=qpkG0eKx4v](https://openreview.net/forum?id=qpkG0eKx4v)
