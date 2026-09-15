---
title: Rationality Measurement and Theory for Reinforcement Learning Agents
title_zh: 强化学习智能体的理性度量与理论
authors: "Kejiang Qian, Amos Storkey, Fengxiang He"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/92cfa06cb8b3b70cc505d77cb296772df506259d.pdf"
tags: ["query:rl"]
score: 8.0
evidence: 面向强化学习智能体的理论与度量
tldr: 理性对强化学习智能体日益关键却鲜有研究。本文提出一套理性度量及其理论，将部署中的动作定义为在最陡方向上最大化隐藏真实价值函数即为完全理性，并把策略动作相对理性动作的期望价值差异定义为期望理性风险，同时给出训练中的经验平均版本。二者的差被称为理性风险缺口，被分解为由训练与部署环境变化引起的外在成分和由算法动态泛化能力导致的内在成分。该工作为评估强化学习智能体的理性提供了理论与度量工具。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 理性这一关键性质在强化学习智能体中很少被系统研究。
method: 提出一套理性度量与理论，定义期望理性风险及理性风险缺口，并将其分解为外在和内在成分。
result: 将部署与训练差异归因于环境变化与算法泛化能力两个方面。
conclusion: 为强化学习智能体的理性评估提供理论与度量工具。
---

## Abstract
This paper proposes a suite of rationality measures and associated theory for reinforcement learning agents, a property increasingly critical yet rarely explored. We define an action in deployment to be perfectly rational if it maximises the hidden true value function in the steepest direction. The expected value discrepancy of a policy's actions against their rational counterparts, culminating over the trajectory in deployment, is defined to be expected rational risk; an empirical average version in training is also defined. Their difference, termed as rational risk gap, is decomposed into (1) an extrinsic component caused by environment shifts between training and deployment, and (2) an intrinsic one due to the algorithm's generalisability in a dynamic environment. They are upper bounded by, respectively, (1) the $1$-Wasserstein distance between transition kernels and initial state distributions in training and deployment, and (2) the empirical Rademacher complexity of the value function class. Our theory suggests hypotheses on the benefits from regularisers (including layer normalisation, $\ell_2$ regularisation, and weight normalisation) and domain randomisation, as well as the harm from environment shifts. Experiments are in full agreement with these hypotheses. The code is available at \href{https://github.com/EVIEHub/Rationality}{https://github.com/EVIEHub/Rationality}.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向强化学习智能体的理论与度量。

### 2. 核心内容
理性对强化学习智能体日益关键却鲜有研究。本文提出一套理性度量及其理论，将部署中的动作定义为在最陡方向上最大化隐藏真实价值函数即为完全理性，并把策略动作相对理性动作的期望价值差异定义为期望理性风险，同时给出训练中的经验平均版本。二者的差被称为理性风险缺口，被分解为由训练与部署环境变化引起的外在成分和由算法动态泛化能力导致的内在成分。该工作为评估强化学习智能体的理性提供了理论与度量工具。

### 3. 对应检索需求
theoretical foundations of reinforcement learning。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=RlEPV6ec7P](https://openreview.net/forum?id=RlEPV6ec7P)
