---
title: Maximum Likelihood Reinforcement Learning
title_zh: 最大似然强化学习
authors: "Fahim Tajwar, Guanning Zeng, Yueer Zhou, Yuda Song, Daman Arora, Yiding Jiang, Jeff Schneider, Ruslan Salakhutdinov, Haiwen Feng, Andrea Zanette"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/41d824814d679ade15cdc28c1f237571aa12a496.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 强化学习目标的理论基础
tldr: 在目标只能通过采样评估且反馈为终端二值的情形下，最大似然本是自然框架，但实践中却用强化学习作为绕过不可微性的变通。本文证明标准期望回报RL仅是似然的一阶近似，进而提出最大似然强化学习MaxRL，构造由计算量索引、在期望回报RL与最大似然之间插值的采样目标族。该工作弥合了RL与最大似然之间的理论错配，为采样式训练提供了更自然的优化目标。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 当反馈为终端二值且目标只能采样评估时，标准期望回报强化学习只是最大似然的一阶近似。
method: 提出MaxRL，构造由计算量索引、在期望回报RL与最大似然间插值的采样式目标族。
result: 理论证明标准期望回报RL仅为一阶近似，并给出随采样计算量扩展的目标族。
conclusion: 弥合强化学习与最大似然之间的错配，提供更自然的训练目标。
---

## Abstract
Reinforcement learning (RL) is the method of choice for training models in setups where the objective function can only be evaluated by sampling from the model. Our key observation is that when the feedback is terminal and binary, models implicitly induce a likelihood over correct rollouts. Maximum likelihood would be the natural framework in such settings, but RL is used instead as a workaround to the non-differentiability. We prove that the standard, expected-reward RL formulation is only a first-order approximation of the likelihood. To remedy this mismatch, we introduce **Maximum Likelihood Reinforcement Learning (MaxRL)**, a compute-indexed family of sample-based objectives that interpolate between expected-reward RL and maximum likelihood as sampling compute is scaled. The resulting objective is a one-line change to standard RL implementations. MaxRL Pareto-dominates existing methods in all tested models and tasks, achieves up to $\mathbf{20\times}$ gains in test-time scaling efficiency over GRPO, and scales more favorably with additional training data and compute.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
强化学习目标的理论基础。

### 2. 核心内容
在目标只能通过采样评估且反馈为终端二值的情形下，最大似然本是自然框架，但实践中却用强化学习作为绕过不可微性的变通。本文证明标准期望回报RL仅是似然的一阶近似，进而提出最大似然强化学习MaxRL，构造由计算量索引、在期望回报RL与最大似然之间插值的采样目标族。该工作弥合了RL与最大似然之间的理论错配，为采样式训练提供了更自然的优化目标。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=EeuLO2BjFN](https://openreview.net/forum?id=EeuLO2BjFN)
