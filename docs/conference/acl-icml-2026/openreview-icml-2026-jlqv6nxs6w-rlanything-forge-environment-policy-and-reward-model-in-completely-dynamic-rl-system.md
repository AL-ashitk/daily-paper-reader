---
title: "RLAnything: Forge Environment, Policy, and Reward Model in Completely Dynamic RL System"
title_zh: RLAnything：在完全动态强化学习系统中锻造环境、策略与奖励模型
authors: "Yinjie Wang, Tianbao Xie, Ke Shen, Mengdi Wang, Ling Yang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/51bd8d71b4067004e4770a8fd39d2af5c1ba5e5c.pdf"
tags: ["query:rl"]
score: 8.0
evidence: 联合优化环境、策略与奖励模型的强化学习框架
tldr: 环境与奖励模型的质量从根本上决定强化学习的效果，但现有方法往往固定或分别处理这些组件。本文提出RLAnything，一个通过闭环优化动态调整各组件、放大学习信号的强化学习框架。策略利用逐步与结果信号的综合反馈训练，奖励模型通过一致性反馈联合优化并反哺策略，环境则借助评论家反馈实现理论驱动的自动适应。该工作展示了组件协同进化对整体系统性能的提升。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 环境与奖励模型质量决定强化学习效果，但各组件常被固定或分开处理。
method: 提出RLAnything框架，以闭环反馈联合优化策略、奖励模型与环境。
result: 逐步与结果反馈、一致性反馈及环境自适应共同放大学习信号并提升性能。
conclusion: 展示组件协同进化的完全动态强化学习系统可增强整体学习效果。
---

## Abstract
The quality of both the environment and the reward model fundamentally governs the effectiveness of reinforcement learning. Accordingly, we propose RLAnything, a reinforcement learning framework that dynamically optimizes each component through closed-loop optimization, amplifying learning signals and strengthening the overall system.
Specifically, the policy is trained with integrated feedback from step-wise and outcome signals, while the reward model is jointly optimized via consistency feedback, which in turn further improves policy training. Moreover, our theory-motivated automatic environment adaptation improves training for both the reward and policy models by leveraging critic feedback from each, enabling learning from experience.
Empirically, each added component consistently improves the overall system, and RLAnything yields substantial gains in practical applications, boosting Qwen3-VL-8B-Thinking by 8.5% on OSWorld and Qwen2.5-7B-Instruct by 21.2% and 12.1% on AlfWorld and LiveBench, respectively.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
联合优化环境、策略与奖励模型的强化学习框架。

### 2. 核心内容
环境与奖励模型的质量从根本上决定强化学习的效果，但现有方法往往固定或分别处理这些组件。本文提出RLAnything，一个通过闭环优化动态调整各组件、放大学习信号的强化学习框架。策略利用逐步与结果信号的综合反馈训练，奖励模型通过一致性反馈联合优化并反哺策略，环境则借助评论家反馈实现理论驱动的自动适应。该工作展示了组件协同进化对整体系统性能的提升。

### 3. 对应检索需求
algorithms for reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=JLQV6NxS6W](https://openreview.net/forum?id=JLQV6NxS6W)
