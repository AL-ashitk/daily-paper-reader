---
title: Distributional Inverse Reinforcement Learning
title_zh: 分布式逆强化学习
authors: "Feiyang Wu, Ye Zhao, Anqi Wu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/bec86146992cdbfd2fddce6fc57b2ddb57cd0624.pdf"
tags: ["query:rl"]
score: 8.0
evidence: 面向奖励与回报分布的分布式离线逆强化学习框架
tldr: 传统逆强化学习通常只能恢复确定性奖励或仅匹配期望回报，难以刻画专家行为的丰富结构。本文提出一种分布式离线逆强化学习框架，联合建模奖励函数的不确定性与完整回报分布，通过最小化一阶随机占优违背并引入失真风险测度来学习策略。理论分析给出了算法的收敛性保证。该方法适用于行为分析与风险感知的模仿学习，拓展了逆强化学习在风险场景下的能力。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 传统逆强化学习仅恢复确定性奖励或匹配期望回报，无法刻画专家行为的分布结构与风险特征。
method: 论文提出分布式离线逆强化学习框架，联合建模奖励不确定性与回报分布，并最小化一阶随机占优违背。
result: 理论分析证明该算法具有收敛保证，能够同时恢复奖励分布与分布感知策略。
conclusion: 该框架适用于行为分析与风险感知的模仿学习，扩展了逆强化学习在风险场景下的适用性。
---

## Abstract
We propose a distributional framework for offline Inverse Reinforcement Learning (IRL) that jointly models uncertainty over reward functions and full distributions of returns. Unlike conventional IRL approaches that recover a deterministic reward estimate or match only expected returns, our method captures richer structure in expert behavior, particularly in learning the reward distribution, by minimizing first-order stochastic dominance (FSD) violations and thus integrating distortion risk measures (DRMs) into policy learning, enabling the recovery of both reward distributions and distribution-aware policies. This formulation is well-suited for behavior analysis and risk-aware imitation learning. Theoretical analysis show that the algorithm converge with $\mathcal{O}(\varepsilon^{-2})$ iteration complexity. Empirical results on synthetic benchmarks, real-world neurobehavioral data, and MuJoCo control tasks demonstrate that our method recovers expressive reward representations and achieves state-of-the-art imitation performance.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向奖励与回报分布的分布式离线逆强化学习框架。

### 2. 核心内容
传统逆强化学习通常只能恢复确定性奖励或仅匹配期望回报，难以刻画专家行为的丰富结构。本文提出一种分布式离线逆强化学习框架，联合建模奖励函数的不确定性与完整回报分布，通过最小化一阶随机占优违背并引入失真风险测度来学习策略。理论分析给出了算法的收敛性保证。该方法适用于行为分析与风险感知的模仿学习，拓展了逆强化学习在风险场景下的能力。

### 3. 对应检索需求
papers on reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=ZcnZ6vs4yX](https://openreview.net/forum?id=ZcnZ6vs4yX)
