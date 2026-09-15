---
title: Reinforcement Learning with Discrete Diffusion Policies for Combinatorial Action Spaces
title_zh: 面向组合动作空间的离散扩散策略强化学习
authors: "Haitong Ma, Ofir Nabati, Aviv Rosenberg, Bo Dai, Oran Lang, Craig Boutilier, Na Li, Shie Mannor, Lior Shani, Guy Tennenholtz"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/df4341e660f60af5a35ed702086f0184bfc3c7d3.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 面向组合动作空间的强化学习算法
tldr: 强化学习在现实问题中常面临大规模组合动作空间，难以有效扩展。本文提出将离散扩散模型训练为策略的新框架，利用策略镜像下降定义理想的正则化目标策略分布，并把策略更新转化为分布匹配问题，让表达力强的扩散模型去拟合这一稳定目标。这种解耦式训练稳定了学习过程并显著提升训练性能，在多个任务上取得最优结果。该工作为组合动作空间提供了可扩展的扩散策略强化学习方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 强化学习难以扩展到现实问题中大规模组合动作空间。
method: 提出将离散扩散模型训练为策略，用策略镜像下降定义正则化目标分布，把策略更新转化为分布匹配问题。
result: 解耦式训练稳定学习并显著提升性能，取得最优结果。
conclusion: 为组合动作空间提供可扩展的扩散策略强化学习方案。
---

## Abstract
Reinforcement learning (RL) struggles to scale to large, combinatorial action spaces common in many real-world problems. This paper introduces a novel framework for training discrete diffusion models as highly effective policies in these complex settings. Our key innovation is an efficient online training process that ensures stable and effective policy improvement and . By leveraging policy mirror descent (PMD) to define an ideal, regularized target policy distribution, we frame the policy update as a distributional matching problem, training the expressive diffusion model to replicate this stable target. This decoupled approach stabilizes learning and significantly enhances training performance. Our method achieves state-of-the-art results and superior sample efficiency across a diverse set of challenging combinatorial benchmarks, including DNA sequence generation, RL with macro-actions, and multi-agent systems. Experiments demonstrate that our diffusion policies attain comparable or superior performance compared to other baselines. Crucially, our extensive empirical analysis reveals a key trade-off: FKL demonstrates superior sample efficiency and faster initial convergence, whereas RKL ensures stable training and higher asymptotic performance on challenging tasks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向组合动作空间的强化学习算法。

### 2. 核心内容
强化学习在现实问题中常面临大规模组合动作空间，难以有效扩展。本文提出将离散扩散模型训练为策略的新框架，利用策略镜像下降定义理想的正则化目标策略分布，并把策略更新转化为分布匹配问题，让表达力强的扩散模型去拟合这一稳定目标。这种解耦式训练稳定了学习过程并显著提升训练性能，在多个任务上取得最优结果。该工作为组合动作空间提供了可扩展的扩散策略强化学习方案。

### 3. 对应检索需求
algorithms for reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=tbz8ixrEKd](https://openreview.net/forum?id=tbz8ixrEKd)
