---
title: Hybrid Reinforcement Learning in Adversarial Markov Decision Processes
title_zh: 对抗马尔可夫决策过程中的混合强化学习
authors: "Duo Cheng, Xingyu Zhou, Bo Ji"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/faa6a4c9e140e2273b2ee465d750fd58ad8e9e45.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 对抗MDP中结合在策略与离策略反馈的混合强化学习
tldr: 该文研究对抗马尔可夫决策过程中的混合强化学习，学习器同时获得执行策略的在策略反馈与固定行为策略的离策略反馈，且损失可随时间任意变化。作者提出新的混合强化学习框架，可处理对抗损失与未知转移，在策略反馈保证对任意比较策略的最坏情况界，离策略反馈给出随覆盖比缩放的依赖覆盖保证。该框架在覆盖比小时能给出比纯在策略更紧的结果，拓展了对抗环境下的强化学习理论。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 在对抗MDP中单一反馈类型难以同时获得最坏情况与依赖覆盖的保证。
method: 提出融合在策略与离策略反馈的混合强化学习框架，适应对抗损失与未知转移。
result: 同时给出最坏情况保证与随覆盖比缩放的依赖覆盖保证，覆盖比小时更紧。
conclusion: 为对抗环境下的混合反馈强化学习提供统一理论框架。
---

## Abstract
We study hybrid reinforcement learning (RL) in adversarial Markov Decision Processes (MDPs), where the learner simultaneously receives on-policy feedback from the executed policy and off-policy feedback from a fixed behavior policy, and loss functions can change arbitrarily over time. On-policy feedback allows exploration and ensures the worst-case guarantee against any comparator policy, while off-policy feedback provides coverage-dependent guarantee that scales with the "mismatch" between the behavior and comparator policies (called coverage ratio) and can be sharper than on-policy results whenever this ratio is small. We propose a new hybrid RL framework that accommodates adversarial losses and unknown transitions, preserving off-policy guarantees while ensuring non-trivial worst-case performance.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
对抗MDP中结合在策略与离策略反馈的混合强化学习。

### 2. 核心内容
该文研究对抗马尔可夫决策过程中的混合强化学习，学习器同时获得执行策略的在策略反馈与固定行为策略的离策略反馈，且损失可随时间任意变化。作者提出新的混合强化学习框架，可处理对抗损失与未知转移，在策略反馈保证对任意比较策略的最坏情况界，离策略反馈给出随覆盖比缩放的依赖覆盖保证。该框架在覆盖比小时能给出比纯在策略更紧的结果，拓展了对抗环境下的强化学习理论。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=rfIFRFon5W](https://openreview.net/forum?id=rfIFRFon5W)
