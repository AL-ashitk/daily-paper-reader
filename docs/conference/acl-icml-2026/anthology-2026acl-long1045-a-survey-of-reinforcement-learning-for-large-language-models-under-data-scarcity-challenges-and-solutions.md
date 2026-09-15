---
title: "A Survey of Reinforcement Learning for Large Language Models under Data Scarcity: Challenges and Solutions"
title_zh: 数据稀缺下面向大语言模型的强化学习综述：挑战与解决方案
authors: "Zhiyin Yu, Yuchen Mou, Juncheng Yan, Junyu Luo, Chunchun Chen, Xing Wei, Yunhui Liu, Hongru Sun, Yuxing Zhang, Jun Xu, Yatao Bian, Ming Zhang, Wei Ye, Tieke He, Jie Yang, Guanjie Zheng, Zhonghai Wu, Bo Zhang, Lei Bai, Xiao Luo"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://aclanthology.org/2026.acl-long.1045.pdf"
tags: ["query:rl"]
score: 9.0
evidence: 数据稀缺下大语言模型强化学习综述
tldr: 强化学习已成为提升大语言模型推理能力的重要后训练范式，但面临高质量外部监督与模型自生成经验不足等数据稀缺挑战。该综述首次系统梳理数据稀缺条件下的面向大语言模型的强化学习研究，提出自底向上的分层框架，从数据中心与训练中心等互补视角组织现有工作。文章总结了数据高效强化学习的关键方法与解决方案，为该方向研究者提供清晰地图与未来方向。
source: ACL-2026-Long
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-001.webp\", \"caption\": \"\", \"page\": 1, \"index\": 1, \"width\": 399, \"height\": 399}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-002.webp\", \"caption\": \"\", \"page\": 1, \"index\": 2, \"width\": 386, \"height\": 393}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-003.webp\", \"caption\": \"\", \"page\": 1, \"index\": 3, \"width\": 390, \"height\": 342}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-004.webp\", \"caption\": \"\", \"page\": 1, \"index\": 4, \"width\": 321, \"height\": 420}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-005.webp\", \"caption\": \"\", \"page\": 1, \"index\": 5, \"width\": 393, \"height\": 402}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-006.webp\", \"caption\": \"\", \"page\": 1, \"index\": 6, \"width\": 396, \"height\": 384}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-007.webp\", \"caption\": \"\", \"page\": 1, \"index\": 7, \"width\": 405, \"height\": 411}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-008.webp\", \"caption\": \"\", \"page\": 1, \"index\": 8, \"width\": 342, \"height\": 389}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-009.webp\", \"caption\": \"\", \"page\": 1, \"index\": 9, \"width\": 399, \"height\": 405}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-010.webp\", \"caption\": \"\", \"page\": 1, \"index\": 10, \"width\": 405, \"height\": 371}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-011.webp\", \"caption\": \"\", \"page\": 1, \"index\": 11, \"width\": 372, \"height\": 372}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-012.webp\", \"caption\": \"\", \"page\": 1, \"index\": 12, \"width\": 401, \"height\": 399}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-013.webp\", \"caption\": \"\", \"page\": 1, \"index\": 13, \"width\": 405, \"height\": 414}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-014.webp\", \"caption\": \"\", \"page\": 1, \"index\": 14, \"width\": 369, \"height\": 380}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-015.webp\", \"caption\": \"\", \"page\": 1, \"index\": 15, \"width\": 392, \"height\": 393}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-016.webp\", \"caption\": \"\", \"page\": 1, \"index\": 16, \"width\": 392, \"height\": 386}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-017.webp\", \"caption\": \"\", \"page\": 1, \"index\": 17, \"width\": 366, \"height\": 408}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-018.webp\", \"caption\": \"\", \"page\": 1, \"index\": 18, \"width\": 389, \"height\": 396}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-019.webp\", \"caption\": \"\", \"page\": 1, \"index\": 19, \"width\": 405, \"height\": 399}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-020.webp\", \"caption\": \"\", \"page\": 1, \"index\": 20, \"width\": 702, \"height\": 346}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-021.webp\", \"caption\": \"\", \"page\": 4, \"index\": 21, \"width\": 512, \"height\": 512}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-022.webp\", \"caption\": \"\", \"page\": 4, \"index\": 22, \"width\": 512, \"height\": 512}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-023.webp\", \"caption\": \"\", \"page\": 4, \"index\": 23, \"width\": 512, \"height\": 512}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-024.webp\", \"caption\": \"\", \"page\": 4, \"index\": 24, \"width\": 512, \"height\": 512}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-025.webp\", \"caption\": \"\", \"page\": 4, \"index\": 25, \"width\": 512, \"height\": 512}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-026.webp\", \"caption\": \"\", \"page\": 5, \"index\": 26, \"width\": 736, \"height\": 356}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-027.webp\", \"caption\": \"\", \"page\": 7, \"index\": 27, \"width\": 512, \"height\": 512}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-028.webp\", \"caption\": \"\", \"page\": 7, \"index\": 28, \"width\": 512, \"height\": 512}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-029.webp\", \"caption\": \"\", \"page\": 7, \"index\": 29, \"width\": 512, \"height\": 512}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-030.webp\", \"caption\": \"\", \"page\": 7, \"index\": 30, \"width\": 512, \"height\": 512}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-031.webp\", \"caption\": \"\", \"page\": 7, \"index\": 31, \"width\": 796, \"height\": 638}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-032.webp\", \"caption\": \"\", \"page\": 7, \"index\": 32, \"width\": 512, \"height\": 512}, {\"url\": \"assets/figures/acl-2026-long/anthology-2026acl-long1045/fig-033.webp\", \"caption\": \"\", \"page\": 17, \"index\": 33, \"width\": 4335, \"height\": 2168}]"
motivation: 面向大语言模型的强化学习受限于高质量监督与自生成经验不足的数据稀缺问题。
method: 首次系统综述该主题，构建数据中心与训练中心等视角的自底向上分层框架。
result: 归纳了数据高效强化学习的挑战与相应解决方案，形成系统化研究地图。
conclusion: 为数据稀缺下的LLM强化学习指明关键方向与可行解决路径。
---

## Abstract
Reinforcement learning (RL) has emerged as a powerful post-training paradigm for enhancing the reasoning capabilities of large language models (LLMs). However, reinforcement learning for LLMs faces substantial data scarcity challenges, including the limited availability of high-quality external supervision and the constrained volume of model-generated experience. These limitations make data-efficient reinforcement learning a critical research direction. In this survey, we present the first systematic review of reinforcement learning for LLMs under data scarcity. We propose a bottom-up hierarchical framework built around three complementary perspectives: the data-centric perspective, the training-centric perspective, and the framework-centric perspective. We develop a taxonomy of existing methods, summarize representative approaches in each category, and analyze their strengths and limitations. Our taxonomy aims to provide a clear conceptual foundation for understanding the design space of data-efficient RL for LLMs and to guide researchers working in this emerging area. We hope this survey offers a comprehensive roadmap for future research and inspires new directions toward more efficient and scalable reinforcement learning post-training for LLMs.

---

## 论文详细总结（自动生成）

# 论文总结：《数据稀缺下面向大语言模型的强化学习综述：挑战与解决方案》

## 1. 核心问题与研究背景

- **研究动机**：强化学习（RL）已成为大语言模型（LLM）后训练阶段提升推理能力的核心范式，DeepSeek-R1、OpenAI-o1 等工作表明 RL 可激发自我反思等涌现行为。然而，**数据稀缺**正成为制约 RL 有效性的关键瓶颈。
- **两类数据稀缺**：
  - **外部数据稀缺**：高质量监督信号获取成本高，如细粒度人类反馈、偏好数据、专家标注、逐步推理轨迹等。
  - **内部数据稀缺**：模型自生成交互受限，包括 rollout 数量、轨迹长度、探索预算等。
- **整体含义**：单纯扩大数据或算力规模收益递减，Silver 与 Sutton（2025）提出的"经验时代"主张从依赖人类监督转向让模型通过经验自我演化，因此研究数据稀缺下的 LLM 强化学习具有重要意义。
- **研究定位**：本文是**首篇系统性综述**数据稀缺下 LLM 强化学习的工作，旨在用统一框架整合碎片化研究，为后续研究提供路线图。与已有综述（LLM/智能体 RL、自演化智能体、数据高效后训练）的区别在于：以数据稀缺为透镜、采用自底向上的分层框架进行统一分析。

## 2. 方法论：三层互补框架与分类体系

论文不提出新算法，而是构建**自底向上、三层互补的概念框架**，并据此设计分类体系（taxonomy）：

### Level 1：数据中心视角（优化数据本身）
- **数据剪枝**：从原始数据中识别最有信息量的子集。
  - *离线剪枝*：基于预定义规则或启发式，如 LIMR（用奖励轨迹与平均学习曲线对齐度筛选高影响 prompt）、LearnAlign（可学习性加权的梯度对齐分数）、EAS（token 级预测熵）。
  - *在线剪枝*：动态选择高信息密度样本，如 LSPO（长度感知动态采样）、MMoPPS（将 prompt 难度建模为潜在成功概率）、BOTS（贝叶斯在线任务选择）、GAIN-RL（用 pre-filling 隐状态角度集中度预测梯度幅度）、RORL（在线 rollout 估计通过率筛选中等难度）、DOTS、SPEED-RL 等。
  - *细粒度剪枝*：更精细的剪枝准则，如 Influence Pruning（用共轭梯度求解器近似影响函数）、GRESO（奖励驱动的跳过策略）、PREPO（基于 prompt 困惑度的易到难课程）、CPPO（组内优势作为细粒度信号）、PODS（下采样奖励方差最大的轨迹子集）。
- **数据合成**：扩大监督规模与分布覆盖。
  - *静态合成*：训练前合成，如 Constitutional AI、UltraFeedback、CodeUltraFeedback、Reasoning Gym、Enigmata、SynLogic、EvoSyn、SynthRL、AdaR。
  - *动态合成*：训练循环内持续生成，如 OSP（自生成软偏好优势）、OAIF（在线 LLM 标注器作为奖励模型）。
  - *困难数据合成*：针对弱项或错误生成新问题，如 SwS（弱点驱动问题合成）、LoopTool（纠错循环）、EVA（奖励引导的 prompt 演化）、WEBRL（从失败交互生成新任务）。
- **数据压缩**：在保持信息密度的前提下压缩数据与计算成本。
  - *Token 级*：如 Shallow Preference Signals、AR-Lopti、TR-GRPO、高熵少数 token 更新（Beyond 80/20）、DEPO。
  - *Step 级*：如 DAST（难度自适应 token 长度预算）、THINKPRUNE（主动剪枝冗余推理步）、S-GRPO（串行分组与衰减奖励实现早退）、Interleaved Reasoning、基于步熵的 CoT 压缩。
  - *Trajectory 级*：如 DAPO（过滤零梯度轨迹组）、PROF（过程奖励与结果奖励一致才保留）。
  - *Dataset 级*：如 One-shot RLVR（单样本达 7.5k 样本相当性能）、Polymath Learning（单样本高信息密度训练集）。

### Level 2：训练中心视角（改进轨迹生成、奖励评估与策略更新）
- **轨迹生成**：
  - *引导探索*：将 MCTS 等规划算法融入解码（AlphaMath、TS-LLM）；LLM-PSRL 采用贝叶斯后验采样；Search-R1 让模型主动发起检索。
  - *选择性/自适应 rollout*：GRESO 的生成前过滤（预测低信息 rollout 直接跳过）；PODS 的生成后采样；token 级掩码只对高熵 token 计算策略梯度。
- **奖励工程**：
  - *过程奖励*：无人工过程标注时利用模型输出的统计性质合成，如 CoVo（正确路径收敛、错误路径发散，利用一致性与波动性自奖励）、Evol-RL（新颖性促进）、L2T（压缩惩罚项鼓励高效思考）。
  - *内在动机*：熵最小化视角（Agarwal 等，认为错误源于解码不确定性）与熵最大化视角（PREPO、CDE，奖励相对熵更高的 rollout 以鼓励探索）存在分歧；SCoRe、ReviewRL 用多轮/多智能体 RL 提供可靠奖励。
  - *一致性与共识机制*：KnowRL（内省与共识）、Intuitor（以模型置信度为唯一奖励实现无监督）、多数投票奖励（TTRL、MM-UPT、SRT）、SVSI（句嵌入语义相似度构造偏好对）、RLCCF（自一致性加权多异构 LLM 投票）。
  - *启发式与代理信号*：Shao 等发现虚假奖励也能提升特定模型数学推理（激活预训练已学模式）；格式正确性与响应长度作为代理奖励；CaT 用并行推理 rollout 合成参考答案转化为无参考奖励；SPPO 将对齐建模为双人常和博弈逼近纳什均衡。
- **策略优化**：
  - *重放机制*：多视角自奖励构造交叉验证内在奖励；课程学习动态调整难度。
  - *样本高效目标*：KTO（用自生成中间推理步作为监督）、IGPO（扩散语言模型的 inpainting 引导策略优化）。

### Level 3：框架中心视角（减少对外部数据的依赖）
- **自演化框架**：单模型同时充当生成器与评估器。自训练类（EasyRL 渐进利用易标注数据与难无标注数据、DPO-Gen、自纠正、S²R、SSR-Zero、SeRL）；自适应学习类（ZeroGUI 自动化 GUI 任务生成、Self-aware RL 能力预测主动请求数据、ASL、AZR 自博弈生成并求解任务）。
- **非对称协同演化框架**：
  - *协作式*：proposer-solver 配对（原始非对称自博弈），扩展到自我提问、难度调整、视觉推理；PasoDoble 解耦 proposer 与 solver 更新以稳定训练。
  - *对抗式*：生成器 vs 判别器，如 SPAG（对抗禁忌游戏）、SPC（"狡猾生成器"欺骗 critic 提升验证能力）、GAR（判别器提供密集逻辑奖励）、SSR（注入-修复循环构造代码修复课程）。
- **多智能体演化框架**：
  - *竞争自博弈*：SPIRAL（多轮扑克等零和游戏激励系统推理）、Vision-Zero（"谁是间谍"游戏用于视觉推理）。
  - *多角色协作*：SPELL、MAE（三元组结构处理长上下文与通用推理）、形式验证信号（Propose-Solve-Verify）、分层 actor-judge 架构。

## 3. 实验设计

- **本文为综述论文，不包含自身实验设计、数据集或 benchmark 对比**，其"论证设计"体现在：
  - 对 **100 余篇文献**进行系统梳理，在附录 D 给出包含 Title、Section/Subsection（三层分类位置）、Year、Venue、Link 六列的详细文献汇总表。
  - 附录 A 做了**发表年份统计**（图 6）：2018 与 2020 年各 1 篇，2021、2022、2023 年各 2 篇，2024 年 8 篇，截至 2025 年 12 月激增至 **109 篇**，显示该方向从新兴方向转变为主流范式。
  - 附录 A 还对论文标题做**词频分析与词云**（图 7），核心词为 Reasoning、Learning、Reinforcement、Training、Data、Model，以及 Self、Evolving、Agent、Verifiable、Rewarding 等。
  - 附录 C 提供**补充分析**：C.1 讨论不确定性感知剪枝（UFO-RL、ReST、BAL-PM、ADPO、Uncertainty-Penalized DPO）；C.2 讨论内部反馈的理论视角与自适应多目标权衡（Fine-grained RLHF、Safe-RLHF、MAESTRO、PAMA、JobRec、IB-GRPO）。
- **对比对象**：论文在"Differences from Previous Surveys"中与已有综述（LLM/agentic RL 综述、自演化智能体综述、数据高效后训练综述）做了定性对比，指出其未系统研究数据稀缺下的 RL。

## 4. 资源与算力

- **论文全文未提及任何 GPU 型号、数量、训练时长或算力消耗信息**。
- 这符合综述论文性质：本文不进行模型训练或实验，因此无算力需求。附录仅说明写作中仅用 LLM 做语法检查与语言润色，并遵守 ACL 关于 AI 写作辅助的政策。

## 5. 实验数量与充分性

- **本文为综述，没有开展控制实验、消融实验或多数据集对比实验**，因此"实验组数"不适用。
- 从综述方法论角度评估其充分性与客观性：
  - **覆盖充分**：文献汇总表覆盖 2018—2025 年的代表性工作，按三层分类体系逐条定位，范围较广。
  - **客观性较好**：对每类方法均同时总结优势与局限，并在每节末尾给出"Key takeaways"；对存在分歧的问题（如熵最小化 vs 熵最大化）如实呈现双方观点。
  - **公平性**：作为文献综述，其"公平"主要体现在分类标准一致、引用来源公开可查；但缺乏对同类方法在统一基准下的定量横向比较。
  - **注意**：综述的"证据强度"依赖原始论文，本文未做元分析（meta-analysis）或统一的定量再评估。

## 6. 主要结论与发现

- **核心结论**：解决数据稀缺不能仅靠扩大监督信号或交互经验，而需要**外部数据处理 + RL 训练中内部数据有效利用 + 可演化框架**三方面协同。
- **关键洞察**：在数据稀缺下，RL 可能**更像一种"重新分配"机制**——锐化预训练阶段已学到的推理模式，而非获取全新能力（Shao 等关于虚假奖励仍有效、Chen 等关于 RLVR/RLIF 收敛与退化的理论分析、Agarwal 等熵最小化的有效性均支持此观点）。
- **各层 Key takeaways**：
  - 数据中心：数据价值估计依赖模型能力，过度强调高贡献数据可能削弱长尾学习；未来应自适应联合调度剪枝、压缩与合成。
  - 训练中心：范式从外部监督转向挖掘内在经验价值；核心挑战是权衡采样成本与自生成奖励的信噪比，并防止 reward hacking 崩溃。
  - 框架中心：自演化框架优先效率，多智能体方法以成本换取更深推理；协同演化引入外部信号打破"回声室"、减少自我幻觉；自生成课程可动态匹配模型演化能力。
- **未来方向**：
  1. **内部奖励可靠性**：一致性、熵、启发式信号噪声大，易 reward hacking 或模型坍塌，需鲁棒过程信号与混合奖励设计。
  2. **向不可验证/开放式任务泛化**：现有方法多集中于数学、代码等可验证领域，需拓展到创意写作、开放对话、科学发现、世界建模与具身智能体等。
  3. **自博弈框架的安全风险**：可能出现 CoT 中的"uh-oh 时刻"、偏见放大与虚假泛化，需在线过滤与安全感知训练机制。

## 7. 优点

- **首创性与系统性**：首篇以"数据稀缺"为统一视角系统梳理 LLM 强化学习的综述，填补研究空白。
- **框架清晰**：提出"数据中心—训练中心—框架中心"自底向上三层框架，从数据治理到轨迹利用再到自主框架，逻辑递进，分类边界明确。
- **分类细致**：每个层面下设多个子类（如数据压缩分 token/step/trajectory/dataset 四级），并配以大量代表性方法，便于研究者按图索骥。
- **兼顾广度与深度**：既有方法罗列，也有理论视角讨论（内部反馈的理论等价性、变分推断解释、q→r→a 两阶段数学框架）与分歧呈现。
- **实践导向**：每节给出 Key takeaways，末章明确挑战与未来方向，并附文献汇总表与统计图表，信息密度高。
- **开放资源**：提供 GitHub 仓库（Data-Efficient-RL）便于跟踪。

## 8. 不足与局限

- **作者自述局限**：领域发展迅速，所提框架需及时更新才能全面覆盖新兴方法。
- **无实验验证**：作为综述，未对各类方法进行统一的定量复现或基准对比，难以判断方法间的相对优劣。
- **分类可能重叠**：部分方法同时涉及数据中心与训练中心（如高熵 token 掩码既属压缩也属轨迹生成），归类存在主观性。
- **覆盖偏斜风险**：所引工作高度集中于 2025 年（109 篇）且多为 arXiv 预印本，部分结论尚未经同行评审验证；同时明显偏重数学、代码等可验证推理领域，对开放式、主观性任务覆盖不足。
- **理论深度有限**：虽有理论视角讨论，但多为引用他人结论，未提出新的理论统一框架。
- **安全与伦理讨论较浅**：仅在挑战部分简要提及自博弈安全风险，缺乏系统性治理方案。
- **应用限制**：综述面向研究路线图，未给出工程落地时的成本-收益量化指南，实际选型仍需读者自行评估。

（完）
