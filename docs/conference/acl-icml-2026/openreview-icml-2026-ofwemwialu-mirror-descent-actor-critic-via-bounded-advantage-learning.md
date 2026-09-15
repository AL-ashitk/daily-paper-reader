---
title: Mirror Descent Actor Critic via Bounded Advantage Learning
title_zh: 通过有界优势学习的镜像下降演员-评论家
authors: Ryo Iwaki
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/f0142beb317f354de9f7a2dea571e500e62f966f.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 带镜像下降正则的强化学习演员-评论家算法
tldr: 该文针对KL-熵正则方法在连续动作域中表现不及纯熵正则的问题，提出镜像下降演员-评论家（MDAC），将镜像下降价值迭代以演员-评论家形式实例化到连续动作空间。方法核心是在评论家损失中对演员的对数概率项进行有界化处理，从而稳定训练并提升性能。实验表明有界化相较朴素实现能显著提升经验表现，为连续控制中的正则化强化学习提供了有效算法。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有KL-熵正则方法在连续动作域中性能不及纯熵正则，需要新的演员-评论家实现。
method: 提出镜像下降演员-评论家MDAC，并对评论家损失中演员对数概率项做有界化处理。
result: 有界化处理相比非有界朴素实现显著提升了连续动作域的经验性能。
conclusion: 为连续动作域提供有效的正则化强化学习算法，凸显有界优势学习的重要性。
---

## Abstract
Regularization is a core component of recent Reinforcement Learning (RL) algorithms. Mirror Descent Value Iteration (MDVI) uses both Kullback-Leibler divergence and entropy as regularizers in its value and policy updates. Despite its empirical success in discrete action domains and strong theoretical guarantees, the performance of KL-entropy-regularized methods does not surpass that of a strong entropy-only-regularized method in continuous action domains. In this study, we propose Mirror Descent Actor Critic (MDAC) as an actor-critic style instantiation of MDVI for continuous action domains, and show that its empirical performance is significantly boosted by bounding the actor's log-probability terms in the critic's loss function, compared to a non-bounded naive instantiation. Further, we relate MDAC to Advantage Learning by recalling that the actor's log-probability is equal to the regularized advantage function in tabular cases, and theoretically discuss when and why bounding the advantage terms is validated and beneficial. We also empirically explore effective choices for the bounding functions, and show that MDAC performs better than strong non-regularized and entropy-only-regularized methods with an appropriate choice of the bounding functions.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
带镜像下降正则的强化学习演员-评论家算法。

### 2. 核心内容
该文针对KL-熵正则方法在连续动作域中表现不及纯熵正则的问题，提出镜像下降演员-评论家（MDAC），将镜像下降价值迭代以演员-评论家形式实例化到连续动作空间。方法核心是在评论家损失中对演员的对数概率项进行有界化处理，从而稳定训练并提升性能。实验表明有界化相较朴素实现能显著提升经验表现，为连续控制中的正则化强化学习提供了有效算法。

### 3. 对应检索需求
algorithms for reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=ofwEMwiaLU](https://openreview.net/forum?id=ofwEMwiaLU)
