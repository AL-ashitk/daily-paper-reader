---
title: Learning Generalizable Skill Policy with Data-Efficient Unsupervised RL
title_zh: 学习可泛化技能策略的数据高效无监督强化学习
authors: "Jongchan Park, Seungjun Oh, Seungho Baek, Yusung Kim"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/336fa9c2dc8ff5721807a88c429239ab8f3f6ceb.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 面向可泛化技能策略的无监督强化学习框架
tldr: 无监督强化学习旨在无外部奖励下预训练可扩展的技能条件策略，但现有离策略方法受技能语义非平稳与泛化脆弱两大瓶颈制约。本文提出统一框架GenDa，引入技能重标记机制缓解非平稳性并显著提升预训练样本效率，并设计互补信息瓶颈（CIB）增强技能策略的泛化能力。实验表明该方法在下游控制任务上兼具数据高效与强泛化性能，为无监督强化学习预训练提供了稳健方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有离策略无监督强化学习存在技能语义非平稳与泛化脆弱两大瓶颈。
method: 提出GenDa框架，包含技能重标记机制与互补信息瓶颈模块。
result: 显著提升预训练样本效率，并在下游控制任务上实现更强泛化。
conclusion: 为稳健且数据高效的无监督强化学习预训练提供了统一框架。
---

## Abstract
Unsupervised Reinforcement Learning (URL) aims to pre-train scalable, skill-conditioned policies without extrinsic rewards, serving as a foundation for downstream control tasks. Despite recent progress, we argue that current off-policy URL methods are limited by two critical, overlooked bottlenecks: (1) non-stationarity skill semantic and (2) brittle generalization. To address these challenges, we propose GenDa (Generalizable Data-efficient Agent), a unified framework for robust unsupervised reinforcement learning. First, we introduce a skill relabeling mechanism to mitigate non-stationarity and significantly improve sample efficiency for pretraining. Second, we propose a Complementary Information Bottleneck(CIB), encouraging the learned skill policy to focus on ego-centric features and become robust to distribution shifts for downstream tasks. Through various experiments, we demonstrate that GenDa significantly enhances the scalability of URL with superior generality and sample efficiency. Our source codes are available in the supplementary materials.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向可泛化技能策略的无监督强化学习框架。

### 2. 核心内容
无监督强化学习旨在无外部奖励下预训练可扩展的技能条件策略，但现有离策略方法受技能语义非平稳与泛化脆弱两大瓶颈制约。本文提出统一框架GenDa，引入技能重标记机制缓解非平稳性并显著提升预训练样本效率，并设计互补信息瓶颈（CIB）增强技能策略的泛化能力。实验表明该方法在下游控制任务上兼具数据高效与强泛化性能，为无监督强化学习预训练提供了稳健方案。

### 3. 对应检索需求
papers on reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=qgAKuqzYBC](https://openreview.net/forum?id=qgAKuqzYBC)
