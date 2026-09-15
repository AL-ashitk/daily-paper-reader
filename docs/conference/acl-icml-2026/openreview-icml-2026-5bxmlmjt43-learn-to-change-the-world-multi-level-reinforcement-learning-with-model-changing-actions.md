---
title: "Learn to change the world: Multi-level reinforcement learning with model-changing actions"
title_zh: 学会改变世界：带模型改变动作的多层强化学习
authors: "Ziqing Lu, Babak Hassibi, Lifeng Lai, Weiyu Xu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/316d60d574dd0e8a2310e72cd4e55e84b7891886.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 具有可配置MDP模型改变动作的多层强化学习
tldr: 传统强化学习假设环境给定且固定，智能体只能被动适应。本文提出多层可配置时变马尔可夫决策过程（MCTVMDP），其中下层MDP的转移函数可通过上层模型改变动作进行配置，使智能体能够主动重构世界动态以提升回报。作者设计了相应的双层优化目标与求解方法，展示了主动改变模型相较被动适应可获得更高奖励，拓展了强化学习对环境建模的假设边界。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 传统强化学习假设环境固定，智能体只能被动适应而无法主动改变世界动态。
method: 提出多层可配置时变MDP，用上层模型改变动作配置下层非平稳转移函数。
result: 通过重构转移过程，智能体可获得比被动适应更高的长期回报。
conclusion: 突破了环境固定的假设，为主动建模与改造环境的强化学习提供新范式。
---

## Abstract
Reinforcement learning usually assumes a given or sometimes even fixed environment in which an agent seeks an optimal policy to maximize its long-term discounted reward. In contrast, we consider agents that are not limited to passive adaptations: they instead have model-changing actions that actively modify the RL model of world dynamics itself. Reconfiguring the underlying transition processes can potentially increase the agents' rewards. Motivated by this setting, we introduce the multi-layer configurable time-varying Markov decision process (MCTVMDP). In an MCTVMDP, the lower-level MDP has a non-stationary transition function that is configurable through upper-level model-changing actions. The agent's objective consists of two parts: Optimize the configuration policies in the upper-level MDP and optimize the primitive action policies in the lower-level MDP to jointly improve its expected long-term reward.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
具有可配置MDP模型改变动作的多层强化学习。

### 2. 核心内容
传统强化学习假设环境给定且固定，智能体只能被动适应。本文提出多层可配置时变马尔可夫决策过程（MCTVMDP），其中下层MDP的转移函数可通过上层模型改变动作进行配置，使智能体能够主动重构世界动态以提升回报。作者设计了相应的双层优化目标与求解方法，展示了主动改变模型相较被动适应可获得更高奖励，拓展了强化学习对环境建模的假设边界。

### 3. 对应检索需求
model-based reinforcement learning papers。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=5BXMlmjt43](https://openreview.net/forum?id=5BXMlmjt43)
