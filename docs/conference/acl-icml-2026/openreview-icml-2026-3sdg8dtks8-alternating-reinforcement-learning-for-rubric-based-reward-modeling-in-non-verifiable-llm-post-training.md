---
title: Alternating Reinforcement Learning for Rubric-Based Reward Modeling in Non-Verifiable LLM Post-Training
title_zh: 面向不可验证LLM后训练中基于评分标准的奖励建模的交替强化学习
authors: "Ran Xu, Tianci Liu, Zihan Dong, Tony Yu, Ilgee Hong, Carl Yang, Linjun Zhang, Tuo Zhao, Haoyu Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/93aaaf0714fe23770e5c336ad4b0a8c93b36916c.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 用于奖励建模的强化学习框架
tldr: 标准奖励模型在创意写作等不可验证领域只能输出标量分数，无法刻画回复质量的多面性。本文提出Rubric-ARM，将评分标准生成建模为隐动作，用偏好反馈强化学习联合优化评分标准生成器与评判器，并设计交替优化策略缓解同步更新的非平稳性。理论分析表明该交替策略能提升评判准确率与训练稳定性。该工作为不可验证任务的奖励建模提供了动态、可学习的评分标准框架。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 标准奖励模型仅输出标量分数，难以刻画创意写作等不可验证任务中回复质量的多面性。
method: 提出Rubric-ARM，将评分标准生成视为隐动作，用偏好反馈强化学习联合优化评分标准生成器与评判器，并采用交替优化缓解非平稳性。
result: 给出理论分析说明交替更新如何稳定训练，并提升评判准确率。
conclusion: 为不可验证领域的奖励建模提供了可学习的动态评分标准方案。
---

## Abstract
Standard reward models typically predict scalar scores that fail to capture the multifaceted nature of response quality in non-verifiable domains, such as creative writing or open-ended instruction following. To address this limitation, we propose Rubric-ARM, a framework that jointly optimizes a rubric generator and a judge using reinforcement learning from preference feedback. Unlike existing methods that rely on static rubrics or disjoint training pipelines, our approach treats rubric generation as a latent action learned to maximize judgment accuracy. We introduce an alternating optimization strategy to mitigate the non-stationarity of simultaneous updates, providing theoretical analysis that demonstrates how this schedule reduces gradient variance during training. Extensive experiments show that Rubric-ARM achieves state-of-the-art performance among baselines on multiple benchmarks and significantly improves downstream policy alignment in both offline and online reinforcement learning settings.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
用于奖励建模的强化学习框架。

### 2. 核心内容
标准奖励模型在创意写作等不可验证领域只能输出标量分数，无法刻画回复质量的多面性。本文提出Rubric-ARM，将评分标准生成建模为隐动作，用偏好反馈强化学习联合优化评分标准生成器与评判器，并设计交替优化策略缓解同步更新的非平稳性。理论分析表明该交替策略能提升评判准确率与训练稳定性。该工作为不可验证任务的奖励建模提供了动态、可学习的评分标准框架。

### 3. 对应检索需求
papers on reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=3SDg8dtkS8](https://openreview.net/forum?id=3SDg8dtkS8)
