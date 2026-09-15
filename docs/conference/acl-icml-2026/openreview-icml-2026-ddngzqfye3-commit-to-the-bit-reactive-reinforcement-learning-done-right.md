---
title: "Commit to the Bit: Reactive Reinforcement Learning Done Right"
title_zh: 坚守比特：正确实现反应式强化学习
authors: "Onno Eberhard, Claire Vernade, Michael Muehlebach"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/812fe53422fd89af54685ae0b323901b295bec6d.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 无需马尔可夫假设的反应式最优策略Committed Q学习
tldr: "强化学习算法通常依赖马尔可夫假设，但实际环境往往部分可观测或需要函数近似。本文研究确定性观测（硬状态聚合）下的最优反应式策略学习，提出新算法Committed Q-learning，并在称为rewire-robustness的直观假设下证明其几乎必然收敛。该假设严格弱于以往使用的q*-可实现条件，从而在更现实的非马尔可夫设定下为反应式策略学习提供了理论保证。"
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多数强化学习算法依赖马尔可夫假设，与实际部分可观测环境不符。
method: 针对确定性观测的反应式策略学习，提出Committed Q-learning算法。
result: 在更弱的rewire-robustness假设下证明了几乎必然收敛到最优反应式策略。
conclusion: 在更现实的非马尔可夫设定下为反应式策略学习建立了新的理论保证。
---

## Abstract
Reinforcement learning algorithms are commonly analyzed (and designed) under the Markov assumption. This is unrealistic, as most environments encountered in practice are either partially observable, or require function approximation that restricts the agent to access non-Markovian state features. We consider the problem of learning an optimal reactive policy in a finite environment with deterministic observations (or equivalently, hard state aggregation). We introduce a new algorithm, _Committed Q-learning_, and prove almost-sure convergence to the optimal reactive policy under an intuitive assumption we call _rewire-robustness_. This assumption is strictly weaker than the $q_\star$-realizability condition used in prior work. Our algorithm is a variant of classical Q-learning in which the behavior policy commits to a single action upon entering a feature, and only resamples actions when the observed feature changes. A crucial part of our analysis is the introduction of _quasi-Markov_ environments.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
无需马尔可夫假设的反应式最优策略Committed Q学习。

### 2. 核心内容
强化学习算法通常依赖马尔可夫假设，但实际环境往往部分可观测或需要函数近似。本文研究确定性观测（硬状态聚合）下的最优反应式策略学习，提出新算法Committed Q-learning，并在称为rewire-robustness的直观假设下证明其几乎必然收敛。该假设严格弱于以往使用的q*-可实现条件，从而在更现实的非马尔可夫设定下为反应式策略学习提供了理论保证。

### 3. 对应检索需求
algorithms for reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=DdNgzQfYE3](https://openreview.net/forum?id=DdNgzQfYE3)
