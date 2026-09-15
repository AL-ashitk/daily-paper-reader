---
title: Instance-Dependent Continuous-Time Reinforcement Learning via Maximum Likelihood Estimation
title_zh: 基于最大似然估计的实例依赖连续时间强化学习
authors: "Runze Zhao, Yue Yu, Ruhan Wang, Chunfeng Huang, Dongruo Zhou"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/e566cb8a761e02adb939228029b02fa091d8b5f4.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 基于最大似然估计的模型式连续时间强化学习
tldr: 连续时间强化学习为交互随时间连续演化的动态环境提供自然建模框架，但其适应不同问题难度的能力尚不清楚。本文研究连续时间强化学习的实例依赖行为，提出一种基于最大似然估计、使用通用函数逼近器的简单模型式算法，且不同于直接估计系统动力学，而是估计状态边缘密度来引导学习。作者推导出实例依赖的遗憾界，给出性能保证，深化了对连续时间强化学习难度适应性的理解。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 连续时间强化学习对不同问题难度的适应能力缺乏理论与实例依赖分析。
method: 提出基于最大似然估计的模型式算法，估计状态边缘密度而非直接估计动力学。
result: 推导出实例依赖的遗憾界，为算法提供性能保证。
conclusion: 为连续时间模型式强化学习建立实例依赖的理论刻画。
---

## Abstract
Continuous-time reinforcement learning (CTRL) provides a natural framework for sequential decision-making in dynamic environments where interactions evolve continuously over time. While CTRL has shown growing empirical success, its ability to adapt to varying levels of problem difficulty remains poorly understood. In this work, we investigate the instance-dependent behavior of CTRL and introduce a simple, model-based algorithm built on maximum likelihood estimation (MLE) with a general function approximator. Unlike existing approaches that estimate system dynamics directly, our method estimates the state marginal density to guide learning. We establish instance-dependent performance guarantees by deriving a regret bound that scales with the total reward variance and measurement resolution. Notably, the regret becomes independent of the specific measurement strategy when the observation frequency adapts appropriately to the problem’s complexity. To further improve performance, our algorithm incorporates a randomized measurement schedule that enhances sample efficiency without increasing measurement cost. These results highlight a new direction for designing CTRL algorithms that automatically adjust their learning behavior based on the underlying difficulty of the environment.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
基于最大似然估计的模型式连续时间强化学习。

### 2. 核心内容
连续时间强化学习为交互随时间连续演化的动态环境提供自然建模框架，但其适应不同问题难度的能力尚不清楚。本文研究连续时间强化学习的实例依赖行为，提出一种基于最大似然估计、使用通用函数逼近器的简单模型式算法，且不同于直接估计系统动力学，而是估计状态边缘密度来引导学习。作者推导出实例依赖的遗憾界，给出性能保证，深化了对连续时间强化学习难度适应性的理解。

### 3. 对应检索需求
model-based reinforcement learning papers。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=aXvTMnyeLj](https://openreview.net/forum?id=aXvTMnyeLj)
