---
title: Emergence of Exploration in Policy Gradient Reinforcement Learning via Retrying
title_zh: 通过重试在策略梯度强化学习中涌现探索行为
authors: "Soichiro Nishimori, Paavo Parmas, Sotetsu Koyamada, Tadashi Kozuno, Toshinori Kitamura, Shin Ishii, Yutaka Matsuo"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/d974678ce91b42860dc0e95ca8fb4cf2830f0df6.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 策略梯度强化学习中经重试目标涌现的探索
tldr: 强化学习中智能体受益于探索，仅因其反复遇到相似状态，若没有重试则贪心策略即为最优。作者用ReMax目标形式化该直觉，以M次采样的期望最大回报评估策略并考虑回报不确定性。优化该目标可在无需显式奖励项的情况下自然涌现随机探索。作者进一步推导其策略梯度并引入RePPO，一种优化ReMax的PPO变体，为探索机制提供了新原理。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 强化学习中探索的价值源于重复遇到相似状态，但缺乏统一的形式化解释。
method: 作者提出ReMax目标，以多次采样期望最大回报评估策略并推导其策略梯度，得到RePPO。
result: 优化该目标可无需显式奖励项而自然涌现随机探索行为。
conclusion: 该工作为策略梯度强化学习中的探索机制提供了新原理与实用算法。
---

## Abstract
In reinforcement learning (RL), agents benefit from exploration *only* because they repeatedly encounter similar states: trying different actions can improve performance or reduce uncertainty; without such retries, a greedy policy is optimal. We formalize this intuition with **ReMax**, an objective that evaluates a policy by the expected maximum return over $M$ samples ($M \in \mathbb{N}$), while accounting for return uncertainty. Optimizing this objective induces stochastic exploration as an emergent property, without explicit bonus terms. For efficient policy optimization, we derive a new policy-gradient formulation for ReMax and introduce **Re**Max **PPO** (**RePPO**), a PPO variant that optimizes ReMax while generalizing the discrete retry count $M$ to a continuous parameter $m > 0$, enabling fine-grained control of exploration. Empirically, RePPO promotes exploration—without any explicit exploration bonuses—on the MinAtar and Craftax benchmarks. The official code is available at https://github.com/nissymori/remax-rl.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
策略梯度强化学习中经重试目标涌现的探索。

### 2. 核心内容
强化学习中智能体受益于探索，仅因其反复遇到相似状态，若没有重试则贪心策略即为最优。作者用ReMax目标形式化该直觉，以M次采样的期望最大回报评估策略并考虑回报不确定性。优化该目标可在无需显式奖励项的情况下自然涌现随机探索。作者进一步推导其策略梯度并引入RePPO，一种优化ReMax的PPO变体，为探索机制提供了新原理。

### 3. 对应检索需求
algorithms for reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=NpvBAOc87E](https://openreview.net/forum?id=NpvBAOc87E)
