---
title: "MEAL: A Benchmark for Continual Multi-Agent Reinforcement Learning"
title_zh: MEAL：面向持续多智能体强化学习的基准
authors: "Tristan Tomilin, Luka van den Boogaard, Samuel Garcin, Constantin Ruhdorfer, Bram Grooten, Fabrice Kusters, Yali Du, Andreas Bulling, Mykola Pechenizkiy, Meng Fang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/f7ee900e02da7357f11c62a903340308441d51d4.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 面向持续多智能体强化学习的基准
tldr: 基准在强化学习研究中居于核心地位，但其计算约束常左右研究范围，多数持续RL工作仅考虑3到10个连续任务，而合作多智能体场景下的持续学习几乎未被探索。本文提出MEAL，这是首个面向持续多智能体强化学习的基准，借助JAX与GPU加速，可在单块GPU上于数小时内完成100个任务的序列训练。研究发现长任务序列会暴露小规模下不出现的失效模式。该基准有力推动了长期与多智能体持续强化学习研究。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 持续强化学习研究因CPU环境限制仅考虑少数任务，合作多智能体持续学习几乎未被探索。
method: 提出MEAL，基于JAX与GPU加速的首个持续多智能体强化学习基准，支持单GPU上百任务序列。
result: 发现长任务序列会暴露小规模下不出现的失效模式。
conclusion: 推动长期与多智能体持续强化学习研究。
---

## Abstract
Benchmarks play a central role in reinforcement learning (RL) research, yet their computational constraints often shape what is studied. Despite the motivation of lifelong learning, most continual RL papers consider only 3–10 sequential tasks, as CPU-bound environments make longer sequences impractical. Meanwhile, continual learning in cooperative multi-agent settings remains largely unexplored. To address these gaps, we introduce **MEAL** (**M**ulti-agent **E**nvironments for **A**daptive **L**earning), the first benchmark for continual multi-agent RL. By leveraging JAX and GPU acceleration, MEAL enables training on sequences of 100 tasks on a single GPU in a few hours. We find that long task sequences reveal failure modes that do not appear at smaller scales.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向持续多智能体强化学习的基准。

### 2. 核心内容
基准在强化学习研究中居于核心地位，但其计算约束常左右研究范围，多数持续RL工作仅考虑3到10个连续任务，而合作多智能体场景下的持续学习几乎未被探索。本文提出MEAL，这是首个面向持续多智能体强化学习的基准，借助JAX与GPU加速，可在单块GPU上于数小时内完成100个任务的序列训练。研究发现长任务序列会暴露小规模下不出现的失效模式。该基准有力推动了长期与多智能体持续强化学习研究。

### 3. 对应检索需求
multi-agent reinforcement learning papers。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=Mxg6mo1Xzj](https://openreview.net/forum?id=Mxg6mo1Xzj)
