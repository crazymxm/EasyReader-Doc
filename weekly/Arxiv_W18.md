# 🗓️ 论文推荐周报 (2026-W18)
> 更新时间: 2026-05-04

--- 

## 📚 学科: `eess.*` (电工、系统与信号处理)
**选文简评：** 本周入选论文聚焦于遥感影像处理的前沿技术（高光谱图像超分与融合分类）以及 5G 通信技术的实地应用验证。这些研究不仅具有深厚的理论基础（多被 IEEE 顶级期刊接收），且提供了开源代码，具有很高的工程参考价值。

### Spectral Dynamic Attention Network for Hyperspectral Image Super-Resolution
- **分数**: 4
- **备注**: Accepted for publication in IEEE GRSL 2026
- **摘要**: 高光谱图像超分辨率对于增强 HSI 数据空间保真度至关重要，但现有深度学习方法常受限于光谱冗余及标准前馈网络（FFN）建模能力不足。为此，我们提出了光谱动态注意力网络（SDANet）。该框架包含：1）动态通道稀疏注意力（DCSA）模块，通过自适应稀疏化选择最具信息量的响应；2）频率增强前馈网络（FE-FFN），结合空间和频域建模以增强非线性表达。实验证明 SDANet 在保持效率的同时达到了 SOTA 性能。
- **链接**: [arXiv:2604.27326](https://arxiv.org/abs/2604.27326v1) | [PDF](https://arxiv.org/pdf/2604.27326v1)

### Representative Spectral Correlation Network for Multi-source Remote Sensing Image Classification
- **分数**: 4
- **备注**: Accepted for publication in IEEE TGRS 2026
- **摘要**: HSI 与 SAR/LiDAR 数据融合在土地覆盖分类中极具潜力，但面临光谱冗余和跨源异构性的挑战。我们提出 RSCNet，通过两个核心组件解决问题：1）关键波段选择模块（KBSM），在跨源引导下自适应选择任务相关的波段，优于传统的 PCA 降维；2）跨源自适应融合模块（CAFM），执行跨源注意力加权和局部-全局上下文精炼。实验表明，RSCNet 在降低计算复杂度的同时，性能优于当前主流方法。
- **链接**: [arXiv:2604.27323](https://arxiv.org/abs/2604.27323v1) | [PDF](https://arxiv.org/pdf/2604.27323v1)

### Experimental Performance of a 5G N78 Reconfigurable Intelligent Surface
- **分数**: 3
- **备注**: Accepted in IEEE ICT2026
- **摘要**: 本文针对 5G N78 频段的可重构智能表面（RIS）原型进行了真实世界的实验分析。不同于仅关注仿真的研究，本系统经过了室内、室外长距离以及商用 5G 独立组网环境下的三阶段验证。结果显示，RIS 能显著提升非视距（NLoS）区域的 RSRP 和 SINR 指标，并在原本无信号的地点恢复 5G 服务，证明了其在商用网络中的覆盖增强潜力。
- **链接**: [arXiv:2604.28044](https://arxiv.org/abs/2604.28044v1) | [PDF](https://arxiv.org/pdf/2604.28044v1)

--- 

## 📚 学科: `cs.*` (计算机科学)
**选文简评：** 本周 CS 领域高质量论文爆发，涵盖了 AI 论文图像法证、自监督动作表征、物理一致性视频生成以及 LLM 在医疗诊断中的应用。这些论文均来自 CVPR、ACL 等顶会，代表了当前 AI 领域在可控性、可解释性及垂直领域落地的最新方向。

### AEGIS: A Holistic Benchmark for Evaluating Forensic Analysis of AI-Generated Academic Images
- **分数**: 6
- **备注**: Accepted to ACL 2026 Main Conference
- **摘要**: 我们推出了 AEGIS，一个用于评估 AI 生成学术图像法证分析的全方位基准。AEGIS 具有三大特点：1）领域复杂性：涵盖 7 大类 39 个细分学术类别，即便是 GPT-5.1 的性能也仅为 48.80%；2）多样化的伪造模拟：涵盖 25 个生成模型的 4 种策略；3）多维度评估：结合检测、推理和定位。AEGIS 揭示了现有模型（包括 MLLM）在学术图像真实性检测方面的根本局限性。
- **链接**: [arXiv:2604.28177](https://arxiv.org/abs/2604.28177v1) | [PDF](https://arxiv.org/pdf/2604.28177v1)

### Action Motifs: Self-Supervised Hierarchical Representation of Human Body Movements
- **分数**: 6
- **备注**: CVPR 2026 (Highlight)
- **摘要**: 有效的人类行为建模依赖于动作的组合性。我们提出了一种层级表征：捕捉原子关节运动的“动作原子”（Action Atoms）和由其组合而成的、跨动作共享的“动作基元”（Action Motifs）。通过嵌套潜变量 Transformer (A4Mer)，我们以全自适应、自监督的方式学习这些表征。实验表明，提取的 Action Motifs 显著提升了动作识别、运动预测和插值任务的性能。
- **链接**: [arXiv:2604.28173](https://arxiv.org/abs/2604.28173v1) | [PDF](https://arxiv.org/pdf/2604.28173v1)

### PhyCo: Learning Controllable Physical Priors for Generative Motion
- **分数**: 4
- **备注**: CVPR 2026
- **摘要**: 现代视频扩散模型在物理一致性方面仍表现欠缺（如物体漂移、碰撞反弹不真实）。PhyCo 框架将物理约束引入视频生成，包括：基于 10 万个物理仿真视频的数据集、利用 ControlNet 进行物理属性微调，以及通过 VLM 引导的奖励优化。该方法使生成模型无需推理时调用仿真器，即可产生符合摩擦力、恢复系数等物理属性的连续可控视频。
- **链接**: [arXiv:2604.28169](https://arxiv.org/abs/2604.28169v1) | [PDF](https://arxiv.org/pdf/2604.28169v1)

### LLM as Clinical Graph Structure Refiner: Enhancing Representation Learning in EEG Seizure Diagnosis
- **分数**: 3
- **备注**: Accepted by IJCAI-ECAI 2026
- **摘要**: 脑电图（EEG）信号中的噪声使癫痫自动检测具有挑战性。我们探索利用大语言模型（LLM）作为图边缘精炼器。框架分为两阶段：首先通过 Transformer 预测初始图连接，随后利用 LLM 的推理能力，结合文本和统计特征识别并剔除冗余连接。在 TUSZ 数据集上的实验表明，该方法不仅提升了检测准确率，还产生更具解释性的脑电图表征。
- **链接**: [arXiv:2604.28178](https://arxiv.org/abs/2604.28178v1) | [PDF](https://arxiv.org/pdf/2604.28178v1)

--- 

## 📚 学科: `astro-ph.*` (天体物理)
**选文简评：** 本周选文侧重于恒星参数的精确建模以及活动星系核（AGN）的观测分析。特别是针对 PLATO 任务的恒星表征研究，为未来的系外行星搜寻提供了关键的技术支撑。

### Asteroseismic modelling of solar-like stars with the FICO procedure
- **分数**: 3
- **备注**: Accepted for publication in Astronomy and Astrophysics
- **摘要**: 本文介绍了使用 FICO 程序对 95 颗主序类日恒星和 Kepler 系外行星宿主星进行的详细震迹建模。FICO 结合了正向和反向反演技术，实现了对质量（2.3%）、半径（0.82%）和年龄（6.9%）的高精度推断，满足了 PLATO 任务的质量要求。结果证实，该方法比传统的表面修正法更能有效减轻高质恒星建模中的偏差。
- **链接**: [arXiv:2604.27842](https://arxiv.org/abs/2604.27842v1) | [PDF](https://arxiv.org/pdf/2604.27842v1)

### Robust AGN and host-galaxy decomposition in optical spectral fitting
- **分数**: 3
- **备注**: Accepted by A&A
- **摘要**: 解开超大质量黑洞的生长与其宿主星系的联系，需要从恒星光谱中精确分离出 AGN 发射。我们提出了一种结合 pPXF 和 PyQSOFit 的新型光谱拟合方法。通过对 SDSS 样本的验证，该方法在 AGN 贡献率不同的情况下均能获得一致的黑洞质量、恒星质量和速度弥散度测量值，为研究变相 AGN 的物理性质提供了稳健工具。
- **链接**: [arXiv:2604.27783](https://arxiv.org/abs/2604.27783v1) | [PDF](https://arxiv.org/pdf/2604.27783v1)

--- 

## 📚 学科: `stat.*` (统计学)
**选文简评：** 统计学论文本周深入探讨了风险评估中的结构性限制及收益最大化的学习曲线。特别是关于“似然比之墙”的研究，对算法公平性和罕见事件预测具有深远的社会与法律启示。

### The Likelihood Ratio Wall: Structural Limits on Accurate Risk Assessment
- **分数**: 3
- **备注**: Accepted to FAccT 2026
- **摘要**: 审前风险评估工具常用于预测罕见暴力犯罪，但面临基本的统计障碍。我们推导出一个通用精度界限——“似然比之墙”。结果表明，当暴力再犯罪率极低（2-5%）时，现有工具极难达到 50% 的阳性预测值。此外，我们证明了“监控天花板”效应：过度执法会结构性地降低被过度执法群体的预测精度。这暗示在缺乏高置信度数据的情况下，不应仅依赖算法做出个体羁押决策。
- **链接**: [arXiv:2604.27282](https://arxiv.org/abs/2604.27282v1) | [PDF](https://arxiv.org/pdf/2604.27282v1)

### On the Learning Curves of Revenue Maximization
- **分数**: 3
- **备注**: To appear in STOC 2026
- **摘要**: 本文研究了收益最大化学习算法的性能如何随数据量增长而提升。在单物品单买家的基本设定下，我们证明了贝叶斯一致算法的存在性，但其收敛速度可能极慢。如果最优收益由有限价格实现，则衰减率为 $1/\sqrt{n}$。对于离散分布，学习曲线呈现接近指数级的衰减，这一速度在传统 PAC 框架下是无法达到的。
- **链接**: [arXiv:2604.26922](https://arxiv.org/abs/2604.26922v1) | [PDF](https://arxiv.org/pdf/2604.26922v1)

--- 
