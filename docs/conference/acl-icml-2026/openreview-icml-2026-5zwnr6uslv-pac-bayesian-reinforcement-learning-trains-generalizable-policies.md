---
title: PAC-Bayesian Reinforcement Learning Trains Generalizable Policies
title_zh: PAC-贝叶斯强化学习训练可泛化策略
authors: "Abdelkrim ZITOUNI, Mehdi hennequin, Juba Agoun, Ryan Horache, NADIA KABACHI, Omar Rivasplata"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/2664f0d4fb0c55c45958800378ac262de05ed355.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 强化学习的PAC-贝叶斯泛化界与PB-SAC算法
tldr: 强化学习中数据的序列相关性破坏了经典泛化界的独立同分布假设，导致难以获得有效保证。本文推导出考虑马尔可夫依赖（通过混合时间刻画）的新型PAC-贝叶斯泛化界，为Soft Actor-Critic等现代离策略算法提供非平凡的置信证书。作者进一步提出PB-SAC算法，在训练中优化该界以引导探索，在多个连续控制任务上验证了方法的有效性，为强化学习泛化理论提供了实用工具。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 强化学习数据的序列相关性破坏经典泛化界的独立性假设，难以获得有效保证。
method: 推导通过混合时间刻画马尔可夫依赖的PAC-贝叶斯泛化界，并提出PB-SAC算法。
result: 该界为Soft Actor-Critic等算法提供非平凡证书，PB-SAC在连续控制任务上有效。
conclusion: 为强化学习泛化提供了可实用的理论界与训练算法。
---

## Abstract
We derive a novel PAC-Bayesian generalization bound for reinforcement learning that explicitly accounts for Markov dependencies in the data, through the chain's mixing time. This contributes to overcoming challenges in obtaining generalization guarantees for reinforcement learning, where the sequential nature of data breaks the independence assumptions underlying classical bounds. The new bound provides non-vacuous certificates for modern off-policy algorithms such as Soft Actor-Critic. We demonstrate the practical utility of the bound through PB-SAC, a novel algorithm that optimizes the bound during training to guide exploration. Experiments across several continuous control tasks show that the proposed approach provides meaningful confidence certificates while maintaining competitive performance.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
强化学习的PAC-贝叶斯泛化界与PB-SAC算法。

### 2. 核心内容
强化学习中数据的序列相关性破坏了经典泛化界的独立同分布假设，导致难以获得有效保证。本文推导出考虑马尔可夫依赖（通过混合时间刻画）的新型PAC-贝叶斯泛化界，为Soft Actor-Critic等现代离策略算法提供非平凡的置信证书。作者进一步提出PB-SAC算法，在训练中优化该界以引导探索，在多个连续控制任务上验证了方法的有效性，为强化学习泛化理论提供了实用工具。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=5Zwnr6uSlv](https://openreview.net/forum?id=5Zwnr6uSlv)
