---
title: "RGMem: Renormalization Group–inspired Memory Evolution for Language Agents"
title_zh: RGMem：受重整化群启发的语言智能体记忆演化
authors: "Ao Tian, Yunfeng Lu, Xinxin Fan, Changhao Wang, Lanzhi Zhou, Yeyao Zhang, Yanfang Liu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/a9944c66058e0655a6bd75242b0d62071a06444d.pdf"
tags: ["query:agent-memory"]
score: 9.0
evidence: 面向语言智能体长期情景记忆的自演化记忆框架
tldr: 基于大模型的对话智能体受限于有限上下文窗口与静态参数记忆，难以建模跨会话的长期用户状态，现有检索增强与显式记忆方法多停留在事实层面，难以从演化且冲突的对话中提炼稳定偏好与深层特质。作者提出RGMem自演化记忆框架，借鉴重整化群的多尺度组织思想，将长期对话记忆建模为多尺度演化过程。该框架把情景交互逐级转化为抽象状态，从而跨会话整合信息并蒸馏稳定用户特质。工作为语言智能体的长期个性化记忆提供新范式。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 大模型对话智能体受限于有限上下文与静态参数记忆，现有方法多停留事实层面，难以从演化冲突对话中提炼稳定偏好与深层特质。
method: 作者提出RGMem自演化记忆框架，借鉴重整化群的多尺度组织思想，将长期对话记忆建模为多尺度演化过程。
result: 该框架把情景交互逐级转化为抽象状态，跨会话整合信息并缓解事实冲突，蒸馏出稳定的用户偏好与深层特质。
conclusion: 工作为语言智能体的长期个性化记忆提供新范式，推动跨会话用户状态建模研究。
---

## Abstract
Personalized and continuous interactions are critical for LLM-based conversational agents, yet finite context windows and static parametric memory hinder the modeling of long-term, cross-session user states. Existing approaches, including retrieval-augmented generation and explicit memory systems, primarily operate at the fact level, making it difficult to distill stable preferences and deep user traits from evolving and potentially conflicting dialogues.To address this challenge, we propose RGMem, a self-evolving memory framework inspired by the renormalization group (RG) perspective on multi-scale organization and emergence. RGMem models long-term conversational memory as a multi-scale evolutionary process: episodic interactions are transformed into semantic facts and user insights, which are then progressively integrated through hierarchical coarse-graining, thresholded updates, and rescaling into a dynamically evolving user profile.By explicitly separating fast-changing evidence from slow-varying traits and enabling non-linear, phase-transition-like dynamics, RGMem enables robust personalization beyond flat retrieval or static summarization. Extensive experiments on the LOCOMO and PersonaMem benchmarks demonstrate that RGMem consistently outperforms SOTA memory systems, achieving stronger cross-session continuity and improved adaptation to evolving user preferences.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向语言智能体长期情景记忆的自演化记忆框架。

### 2. 核心内容
基于大模型的对话智能体受限于有限上下文窗口与静态参数记忆，难以建模跨会话的长期用户状态，现有检索增强与显式记忆方法多停留在事实层面，难以从演化且冲突的对话中提炼稳定偏好与深层特质。作者提出RGMem自演化记忆框架，借鉴重整化群的多尺度组织思想，将长期对话记忆建模为多尺度演化过程。该框架把情景交互逐级转化为抽象状态，从而跨会话整合信息并蒸馏稳定用户特质。工作为语言智能体的长期个性化记忆提供新范式。

### 3. 对应检索需求
memory mechanisms in autonomous agents and agent memory architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=FtvNZxhW9W](https://openreview.net/forum?id=FtvNZxhW9W)
