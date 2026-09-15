---
title: Black-Box Combinatorial Optimization with Order-Invariant Reinforcement Learning
title_zh: 基于顺序不变强化学习的黑盒组合优化
authors: "Olivier Goudet, Quentin Suire, Adrien Goëffon, Frédéric Saubion, Sylvain Lamprier"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/bd8e5a14727ae7966fe7d5321582ad3519a2c2d9.pdf"
tags: ["query:rl"]
score: 8.0
evidence: 用于黑盒组合优化的顺序不变强化学习
tldr: 经典分布估计算法在黑盒组合优化中依赖显式变量依赖图，代价高且难以捕捉复杂交互。作者提出顺序不变的强化学习框架，参数化多元自回归生成模型并在训练中采样随机生成顺序，以信息保持式丢弃促使模型对变量顺序不变。该设计提升搜索空间多样性与样本效率，并适配组相对策略优化，改善了组合优化效果。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 经典分布估计算法依赖显式变量依赖图，代价高且难以捕捉复杂交互。
method: 作者提出顺序不变强化学习框架，用随机生成顺序训练自回归模型并适配GRPO。
result: 该方法提升搜索空间多样性与样本效率，改善黑盒组合优化性能。
conclusion: 该工作为黑盒组合优化提供了无需固定变量顺序的强化学习方案。
---

## Abstract
We introduce an order-invariant reinforcement learning framework for black-box combinatorial optimization. Classical estimation-of-distribution algorithms (EDAs) often rely on learning explicit variable dependency graphs, which can be costly and may fail to capture complex interactions efficiently. In contrast, we parameterize a multivariate autoregressive generative model trained without a fixed variable ordering. By sampling random generation orders during training, a form of information-preserving dropout, the model is encouraged to be invariant to variable order, promoting search-space diversity, and shaping the model to focus on the most relevant variable dependencies, improving sample efficiency. We adapt Group Relative Policy Optimization (GRPO) to this setting, providing stable policy-gradient updates from scale-invariant advantages. Across a wide range of benchmark problem instances of varying sizes, our method frequently achieves the best performance and consistently avoids catastrophic failures.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
用于黑盒组合优化的顺序不变强化学习。

### 2. 核心内容
经典分布估计算法在黑盒组合优化中依赖显式变量依赖图，代价高且难以捕捉复杂交互。作者提出顺序不变的强化学习框架，参数化多元自回归生成模型并在训练中采样随机生成顺序，以信息保持式丢弃促使模型对变量顺序不变。该设计提升搜索空间多样性与样本效率，并适配组相对策略优化，改善了组合优化效果。

### 3. 对应检索需求
papers on reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=bcRBqG8FFN](https://openreview.net/forum?id=bcRBqG8FFN)
