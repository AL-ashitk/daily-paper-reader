---
title: Model-Free Robust Average-Reward Reinforcement Learning with Sample Complexity Analysis
title_zh: 免模型鲁棒平均奖励强化学习及其样本复杂度分析
authors: "Zachary Andrew Roch, George K. Atia, Yue Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/86321fb56605ffefa4601f37c11cbb6b6778224a.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 带有限样本复杂度分析的免模型鲁棒平均奖励强化学习
tldr: 鲁棒强化学习在平均奖励准则下对长期决策至关重要，尤其在环境动态与训练时不同时。然而现有研究多集中于基于模型的设置且仅给出渐近保证，难以在数据受限场景下理解与部署。作者提出免模型算法鲁棒Halpern迭代，基于黑盒采样预言机估计最坏情形性能，并推导其有限样本复杂度。该工作填补了鲁棒平均奖励强化学习在数据有限情形下的理论空白。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 鲁棒平均奖励强化学习现有研究多基于模型且仅有渐近保证，难以在数据受限场景部署。
method: 作者提出免模型算法鲁棒Halpern迭代，基于黑盒采样预言机估计最坏情形性能。
result: 理论推导出该算法在生成模型设置下的有限样本复杂度。
conclusion: 该工作填补了鲁棒平均奖励强化学习的有限样本理论空白。
---

## Abstract
Robust reinforcement learning (RL) under the average-reward criterion is essential for long-term decision-making, particularly when the environment may differ from its training dynamics. However, most existing studies focus on model-based settings and provide only asymptotic guarantees, hindering their principled understanding and practical deployment, especially in data-limited scenarios. We aim to close this gap by proposing a model-free algorithm, **Robust Halpern Iteration (RHI)**. We first design our algorithm based on a black-box sampling oracle, which can estimate the worst-case performance accurately. We then derive the finite sample complexity of RHI under the generative model setting, assuming the sampling oracle. To concretely design such an oracle, we propose a $K$-order multi-level Monte-Carlo estimator, which is shown to have a lower bias compared to prior methods. We further instantiate our design for multiple uncertainty models, including KL and $\chi^2$ divergence sets, and show that our RHI algorithm achieves an $\varepsilon$-optimal robust policy with a sample complexity of $\tilde{\mathcal{O}}\left( \frac{SA\mathcal{H}^2}{\varepsilon^{(2+o(1))}}\right)$, where $S,A$ are the number of states and actions, and $\mathcal{H}$ is the robust optimal span. Our result asymptotically matches the best complexity in robust average reward RL.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
带有限样本复杂度分析的免模型鲁棒平均奖励强化学习。

### 2. 核心内容
鲁棒强化学习在平均奖励准则下对长期决策至关重要，尤其在环境动态与训练时不同时。然而现有研究多集中于基于模型的设置且仅给出渐近保证，难以在数据受限场景下理解与部署。作者提出免模型算法鲁棒Halpern迭代，基于黑盒采样预言机估计最坏情形性能，并推导其有限样本复杂度。该工作填补了鲁棒平均奖励强化学习在数据有限情形下的理论空白。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=GMIHHrJ6Wp](https://openreview.net/forum?id=GMIHHrJ6Wp)
