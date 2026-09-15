---
title: "Trust Region Inverse Reinforcement Learning: Explicit Dual Ascent using Local Policy Updates"
title_zh: 信任域逆强化学习：基于局部策略更新的显式对偶上升
authors: "Anish Abhijit Diwan, Davide Tateo, Christopher Mower, Haitham Bou Ammar, Jan Peters, Oleg Arenz"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/317e7cbcf69d8e60fe6fdd16bf3e39a8ff9488dd.pdf"
tags: ["query:rl"]
score: 8.0
evidence: 逆强化学习理论与对偶上升
tldr: 逆强化学习常被表述为在匹配专家轨迹分布下最大化熵，经典对偶上升方法保证单调改进但每步需完整求解一个RL问题，而对抗式方法虽高效却牺牲了稳定性与单调性。本文利用信任域优化的理论洞察，在无需每步完整求解RL问题的情况下实现奖励函数与策略的单调改进。该方法弥合了经典对偶上升与对抗式IRL之间的差距，兼顾了理论保证与计算效率。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 经典对偶上升逆强化学习每步需完整求解RL问题，而对抗式方法牺牲了稳定性与单调性。
method: 利用信任域优化洞察，在无需完整求解RL问题的前提下实现奖励与策略的单调改进。
result: 兼顾经典方法的单调保证与对抗方法的计算效率。
conclusion: 弥合了逆强化学习两类主流方法之间的差距。
---

## Abstract
Inverse reinforcement learning (IRL) is typically formulated as maximizing entropy subject to matching the distribution of expert trajectories. Classical (dual-ascent) IRL guarantees monotonic performance improvement but requires fully solving an RL problem each iteration to compute dual gradients. More recent adversarial methods avoid this cost at the expense of stability and monotonic dual improvement, by directly optimizing the primal problem and using a discriminator to provide rewards. In this work, we bridge the gap between these approaches by enabling monotonic improvement of the reward function and policy without having to fully solve an RL problem at every iteration. Our key theoretical insight is that a trust-region-optimal policy for a reward function update can be globally optimal for a smaller update in the same direction. This smaller update allows us to explicitly optimize the dual objective while only relying on a local search around the current policy. In doing so, our approach avoids the training instabilities of adversarial methods, offers monotonic performance improvement, and learns a reward function in the traditional sense of IRL—one that can be globally optimized to match expert demonstrations. Our proposed algorithm, *Trust Region Inverse Reinforcement Learning (TRIRL)*, outperforms state-of-the-art imitation learning methods across multiple challenging tasks by a factor of 2.4x in terms of aggregate inter-quartile mean, while recovering reward functions that generalize to system dynamics shifts.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
逆强化学习理论与对偶上升。

### 2. 核心内容
逆强化学习常被表述为在匹配专家轨迹分布下最大化熵，经典对偶上升方法保证单调改进但每步需完整求解一个RL问题，而对抗式方法虽高效却牺牲了稳定性与单调性。本文利用信任域优化的理论洞察，在无需每步完整求解RL问题的情况下实现奖励函数与策略的单调改进。该方法弥合了经典对偶上升与对抗式IRL之间的差距，兼顾了理论保证与计算效率。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=XSYX75R6RC](https://openreview.net/forum?id=XSYX75R6RC)
