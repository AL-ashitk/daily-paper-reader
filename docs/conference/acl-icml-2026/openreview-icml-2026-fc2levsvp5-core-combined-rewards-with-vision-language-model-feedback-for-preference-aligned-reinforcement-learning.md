---
title: "CoRe: Combined Rewards with Vision-Language Model Feedback for Preference-Aligned Reinforcement Learning"
title_zh: CoRe：结合奖励与视觉语言模型反馈的偏好对齐强化学习
authors: "Hexian Ni, Tao Lu, Yinghao Cai"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/7d86ff59db062a8752010caf77fd1058bde98042.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 结合奖励与视觉语言模型反馈的偏好对齐强化学习
tldr: 奖励设计是强化学习的核心难题，手工奖励难以指定且可能导致次优策略，而基于偏好学习的奖励又存在效率低与训练不稳的问题。受认知科学中人类学习双重性的启发，作者将奖励分解为基于任务知识设计的正式奖励与从观测中学习隐式偏好的残差奖励。基于此提出混合框架CoRe，融合视觉语言模型反馈以获得偏好对齐策略，兼顾效率与稳定性。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 强化学习中手工奖励难指定，偏好学习奖励又效率低且训练不稳。
method: 作者将奖励分解为正式奖励与残差奖励，提出融合视觉语言模型反馈的CoRe框架。
result: 该框架兼顾任务知识与隐式偏好，实现更高效的偏好对齐策略。
conclusion: 该工作为强化学习奖励设计提供了结合知识与模型反馈的新思路。
---

## Abstract
Reward design remains a central challenge in reinforcement learning (RL). Hand-crafted rewards are often difficult to specify and may lead to suboptimal policies, while learned rewards from preferences can suffer from inefficiency and unstable training. Inspired by the dual nature of human learning explored in cognitive science, we decompose rewards into two complementary components: Formal Rewards (FR), explicitly designed based on task knowledge, and Residual Rewards (RR), learned from observations to capture implicit and nuanced preferences. Based on this decomposition, we propose CoRe, a hybrid framework that integrates FR and RR with vision-language models (VLMs) feedback to achieve preference-aligned policies without human involvement. Our contributions are twofold: (1) We propose a Formal Reward Module (FRM) that leverages VLMs to iteratively design and optimize FR based on task knowledge and preference feedback, enabling the continual improvement of policy during training; (2) We introduce a Residual Reward Module (RRM) that learns RR from video-level preference by employing VLMs to generate preference labels and capturing nuanced rewards that complement FR, ensuring alignment with human intent. Through the synergy of FRM and RRM, CoRe enables the automatic construction of reliable rewards that are efficient and preference-aligned. Extensive experiments demonstrate that CoRe outperforms existing approaches in terms of policy learning effectiveness and efficiency on ten robotic manipulation tasks in simulation and five real-worlds.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
结合奖励与视觉语言模型反馈的偏好对齐强化学习。

### 2. 核心内容
奖励设计是强化学习的核心难题，手工奖励难以指定且可能导致次优策略，而基于偏好学习的奖励又存在效率低与训练不稳的问题。受认知科学中人类学习双重性的启发，作者将奖励分解为基于任务知识设计的正式奖励与从观测中学习隐式偏好的残差奖励。基于此提出混合框架CoRe，融合视觉语言模型反馈以获得偏好对齐策略，兼顾效率与稳定性。

### 3. 对应检索需求
algorithms for reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=FC2LEVsvP5](https://openreview.net/forum?id=FC2LEVsvP5)
