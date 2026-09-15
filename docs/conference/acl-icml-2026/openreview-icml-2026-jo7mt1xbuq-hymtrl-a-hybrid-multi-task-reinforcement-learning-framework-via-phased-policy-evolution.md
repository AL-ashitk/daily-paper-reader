---
title: "HyMTRL: A Hybrid Multi-Task Reinforcement Learning Framework via Phased Policy Evolution"
title_zh: HyMTRL：通过分阶段策略演化的混合多任务强化学习框架
authors: "Jinmin He, Kai Li, Xiaoyi Dong, Yifan Zang, Yuheng Jing, Yifan Zhang, Junliang Xing, Jian Cheng"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/be055576acdc2e71ee6f2f437a12f49557eb0b80.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 通过分阶段策略演化的混合多任务强化学习
tldr: 多任务强化学习通过共享知识提升样本效率，但任务难度差异导致收敛速度不同步，给共享评论家网络带来巨大表示压力，成为性能瓶颈。本文提出混合多任务强化学习框架HyMTRL，采用分阶段策略演化策略，将任务学习划分为强化探索阶段与模仿精炼阶段，把已掌握任务从强化学习策略优化过渡到模仿学习。实验表明该方法缓解了评论家过载，提升了多任务学习的样本效率与整体性能。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多任务强化学习因任务难度差异导致收敛不同步，给共享评论家网络带来过载。
method: 提出HyMTRL框架，通过分阶段策略演化将任务分为强化探索与模仿精炼两阶段。
result: 缓解评论家过载，提升多任务学习的样本效率与整体性能。
conclusion: 为多任务强化学习提供了一种缓解共享网络瓶颈的分阶段混合框架。
---

## Abstract
Multi-task reinforcement learning (MTRL) aims to improve sample efficiency by sharing knowledge across related tasks, but it often suffers from asynchronous convergence speed caused by inherent differences in task difficulty. This imbalance places substantial representational strain on the shared critic network, which emerges as a major performance bottleneck. To address this issue, we propose Hybrid Multi-Task Reinforcement Learning (HyMTRL), a framework that alleviates critic overload through a phased policy evolution strategy. HyMTRL divides task learning into a reinforcement exploration phase and an imitation refinement phase. By transitioning mastered tasks from reinforcement learning–based policy optimization to imitation learning–based behavior consolidation, these tasks are removed from the critic’s optimization objective, effectively reducing representational strain. In addition, a critic reset mechanism restores network capacity while preserving learned policy and historical experience. HyMTRL is a general framework that can be easily integrated with a wide range of existing MTRL methods. Empirical evaluations on the MetaWorld benchmark demonstrate that HyMTRL leads to significant improvements in both learning efficiency and final performance.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
通过分阶段策略演化的混合多任务强化学习。

### 2. 核心内容
多任务强化学习通过共享知识提升样本效率，但任务难度差异导致收敛速度不同步，给共享评论家网络带来巨大表示压力，成为性能瓶颈。本文提出混合多任务强化学习框架HyMTRL，采用分阶段策略演化策略，将任务学习划分为强化探索阶段与模仿精炼阶段，把已掌握任务从强化学习策略优化过渡到模仿学习。实验表明该方法缓解了评论家过载，提升了多任务学习的样本效率与整体性能。

### 3. 对应检索需求
papers on reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=Jo7Mt1XbuQ](https://openreview.net/forum?id=Jo7Mt1XbuQ)
