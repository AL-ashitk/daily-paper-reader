---
title: "Learning from Less: Guiding Deep Reinforcement Learning with Differentiable Symbolic Planning"
title_zh: 以少学多：用可微符号规划引导深度强化学习
authors: "Zihan Ye, Oleg Arenz, Kristian Kersting"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/a730abdc0b2f930c5282ddc543d630c47d641be1.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 用可微符号规划引导深度强化学习以提升样本效率
tldr: 深度强化学习智能体缺乏人类式的任务分解与动态改计划先验，通常需要大量交互才能学会自适应行为。本文提出可微符号规划器Dylan，将符号规划融入深度强化学习，为智能体提供类似人类的先验，使其能随观测灵活修正子任务计划。该框架旨在减少训练交互次数，在复杂任务上提升样本效率，为结合符号推理与深度强化学习提供了新思路。
source: ICML-2026-Rejected-Public
selection_source: conference_retrieval
motivation: 深度强化学习智能体缺乏人类式任务分解与改计划先验，样本效率低。
method: 提出可微符号规划器Dylan，将符号规划集成进深度强化学习。
result: 智能体可随观测灵活修正子任务计划，用更少交互学习复杂任务。
conclusion: 为符号规划与深度强化学习结合以提升样本效率提供新框架。
---

## Abstract
Humans solve complex tasks by decomposing them into subtasks and flexibly revising plans based on observations. For example, when making coffee at a friend’s place, you may initially plan to fetch coffee beans but skip this step upon noticing the machine is already full. In contrast, deep reinforcement learning agents lack such priors and typically require  more interactions to achieve such adaptive behavior. This raises a key question: How can we endow reinforcement learning (RL) agents with similar ``human'' priors, allowing the agent to learn with fewer training interactions? To address this challenge, We propose differentiable symbolic planner (Dylan), a novel framework that integrates symbolic planning into reinforcement learning. Dylan functions as a differentiable reward model that incorporates human priors to shape rewards over intermediate subtasks, enabling more efficient exploration. Beyond reward shaping, Dylan can also act as a high-level planner that composes logic-based options to generate new behaviors while avoiding common symbolic planning pitfalls such as infinite execution loops. We validate Dylan on challenging exploration and generalization tasks, where it effectively overcomes reward sparsity through structured, symbolic guidance, and enables zero-shot generalization to novel tasks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
用可微符号规划引导深度强化学习以提升样本效率。

### 2. 核心内容
深度强化学习智能体缺乏人类式的任务分解与动态改计划先验，通常需要大量交互才能学会自适应行为。本文提出可微符号规划器Dylan，将符号规划融入深度强化学习，为智能体提供类似人类的先验，使其能随观测灵活修正子任务计划。该框架旨在减少训练交互次数，在复杂任务上提升样本效率，为结合符号推理与深度强化学习提供了新思路。

### 3. 对应检索需求
deep reinforcement learning research papers。

### 4. 来源与原文
- Source：ICML-2026-Rejected-Public
- OpenReview：[https://openreview.net/forum?id=pITxfp6Fu5](https://openreview.net/forum?id=pITxfp6Fu5)
