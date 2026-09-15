---
title: Revisiting Regularized Policy Optimization for Stable and Efficient Reinforcement Learning in Two-Player Games
title_zh: 重新审视正则化策略优化：双人博弈中稳定高效的强化学习
authors: "Kazuki Ota, Takayuki Osa, Motoki Omura, Tatsuya Harada"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/6c57d79bfd131442d14682a09aa60272e6198f22.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 双人零和博弈中带收敛保证的正则化策略优化
tldr: 针对双人零和博弈中策略优化稳定性与效率不足的问题，本文重新审视结合反向KL正则与熵正则的策略优化方法，在规范式博弈与有限长度博弈两种理论设定下分析策略更新规则的稳定性，给出新的收敛性保证，并推导出实用的无模型强化学习算法。数值实验验证了理论结果，为博弈场景下的稳定高效强化学习提供了理论与实践支持。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 双人零和博弈中的策略优化在稳定性与样本效率方面仍存在不足。
method: 重新审视反向KL与熵正则结合的策略优化，在两类博弈设定下分析并推导无模型算法。
result: 给出新的收敛性保证，并通过合成博弈与数值实验验证理论。
conclusion: 为双人博弈场景提供了稳定高效且具理论保证的强化学习策略优化方法。
---

## Abstract
Two-player games such as board games have long been used as traditional benchmarks for reinforcement learning. This work revisits a policy optimization method with reverse Kullback-Leibler regularization and entropy regularization and analyzes this combination in two-player zero-sum settings from theoretical and empirical perspectives. From a theoretical perspective, we investigate the stability of the policy update rule in two theoretical settings: game-theoretic normal-form games and finite-length games. We provide novel convergence guarantees and verify our theoretical results through numerical experiments on synthetic games. From an empirical perspective, we derive a practical model-free reinforcement learning algorithm based on the regularized policy optimization. We validate the training efficiency of our algorithm through comprehensive experiments on five board games: Animal Shogi, Gardner Chess, Go, Hex, and Othello. Experimental results show that our agent learns more efficiently than existing methods across environments.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
双人零和博弈中带收敛保证的正则化策略优化。

### 2. 核心内容
针对双人零和博弈中策略优化稳定性与效率不足的问题，本文重新审视结合反向KL正则与熵正则的策略优化方法，在规范式博弈与有限长度博弈两种理论设定下分析策略更新规则的稳定性，给出新的收敛性保证，并推导出实用的无模型强化学习算法。数值实验验证了理论结果，为博弈场景下的稳定高效强化学习提供了理论与实践支持。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=sSQdICPJv1](https://openreview.net/forum?id=sSQdICPJv1)
