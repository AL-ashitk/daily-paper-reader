---
title: Near-Minimax Multi-Objective RL under Predictable Adversarial Preferences and Preference-Free Exploration in Linear MDPs
title_zh: 可预测对抗偏好与线性MDP无偏好探索下的近极小极大多目标强化学习
authors: "Mingxi Hu, Meiling Yu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/ba07bcdbfd7c0595a11db3c1c5c467417d65fb9b.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 线性MDP下的多目标强化学习与探索
tldr: 该论文研究线性MDP下的多目标强化学习问题，需支持在线变化或采集后才指定的偏好。作者针对可预测对抗偏好与无偏好探索两种协议，指出标准标量化会破坏自归一化置信界所需的鞅结构，并提出协议安全的方法。理论分析给出了近极小极大遗憾界，为多目标强化学习在动态偏好场景下的可靠学习提供了理论基础。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多目标强化学习需支持在线变化或采集后才指定的偏好，但标准归约方法在协议下并不安全。
method: 作者研究线性MDP下向量反馈的多目标强化学习，设计协议安全的归约与超体积评估方法。
result: 理论分析证明所提方法达到近极小极大遗憾界，克服了鞅结构被破坏的问题。
conclusion: 该工作为动态偏好下的多目标强化学习提供了可靠的理论保证与探索协议。
---

## Abstract
Multi-objective reinforcement learning (MORL) must often support preferences that change online or are specified only after data collection.
We study finite-horizon MORL with vector feedback in linear MDPs under two protocols: (i) predictable adversarial preferences revealed before each episode, and (ii) reward-free preference-free exploration (PFE), where exploration observes only transitions and must later answer arbitrary preference queries.
Standard reductions are protocol-unsafe: re-scalarizing past stochastic rewards with future weights breaks the martingale structure needed for self-normalized confidence bounds, and hypervolume evaluation must account for episode-start randomization, which yields a deployable convex hull of return vectors.
We propose a protocol-safe reward interface that estimates each reward coordinate via regression and performs scalarization only at query time, and we formalize deployable hypervolume semantics with a stability chain from support-function error to hypervolume error.
Consequently, we obtain filtration-safe regret bounds for any predictable preference sequence without discretizing the simplex (only $\log m$ dependence) and matching near-minimax rates in linear MDPs, as well as sharp reward-free PFE guarantees: a (near-)minimax decision-optimal query answering rate $\tilde{O}(d^2 U_{\mathrm{ret}}^2/\varepsilon^2)$ and a tight separation from explicit transition-model recovery $\Theta(d(|\mathcal{S}|-1)/\varepsilon_P^2)$.
These results connect online learning, preference-free deployment, and hypervolume-aware evaluation through a single protocol-aligned theory.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
线性MDP下的多目标强化学习与探索。

### 2. 核心内容
该论文研究线性MDP下的多目标强化学习问题，需支持在线变化或采集后才指定的偏好。作者针对可预测对抗偏好与无偏好探索两种协议，指出标准标量化会破坏自归一化置信界所需的鞅结构，并提出协议安全的方法。理论分析给出了近极小极大遗憾界，为多目标强化学习在动态偏好场景下的可靠学习提供了理论基础。

### 3. 对应检索需求
papers on reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=4X1XzWFZE3](https://openreview.net/forum?id=4X1XzWFZE3)
