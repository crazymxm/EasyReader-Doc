精选论文，用EasyRader可全文翻译、生成结构化导读、思维导图，节省80%阅读时间 。

EasyRader"论文周选"功能可以查看每周精选内容。

现在下载，开启高效科研阅读新体验！[EasyReader论文阅读 - 易读论文阅读 科研文献翻译](https://www.easyreader.com.cn/)

# 🗓️ 周报 (2026-W19)
> 更新时间: 2026-05-10

--- 
## 📚 学科: `eess.*`
**学科总结**：本次 eess 领域论文涵盖了语音信号处理、无线通信效率、电力系统稳定性、系统控制及机器人监控。研究重点在于结合生成式先验提升语音增强性能（如 SIPS 框架），以及在计算资源受限环境下通过门控融合（CSI 预测）和主动学习（暂态稳定性评估）实现高效的系统建模与控制。这些工作展示了深度学习与传统信号处理理论在解决复杂工程问题中的深度融合。

### Predictive-Generative Drift Decomposition for Speech Enhancement and Separation
- **分数**: 4
- **链接**: https://arxiv.org/abs/2605.06189v1
- **作者**: Julius Richter, Yoshiki Masuyama, Christoph Boeddeker, Takahiro Edo, Gordon Wichern, Jonathan Le Roux
- **备注**: Submitted to NeurIPS 2026
- **摘要**: 我们提出了一种用于语音增强和分离的即插即用框架，该框架通过生成式语音先验增强了预测方法。我们的方法被称为语音随机插值先验（SIPS），建立在随机插值的基础上，并利用其灵活性来连接预测建模和生成建模。具体而言，我们将插值动力学分解为任务特定的漂移和随机去噪组件，从而允许将预测估计直接集成到生成采样过程中。这产生了一个数学基础扎实的框架，用于将强大的预训练预测器与生成模型的表现力相结合。为此，我们仅使用清洁语音训练评分模型，从而产生一个与降质无关的先验，可以在不同任务中重复使用。在推理过程中，预测器提供确定性漂移，引导采样过程走向任务一致的估计，而评分模型则保持知觉自然度。与以往通常依赖于特定架构条件且绑定到特定预测器或降质设置的混合方法不同，SIPS 提供了一个统一框架，可以推广到各种预测器和加性降质任务。我们使用 SEMamba 和 FlexIO 等最新预测器证明了其在语音增强和语音分离方面的有效性。所提方法持续提高了知觉质量，在语音分离任务中 NISQA 评分提升高达 +1.0。
- **PDF**: https://arxiv.org/pdf/2605.06189v1

### Resource-Efficient CSI Prediction: A Gated Fusion and Factorized Projection Approach
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.06578v1
- **作者**: Mohammad Hussain, Maedeh Adibag, Dilara Gurer, Gokhan Kalem, Kerim Serin, Sinem Coleri
- **备注**: Accepted for publication in IEEE Communications Letters. 5 pages, 2 figures
- **摘要**: 精确的信道状态信息 (CSI) 预测对于动态多输入多输出 (MIMO) 系统至关重要，但计算需求很大。本文提出了一种资源高效的预测器，它结合了门控循环单元 (GRU) 编码器、Luong 注意力机制、瓶颈门控融合模块和维度可分离线性头 (DSLH)。门控融合模块集成了局部循环特征与全局注意力上下文，而 DSLH 则降低了输出映射的成本。在符合 3GPP TR 38.901 标准的信道上进行评估，所提模型实现了 -13.84 dB 的平均 NMSE，参数减少了 26%，推理吞吐量比维度匹配的 LinFormer 基线高出约 2.3 倍。该模型最适合视距 (LOS) 和混合条件场景，为中等序列长度的短期 CSI 预测提供了实用的准确性与效率权衡。
- **PDF**: https://arxiv.org/pdf/2605.06578v1

### Probabilistic Assessment of Rare Transient Instability Events via Kriging-based Active Learning Framework
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.06442v1
- **作者**: Jingyu Liu, Xiaoting Wang, Xiaozhe Wang
- **备注**: Accepted by International Journal of Electrical Power and Energy Systems for future publication
- **摘要**: 现代电力系统中由于间歇性能源和可变负载集成而日益增加的不确定性，强调了概率暂态稳定性评估的必要性。然而，现有的评估方法主要集中在平均系统稳定行为上，在识别罕见暂态不稳定事件时可能面临挑战或产生高昂的计算成本，而这些事件对于确保系统韧性至关重要。为了解决这一问题，本文提出了一种基于 Kriging 的主动学习框架，以准确表征输入不确定性空间内的罕见不稳定区域，并估算相关的小概率不稳定事件，同时仅需有限数量的高昂时域仿真。该主动学习 (AL) 框架在模拟负载和风电不确定性的改进型 IEEE 59 节点系统以及结合真实风电和太阳能发电数据的 WECC 240 节点系统上进行了测试。与现有的基于随机森林的主动学习方法及三种非主动学习方法的对比研究表明，所提 AL 框架具有更高的精度和计算效率。
- **PDF**: https://arxiv.org/pdf/2605.06442v1

### Unbalanced Optimal Transport and Density Control for Discrete-Time Linear Systems
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.06391v1
- **作者**: Haruto Nakashima, Siddhartha Ganguly, Kenji Kashima
- **备注**: To appear in the Proceedings of MTNS 2026
- **摘要**: 本文研究了一类受限离散线性系统的非平衡最优传输 (UOT) 及其动力学扩展——非平衡密度控制 (UDC)。UOT 通过平衡传输成本和与参考度量的忠实度来比较总质量不相等的度量，而 UDC 则将系统动力学和约束纳入此框架。针对高斯参考和离散时间线性系统，我们证明这两个问题都允许全局最优的凸公式，类似于协方差控制。文中提供了一个数值实验来阐明我们的方法。
- **PDF**: https://arxiv.org/pdf/2605.06391v1

### Monitoring autonomous persistent surveillance missions using invariance
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.06062v1
- **作者**: Vladislav Nenchev, Prodromos Sotiriadis
- **备注**: Accepted at IEEE ICRA 2026
- **摘要**: 本文研究了当自主栈为黑盒时，自主机器人执行持久监控任务的运行时监测问题。环境被划分为有限个部分，每个部分带有一个不确定性状态，该状态在被观察时降低，否则增加。我们将闭环建模为一个具有线性参数变化动力学的状态相关混合系统，并设计了一个基于离线计算的不变量的监测器。由于这种不变量在大范围待监控空间中通常难以获取，我们提出了一种组合式监测器，通过分散计算每个不确定性区域的低维不变集并在运行时检查它们的合取来实现。在常见的独立性假设下，该组合式监测器对于全系统不变量是可靠且完备的。该方法在真实机器人持久监控迷宫的案例研究中得到了应用，强调了其实际适用性。
- **PDF**: https://arxiv.org/pdf/2605.06062v1

--- 
## 📚 学科: `q-bio.*`
**学科总结**：本周定量生物学领域关注蛋白质序列优化与生物行为建模。MP2D 框架利用条件离散扩散与蒙特卡洛树搜索解决了多目标蛋白质设计的权衡难题；另一项研究则重新审视了细菌趋化性的感官极限，提出鲁棒性并非仅取决于信息效率，还源于运动策略与对称性平均的平衡。这两项工作分别展示了 AI 辅助设计与基础生物物理理论在理解生命机制方面的最新进展。

### MP2D: Constrained Monte Carlo Tree-Guided Diffusion for Multi-Objective Protein Sequence Design
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.05829v1
- **作者**: Zitai Kong, Yifan Dong, Yixuan Wu, Zhaokang Liang, Jian Wu, Hongxia Xu
- **备注**: Accepted by IJCAI 2026
- **摘要**: 设计满足多种预期属性的功能性蛋白质序列是蛋白质工程的核心研究重点。以往的方法在处理众多且往往冲突的属性时，表现出能力不足或效率低下的问题。我们提出了多属性蛋白质扩散 (MP2D)，这是一个统一的多目标蛋白质序列优化框架，它集成了条件离散扩散、受限蒙特卡洛树搜索 (MCTS) 和全局迭代优化。MP2D 将扩散去噪建模为一个受限的序列决策过程，并利用 MCTS 在基于帕累托奖励的引导下探索多样化的去噪轨迹。全局迭代优化策略进一步实现了候选序列的重复掩码和再优化，而动态帕累托约束则防止了候选序列冗余并保持了目标间的平衡权衡。我们在两项具有挑战性的多目标蛋白质设计任务上评估了 MP2D：抗菌肽和蛋白质结合剂优化，涉及四到五个冲突属性。实验结果表明，MP2D 在无需重新训练生成模型的情况下，始终优于现有的多目标基线，在所有目标上实现了稳健且平衡的提升。
- **PDF**: https://arxiv.org/pdf/2605.05829v1

### Robust chemotaxis beyond sensing limits: signal, noise, and strategy
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.03632v1
- **作者**: Robert G. Endres
- **备注**: Accepted for Physical Biology (IOP Publishing)
- **摘要**: 长期以来，细菌趋化性被认为是在接近 Berg 和 Purcell 最初阐述的感官物理极限下运行的。最近的信息论分析挑战了这一观点，表明大肠杆菌仅利用配体到达统计中可用信息的一小部分来偏置其运动。这种低信息效率在行为层面应如何解读？在这里，我认为趋化性能不仅由信息传输和噪声决定，还受到运动策略本身的影响。通过简单的标度分析和极简模型，我展示了即使内部信息处理效率低下，运行-翻转（run-and-tumble）趋化性如何通过对称性和时间平均保持对噪声的鲁棒性。通过比较细菌和真核细胞的趋化性，强调了不同的感官策略如何将物理极限转化为可观察的行为。这些考量表明，低信息效率并不一定意味着性能低下，反而可能反映了鲁棒性、简洁性和功能之间进化出的平衡。
- **PDF**: https://arxiv.org/pdf/2605.03632v1

--- 
## 📚 学科: `cs.*`
**学科总结**：本次 CS 领域的论文质量极高，涵盖了 GUI 智能体定位、多智能体协同、LLM 内部机制剖析以及视觉重照明技术。特别是 CVPR 和 ICML 的多篇入选论文分别解决了 GUI 定位中的精度偏置（BAMI）、LLM 注意力汇聚的机械原理、以及多智能体系统的联合提示优化（MASPO）。这些研究深入到模型结构的微观层面及复杂任务的宏观协作，代表了当前 AI 领域的前沿突破。

### BAMI: Training-Free Bias Mitigation in GUI Grounding
- **分数**: 7
- **链接**: https://arxiv.org/abs/2605.06664v1
- **作者**: Borui Zhang, Bo Zhang, Bo Wang, Wenzhao Zheng, Yuhao Cheng, Liang Tang, Yiqiang Yan, Jie Zhou, Jiwen Lu
- **备注**: Accepted by CVPR 2026
- **摘要**: GUI 定位是使 GUI 智能体能够执行点击和拖动等任务的关键能力。然而，在像 ScreenSpot-Pro 基准这样的复杂场景中，现有模型的表现往往不尽如人意。利用提出的掩码预测分布 (MPD) 归因方法，我们发现错误的主要来源有两个：高图像分辨率（导致精度偏置）和复杂的界面元素（导致歧义偏置）。为了应对这些挑战，我们引入了偏置感知操控推理 (BAMI)，它结合了两个关键操控：粗到细的聚焦和候选选择，以有效缓解这些偏置。我们广泛的实验结果表明，BAMI 在无需训练的情况下显著提高了各种 GUI 定位模型的准确性。例如，将我们的方法应用于 TianXi-Action-7B 模型，使其在 ScreenSpot-Pro 基准上的准确率从 51.9% 提升至 57.8%。此外，消融研究证实了 BAMI 方法在不同参数配置下的鲁棒性，突出了其稳定性和有效性。
- **PDF**: https://arxiv.org/pdf/2605.06664v1

### MASPO: Joint Prompt Optimization for LLM-based Multi-Agent Systems
- **分数**: 7
- **链接**: https://arxiv.org/abs/2605.06623v1
- **作者**: Zhexuan Wang, Xuebo Liu, Li Wang, Zifei Shan, Yutong Wang, Zhenxi Song, Min Zhang
- **备注**: Accepted at ICML 2026
- **摘要**: 基于大语言模型 (LLM) 的多智能体系统 (MAS) 在处理复杂协作任务方面表现出潜力，其中智能体通常通过特定角色的提示词进行协调。虽然这些提示词的质量至关重要，但在相互作用的智能体之间联合优化它们仍然是一个非平凡的挑战，这主要是由于局部智能体目标与整体系统目标之间的失配。为了解决这个问题，我们引入了 MASPO，这是一个旨在跨整个系统自动且迭代地优化提示词的新型框架。MASPO 的核心创新是其联合评估机制，它不仅根据提示词的局部有效性，还根据其促进后续智能体成功的能力来评估提示词。这有效地弥合了局部交互与全局结果之间的差距，而不依赖于地面真值标签。此外，MASPO 采用数据驱动的进化束搜索来高效地在高维提示空间中导航。在 6 个多样化任务上的广泛实验评估表明，MASPO 始终优于最先进的提示优化方法，平均准确率提升了 2.9。
- **PDF**: https://arxiv.org/pdf/2605.06623v1

### The Structural Origin of Attention Sink: Variance Discrepancy, Super Neurons, and Dimension Disparity
- **分数**: 6
- **链接**: https://arxiv.org/abs/2605.06611v1
- **作者**: Siquan Li, Kaiqi Jiang, Jiacheng Sun, Tianyang Hu
- **备注**: Accepted to ICML 2026
- **摘要**: 尽管大语言模型 (LLM) 中普遍存在注意力汇聚 (Attention Sink) 现象——即初始 Token 不成比例地垄断了注意力得分，但其结构根源仍不清楚。本研究为该现象提供了机械论层面的解释。首先，我们将其根源追踪到自注意力机制中固有的值聚合过程，该过程诱导了系统性的方差差异。我们进一步证明，这种差异被前馈网络 (FFN) 层内超级神经元的激活大幅放大。具体而言，通道稀疏的下投影触发了第一个 Token 表示的维度差距，使得注意力汇聚作为结构锚点成为必然。随后，我们通过两种受控干预验证了这一因果链：(i) 通过修改注意力掩码隔离聚合效应，以及 (ii) 放大特定 Token 表示的方差。两种干预都能在任意位置复制注意力汇聚。我们的机制理解为系统性控制汇聚形成奠定了基础。最后，作为概念验证，我们提出了 Head-wise RMSNorm，这是一种在预训练期间稳定值聚合输出的架构修改。实验表明，恢复位置间的统计均等可显著加速收敛。
- **PDF**: https://arxiv.org/pdf/2605.06611v1

### Relit-LiVE: Relight Video by Jointly Learning Environment Video
- **分数**: 4
- **链接**: https://arxiv.org/abs/2605.06658v1
- **作者**: Weiqing Xiao, Hong Li, Xiuyu Yang, Houyuan Chen, Wenyi Li, Tianqi Liu, Shaocong Xu, Chongjie Ye, Hao Zhao, Beibei Wang
- **备注**: Accepted at SIGGRAPH 2026
- **摘要**: 最近的进展表明，大规模视频扩散模型可以通过先将视频分解为内在场景表示，然后在新的照明下进行前向渲染，从而重新用作神经渲染器。虽然前景光明，但这一范式从根本上依赖于精确的内在分解，而这对于真实视频来说仍然高度不可靠，往往导致重照明过程中出现外观扭曲、材质损坏和累积的时间伪影。在这项工作中，我们提出了 Relit-LiVE，这是一种新型视频重照明框架，可以在无需先验相机位姿知识的情况下产生物理一致且时间稳定的结果。我们的核心见解是在渲染过程中显式引入原始参考图像，使模型能够恢复内在表示中不可避免丢失或损坏的关键场景线索。此外，我们提出了一种新型环境视频预测公式，在单个扩散过程中同时生成重照明视频和与每个相机视角对齐的逐帧环境贴图。这种联合预测强制执行了强大的几何-照明对齐，并自然地支持动态照明和相机运动。实验证明，Relit-LiVE 在合成和真实基准测试中始终优于最先进的视频重照明和神经渲染方法。
- **PDF**: https://arxiv.org/pdf/2605.06658v1

### Multi-Robot Coordination in V2X Environments
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.06662v1
- **作者**: John Pravin Arockiasamy, Alexey Vinel
- **备注**: Accepted at IEEE ITSC 2026
- **摘要**: 本文提出了一种车联网 (V2X) 通信框架，使在复杂城市交通环境中运行的社交机器人能够实现去中心化协作。基于 ETSI 协作感知和机动协调服务，该框架引入了两个以机器人为中心的设施层服务：机器人感知服务 (RAS) 和机器人机动协调服务 (RMCS)，分别通过机器人感知消息 (RAM) 和机器人机动协调消息 (RMCM) 实现。RAS 支持角色感知、任务导向的机器人感知，同时将外部检测到的弱势道路使用者 (VRU，包括非 V2X 行人) 整合到协作感知中。RMCS 支持在明确建立的角色下实现事件驱动、低延迟的机器人机动机调，无需集中式基础设施或预先配对。真实世界的概念验证展示了类人机器人和四足机器人在道路穿越场景中协助行人的确定性多机器人协作。补充仿真评估表明，基于 RAS 的聚类在集成安全关键区域的非 V2X VRU 的同时，减少了来自 V2X VRU 的冗余传输，从而降低了信道负载。
- **PDF**: https://arxiv.org/pdf/2605.06662v1

--- 
## 📚 学科: `math.*`
**学科总结**：本周数学学科关注点集中在几何问题的非迭代求解、双层优化收敛率加速以及最优传输在动力系统中的应用。亮点包括利用 FFT 插值技术规避矩阵求逆，从而极大地提升极小问题的求解稳定性；以及提出二阶双层近似方法 FSBA，在非凸-强凸优化中实现了加速收敛。这些理论进展为计算机视觉与机器学习中的底层计算提供了坚实的数学支撑。

### Solving Minimal Problems Without Matrix Inversion Using FFT-Based Interpolation
- **分数**: 6
- **链接**: https://arxiv.org/abs/2605.06572v1
- **作者**: Haidong Wu, Snehal Bhayani, Janne Heikkilä
- **备注**: Accepted to CVPR 2026
- **摘要**: 估计相机几何通常涉及求解构造为多元多项式方程组的极小问题，由于在线求解器中需要矩阵求逆，现有的基于 Gröbner 基或结式的方法往往面临计算挑战。在此，我们提出了一种基于采样的、免矩阵求逆的方法，使用稀疏隐变量结式构造求解器。隐变量中的行列式多项式通过采样的逆快速傅里叶变换 (IFFT) 插值高效重构，避免了符号展开。求解该多项式可得到隐变量，其余未知数通过识别秩 1 亏损子矩阵并应用克莱姆法则恢复。一种基于最大公约数的准则确保了在噪声下子矩阵识别的鲁棒性。在各种极小问题上的实验表明，所提求解器具有强大的数值稳定性和极具竞争力的运行时间，特别是对于小规模问题，为传统的基于 Gröbner 基和结式的求解器提供了一个实用的替代方案。
- **PDF**: https://arxiv.org/pdf/2605.06572v1

### Second-Order Bilevel Optimization with Accelerated Convergence Rates
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.06431v1
- **作者**: Sheng Yang, Chengchang Liu, Lesi Chen, John C. S. Lui
- **备注**: Accepted by ICML 2026
- **摘要**: 本文研究了非凸-强凸双层优化的二阶方法。我们提出了一种新型的全二阶双层近似方法 (FSBA)，在寻找超目标函数的二阶平稳点时实现了 $\tilde{\mathcal{O}}(ε^{-1.5})$ 的迭代复杂度。我们的结果证明，在双层优化中，二阶方法可以实现比一阶方法更快的收敛速度。为了解决与二阶算子相关的高昂计算成本，我们引入了 FSBA 的延迟变体 LFSBA，它在多次迭代中重用二阶信息。我们证明 LFSBA 的计算复杂度比 FSBA 提高了一个因子 $\sqrt{d}$（$d$ 为维度）。我们还将类似思路应用于非凸强凹极大极小优化，提出了延迟极大极小三次正则化牛顿法 (LMCN)。
- **PDF**: https://arxiv.org/pdf/2605.06431v1

--- 
## 📚 学科: `astro-ph.*`
**学科总结**：本次天文物理选取的论文聚焦于观测技术、探测管线与物理特性分析。涵盖了 LIFE 空间任务的干涉仪基线优化、多星湍流监测仪 (MTM) 的性能评估、贝加尔湖中微子望远镜的轨道重建、极高 [OIII]/[OII] 比例星系的化学丰度研究，以及利用深度学习自动识别 LoTSS-DR3 巡天中的弥散射电辐射。这些研究体现了精密仪器、自动化管线与多波段分析在理解宇宙结构中的协同作用。

### A preliminary exploration of the effects of baseline length for the LIFE space mission
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.06648v1
- **作者**: Jonah T. Hansen et al.
- **备注**: Accepted for publication in PASP
- **摘要**: LIFE 空间任务旨在通过消零干涉技术发现和表征数十个宜居系外行星。此类任务的关键参数之一是消零基线长度。随着行星发生率统计和仿真工具的进步，我们现在可以更详细地重新审视这一假设，特别是考虑到减少基线范围以降低任务实施难度。我们利用 LIFEsim 模拟器和修正的数学工具，确定是否可以在不显著影响行星产量和条纹跟踪性能的情况下缩小基线范围。我们发现，LIFE 确实可以利用相当短的基线范围（如 25-80 米），甚至离散基线，而不会损失太多性能（<10%）。然而，必须在性能和实施简化之间进行谨慎权衡。
- **PDF**: https://arxiv.org/pdf/2605.06648v1

### Atmospheric turbulence profiling with the Multistar Turbulence Monitor
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.06449v1
- **作者**: Weisen Huang, Bin Ma et al.
- **摘要**: 大气光学湍流的精确表征对于评估天文选址和优化自适应光学系统至关重要。多星湍流监测仪 (MTM) 通过测量短曝光帧中多个恒星对之间的微分图像运动，推断折射率结构常数 $C_n^2(z)$ 的垂直分布。我们对 MTM 方法进行了全面研究。基于标准 HV 湍流模型的模拟证明，反演管线在现实噪声下能稳健地恢复积分视宁度和垂直湍流剖面。在稻城天文站的三晚实测数据表明，MTM 推导的视宁度与同步的 DIMM 结果高度一致。
- **PDF**: https://arxiv.org/pdf/2605.06449v1

### Muon Track Reconstruction Procedures at the Baikal-GVD Neutrino Telescope
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.06428v1
- **作者**: Grigory Safronov
- **摘要**: 贝加尔湖中微子望远镜 (Baikal-GVD) 是北半球同类中最大的探测器。中微子在探测器附近相互作用产生的 μ 子会在探测器中留下轨迹响应，从而可以重建中微子的到达方向，精度可达 0.2 度。Baikal-GVD 合作组开发了多种用于轨迹类事件分析的方法。本报告讨论了轨迹方向、能量重建及中微子候选事件选择的方法，并展示了 2019 至 2021 观测季数据的初步分析结果。
- **PDF**: https://arxiv.org/pdf/2605.06428v1

### Galaxy clusters in the LoTSS-DR3: Catalogues and detection pipeline for diffuse radio emission
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.06400v1
- **作者**: C. Stuardi et al.
- **摘要**: LOFAR 两米天际巡天 (LoTSS) 的第三次数据发布提供了 144 MHz 下北半球星空的空前视图。识别与星系团相关的弥散射电辐射仍需专用处理和人工检查。我们开发了一个自动化管线，利用 Radio U-Net（一种为图像分割优化的卷积神经网络）从 LoTSS-DR3 图像中构建托管弥散射电辐射的星系团目录。我们将网络输出与来自 X 射线和 SZ 选定的 3822 个星系团的信息相结合，验证了星系团中弥散射电源的探测率随质量和红移而增加。
- **PDF**: https://arxiv.org/pdf/2605.06400v1

--- 
## 📚 学科: `stat.*`
**学科总结**：统计学领域的论文关注点涵盖了深度神经网络的机制解释与实际生物营养学中的贝叶斯建模。研究揭示了 Transformer 架构中“注意力汇聚”现象背后的统计方差失衡机制，并提出了有效的架构改进建议；同时，针对鱼类营养实验中的剂量评估问题，引入了灵活的贝叶斯分数多项式框架，展示了统计建模在处理非线性响应和量化不确定性方面的强大能力。

### Bayesian Fractional Polynomials for Optimal Dosage Estimation with Fish Nutrition Applications
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.06237v1
- **作者**: Aliaksandr Hubin, Åshild Krogdahl, Guro Løkka, Trond M. Kortner
- **备注**: Accepted to IWSM 2026
- **摘要**: 最优剂量估计问题出现在从药理学、毒理学到水产养殖和环境研究的各个科学领域。对非线性剂量-反应关系进行统计建模对于量化生物学效应和确定反应最优水平至关重要。本文介绍了一种灵活的贝叶斯分数多项式 (BFP) 框架，用于对这种关系进行建模，允许通过贝叶斯模型平均进行模型不确定性量化和稳健预测。广泛的模拟结果表明，所提 BFP 方法能够准确估计最优剂量水平，显著优于基准方法。该方法在鱼类营养需求实验的真实数据上得到了演示。
- **PDF**: https://arxiv.org/pdf/2605.06237v1

--- 
## 📚 学科: `econ.*`
**学科总结**：本周经济学领域收录了一篇关于计算方法创新的论文，提出了一种基于特征值的快速蒙特卡洛（Fast Monte-Carlo）算法。该方法通过小样本近似显著降低了传统 MCMC 模拟所需的路径数量，在保持分布稳健性的同时大幅提升了计算效率，对于需要高频、快速响应的经济预测与金融风险管理场景具有极高的实用价值。

### Fast Monte-Carlo
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.02085v1
- **作者**: Irene Aldridge
- **备注**: Originally published in the proceedings of WSC 2025
- **摘要**: 本文提出了一种基于特征值的小样本近似方法，用于改进著名的马尔可夫链蒙特卡洛 (MCMC) 算法，该方法产生的平稳分布与传统蒙特卡洛方法一致。所提出的基于特征值的方法将蒙特卡洛所需的路径数量从多达 1,000,000 条减少到最少 10 条（取决于模拟时间跨度 $T$），并能产生在 Wasserstein 距离衡量下具有可比性且分布稳健的结果。该方法还显著降低了平稳分布的方差。
- **PDF**: https://arxiv.org/pdf/2605.02085v1

---