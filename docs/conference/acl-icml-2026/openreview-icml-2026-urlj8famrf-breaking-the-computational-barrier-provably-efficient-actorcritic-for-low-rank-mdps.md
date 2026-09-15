---
title: "Breaking the Computational Barrier: Provably Efficient Actor–Critic for Low-Rank MDPs"
title_zh: 突破计算瓶颈：面向低秩MDP的可证明高效Actor-Critic算法
authors: "Ruiquan Huang, Donghao Li, Yingbin Liang, Jing Yang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/5b04589071c847d6c2fe7573e791c8a844f8e9fd.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 低秩MDP下可证明高效的actor-critic强化学习理论与oracle层级
tldr: 在带函数逼近的强化学习中，许多算法虽有良好样本复杂度，却依赖计算上不可行的预言机。本文以监督学习作为计算代理，在低秩MDP下建立常用RL预言机的计算层级，指出策略评估是最高效的预言机。据此提出一种新的乐观actor-critic算法，并给出可证明的高效性保证。该工作为强化学习算法的计算可行性提供了理论基础与实用算法设计思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有带函数逼近的强化学习算法虽样本复杂度良好，但常依赖计算上不可行的预言机，限制其实用性。
method: 论文以监督学习作为计算代理，在低秩MDP下建立常用RL预言机的计算层级，并提出乐观actor-critic算法。
result: 分析表明策略评估是最高效的预言机，所提算法在可计算条件下实现了可证明的高效性。
conclusion: 该工作厘清了RL预言机的计算可行性层级，为高效强化学习算法设计提供了理论指导。
---

## Abstract
Reinforcement learning (RL) is a fundamental framework for sequential decision-making, in which an agent learns an optimal policy through interactions with an unknown environment. In settings with function approximation, many existing RL algorithms achieve favorable sample complexity, but often rely on computationally intractable oracles. In this paper, we use supervised learning as a computational proxy to establish a clear hierarchy of commonly adopted RL oracles under low-rank Markov Decision Processes (MDPs). This hierarchy shows that policy evaluation is the most computationally efficient oracle, provided that supervised learning can be efficiently solved. Motivated by this observation, we propose a novel optimistic actor–critic algorithm that relies solely on the policy evaluation oracle. We prove that our algorithm outperforms the existing sample complexity guarantees for low-rank MDPs while avoiding computationally expensive planning or optimization oracles commonly assumed in prior works. We further extend our theoretical results to approximately low-rank MDPs and demonstrate that this setting captures a broad class of real-world environments. Finally, we validate our theoretical results with experiments on several standard Gym benchmarks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
低秩MDP下可证明高效的actor-critic强化学习理论与oracle层级。

### 2. 核心内容
在带函数逼近的强化学习中，许多算法虽有良好样本复杂度，却依赖计算上不可行的预言机。本文以监督学习作为计算代理，在低秩MDP下建立常用RL预言机的计算层级，指出策略评估是最高效的预言机。据此提出一种新的乐观actor-critic算法，并给出可证明的高效性保证。该工作为强化学习算法的计算可行性提供了理论基础与实用算法设计思路。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=urlj8fAMrf](https://openreview.net/forum?id=urlj8fAMrf)
