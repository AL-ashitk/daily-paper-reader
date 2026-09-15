---
title: Stable Deep Reinforcement Learning via Isotropic Gaussian Representations
title_zh: 通过各向同性高斯表示实现稳定的深度强化学习
authors: "Ali Saheb Pasand, Johan Obando-Ceron, Aaron Courville, Pouya Bashivan, Pablo Samuel Castro"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/48f5bab87262f68caf4f6bf0b1473ea60453a395.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 基于各向同性高斯表示的稳定深度强化学习
tldr: 深度强化学习系统常因非平稳性导致训练不稳定，学习目标与数据分布随时间演变。作者证明在非平稳目标下，各向同性高斯嵌入具有可证明的优势，能稳定跟踪线性读出器的时变目标并在固定方差预算下实现最大熵。基于此提出草图化各向同性高斯正则，将表示训练时拉向各向同性高斯分布，实验表明该方法提升了智能体的适应性与训练稳定性。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 深度强化学习因非平稳性常出现训练不稳定，目标与数据分布随时间演变。
method: 作者证明各向同性高斯嵌入的优势，并提出草图化各向同性高斯正则塑造表示。
result: 实验显示该方法提升了智能体的适应性与训练稳定性。
conclusion: 该工作为稳定深度强化学习表示学习提供了理论与实用方法。
---

## Abstract
Deep reinforcement learning systems often suffer from unstable training dynamics due to non-stationarity, where learning objectives and data distributions evolve over time. We show that under non-stationary targets, isotropic Gaussian embeddings are provably advantageous. In particular, they induce stable tracking of time-varying targets for linear readouts, achieve maximal entropy under a fixed variance budget, and encourage a balanced use of all representational dimensions--all of which enable agents to be more adaptive and stable. Building on this insight, we propose the use of Sketched Isotropic Gaussian Regularization for shaping representations toward an isotropic Gaussian distribution during training. We demonstrate empirically, over a variety of domains, that this simple and computationally inexpensive method improves performance under non-stationarity while reducing representation collapse, neuron dormancy, and training instability.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
基于各向同性高斯表示的稳定深度强化学习。

### 2. 核心内容
深度强化学习系统常因非平稳性导致训练不稳定，学习目标与数据分布随时间演变。作者证明在非平稳目标下，各向同性高斯嵌入具有可证明的优势，能稳定跟踪线性读出器的时变目标并在固定方差预算下实现最大熵。基于此提出草图化各向同性高斯正则，将表示训练时拉向各向同性高斯分布，实验表明该方法提升了智能体的适应性与训练稳定性。

### 3. 对应检索需求
deep reinforcement learning research papers。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=gc7Gg18ejz](https://openreview.net/forum?id=gc7Gg18ejz)
