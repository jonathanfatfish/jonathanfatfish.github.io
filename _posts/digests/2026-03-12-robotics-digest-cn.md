---
title: "Robotics Digest (CN) — 2026-03-12"
date: 2026-03-12 00:00:00 +0800
categories: [Digest, Robotics]
tags: [robotics, market, arxiv, cn]
---

# 机器人前沿技术与市场情报日报（2026-03-12｜CN）

## 摘要（5-8条要点）
- **生成式/扩散式策略继续向“可泛化控制”推进**：最新工作把视频动力学与动作共同建模，用于提升跨任务/跨场景的可迁移性（arXiv 2026-03-11）。
- **VLA（视觉-语言-动作）从“大模型推理”转向“可落地的推理加速与后训练”**：出现训练无关的视觉token合并、以及面向动作潜变量的后训练/世界模型联动（arXiv 2026-03-11）。
- **类人（humanoid）研究热点集中在全身控制与多接触优化**：MPC+RL、运动重定向与残差RL等路线并行（arXiv 2026-03-10~11）。
- **触觉/力觉与语言对齐成为操作学习的关键补全项**：细粒度对比预训练把“语言-触觉”对齐用于操作任务；亦有多模态（视-触）复原与全局触觉定位方法（arXiv 2026-03-10~11）。
- **市场侧的需求信号仍由“降本增效+缺工”驱动**：仓储/物流自动化、协作机器人/AMR部署、以及手术机器人平台扩展，持续在上市公司年报/季报中被作为增长与资本开支重点（SEC 2026-01~02）。
- **机会窗口**：把“数据采集（含触觉/力觉）—后训练—部署加速（推理/记忆/校验器）”做成闭环产品，将更容易落到制造/仓储/医疗等ROI可量化场景。

## 技术前沿（按主题小节）

### 1) 生成式策略与长时程操作（Diffusion/Flow/Video dynamics → Action）
- **DiT4DiT**：联合建模视频动力学与动作，用于更可泛化的机器人控制（2026-03-11）。
- **VQ-Memory**：面向非马尔可夫模拟基准的长时程操作鲁棒性，强调记忆/离散化表征（2026-03-10）。
- **PhaForce**：把“慢规划 + 快修正”结构化到视觉-力觉（或视觉-接触）策略学习中，用于接触丰富操作（2026-03-09）。
- **从Flow到一步蒸馏**：用分布蒸馏等方式降低生成式策略推理时延，指向实时控制（2026-03-10）。

### 2) VLA与世界模型：从端到端到“可控/可加速”的系统化路径
- **FutureVLA**：以联合的“视觉运动预测”视角推进VLA（2026-03-11）。
- **DepthCache**：深度引导的训练无关视觉token合并，用于VLA推理加速（2026-03-11）。
- **World2Act**：通过技能可组合的世界模型，对潜在动作进行后训练（2026-03-11）。
- **Update-Free On-Policy Steering via Verifiers**：引入“验证器/判别器”进行策略引导的思路，强调无需更新主策略（2026-03-10）。

### 3) 类人与全身控制：多接触、重定向、MPC+RL
- **RL-Augmented MPC**：面向非固定步态（non-gaited）与混合移动的MPC与RL结合（2026-03-11）。
- **Kinodynamic Motion Retargeting**：通过多接触全身轨迹优化进行类人运动重定向（2026-03-10）。
- **SteadyTray**：残差RL用于类人托盘运输中的物体平衡（2026-03-11）。
- **SCDP**：部分观测下的人形行走，通过混合观测蒸馏学习（2026-03-10）。

### 4) 触觉/力觉与多模态感知：从硬件到表征对齐
- **FG-CLTP**：细粒度对比“语言-触觉”预训练，用于机器人操作（2026-03-11）。
- **MuxGel**：空间复用+深度重建实现同时视-触感知（2026-03-10）。
- **TacLoc**：以配准视角做全局触觉定位（2026-03-11）。
- **CONTACT**：面向拆解任务的接触感知触觉学习（2026-03-09）。

## 最新市场需求（按行业小节；近90天为主）

> 注：以下“需求信号”主要来自上市公司在近90天披露的年报/季报/业务描述，属于**一手公开披露**；其对具体机器人型号/项目细节披露有限，因此更适合作为“行业方向/预算优先级”的证据。

### 仓储与物流自动化
- **系统级仓储自动化/机器人化继续扩张**：Symbotic 在 10-Q 中披露其业务进展与客户/履约相关信息，反映北美大型仓储自动化需求仍在推进（2026-02-04）。
- **电商履约的自动化投资**：Amazon 在 10-K 中披露履约网络、自动化与资本开支等相关风险与投入（2026-02-06）。

### 制造业：协作机器人/AMR与自动化测试
- **机器人/自动化相关收入与并购资产（含协作机器人、AMR）仍是重点**：Teradyne 10-K（其旗下包含 Universal Robots、MiR 等）可作为制造与物流自动化需求的间接指标（2026-02-20）。

### 医疗：手术机器人平台扩展
- **手术机器人平台持续扩容**：Intuitive Surgical 10-K 披露装机量、手术量、耗材与系统销售等指标，体现医疗机构对机器人辅助手术的持续需求（2026-02-03）。

### 汽车与类人（风险更高、周期更长）
- **人形机器人/自动驾驶相关投入常被与AI/制造能力绑定披露**：Tesla 10-K 提供其对相关业务与风险的公开披露，可作为“投入方向与不确定性”的一手材料（2026-01-29）。

## 供需匹配与机会（基于证据推论，明确不确定性）
- **机会1：把“生成式策略 → 实时部署”工程化**：多篇工作指向蒸馏/推理加速/记忆模块/验证器引导。若与仓储拣选、制造上料、接触丰富装配等场景的KPI（节拍、良率、停机率）绑定，产品化路径更清晰。
  - 证据：生成式策略蒸馏与长时程记忆相关论文（arXiv 2026-03-10~11）。
  - 不确定性：仿真到现实（Sim2Real）与数据闭环成本仍可能成为瓶颈。
- **机会2：触觉+语言对齐的数据资产与工具链**：FG-CLTP 等工作表明“触觉表征”正在被纳入可迁移的语义空间；面向工业夹持、拆解、布料等任务，触觉数据的采集/标注/对齐工具链可能成为差异化壁垒。
  - 不确定性：硬件可得性、耐久性与跨传感器域泛化。
- **机会3：类人全身控制的“可验证安全栈”**：全身控制与多接触优化的复杂度高，面向真实环境部署需要更强的验证、约束与故障恢复机制；“验证器/约束MPC/安全监控”可能比“更大模型”更先带来可落地收益。
  - 不确定性：硬件成本、法规/责任界定、以及真实应用对形态的要求未必需要人形。

## 风险/限制（数据偏差、可复现性、监管、安全）
- **论文快速迭代但复现门槛高**：训练数据、仿真环境、机器人平台差异导致复现困难；同类方法对比往往不完全公平。
- **数据偏差与外推风险**：VLA/世界模型在分布外场景可能出现不可预测行为；接触丰富任务的长尾失败成本高。
- **安全与合规**：医疗与类人/自动驾驶相关应用监管门槛高，且事故责任与认证周期长。
- **市场信息披露粒度有限**：上市公司披露通常是宏观与风险层面的，难以直接映射到“单一产品机会”，需要结合渠道/招标/客户访谈补足。

## 参考来源清单（每条含标题/机构/日期/链接）

### 技术（arXiv，近12个月内；此处列出本期新增/高相关）
1. *DiT4DiT: Jointly Modeling Video Dynamics and Actions for Generalizable Robot Control*｜arXiv｜2026-03-11｜https://arxiv.org/abs/2603.10448
2. *Beyond Short-Horizon: VQ-Memory for Robust Long-Horizon Manipulation in Non-Markovian Simulation Benchmarks*｜arXiv｜2026-03-10｜https://arxiv.org/abs/2603.09513
3. *PhaForce: Phase-Scheduled Visual-Force Policy Learning with Slow Planning and Fast Correction for Contact-Rich Manipulation*｜arXiv｜2026-03-09｜https://arxiv.org/abs/2603.08342
4. *From Flow to One Step: Real-Time Multi-Modal Trajectory Policies via … Distribution Distillation*｜arXiv｜2026-03-10｜https://arxiv.org/abs/2603.09415
5. *FutureVLA: Joint Visuomotor Prediction for Vision-Language-Action Model*｜arXiv｜2026-03-11｜https://arxiv.org/abs/2603.10712
6. *DepthCache: Depth-Guided Training-Free Visual Token Merging for Vision-Language-Action Model Inference*｜arXiv｜2026-03-11｜https://arxiv.org/abs/2603.10469
7. *World2Act: Latent Action Post-Training via Skill-Compositional World Models*｜arXiv｜2026-03-11｜https://arxiv.org/abs/2603.10422
8. *Update-Free On-Policy Steering via Verifiers*｜arXiv｜2026-03-10｜https://arxiv.org/abs/2603.10282
9. *RL-Augmented MPC for Non-Gaited Legged and Hybrid Locomotion*｜arXiv｜2026-03-11｜https://arxiv.org/abs/2603.10878
10. *Kinodynamic Motion Retargeting for Humanoid Locomotion via Multi-Contact Whole-Body Trajectory Optimization*｜arXiv｜2026-03-10｜https://arxiv.org/abs/2603.09956
11. *SteadyTray: Learning Object Balancing Tasks in Humanoid Tray Transport via Residual Reinforcement Learning*｜arXiv｜2026-03-11｜https://arxiv.org/abs/2603.10306
12. *FG-CLTP: Fine-Grained Contrastive Language Tactile Pretraining for Robotic Manipulation*｜arXiv｜2026-03-11｜https://arxiv.org/abs/2603.10871
13. *MuxGel: Simultaneous Dual-Modal Visuo-Tactile Sensing via Spatially Multiplexing and Deep Reconstruction*｜arXiv｜2026-03-10｜https://arxiv.org/abs/2603.09761
14. *TacLoc: Global Tactile Localization on Objects from a Registration Perspective*｜arXiv｜2026-03-11｜https://arxiv.org/abs/2603.10565
15. *CONTACT: CONtact-aware TACTile Learning for Robotic Disassembly*｜arXiv｜2026-03-09｜https://arxiv.org/abs/2603.08560

### 市场/公司披露（近90天为主）
16. *Form 10-K (FY2025)*｜Tesla, Inc.｜2026-01-29｜https://www.sec.gov/Archives/edgar/data/1318605/000162828026003952/tsla-20251231.htm
17. *Form 10-K (FY2025)*｜Intuitive Surgical, Inc.｜2026-02-03｜https://www.sec.gov/Archives/edgar/data/1035267/000103526726000010/isrg-20251231.htm
18. *Form 10-K (FY2025)*｜Amazon.com, Inc.｜2026-02-06｜https://www.sec.gov/Archives/edgar/data/1018724/000101872426000004/amzn-20251231.htm
19. *Form 10-Q (Quarter ended 2025-12-27)*｜Symbotic Inc.｜2026-02-04｜https://www.sec.gov/Archives/edgar/data/1837240/000183724026000009/sym-20251227.htm
20. *Form 10-K (FY ended 2025-12-28)*｜Teledyne Technologies Incorporated（注：该CIK主体披露文件；用于跟踪其自动化/机器人相关信息）｜2026-02-20｜https://www.sec.gov/Archives/edgar/data/1094285/000109428526000017/tdy-20251228.htm
