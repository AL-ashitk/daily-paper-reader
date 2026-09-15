---
title: "Learning to Explore: Scaling Agentic Reasoning via Exploration-Aware Policy Optimization"
title_zh: 学会探索：通过探索感知策略优化扩展智能体推理
authors: "Xingyuan Hua, Sheng Yue, Ju Ren"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/1eaaa70094a1d7c3a9a83f5516f18234624bca0c.pdf"
tags: ["query:rl"]
score: 8.0
evidence: 面向自适应智能体推理的探索感知强化学习框架
tldr: 现有智能体测试时扩展方法采用无差别探索策略，无法自适应判断何时真正需要探索。本文提出探索感知强化学习框架，使大语言模型智能体仅在高不确定性时进行探索，并通过变分推断设计细粒度奖励函数，显式评估探索动作提升未来决策的潜力，同时引入探索感知分组机制。实验表明该方法能更高效地分配探索预算，提升智能体推理的可扩展性与决策质量。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有智能体方法采用无差别探索，无法判断何时真正需要探索。
method: 提出探索感知强化学习框架，用变分推断奖励与探索分组机制自适应探索。
result: 使智能体仅在高不确定性时探索，更高效地提升推理与决策表现。
conclusion: 为智能体推理的可扩展测试时探索提供了自适应且高效的强化学习方案。
---

## Abstract
Recent advancements in agentic test-time scaling allow models to gather environmental feedback before committing to final actions. A key limitation of existing methods is that they typically employ undifferentiated exploration strategies, lacking the ability to adaptively distinguish when exploration is truly required. In this paper, we propose an exploration-aware reinforcement learning framework that enables LLM agents to adaptively explore only when uncertainty is high. Our method introduces a fine-grained reward function via variational inference that explicitly evaluates exploratory actions by estimating their potential to improve future decision-making, together with an exploration-aware grouping mechanism that separates exploratory actions from task-completion actions during optimization. By targeting informational gaps, this design allows agents to explore selectively and transition to execution as soon as the task context is clear. Empirically, we demonstrate that our approach achieves consistent improvements across a range of challenging text-based and GUI-based agent benchmarks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向自适应智能体推理的探索感知强化学习框架。

### 2. 核心内容
现有智能体测试时扩展方法采用无差别探索策略，无法自适应判断何时真正需要探索。本文提出探索感知强化学习框架，使大语言模型智能体仅在高不确定性时进行探索，并通过变分推断设计细粒度奖励函数，显式评估探索动作提升未来决策的潜力，同时引入探索感知分组机制。实验表明该方法能更高效地分配探索预算，提升智能体推理的可扩展性与决策质量。

### 3. 对应检索需求
algorithms for reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=YNPHJ2A2oV](https://openreview.net/forum?id=YNPHJ2A2oV)
