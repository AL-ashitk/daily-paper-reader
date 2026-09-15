---
title: Doubly Regularized Markov Decision Processes for Robust Reinforcement Learning
title_zh: 面向鲁棒强化学习的双重正则化马尔可夫决策过程
authors: "Yiting He, Zhishuai Liu, Pan Xu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/631ef490b04c4af919d8164648d22418e43b9044.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 面向强化学习的正则化MDP理论分析
tldr: 正则化能提升强化学习的稳定性与效率，但其理论分析多局限于标准RL设定。本文从鲁棒强化学习视角研究正则化MDP，提出结合策略正则化与动力学正则化的双重正则化MDP框架，在自然支持连续动作空间的同时实现鲁棒策略学习。在此框架下，作者设计了基于乐观思想的在线算法，并在表格与线性设定中给出首个有限样本遗憾保证。该工作扩展了正则化MDP的鲁棒强化学习理论与算法。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 正则化强化学习的理论分析多局限于标准设定，缺乏鲁棒视角。
method: 提出双重正则化MDP框架，结合策略与动力学正则化，并设计基于乐观思想的在线算法。
result: 在表格与线性设定下给出首个有限样本遗憾保证。
conclusion: 扩展了正则化MDP的鲁棒强化学习理论与算法。
---

## Abstract
Empirical successes show that regularization improves the stability and efficiency of reinforcement learning (RL), with applications in robotics and post-training of large language models. Yet, theoretical analyses of regularized Markov decision processes (MDPs) have mostly been confined to the standard RL setting. In this work, we investigate regularized MDPs through the lens of robust RL. We introduce a doubly regularized MDP framework that combines policy and dynamics regularizations, enabling robust policy learning while naturally accommodating continuous action spaces. Within this framework, we develop an optimism-based online algorithm and provide the first finite-sample regret guarantees in both tabular and linear settings. Our results show that algorithms for doubly regularized MDPs are as sample-efficient as well-studied robust MDP algorithms, while additionally benefiting from the flexibility of soft policies. We further design practical algorithmic variants for both settings and demonstrate empirically that our approach efficiently and effectively handles function approximation and exploration in large state-action spaces, achieving robust performances.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向强化学习的正则化MDP理论分析。

### 2. 核心内容
正则化能提升强化学习的稳定性与效率，但其理论分析多局限于标准RL设定。本文从鲁棒强化学习视角研究正则化MDP，提出结合策略正则化与动力学正则化的双重正则化MDP框架，在自然支持连续动作空间的同时实现鲁棒策略学习。在此框架下，作者设计了基于乐观思想的在线算法，并在表格与线性设定中给出首个有限样本遗憾保证。该工作扩展了正则化MDP的鲁棒强化学习理论与算法。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=eeoU8iz7w1](https://openreview.net/forum?id=eeoU8iz7w1)
