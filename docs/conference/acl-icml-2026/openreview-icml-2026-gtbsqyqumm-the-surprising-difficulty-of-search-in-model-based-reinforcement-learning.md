---
title: The Surprising Difficulty of Search in Model-Based Reinforcement Learning
title_zh: 模型强化学习中搜索的惊人困难
authors: "Wei-Di Chang, Mikael Henaff, Brandon Amos, Gregory Dudek, Scott Fujimoto"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/24e24d6737811a8652e6ee09e4073412149557b1.pdf"
tags: ["query:rl"]
score: 10.0
evidence: 模型强化学习中搜索作用的研究
tldr: 通常认为长期预测与误差累积是模型强化学习的主要障碍。作者对此提出挑战，发现搜索并非学习策略的即插即用替代，即便模型高度准确，搜索也可能损害性能。研究表明缓解高估偏差比提升模型或价值函数精度更重要，并对价值函数集成取最小值可有效应对该偏差。基于此方法在多个主流基准上达到最先进性能，重新审视了模型强化学习中搜索的作用。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 传统观点认为长期预测与误差累积是模型强化学习的主要障碍。
method: 作者系统研究模型强化学习中的搜索，并对价值函数集成取最小值以缓解高估偏差。
result: 实验表明缓解高估偏差比提升精度更关键，方法在多个基准达到最先进性能。
conclusion: 该工作重新审视了搜索在模型强化学习中的作用与关键障碍。
---

## Abstract
This paper investigates search in model-based reinforcement learning (RL). Conventional wisdom holds that long-term predictions and compounding errors are the primary obstacles for model-based RL. We challenge this view, showing that search is not a drop-in replacement for a learned policy. Surprisingly, we find that search can harm performance even when the model is highly accurate. Instead, we show that mitigating overestimation bias matters more than improving model or value function accuracy. Building on this insight, we identify that taking the minimum over an ensemble of value functions effectively addresses this bias and enables effective search, achieving state-of-the-art performance across multiple popular benchmark domains. Code can be found at https://github.com/facebookresearch/MRSQ.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
模型强化学习中搜索作用的研究。

### 2. 核心内容
通常认为长期预测与误差累积是模型强化学习的主要障碍。作者对此提出挑战，发现搜索并非学习策略的即插即用替代，即便模型高度准确，搜索也可能损害性能。研究表明缓解高估偏差比提升模型或价值函数精度更重要，并对价值函数集成取最小值可有效应对该偏差。基于此方法在多个主流基准上达到最先进性能，重新审视了模型强化学习中搜索的作用。

### 3. 对应检索需求
model-based reinforcement learning papers。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=gTbSqYqumM](https://openreview.net/forum?id=gTbSqYqumM)
