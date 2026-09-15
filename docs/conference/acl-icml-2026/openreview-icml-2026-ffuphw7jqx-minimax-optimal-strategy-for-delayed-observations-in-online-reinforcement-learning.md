---
title: Minimax Optimal Strategy for Delayed Observations in Online Reinforcement Learning
title_zh: 在线强化学习中延迟观测的极小极大最优策略
authors: "Harin Lee, Kevin Jamieson"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/6b7ad30fab7a8ab4fba00f35b98bcc20190e5b6d.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 在线强化学习延迟观测的极小极大最优算法
tldr: 该文研究延迟状态观测下的在线强化学习，智能体在若干时间步后才观测到当前状态。作者提出结合状态增广与置信上界方法的算法，并针对表格型马尔可夫决策过程推导出随最大延迟缩放的遗憾界。文中进一步给出匹配的下界，证明所提方法在极小极大意义下最优。其分析框架将该问题视为更广类MDP的特例，拓展了延迟反馈在线强化学习的理论。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 在线强化学习中状态观测存在随机延迟，缺乏最优性理论刻画。
method: 提出结合状态增广与置信上界（UCB）的算法处理延迟观测。
result: 得到随最大延迟缩放的遗憾上界，并给出匹配下界证明最优性。
conclusion: 建立延迟观测在线强化学习的极小极大最优理论框架。
---

## Abstract
We study reinforcement learning with delayed state observation, where the agent observes the current state after some random number of time steps.
We propose an algorithm that combines the augmentation method and the upper confidence bound approach.
For tabular Markov decision processes (MDPs), we derive a regret bound of $\tilde{\mathcal{O}}(H \sqrt{D_{\max} SAK})$, where $S$ and $A$ are the cardinalities of the state and action spaces, $H$ is the time horizon, $K$ is the number of episodes, and $D_{\max}$ is the maximum length of the delay.
We also provide a matching lower bound up to logarithmic factors, showing the optimality of our approach.
Our analytical framework formulates this problem as a special case of a broader class of MDPs, where their transition dynamics decompose into a known component and an unknown but structured component.
We establish general results for this abstract setting, which may be of independent interest.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
在线强化学习延迟观测的极小极大最优算法。

### 2. 核心内容
该文研究延迟状态观测下的在线强化学习，智能体在若干时间步后才观测到当前状态。作者提出结合状态增广与置信上界方法的算法，并针对表格型马尔可夫决策过程推导出随最大延迟缩放的遗憾界。文中进一步给出匹配的下界，证明所提方法在极小极大意义下最优。其分析框架将该问题视为更广类MDP的特例，拓展了延迟反馈在线强化学习的理论。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=fFupHW7Jqx](https://openreview.net/forum?id=fFupHW7Jqx)
