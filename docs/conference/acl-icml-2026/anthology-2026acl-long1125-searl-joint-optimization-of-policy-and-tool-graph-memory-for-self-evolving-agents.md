---
title: "SEARL: Joint Optimization of Policy and Tool Graph Memory for Self-Evolving Agents"
title_zh: SEARL：面向自演化智能体的策略与工具图记忆联合优化
authors: "Xinshun Feng, Xinhao Song, Lijun Li, Gongshen Liu, Jing Shao"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://aclanthology.org/2026.acl-long.1125.pdf"
tags: ["query:rl"]
score: 8.0
evidence: 面向自演化工具记忆智能体的可验证奖励强化学习
tldr: 可验证奖励强化学习在单轮推理任务上表现突出，但现有自演化智能体方法依赖大规模模型或多智能体框架，难以在资源受限环境中部署，且结果奖励稀疏带来挑战。本文提出基于工具记忆的自演化智能体框架SEARL，联合优化策略与工具图记忆，使模型能够通过合成工具与积累经验持续自我演化。该方法缓解了奖励稀疏问题，提升了在受限资源下的自演化学习效率。
source: ACL-2026-Long
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1125/fig-001.webp\", \"caption\": \"\", \"page\": 1, \"index\": 1, \"width\": 521, \"height\": 479}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1125/fig-002.webp\", \"caption\": \"\", \"page\": 1, \"index\": 2, \"width\": 537, \"height\": 439}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1125/fig-003.webp\", \"caption\": \"\", \"page\": 1, \"index\": 3, \"width\": 560, \"height\": 446}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1125/fig-004.webp\", \"caption\": \"\", \"page\": 4, \"index\": 4, \"width\": 8254, \"height\": 4172}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1125/fig-005.webp\", \"caption\": \"\", \"page\": 7, \"index\": 5, \"width\": 2178, \"height\": 1519}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1125/fig-006.webp\", \"caption\": \"\", \"page\": 7, \"index\": 6, \"width\": 2185, \"height\": 1524}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1125/fig-007.webp\", \"caption\": \"\", \"page\": 7, \"index\": 7, \"width\": 2194, \"height\": 1513}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1125/fig-008.webp\", \"caption\": \"\", \"page\": 7, \"index\": 8, \"width\": 2196, \"height\": 1516}]"
motivation: 现有自演化智能体依赖大规模模型且结果奖励稀疏，难以在受限环境部署。
method: 提出SEARL框架，联合优化策略与工具图记忆以支持自演化学习。
result: 通过工具合成与经验积累缓解奖励稀疏，提升受限资源下的学习效率。
conclusion: 为资源受限场景下的自演化智能体提供了高效的可验证奖励强化学习框架。
---

## Abstract
Recent advances in Reinforcement Learning with Verifiable Rewards (RLVR) have demonstrated significant potential in single-turn reasoning tasks. With the paradigm shift toward self-evolving agentic learning, models are increasingly expected to learn from trajectories by synthesizing tools or accumulating explicit experiences. However, prevailing methods typically rely on large-scale LLMs or multi-agent frameworks, which hinder their deployment in resource-constrained environments. The inherent sparsity of outcome-based rewards also poses a substantial challenge, as agents typically receive feedback only upon task completion. To address these limitations, we introduce a Tool-Memory based self-evolving agentic framework SEARL. Unlike approaches that directly utilize interaction experiences, our method constructs a structured experience memory that integrates planning with execution. This provides a novel form of state abstraction that facilitates the aggregation of actions within functionally analogous contexts, such as tool reuse. Consequently, agents not only extract explicit knowledge from historical data but also leverage inter-trajectory correlations to densify reward signals. We evaluate our framework on knowledge reasoning and complex search tasks, demonstrating its effectiveness in achieving more practical and efficient agentic learning.

---

## 论文详细总结（自动生成）

# SEARL 论文中文总结

## 1. 核心问题与整体含义
- **研究背景**：基于可验证奖励的强化学习（RLVR）在单轮推理任务中表现突出，但智能体学习正转向“自演化”范式，要求模型能从轨迹中合成工具、积累显式经验。
- **核心问题**：
  - 现有方法多依赖大规模 LLM 或多智能体框架，难以部署在资源受限环境。
  - 结果型奖励高度稀疏，智能体通常只在任务完成时获得反馈。
  - 工具生成方法常把工具存入非结构化仓库，缺乏显式依赖关系，导致复用性、组合性和细粒度规划能力不足。
  - 小模型生成单体工具容易失败；复杂任务更适合拆分为子任务并生成模块化工具。
  - 现有 RL/经验驱动方法忽略工具间显式依赖，且多只优化策略参数，未把外部记忆作为可共同演化的对象。
- **整体含义**：论文提出 SEARL，将策略模型与工具图记忆联合优化，使智能体在训练中同时提升决策策略和外部工具记忆，从而在资源受限条件下实现更实用、高效的自演化学习。

## 2. 方法论
- **核心思想**：构建结构化的 **Tool Graph Memory**，工具为节点、执行依赖为边；策略模型与工具图在训练中共同演化。智能体通过检索、复用、创建工具，并从历史轨迹中抽取显式知识，利用轨迹间相关性稠密化奖励信号。
- **形式化建模**：
  - 定义“自演化智能体”：通过工具进化或记忆进化提升问题解决能力。
  - 定义“工具记忆增强 MDP”：\(\langle S, A, P, R, TG \rangle\)，其中 \(TG=(V,E)\) 为图结构工具记忆。
  - 策略为 \(\pi_\theta(a_t|s_t,x,TG)\)，训练目标最大化期望奖励并约束与参考策略的 KL 散度。
- **轨迹生成四阶段**：轨迹概率分解为 Retrieve、Reuse、Creation、Transition：
  1. 从记忆中检索相关工具；
  2. 决定是否复用检索到的工具；
  3. 决定是否创建新通用工具并加入记忆；
  4. 环境转移到下一状态。
- **结构化轨迹**：用 XML 标签划分 Planning、Retrieve、Think、Action；工具创建也统一为常规工具调用。
- **奖励设计**：
  - **结果奖励**：任务成功且答案正确为 1，否则为 0。
  - **行为奖励**：规划奖励、工具创建奖励、工具执行奖励。
  - **格式奖励**：输出符合结构时给予正奖励。
- **优势估计**：
  - **Episode-level 相对优势**：对同一任务下的多条轨迹计算总回报，提供任务级粗粒度信号。
  - **Step-level 相对优势**：不以原始环境状态分组，而以“工具使用锚点”分组。将轨迹组中出现的不同 MCP 工具作为锚点，把使用同一工具的动作聚合为步级组，再计算相对优势。
  - 最终优势为 episode 优势与 step 优势的加权组合：\(A = A_E + \omega A_S\)。
- **策略优化**：采用类似 PPO/GRPO 的裁剪目标，加入 KL 惩罚，优化 LLM 策略。
- **工具图记忆生命周期**：
  1. **子图提取**：规划阶段将任务拆为子任务，形成依赖图并投影到工具空间。
  2. **工具注册**：通过 MCP 创建工具，成功执行者进入候选池，按累积奖励筛选后注册。
  3. **工具检索**：根据子计划与工具描述对齐，检索 top-k 相关工具，作为推荐而非强制约束。
  4. **记忆更新与合并**：用工具名称/描述嵌入的余弦相似度判断等价，超过阈值则合并节点，并重定向边，保留轨迹级先后依赖。

## 3. 实验设计
- **数据集 / Benchmark**：
  - **数学推理**：AIME2024、MATH500、GSM8K。
  - **知识密集型推理**：WebWalker；以及 Wikipedia 开放域 QA：HotpotQA、2WikiMultihopQA、MuSiQue、Bamboogle。
  - 主结果表覆盖数学 3 个和多跳 QA
