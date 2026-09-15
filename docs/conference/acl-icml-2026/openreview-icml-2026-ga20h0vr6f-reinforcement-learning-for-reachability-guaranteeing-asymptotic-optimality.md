---
title: "Reinforcement Learning for Reachability: Guaranteeing Asymptotic Optimality"
title_zh: 面向可达性的强化学习：保证渐近最优性
authors: "Amogh Palasamudram, Jakub Svoboda, Suguman Bansal, Krishnendu Chatterjee"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/b9e231717dfa8316240f34b1e452abdbf0a3e890.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 面向可达性规范并保证渐近最优的强化学习
tldr: 面向可达性规范的强化学习在序贯决策中至关重要，但其理论保证仍不充分，已有方法虽能达到渐近最优却对收敛动态刻画有限。本文提出一种新方法，基于带假设的PAC学习，通过迭代细化并估计原本未知的最小转移概率等MDP内部参数，获得对收敛过程的更深入理解。该方法能在有限时间内以高置信度给出近最优策略，并保证渐近最优性，深化了可达性强化学习的理论基础。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 可达性强化学习理论保证不足，已有渐近最优方法对收敛动态刻画有限。
method: 基于带假设的PAC学习，迭代细化估计最小转移概率等未知MDP参数。
result: 能在有限时间以高置信度获得近最优策略并保证渐近最优性。
conclusion: 为可达性强化学习提供更深入的收敛理论与最优性保证。
---

## Abstract
Reinforcement learning (RL) for reachability specifications is fundamental in sequential decision-making, yet theoretical guarantees remain less explored. A recent work achieves asymptotic convergence to optimal policies. However, this approach provides limited insight into convergence dynamics. In this work, we present an alternative approach that provides deeper theoretical insights into convergence. Our approach builds on PAC learning with assumptions. PAC learning guarantees near-optimal policies with high confidence in finite time but requires knowing internal MDP parameters like minimum transition probability. We argue that while these parameters are unknown in RL, they can be iteratively refined and estimated with increasing accuracy. By iteratively satisfying PAC conditions, we show that exact optimality can be achieved in the limit. Empirical evaluations on standard benchmarks validate our theoretical insights into convergence dynamics.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向可达性规范并保证渐近最优的强化学习。

### 2. 核心内容
面向可达性规范的强化学习在序贯决策中至关重要，但其理论保证仍不充分，已有方法虽能达到渐近最优却对收敛动态刻画有限。本文提出一种新方法，基于带假设的PAC学习，通过迭代细化并估计原本未知的最小转移概率等MDP内部参数，获得对收敛过程的更深入理解。该方法能在有限时间内以高置信度给出近最优策略，并保证渐近最优性，深化了可达性强化学习的理论基础。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=ga20H0vR6f](https://openreview.net/forum?id=ga20H0vR6f)
