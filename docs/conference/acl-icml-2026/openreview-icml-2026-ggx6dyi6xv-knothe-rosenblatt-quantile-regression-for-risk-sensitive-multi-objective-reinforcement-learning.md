---
title: Knothe-Rosenblatt Quantile Regression for Risk-sensitive Multi-objective Reinforcement Learning
title_zh: 面向风险敏感多目标强化学习的Knothe-Rosenblatt分位数回归
authors: "Gwangpyo Yoo, Woo Kyung Kim, Honguk Woo"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/095cf5180b1c9097680b6a3cdab62e2dc0f5fe7f.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 分布式多目标强化学习
tldr: 本文旨在把分布式强化学习扩展到风险敏感的多目标场景，应用于金融与机器人等领域。作者采用向量风险度量并用Knothe-Rosenblatt分位数回归进行近似，直接扩展IQN框架，从而与向量风险度量的公理化定义对齐，并保证评判器在分布式Bellman算子下收敛。为缓解KR映射引入的人为排序，方法使用无位置编码的Transformer架构并引入MO-TQC以稳定训练。实验显示其多目标任务表现更优。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 需要将分布式强化学习扩展到风险敏感的多目标决策场景。
method: 采用向量风险度量并用Knothe-Rosenblatt分位数回归近似，扩展IQN框架，结合无位置编码Transformer与MO-TQC。
result: 保证评判器在分布式Bellman算子下收敛，并在多目标任务上取得更优表现。
conclusion: 提供风险敏感多目标分布式强化学习框架。
---

## Abstract
In this work, we extend distributional reinforcement learning (RL) to develop a risk-sensitive multi-objective RL framework, with applications to domains such as finance and robotics. We achieve this by adopting vector-risk measures and approximating them via Knothe-Rosenblatt (KR) quantile regression. This approach directly extends the IQN framework to the multi-objective setting, aligns with the axiomatic definition of vector-risk measures, and guarantees that critics converge under the distributional Bellman operator. To mitigate the artificial ordering imposed by the KR map, we employ a transformer architecture without positional encoding, and introduce MO-TQC for training stability. We demonstrate improved performance on MO-Gymnasium benchmarks and use our framework to study risk-sensitive policies in multi-objective tasks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
分布式多目标强化学习。

### 2. 核心内容
本文旨在把分布式强化学习扩展到风险敏感的多目标场景，应用于金融与机器人等领域。作者采用向量风险度量并用Knothe-Rosenblatt分位数回归进行近似，直接扩展IQN框架，从而与向量风险度量的公理化定义对齐，并保证评判器在分布式Bellman算子下收敛。为缓解KR映射引入的人为排序，方法使用无位置编码的Transformer架构并引入MO-TQC以稳定训练。实验显示其多目标任务表现更优。

### 3. 对应检索需求
papers on reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=gGx6DyI6Xv](https://openreview.net/forum?id=gGx6DyI6Xv)
