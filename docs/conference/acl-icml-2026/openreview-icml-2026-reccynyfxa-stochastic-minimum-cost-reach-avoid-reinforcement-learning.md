---
title: Stochastic Minimum-Cost Reach-Avoid Reinforcement Learning
title_zh: 随机最小代价到达-避障强化学习
authors: "Jingduo Pan, Taoran Wu, Yiling Xue, Bai Xue"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/a4a1054daedc0496803b40c7484c398d8861b502.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 带概率证书的到达-避障约束强化学习
tldr: 针对随机环境中安全约束强化学习难以同时满足概率到达-避障约束与代价优化的问题，本文提出到达-避障概率证书（RAPC），用于识别可满足约束的状态，并构建基于压缩的贝尔曼形式化，将到达-避障要求融入强化学习目标。实验表明该方法能在保证约束满足概率的同时优化期望累计代价，为安全约束强化学习提供了新的原则性框架。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有安全与约束强化学习方法难以在随机环境中同时满足概率到达-避障约束并优化代价。
method: 提出到达-避障概率证书并构建基于压缩的贝尔曼形式化，作为整合约束的替代目标。
result: 实验显示该方法能在满足约束概率下同时优化期望累计代价。
conclusion: 为随机安全约束强化学习提供了兼具约束满足与代价最优的原则性方法。
---

## Abstract
We study stochastic minimum-cost reach-avoid reinforcement learning, where an agent must satisfy a reach-avoid specification with probability at least $p$ while minimizing expected cumulative costs in stochastic environments. Existing safe and constrained reinforcement learning methods typically fail to jointly enforce probabilistic reach-avoid constraints and optimize cost in the learning setting in stochastic environments. To address this challenge, we introduce reach-avoid probability certificates (RAPCs), which identify states from which stochastic reach-avoid constraints are satisfiable. Building on RAPCs, we develop a contraction-based Bellman formulation that serves as a principled surrogate for integrating reach-avoid considerations into reinforcement learning, enabling cost optimization under probabilistic constraints. We establish almost sure convergence of the proposed algorithms to locally optimal policies with respect to the resulting objective. Experiments in the MuJoCo simulator demonstrate improved cost performance and consistently higher reach-avoid satisfaction rates.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
带概率证书的到达-避障约束强化学习。

### 2. 核心内容
针对随机环境中安全约束强化学习难以同时满足概率到达-避障约束与代价优化的问题，本文提出到达-避障概率证书（RAPC），用于识别可满足约束的状态，并构建基于压缩的贝尔曼形式化，将到达-避障要求融入强化学习目标。实验表明该方法能在保证约束满足概率的同时优化期望累计代价，为安全约束强化学习提供了新的原则性框架。

### 3. 对应检索需求
papers on reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=ReCCYnyfXa](https://openreview.net/forum?id=ReCCYnyfXa)
