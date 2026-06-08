# 具身智能论文清单 · Embodied AI Paper List

> 按 **8 个研究方向**整理的具身智能(Embodied AI)代表性与前沿论文。每篇给出**论文全名 + 年份·机构 + 一句话梗概**。
> 本清单提炼自一份对近年具身智能的系统性综述与汇报,聚焦每个方向**最具代表性(奠基/经典)+ 最前沿(2024–2025)**的工作。欢迎提 PR 补充与勘误。

**目录**:① 具身感知 · ② VLA 具身大模型 · ③ 操作与策略学习 · ④ 导航与 VLN · ⑤ 规划与推理 · ⑥ 仿真·Sim2Real·世界模型 · ⑦ 人形与全身控制 · ⑧ 数据·Benchmark·评测

---

## ① 具身感知(看懂 3D 世界与空间)

**🏛 代表作 / 奠基**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| 3D-LLM: Injecting the 3D World into Large Language Models | 2023 · UMass | 把 3D 点云接入大语言模型,统一做 3D 问答/grounding/导航。 |
| ConceptGraphs: Open-Vocabulary 3D Scene Graphs for Perception and Planning | 2023 · ICRA | 2D 基模特征融进 3D 场景图,可被语言查询,供导航/规划。 |
| OpenEQA: Embodied Question Answering in the Era of Foundation Models | 2024 · Meta | 现代 EQA 基准(1600+ 真实问题)+ LLM 自动评测协议。 |

**🆕 前沿**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| SpatialVLM: Endowing Vision-Language Models with Spatial Reasoning Capabilities | 2024 · Google | 用海量自动生成的空间 QA 训练,赋予 VLM 距离/方位等空间推理。 |
| 3D-VLA: A 3D Vision-Language-Action Generative World Model | 2024 · ICML | 把 3D 感知-推理-动作统一进生成式世界模型。 |

---

## ② VLA 具身大模型(看 + 语言 → 动作)

**🏛 代表作 / 奠基**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| RT-1: Robotics Transformer for Real-World Control at Scale | 2022 · Google | tokenize 图像+指令→动作的 Transformer 通才策略,VLA 范式起点。 |
| RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control | 2023 · DeepMind | 首个把 VLM 互联网知识共训成端到端机器人控制,定义"VLA"。 |
| Octo: An Open-Source Generalist Robot Policy | 2024 · UC Berkeley | Open X-Embodiment 上训练的开源通才策略,扩散头、可微调。 |
| OpenVLA: An Open-Source Vision-Language-Action Model | 2024 · Stanford | 7B 全开源 VLA,反超 55B RT-2-X;LoRA+4bit 进消费级 GPU。 |

**🆕 前沿**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| RDT-1B: a Diffusion Foundation Model for Bimanual Manipulation | 2024 · 清华 | 1.2B 扩散基础模型,统一动作空间,双臂灵巧操作。 |
| π0: A Vision-Language-Action Flow Model for General Robot Control | 2024 · Physical Intelligence | VLM + flow matching 动作专家,50Hz 灵巧长程操作。 |
| GR00T N1: An Open Foundation Model for Generalist Humanoid Robots | 2025 · NVIDIA | 人形通才模型,VLM 慢思考 + 扩散动作快系统的双系统架构。 |
| Gemini Robotics: Bringing AI into the Physical World | 2025 · DeepMind | 基于 Gemini 2.0 的通才 VLA,泛化能力大幅提升。 |
| π0.5: a Vision-Language-Action Model with Open-World Generalization | 2025 · Physical Intelligence | π0 后续,异构数据共训实现开放世界(陌生家居)泛化。 |

---

## ③ 操作与策略学习(怎么学操作技能)

**🏛 代表作 / 奠基**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| Diffusion Policy: Visuomotor Policy Learning via Action Diffusion | 2023 · RSS | 把动作生成写成条件去噪扩散,处理多模态、训练稳,成默认 backbone。 |
| Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware (ACT / ALOHA) | 2023 · RSS | 动作分块 Transformer(CVAE)缓解误差累积 + 低成本双臂遥操作。 |
| Universal Manipulation Interface (UMI): In-The-Wild Robot Teaching Without In-The-Wild Robots | 2024 · RSS | 手持夹爪采集野外人类演示,硬件无关、可直接部署策略。 |

**🆕 前沿**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| 3D Diffusion Policy: Generalizable Visuomotor Policy Learning via Simple 3D Representations | 2024 · RSS | 点云 + 扩散策略,~10 条 demo 即高样本效率。 |
| Mobile ALOHA: Learning Bimanual Mobile Manipulation with Low-Cost Whole-Body Teleoperation | 2024 · Stanford | ALOHA 加移动底盘 + 全身遥操作,学移动双臂操作。 |

---

## ④ 导航与 VLN(按指令在环境中移动)

**🏛 代表作 / 奠基**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| Vision-and-Language Navigation: Interpreting Visually-Grounded Navigation Instructions in Real Environments (R2R) | 2018 · CVPR | VLN 奠基 + Matterport3D 模拟器与 R2R 基准。 |
| VLFM: Vision-Language Frontier Maps for Zero-Shot Semantic Navigation | 2023 · ICRA | 用 VLM 给前沿点打语义分,零样本语义导航,可上真机。 |

**🆕 前沿**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| NaVid: Video-based VLM Plans the Next Step for Vision-and-Language Navigation | 2024 · RSS | 仅用单目 RGB 视频流即达 SOTA,无地图/里程计/深度。 |
| Uni-NaVid: A Video-based Vision-Language-Action Model for Unifying Embodied Navigation Tasks | 2024 | 统一 VLN / ObjectNav / EQA / 人类跟随 的视频 VLA。 |

---

## ⑤ 规划与推理(用大模型拆长程任务)

**🏛 代表作 / 奠基**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| Do As I Can, Not As I Say: Grounding Language in Robotic Affordances (SayCan) | 2022 · Google | LLM 评分 × 可供性价值,语言→可执行技能序列的奠基骨架。 |
| Code as Policies: Language Model Programs for Embodied Control | 2022 · Google | LLM 直接生成调用控制原语的机器人策略代码。 |
| Inner Monologue: Embodied Reasoning through Planning with Language Models | 2022 · Google | 引入环境语言反馈形成闭环,边做边纠错。 |
| PaLM-E: An Embodied Multimodal Language Model | 2023 · Google | 端到端多模态大模型做具身推理与规划(端到端路线代表)。 |

**🆕 前沿**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models | 2023 · Stanford | LLM 写代码合成 3D 价值图,零样本免训练轨迹合成。 |

---

## ⑥ 仿真 · Sim2Real · 世界模型(在哪训、怎么迁、怎么"想象")

**🏛 代表作 / 奠基**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| Domain Randomization for Transferring Deep Neural Networks from Simulation to the Real World | 2017 · IROS | Sim2Real 最通用手段(域随机化)的奠基。 |
| Isaac Gym: High Performance GPU-Based Physics Simulation for Robot Learning | 2021 · NVIDIA | GPU 原生并行物理仿真,大规模 RL 训练奠基设施。 |
| Mastering Diverse Domains through World Models (DreamerV3) | 2023 · DeepMind | 通用世界模型 RL,单一配置跨 150+ 任务"想象中学习"。 |
| Learning Interactive Real-World Simulators (UniSim) | 2023 · Google | 生成式学习的通用可交互真实世界模拟器,零样本迁真机。 |

**🆕 前沿**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| Genie: Generative Interactive Environments | 2024 · DeepMind | 从无标注视频学到可交互、动作可控的环境(基础世界模型)。 |
| Cosmos World Foundation Model Platform for Physical AI | 2025 · NVIDIA | 物理 AI 的世界基础模型平台(数据策展 + 预训练 WFM + tokenizer)。 |

---

## ⑦ 人形与全身控制(把能力装进最难的身体)

**🏛 代表作 / 奠基**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| Learning Agile and Dynamic Motor Skills for Legged Robots | 2019 · ETH(Science Robotics) | 腿足 RL + Sim2Real 奠基(ANYmal),含执行器网络提保真。 |
| Learning Quadrupedal Locomotion over Challenging Terrain | 2020 · ETH(Science Robotics) | 盲式本体感知四足越野,teacher-student sim2real 范式经典。 |
| Expressive Whole-Body Control for Humanoid Robots (ExBody) | 2024 · RSS | 富表现力全身控制:上身模仿 + 下身鲁棒行走。 |
| Learning Human-to-Humanoid Real-Time Whole-Body Teleoperation (H2O) | 2024 · IROS | 单 RGB 实时人到人形全身遥操作,"sim-to-data"过滤不可行动作。 |

**🆕 前沿**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| HumanPlus: Humanoid Shadowing and Imitation from Humans | 2024 · Stanford | 全栈人形 shadowing + 模仿,人到人形数据闭环。 |
| OmniH2O: Universal and Dexterous Human-to-Humanoid Whole-Body Teleoperation and Learning | 2024 · CoRL | H2O 升级,通用灵巧全身遥操作 + 自主执行。 |
| ASAP: Aligning Simulation and Real-World Physics for Learning Agile Humanoid Whole-Body Skills | 2025 | 学残差动作模型对齐 sim/real 物理差,Unitree G1 敏捷全身技能。 |

---

## ⑧ 数据 · Benchmark · 评测(燃料、量尺与综述)

**🏛 常用基准 / 数据集**

| 论文全名 | 年·机构 | 梗概 |
|---|---|---|
| RLBench: The Robot Learning Benchmark & Learning Environment | 2019 | 100 个手工任务的机器人学习经典 benchmark 环境。 |
| Meta-World: A Benchmark and Evaluation for Multi-Task and Meta RL | 2019 · CoRL | 50 个操作任务的多任务/元 RL 经典 benchmark。 |
| CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation | 2022 · RA-L | 长程、语言条件操作 benchmark(34 技能连续链)。 |
| Open X-Embodiment: Robotic Learning Datasets and RT-X Models | 2023 · 多机构 | 跨 22 本体、百万轨迹的最大开源数据集(事实标准)。 |
| LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning | 2023 · NeurIPS | 终身机器人学习 benchmark,VLA 评测标配。 |
| DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset | 2024 | 76k 轨迹、13 机构众包的野外操作数据集。 |
| BEHAVIOR-1K: A Human-Centered Embodied AI Benchmark with 1,000 Everyday Activities | 2024 · Stanford | 1000 日常活动的人本具身 AI benchmark(OmniGibson)。 |
| Evaluating Real-World Robot Manipulation Policies in Simulation (SimplerEnv) | 2024 · CoRL | 在仿真中公平复现真机策略评测,降低评测成本。 |

**📚 权威综述**

| 论文全名 | 年 | 梗概 |
|---|---|---|
| Aligning Cyber Space with Physical World: A Comprehensive Survey on Embodied AI | 2024 | 领域权威全景综述(感知/交互/agent/sim2real 四支柱)。 |
| A Survey on Vision-Language-Action Models for Embodied AI | 2024 | VLA 谱系综述(组件/低层控制/高层规划三支)。 |
| Large Model Empowered Embodied AI: A Survey on Decision-Making and Embodied Learning | 2025 | 大模型驱动的具身决策与学习(分层 vs 端到端)。 |
| A Comprehensive Survey on World Models for Embodied AI | 2025 | 世界模型专题综述(功能/时序/空间三轴)。 |

---

*持续更新 · 欢迎 PR 补充论文与勘误。*
