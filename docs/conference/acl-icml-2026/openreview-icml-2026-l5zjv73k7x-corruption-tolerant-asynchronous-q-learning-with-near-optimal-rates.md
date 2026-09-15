---
title: Corruption-Tolerant Asynchronous Q-Learning with Near-Optimal Rates
title_zh: 容忍污染的异步Q学习及近最优速率
authors: "Sreejeet Maity, Aritra Mitra"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/fbb2c541b0f6d55195388ab66fa723cebb09f5cd.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 具近最优有限时间率的容忍污染异步Q学习
tldr: 针对奖励被对抗性污染的无折扣无限时域强化学习问题，本文提出一种鲁棒的Q学习变体，并在具有时间相关数据的异步采样模型下进行分析。作者证明该算法在存在污染时仍能达到与现有界相匹配的有限时间保证，误差仅随污染样本比例线性增加，并给出信息论下界说明其近最优性。该工作首次为污染环境下的异步Q学习提供了有限时间鲁棒性保证。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 奖励被对抗性污染时，现有强化学习算法的有限时间保证失效。
method: 提出鲁棒Q学习变体，在时间相关的异步采样模型下进行分析。
result: 证明其有限时间界与现有最优界仅差污染比例项，并给出匹配的信息论下界。
conclusion: 首次为污染环境下的异步Q学习提供近最优的有限时间鲁棒性保证。
---

## Abstract
We study the problem of learning the optimal policy in a discounted, infinite-horizon reinforcement learning (RL) setting in the presence of adversarially corrupted rewards. To address this problem, we develop a novel robust variant of the Q-learning algorithm and analyze it under the challenging asynchronous sampling model with time-correlated data. Despite corruption, we prove that the finite-time guarantees of our approach match existing bounds, up to an additive term that scales with the fraction of corrupted samples. We also establish an information-theoretic lower bound, revealing that our guarantees are near-optimal. Notably, our algorithm is agnostic to the underlying reward distribution and provides the first finite-time robustness guarantees for asynchronous Q-learning. A key element of our analysis is a refined Azuma-Hoeffding inequality for almost-martingales, which may have broader applicability in the study of RL algorithms.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
具近最优有限时间率的容忍污染异步Q学习。

### 2. 核心内容
针对奖励被对抗性污染的无折扣无限时域强化学习问题，本文提出一种鲁棒的Q学习变体，并在具有时间相关数据的异步采样模型下进行分析。作者证明该算法在存在污染时仍能达到与现有界相匹配的有限时间保证，误差仅随污染样本比例线性增加，并给出信息论下界说明其近最优性。该工作首次为污染环境下的异步Q学习提供了有限时间鲁棒性保证。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=L5ZJv73k7x](https://openreview.net/forum?id=L5ZJv73k7x)
