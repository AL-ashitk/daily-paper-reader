---
title: Long-Horizon Model-Based Offline Reinforcement Learning Without Explicit Conservatism
title_zh: 无需显式保守性的长时域模型式离线强化学习
authors: "Tianwei Ni, Esther Derman, Vineet Jain, Vincent Taboga, Siamak Ravanbakhsh, Pierre-Luc Bacon"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/9c7973383e3949e25bd86a213eeb113784d4c6ca.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 无需显式保守性的长时域模型式离线强化学习
tldr: 主流离线强化学习依赖显式保守性，通过惩罚数据外动作或限制展开时域来抑制价值高估，本文质疑该原则的普适性。作者重新审视用于测试时自适应的贝叶斯视角，对世界模型建模后验并训练依赖历史的智能体最大化期望回报，从而无需显式保守性即可处理认知不确定性。实验表明在低质量数据集上贝叶斯方法优于保守方法，而在真实任务中长时域展开对控制价值高估至关重要。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 主流离线强化学习依赖显式保守性，其普适性受到质疑。
method: 采用世界模型后验的贝叶斯视角，训练依赖历史的智能体最大化期望回报。
result: 低质量数据上贝叶斯方法优于保守方法，长时域展开可控制价值高估。
conclusion: 表明无需显式保守性也能实现有效的长时域模型式离线强化学习。
---

## Abstract
Popular offline reinforcement learning (RL) methods rely on *explicit conservatism*, penalizing out-of-dataset actions or restricting rollout horizons. We question the universality of this principle and revisit a complementary Bayesian perspective for test-time adaptation. By modeling a posterior over world models and training a history-dependent agent to maximize expected return, the Bayesian approach directly addresses epistemic uncertainty without explicit conservatism. We first illustrate in a bandit setting that Bayesianism excels on low-quality datasets where conservatism fails. Scaling to realistic tasks, we find that *long-horizon rollouts* are essential to control value overestimation once conservatism is removed. We introduce design choices that enable learning from long-horizon rollouts while mitigating compounding model errors, yielding our algorithm, NEUBAY, grounded in the neutral Bayesian principle. On D4RL and NeoRL benchmarks, NEUBAY is competitive with leading conservative algorithms, achieving new state-of-the-art on 7 datasets with rollout horizons of several hundred steps. Finally, we characterize datasets by quality and coverage to identify when NEUBAY is preferable to conservative methods.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
无需显式保守性的长时域模型式离线强化学习。

### 2. 核心内容
主流离线强化学习依赖显式保守性，通过惩罚数据外动作或限制展开时域来抑制价值高估，本文质疑该原则的普适性。作者重新审视用于测试时自适应的贝叶斯视角，对世界模型建模后验并训练依赖历史的智能体最大化期望回报，从而无需显式保守性即可处理认知不确定性。实验表明在低质量数据集上贝叶斯方法优于保守方法，而在真实任务中长时域展开对控制价值高估至关重要。

### 3. 对应检索需求
model-based reinforcement learning papers。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=NHu6haXTM9](https://openreview.net/forum?id=NHu6haXTM9)
