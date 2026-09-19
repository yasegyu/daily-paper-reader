---
title: "MEMO: Memory-Augmented Model Context Optimization for Robust Multi-Turn Multi-Agent LLM Games"
title_zh: MEMO：面向稳健多轮多智能体LLM博弈的记忆增强模型上下文优化
authors: "Yunfei Xie, Kevin Wang, Bobby Cheng, Jianzhu Yao, Zhizhou Sha, Alexander Duffy, Yihan Xi, Hongyuan Mei, Cheston Tan, Chen Wei, Pramod Viswanath, Zhangyang Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/4af9558429e2700edbb7d5354fd8e69260183bb0.pdf"
tags: ["query:agent-memory"]
score: 8.0
evidence: 面向多智能体LLM博弈的记忆增强上下文优化
tldr: 多轮多智能体LLM博弈评估存在显著的运行间方差，长程交互中的小偏差会跨轮累积并被多智能体耦合放大，从而偏置胜率估计并动摇比较排名，提示词选择还会进一步加剧这种不稳定。MEMO提出一种自博弈框架，把推理时上下文视为可优化的智能体对象，通过保留与探索的耦合，将自博弈轨迹蒸馏为持久的结构化记忆库，在缓解评估不稳定性的同时提升博弈表现，为多智能体交互提供了记忆增强的上下文优化方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多轮多智能体LLM博弈评估存在显著的运行间方差，长期交互中小偏差跨轮累积并被多智能体耦合放大，导致胜率估计偏差与排名不稳。
method: 提出自博弈框架MEMO，把推理时上下文视为可优化的智能体对象，通过保留与探索耦合，将自博弈轨迹蒸馏为持久记忆库。
result: 该方法缓解了评估不稳定并提升了博弈表现。
conclusion: 为多智能体LLM博弈提供记忆增强的上下文优化方案。
---

## Abstract
Multi-turn, multi-agent LLM game evaluations exhibit substantial run-to-run variance. In long-horizon interactions, small deviations compound across turns and are amplified by multi-agent coupling, biasing win rate estimates and destabilizing comparative rankings across repeated tournaments. Prompt choice exacerbates this by inducing different effective policies and interaction dynamics. We address both instability and underperformance in games with **MEMO:** (**Me**mory-augmented **MO**del context optimization), a self-play framework that treats inference-time context as an optimizable, agentic object by coupling **retention** and **exploration**. Retention distills self-play trajectories into a persistent memory bank of structured insights that act as priors; exploration combines tournament-style prompt evolution under TrueSkill with prioritized replay over decisive states. Across five text-based games and a 2,000-game budget per task, MEMO raises mean win rate from 25.1% to 49.5% for GPT-4o-mini and from 20.9% to 45.0% for Qwen-2.5-7B, while sharply reducing run-to-run dispersion. These results suggest substantial headroom in multi-agent LLM game performance and robustness can be unlocked through memory, with MEMO achieving gains in negotiation and imperfect-information settings, while RL remains more effective in perfect-information settings. Project website: https://yunfeixie233.github.io/MEMO/.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向多智能体LLM博弈的记忆增强上下文优化。

### 2. 核心内容
多轮多智能体LLM博弈评估存在显著的运行间方差，长程交互中的小偏差会跨轮累积并被多智能体耦合放大，从而偏置胜率估计并动摇比较排名，提示词选择还会进一步加剧这种不稳定。MEMO提出一种自博弈框架，把推理时上下文视为可优化的智能体对象，通过保留与探索的耦合，将自博弈轨迹蒸馏为持久的结构化记忆库，在缓解评估不稳定性的同时提升博弈表现，为多智能体交互提供了记忆增强的上下文优化方案。

### 3. 对应检索需求
shared memory and communication in multi-agent systems。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=bYDjZyqKxq](https://openreview.net/forum?id=bYDjZyqKxq)
