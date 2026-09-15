---
title: Finite-time Convergence Analysis of Actor-Critic with Evolving Reward
title_zh: 演化奖励下演员-评论家算法的有限时间收敛分析
authors: "Rui Hu, Yu Chen, Longbo Huang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/af577ef0f015537968f5e2a4caea9f007538fb06.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 演化奖励下演员-评论家的有限时间收敛分析
tldr: 奖励塑形、熵正则与课程学习等实践常用演化奖励函数，但其理论基础的收敛分析尚不完善。本文首次在马尔可夫采样下对单时间尺度演员-评论家算法在奖励参数逐步变化时进行有限时间收敛分析，同时刻画策略优化与价值估计。作者在标准假设下给出演员与评论家的非渐近误差界，得到O(1/√T)收敛速率，与已知最优速率相当，为演化奖励强化学习提供理论支撑。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 实践中广泛使用的演化奖励函数缺乏有限时间收敛的理论保证。
method: 在马尔可夫采样下对单时间尺度演员-评论家算法做非渐近收敛分析。
result: 得到演员与评论家误差的O(1/√T)收敛速率，匹配已知最优速率。
conclusion: 为带演化奖励的强化学习算法奠定理论基础。
---

## Abstract
Many popular practical reinforcement learning (RL) algorithms employ evolving reward functions—through techniques such as reward shaping, entropy regularization, or curriculum learning—yet their theoretical foundations remain underdeveloped. This paper provides the first finite-time convergence analysis of a single-timescale actor-critic algorithm in the presence of an evolving reward function under Markovian sampling. We consider a setting where the reward parameters may change at each time step, affecting both policy optimization and value estimation. Under standard assumptions, we derive non-asymptotic bounds for both actor and critic errors. Our result shows that an $O(1/\sqrt{T})$ convergence rate is achievable, matching the best-known rate for static rewards, provided the reward parameters evolve slowly enough. This rate is preserved when the reward is updated via a gradient-based rule with bounded gradient and on the same timescale as the actor and critic, offering a theoretical foundation for many popular RL techniques. As a secondary contribution, we introduce a novel analysis of distribution mismatch under Markovian sampling, improving the best-known rate by a factor of $\log^2T$ in the static-reward case.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
演化奖励下演员-评论家的有限时间收敛分析。

### 2. 核心内容
奖励塑形、熵正则与课程学习等实践常用演化奖励函数，但其理论基础的收敛分析尚不完善。本文首次在马尔可夫采样下对单时间尺度演员-评论家算法在奖励参数逐步变化时进行有限时间收敛分析，同时刻画策略优化与价值估计。作者在标准假设下给出演员与评论家的非渐近误差界，得到O(1/√T)收敛速率，与已知最优速率相当，为演化奖励强化学习提供理论支撑。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=hocdjAEAIm](https://openreview.net/forum?id=hocdjAEAIm)
