---
title: "From Outcomes to Actions: Leveraging Hindsight for Long-Horizon Language Agent Training"
title_zh: 从结果到动作：利用事后视角进行长时程语言智能体训练
authors: "Zishang Jiang, tingyun li, Jinyi Han, Xinyi Wang, Sihang Jiang, Yizhou Ying, Xiaojun Meng, Jiansheng Wei, Jiaqing Liang, Yanghua Xiao"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/d24115c5f15c478dbea0922c0351dacaf89fccdc.pdf"
tags: ["query:rl"]
score: 8.0
evidence: 面向强化学习训练的新型策略梯度算法
tldr: 强化学习已成为提升大语言模型复杂任务能力的主流技术，但现有方法在长时程交互训练中难以区分不同动作的贡献，导致优化方差过高。本文提出新颖的策略梯度方法Hindsight Policy Optimization，将当前策略分布与事后分布投影到意图空间，并利用二者间的Wasserstein距离提取低方差学习信号。理论与实验表明，聚合语义信号能有效降低方差并改善长时程智能体训练效果。该工作为长时程语言智能体的强化学习训练提供了低方差的策略梯度方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有强化学习在长时程交互中难以区分各动作贡献，导致优化方差过高。
method: 提出Hindsight Policy Optimization，将当前策略分布与事后分布投影到意图空间，用Wasserstein距离提取低方差学习信号。
result: 理论与实验表明聚合语义信号能降低方差并提升长时程训练效果。
conclusion: 为长时程语言智能体强化学习训练提供低方差策略梯度方法。
---

## Abstract
Reinforcement learning (RL) has become a widely adopted technique for improving large language models (LLMs) on complex tasks. Despite this progress, existing RL methods still face challenges in training agents with longer-horizon interactions. One major bottleneck is distinguishing the contribution of different actions in long-horizon interaction, leading to high optimization variance. To address this, we introduce a novel policy gradient method, Hindsight Policy Optimization (HPO), that projects both the current policy distribution and the hindsight distribution into an intent space and extracts low-variance learning signals from the Wasserstein distance between them. We theoretically and empirically show that aggregating semantically similar states and actions in the intent space yields a bounded-variance estimator and improves policy performance stably. Our code is available online.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向强化学习训练的新型策略梯度算法。

### 2. 核心内容
强化学习已成为提升大语言模型复杂任务能力的主流技术，但现有方法在长时程交互训练中难以区分不同动作的贡献，导致优化方差过高。本文提出新颖的策略梯度方法Hindsight Policy Optimization，将当前策略分布与事后分布投影到意图空间，并利用二者间的Wasserstein距离提取低方差学习信号。理论与实验表明，聚合语义信号能有效降低方差并改善长时程智能体训练效果。该工作为长时程语言智能体的强化学习训练提供了低方差的策略梯度方案。

### 3. 对应检索需求
algorithms for reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=iK3yDEvQ4y](https://openreview.net/forum?id=iK3yDEvQ4y)
