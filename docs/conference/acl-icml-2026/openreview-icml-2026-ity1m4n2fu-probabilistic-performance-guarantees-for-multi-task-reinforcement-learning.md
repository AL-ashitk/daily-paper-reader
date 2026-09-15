---
title: Probabilistic Performance Guarantees for Multi-Task Reinforcement Learning
title_zh: 多任务强化学习的概率性能保证
authors: "Yannik Schnitzer, Mathias Jackermeier, Alessandro Abate, David Parker"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/42e6f33a9922f0ab1fcd7ddd6b25440b04832259.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 多任务强化学习的正式性能保证
tldr: 多任务强化学习训练通用策略执行多个任务，但现有方法很少提供正式性能保证，这在安全关键场景中难以部署。作者提出一种新的泛化界，将有限回合得到的逐任务下置信界与有限采样任务的任务级泛化相结合。实验表明该方法能为来自未知分布的新任务给出高置信性能保证，为多任务策略的可靠性评估提供了理论工具。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多任务强化学习缺乏正式性能保证，难以应用于安全关键场景。
method: 作者提出新的泛化界，将逐任务下置信界与任务级泛化相结合。
result: 该方法能为来自未知分布的新任务计算高置信性能保证。
conclusion: 该工作为多任务策略提供了可部署的可靠性能评估理论。
---

## Abstract
Multi-task reinforcement learning trains generalist policies that can execute multiple tasks. While recent years have seen significant progress, existing approaches rarely provide formal performance guarantees, which are indispensable when deploying policies in safety-critical settings. We present an approach for computing high-confidence guarantees on the performance of a multi-task policy on tasks not seen during training. Concretely, we introduce a new generalisation bound that composes (i) per-task lower confidence bounds from finitely many rollouts with (ii) task-level generalisation from finitely many sampled tasks, yielding a high-confidence guarantee for new tasks drawn from the same arbitrary and unknown distribution. Across state-of-the-art multi-task RL methods, we show that the guarantees are theoretically sound and informative at realistic sample sizes.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
多任务强化学习的正式性能保证。

### 2. 核心内容
多任务强化学习训练通用策略执行多个任务，但现有方法很少提供正式性能保证，这在安全关键场景中难以部署。作者提出一种新的泛化界，将有限回合得到的逐任务下置信界与有限采样任务的任务级泛化相结合。实验表明该方法能为来自未知分布的新任务给出高置信性能保证，为多任务策略的可靠性评估提供了理论工具。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=iTy1M4N2FU](https://openreview.net/forum?id=iTy1M4N2FU)
