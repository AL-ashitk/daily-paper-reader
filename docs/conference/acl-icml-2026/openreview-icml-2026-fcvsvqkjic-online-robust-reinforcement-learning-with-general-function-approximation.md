---
title: Online Robust Reinforcement Learning with General Function Approximation
title_zh: 通用函数逼近下的在线鲁棒强化学习
authors: "Debamita Ghosh, George K. Atia, Yue Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/d3ad036428a24f353eac4ec64502314ac25dce07.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 通用函数逼近的在线鲁棒强化学习算法
tldr: 强化学习在真实任务中常因训练与部署环境的分布偏移而性能下降。分布鲁棒强化学习通过在最坏情形动态上优化来缓解该问题，但现有方法多依赖生成模型或离线数据且局限于表格情形。作者提出一种纯在线、采用通用函数逼近的分布鲁棒强化学习算法，可直接从交互中学习鲁棒策略，无需先验知识或预采集数据。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有分布鲁棒强化学习依赖强数据访问假设且多局限于表格设置。
method: 作者提出纯在线的分布鲁棒强化学习算法，采用通用函数逼近直接交互学习。
result: 该方法无需先验知识或预采集数据即可学习鲁棒策略。
conclusion: 该工作放宽了鲁棒强化学习的数据访问限制，拓展了其适用范围。
---

## Abstract
Reinforcement learning (RL) in real-world tasks often suffers from the performance degradation due to the distribution shift between training and deployment environments. Distributionally Robust RL (DR-RL) addresses this issue by optimizing the worst-case performance over an uncertainty set of transition dynamics, providing an optimized baseline performance upon deployment. However, existing methods typically require strong data access assumptions (e.g., a generative model or comprehensive offline datasets) and mostly focus on tabular settings. In this paper, we introduce a purely online DR-RL algorithm with general function approximation that learns a robust policy directly from interaction, without any prior knowledge or pre-collected data. Our method uses a dual-based fitted robust Bellman update to jointly learn the value function and the robust backup operator. We establish the first regret guarantee for online DR-RL in terms of an intrinsic complexity measure—the robust Bellman–Eluder (BE) dimension, for general $\phi$-divergence uncertainty sets. Our regret bound is sublinear and independent of $|\mathcal{S}|$ and $|\mathcal{A}|$, and recovers sharp rates in structured regimes, providing a scalable method for practical DR-RL.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
通用函数逼近的在线鲁棒强化学习算法。

### 2. 核心内容
强化学习在真实任务中常因训练与部署环境的分布偏移而性能下降。分布鲁棒强化学习通过在最坏情形动态上优化来缓解该问题，但现有方法多依赖生成模型或离线数据且局限于表格情形。作者提出一种纯在线、采用通用函数逼近的分布鲁棒强化学习算法，可直接从交互中学习鲁棒策略，无需先验知识或预采集数据。

### 3. 对应检索需求
algorithms for reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=fcVsVQkjIc](https://openreview.net/forum?id=fcVsVQkjIc)
