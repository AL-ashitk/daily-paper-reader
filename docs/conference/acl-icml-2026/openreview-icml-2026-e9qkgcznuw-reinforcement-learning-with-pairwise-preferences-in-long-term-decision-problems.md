---
title: Reinforcement Learning with Pairwise Preferences in Long-Term Decision Problems
title_zh: 长期决策问题中基于成对偏好的强化学习
authors: "Jonathan Colaço Carr, Prakash Panangaden, Doina Precup, Benjamin Van Roy"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/da4b34abc83c37e88fe88853cdfaa6cfadbfc1b1.pdf"
tags: ["query:rl"]
score: 8.0
evidence: 基于成对偏好的强化学习理论
tldr: 强化学习通常把目标定义为最大化标量奖励的期望，但成对偏好往往更易指定，且能表达标量奖励无法刻画的目标。然而现有多数偏好型方法在长时程问题上效率低下，且缺乏马尔可夫策略相对历史依赖策略的性能保证。本文提出马尔可夫决策竞赛这一新的问题模型，并证明平稳策略的相关性能保证。该工作弥合了历史依赖策略与马尔可夫策略之间的理论与实践差距，为偏好型长期决策提供了有保证的强化学习框架。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 标量奖励难以表达某些目标，而成对偏好方法在长时程问题中效率低且缺乏策略性能保证。
method: 提出马尔可夫决策竞赛这一新问题模型，并证明平稳策略的性能保证。
result: 弥合了历史依赖策略与马尔可夫策略之间的理论与实践差距。
conclusion: 为偏好型长期决策提供高效且有理论保证的强化学习框架。
---

## Abstract
Reinforcement-learning problems typically define the goal as maximizing the expected value of a scalar reward function. But, pairwise preferences are often easier to specify than scalar rewards, and they express certain goals that scalar rewards cannot. Methods for reinforcement learning with pairwise preferences have thus received growing interest. Unfortunately, these methods are inefficient in problems with long time horizons, and they lack guarantees on the performance of Markov policies relative to history-dependent policies, which bridge the theory and practice of reinforcement learning. We therefore propose the *Markov decision contest* as a new problem model for reinforcement learning with pairwise preferences. We prove that stationary Markov policies are optimal among all history-dependent policies, that solving a Markov decision contest exactly is in P, and that a simple iterative algorithm converges to an optimal policy at a sublinear rate. Lastly, in a set of high-dimensional decision problems with long time horizons, we show that our approximate algorithm is significantly more learning-efficient than prior work.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
基于成对偏好的强化学习理论。

### 2. 核心内容
强化学习通常把目标定义为最大化标量奖励的期望，但成对偏好往往更易指定，且能表达标量奖励无法刻画的目标。然而现有多数偏好型方法在长时程问题上效率低下，且缺乏马尔可夫策略相对历史依赖策略的性能保证。本文提出马尔可夫决策竞赛这一新的问题模型，并证明平稳策略的相关性能保证。该工作弥合了历史依赖策略与马尔可夫策略之间的理论与实践差距，为偏好型长期决策提供了有保证的强化学习框架。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=E9QkGczNUw](https://openreview.net/forum?id=E9QkGczNUw)
