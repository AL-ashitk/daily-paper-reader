---
title: What Makes Value Learning Efficient in Residual Reinforcement Learning?
title_zh: 是什么让残差强化学习中的价值学习高效
authors: "Guozheng Ma, Lu Li, Haoyu Wang, Zixuan Liu, Pierre-Luc Bacon, Dacheng Tao"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/ebd90c4553944cff7ac36ef3d715054e374d9d7a.pdf"
tags: ["query:rl"]
score: 8.0
evidence: 残差强化学习中的价值学习效率
tldr: 残差强化学习通过冻结基策略并仅学习有界修正来稳定地在线改进预训练策略，但其价值学习面临的独特挑战尚不清晰。作者识别出冷启动病态与结构尺度失配两个关键瓶颈，前者指评论家不了解基策略周围的价值景观，后者指残差贡献被基动作淹没。研究表明简单原则性方案即可解决，如以基策略转移作为价值锚进行隐式预热并对评论家归一化，从而提升价值学习效率。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 残差强化学习的价值学习面临冷启动与结构尺度失配等独特挑战。
method: 作者系统分析两类瓶颈机制，提出以基策略转移为价值锚并对评论家归一化。
result: 研究表明这些简单方案即可有效缓解瓶颈并提升价值学习效率。
conclusion: 该工作揭示了残差强化学习价值学习的关键机制与实用改进。
---

## Abstract
Residual reinforcement learning (RL) enables stable online refinement of expressive pretrained policies by freezing the base and learning only bounded corrections. However, value learning in residual RL poses unique challenges that remain poorly understood. In this work, we identify two key bottlenecks: cold start pathology, where the critic lacks knowledge of the value landscape around the base policy, and structural scale mismatch, where the residual contribution is dwarfed by the base action. Through systematic investigation, we uncover the mechanisms underlying these bottlenecks, revealing that simple yet principled solutions suffice: base-policy transitions serve as an essential value anchor for implicit warmup, and critic normalization effectively restores representation sensitivity for discerning value differences. Based on these insights, we propose DAWN (Data-Anchored Warmup and Normalization), a minimal approach targeting efficient value learning in residual RL. By addressing these bottlenecks, DAWN demonstrates substantial efficiency gains across diverse benchmarks, policy architectures, and observation modalities.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
残差强化学习中的价值学习效率。

### 2. 核心内容
残差强化学习通过冻结基策略并仅学习有界修正来稳定地在线改进预训练策略，但其价值学习面临的独特挑战尚不清晰。作者识别出冷启动病态与结构尺度失配两个关键瓶颈，前者指评论家不了解基策略周围的价值景观，后者指残差贡献被基动作淹没。研究表明简单原则性方案即可解决，如以基策略转移作为价值锚进行隐式预热并对评论家归一化，从而提升价值学习效率。

### 3. 对应检索需求
algorithms for reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=tSMZHXtJwZ](https://openreview.net/forum?id=tSMZHXtJwZ)
