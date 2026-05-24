# 🗓️ 周报 (2026-W21)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-05-24

--- 
## 📚 学科: `eess.*`

本周 `eess.*` 领域涵盖了视觉推理分割、自动泊车、生物信号提取、安全强化学习及语音识别等多个方向。重点论文包括利用稀疏自编码器提升推理分割可解释性的 SegCompass，以及通过三阶段学习大幅加速自动泊车路径规划的 N3P 框架。此外，针对远程光电容积脉搏波（rPPG）的信号分离和具备概率安全保证的核嵌入强化学习算法也展示了该学科在智能化与鲁棒性方面的最新进展。

### SegCompass: Exploring Interpretable Alignment with Sparse Autoencoders for Enhanced Reasoning Segmentation
- **分数**: 7
- **链接**: https://arxiv.org/abs/2605.22658v1
- **备注**: Accepted by CVPR 2026.
- **摘要**: 尽管大语言模型提供了强大的组合推理能力，但现有的推理分割流水线无法透明地将这种推理与视觉感知联系起来。我们提出了 SegCompass，这是一个端到端模型，利用稀疏自编码器 (SAE) 构建了一个显式、可解释且可微的对齐路径。给定图像-指令对，SegCompass 首先生成思维链 (CoT) 轨迹。其核心是将 CoT 和视觉标记映射到共享的高维稀疏概念空间中。通过 SAE 驱动的界面，模型提供了一个比隐式查询更具追溯性的“白盒”连接。在五个挑战性基准测试上的实验表明，SegCompass 达到或超越了现有顶尖性能，并证明了学习到的稀疏概念质量与掩码准确度之间存在强相关性。
- **PDF**: https://arxiv.org/pdf/2605.22658v1

### N3P: Accelerated Automated Parking via a Learning-Based Naturalistic Three-Stage Scheme
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.22722v1
- **备注**: Accepted at IEEE ITSC 2026.
- **摘要**: 自动泊车需要在受限环境中进行高效的路径规划。我们提出了 N3P，一种快速的基于学习的三阶段自动泊车框架。通过引入中间准备位姿并使用学习模块对其进行预测，N3P 将复杂的机动动作分解为更简单的子问题，从而降低计算复杂度并加速路径生成。在垂直和平行泊车场景中的实验表明，增强后的 Hybrid A* 算法规划速度提升了 80% 以上，且在成功率和轨迹质量（更短的轨迹、更少的换挡次数）方面均优于强化学习基准方法。
- **PDF**: https://arxiv.org/pdf/2605.22722v1

### Time-varying rPPG signal separation via block-sparse signal model
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.22425v1
- **备注**: Accepted by IEEE ICIP 2026.
- **摘要**: 远程光电容积脉搏波 (rPPG) 通过分析面部视频中的细微颜色变化来实现心率信号的非接触式测量。由于信号强度极其微弱且易受光照噪声干扰，提取工作极具挑战。本文提出了一种利用 rPPG 信号拟周期特性的提取方法。我们将时频域中的拟周期性建模为块稀疏结构，并构建了一个时变信号分离框架，以实现光照波动下的自适应信号分离。在公开数据集上的实验验证了该方法的有效性。
- **PDF**: https://arxiv.org/pdf/2605.22425v1

### Kernel-Based Safe Exploration in Deep Reinforcement Learning
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.22207v1
- **备注**: Accepted at L4DC Conference 2026.
- **摘要**: 在现实世界中部署深度强化学习时，安全性是一个主要问题。我们展示了如何使用核嵌入在未知动力学的随机系统学习过程中同步学习障碍函数。我们的算法 KBSE（基于核的安全探索）在探索过程中同时学习最优策略和障碍函数。障碍函数以条件均值嵌入的形式表示，随着探索的增加提供更好的概率安全保证。当检测到安全违规时，算法会干预并将不安全动作修改为安全动作，从而确保探索被限制在能够限制到达不安全状态概率的动作内。
- **PDF**: https://arxiv.org/pdf/2605.22207v1

### Effective User-defined Keyword Spotting with Dual-stage Matching, Multi-modal Enrollment, and Continual Adaptation
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.22120v1
- **备注**: Accepted by TASLP.
- **摘要**: 用户自定义关键词检测 (KWS) 对个性化语音交互至关重要。我们引入了 DMA-KWS 框架：首先采用双阶段匹配流水线（CTC 解码配合流式音素搜索，随后进行精细化验证）；其次，多模态注册融合了用户特定语音与文本嵌入以提高准确性；最后，提出一种参数高效的持续适配机制，使用合成和真实数据进行轻量级更新。实验表明，DMA-KWS 在 LibriPhrase 数据集上达到了 97.85% 的 AUC，且仅需更新 187k 参数即可实现高效的设备端部署。
- **PDF**: https://arxiv.org/pdf/2605.22120v1

--- 
## 📚 学科: `q-bio.*`

本周 `q-bio.*` 领域的研究集中在蛋白质-配体相互作用、社会动力学建模及药物分子筛选。HCLBind 通过分层对比学习提升了多结构域蛋白质结合亲和力的预测精度。另一项研究则利用 SIR 模型和平均场理论探讨了在线仇恨内容的传播规律及其治理政策的潜在反作用。此外，TACK 论文对 PROTAC 降解活性预测进行了系统性的统计评估，挑战了复杂模型必然优于传统方法的假设，并提供了不确定性量化的新工具。

### Hierarchical Contrastive Learning for Multi-Domain Protein-Ligand Binding
- **分数**: 4
- **链接**: https://arxiv.org/abs/2605.19902v1
- **备注**: Accepted by ISBRA 2026.
- **摘要**: 预测多结构域蛋白质的配体结合亲和力仍然是一个难题。我们引入了 HCLBind，这是一个将几何表示学习与亲和力回归解耦的自监督框架。HCLBind 提出了一种新型的分层负采样策略：模型通过单结构域蛋白质的坐标扰动学习局部物理化学约束，并通过多结构域复合物的域间旋转学习全局构象几何。实验证明，HCLBind 能有效学习判别性的界面特征并提供鲁棒的不确定性估计，克服了标准监督学习的局限性。
- **PDF**: https://arxiv.org/pdf/2605.19902v1

### How hate spreads online and why it returns: Re-entrant phases driven by collective behavior
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.21129v1
- **摘要**: 迫切需要理解新生成的仇恨内容如何及何时在线上传播。我们提出了一个结合易感-感染-恢复 (SIR) 动力学的双物种聚合-断裂模型，纳入了真实世界的特征：仇恨社区在监管较少的平台上生成内容，并跨平台建立链接。解析解和数值模拟均表明，传播受“回返阈值相位”支配：随着仇恨社区比例的变化，系统可能从传播转为不传播，再回到传播。这警示稳步减少仇恨社区数量的政策最初可能成功，但若推进过度则可能适得其反。
- **PDF**: https://arxiv.org/pdf/2605.21129v1

### TACK: A statistical evaluation of degradation activity on a novel TArgeting Chimeras Knowledge dataset
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.19579v1
- **备注**: Accepted to KDD '26.
- **摘要**: 蛋白降解靶向嵌合体 (PROTAC) 设计具有挑战性。我们介绍了 TACK，这是一个包含 3,514 种 PROTAC 及其降解终点的标准化数据集。通过严格的统计比较，我们发现经典方法（XGBoost 和 MLP）在活性预测方面显著优于领域专用的图神经网络模型（PROTAC-STAN）。此外，特征消融实验显示细胞上下文特征的重要性。最后，我们提出了基于集成的不确定性量化方法，实现了置信度感知的实验优先级排序。
- **PDF**: https://arxiv.org/pdf/2605.19579v1

--- 
## 📚 学科: `cs.*`

本周 `cs.*` 领域的精选论文涵盖了视觉语言导航、自动驾驶数据生成、生成式视频推理及医疗影像等前沿方向。CVPR 2026 接收的 AwareVLN 增强了导航智能体的自我感知能力，而 Sensor2Sensor 则利用生成式模型将普通行车视频转化为昂贵的自动驾驶多模态数据。此外，针对儿科罕见病识别中数据稀缺的问题，研究探讨了纯合成数据的有效性；在算法理论方面，SWAT 2026 的论文深入研究了最小和半径聚类问题的参数化复杂度。

### AwareVLN: Reasoning with Self-awareness for Vision-Language Navigation
- **分数**: 7
- **链接**: https://arxiv.org/abs/2605.22816v1
- **备注**: Accepted to CVPR 2026.
- **摘要**: 视觉语言导航 (VLN) 要求智能体将指令对应到视觉环境中的移动。我们提出了 AwareVLN，一个为导航模型配备自我感知推理机制的框架。该方法包含两大创新：(1) 培养空间和任务导向自我感知的结构化推理模块；(2) 带有进度划分的自动化数据引擎。在 Habitat 模拟器上的实验表明，AwareVLN 显著优于之前的顶尖方法，能在不依赖额外 3D 传感器的情况下实现显式且可解释的推理。
- **PDF**: https://arxiv.org/pdf/2605.22816v1

### Sensor2Sensor: Cross-Embodiment Sensor Conversion for Autonomous Driving
- **分数**: 6
- **链接**: https://arxiv.org/abs/2605.22809v1
- **备注**: Accepted by CVPR 2026.
- **摘要**: 自动驾驶系统的训练需要海量多模态数据。我们提出 Sensor2Sensor，一种将野外单目行车记录仪视频转换为高保真、多模态传感器套件（包括多视图图像和 LiDAR 点云）的新型生成建模范式。通过 4D 高斯溅射 (4DGS) 重建和扩散架构，我们克服了缺乏配对训练数据的挑战。该工具能将海量的互联网视频转化为可用于自动驾驶系统验证和训练的多模态格式。
- **PDF**: https://arxiv.org/pdf/2605.22809v1

### MotiMotion: Motion-Controlled Video Generation with Visual Reasoning
- **分数**: 4
- **链接**: https://arxiv.org/abs/2605.22818v1
- **备注**: ICML 2026.
- **摘要**: 当前的运动控制视频生成模型往往僵硬地遵循用户轨迹，忽略了次要的因果后果。我们提出 MotiMotion 框架，将运动控制重新表述为“推理后生成”问题。利用无需训练的视觉语言推理器来细化主轨迹并幻化合理的次要运动。此外，置信度感知控制方案能够利用生成先验校正低置信度输入下的伪影。在交互中心化的 MotiBench 基准上，该方法生成的视频在物体行为和交互合理性方面表现更优。
- **PDF**: https://arxiv.org/pdf/2605.22818v1

### Synthetic Data Alone is Enough? Rethinking Data Scarcity in Pediatric Rare Disease Recognition
- **分数**: 4
- **链接**: https://arxiv.org/abs/2605.22767v1
- **备注**: CVPR 2026 Workshop.
- **摘要**: 患有罕见遗传病的儿童通常具有独特的面部表型，但数据稀缺和隐私限制阻碍了自动诊断模型的发展。我们研究了在极低资源环境下仅使用合成数据的可行性。实验发现，在足够规模下，完全在表型感知合成面部图像上训练的模型可以达到与真实数据基准相当的性能。这表明高保真合成数据可以近似临床上有意义的分布，从而在保护隐私的同时支持遗传教育和临床辅助诊断。
- **PDF**: https://arxiv.org/pdf/2605.22767v1

### On the Parameterized Complexity of Min-Sum-Radii
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.22804v1
- **备注**: Accepted for SWAT 2026.
- **摘要**: 在最小和半径 (MSR) 聚类问题中，目标是在度量空间中找到最多 k 个簇以最小化半径总和。本文研究了无向图诱导度量下 MSR 的参数化复杂度。我们证明了 MSR 在加权二分图上是 W[1]-困难的（以簇数 k 为参数）。此外，我们展示了即使在顶点覆盖数加 k 的参数下，该问题在加权图上依然困难，但在参数为树宽加聚类成本时属于 FPT（固定参数可解）。
- **PDF**: https://arxiv.org/pdf/2605.22804v1

--- 
## 📚 学科: `math.*`
_本周缺少高价值论文_

--- 
## 📚 学科: `astro-ph.*`

本周天体物理学领域的精选论文涵盖了从恒星物理到星系演化的广阔尺度。研究内容包括利用 VLA 对碰撞风联星同步辐射极化信号的搜索，基于印度 Aditya-L1 卫星对太阳耀斑铁荧光特征的首次详尽分析，以及在原恒星核 L1544 中对双极扩散现象的直接探测。此外，爱尔兰 LOFAR 单站的脉冲星计时成果证明了低频射电阵列在长期监测中的潜力，而关于大质量星系宜居性的模拟研究则揭示了化学解耦与淬灭过程对系外行星生存环境的复杂影响。

### Search for radio polarization in the particle-accelerating colliding-wind binaries WR 147 and HD 167971
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.22617v1
- **摘要**: 粒子加速碰撞风联星 (PACWB) 是由大质量恒星组成的系统，其强烈的恒星风碰撞会将粒子加速至相对论能量并产生同步辐射。我们利用 VLA 观测了 WR 147 和 HD 167971。尽管预期存在线性极化，但在 L 和 C 波段均未探测到显著信号（极化度上限约 1%）。这可能是由于辐射区磁场的湍流性质、法拉第旋转引起的去极化以及由于热发射导致的稀释效应所致。
- **PDF**: https://arxiv.org/pdf/2605.22617v1

### Iron Fluorescence in X-class Solar Flares: Aditya-L1/SoLEXS Observations
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.22573v1
- **摘要**: 太阳耀斑期间，日冕 X 射线照射光球层会产生铁荧光。本研究利用印度 Aditya-L1 任务中的 SoLEXS 载荷，对 47 个 X 级耀斑的铁 Kα 荧光特征进行了首次综合分析。研究确定了铁 Kα 流量与激发流量之间的稳定关系，并观察到符合理论模型的中心到边缘依赖性。这证明了现代硅漂移探测器 (SDD) 即使光谱分辨率较低，也能作为探测日冕源高度和观察几何的新诊断工具。
- **PDF**: https://arxiv.org/pdf/2605.22573v1

### Probing the ion-neutral drift velocity towards the L1544 prestellar core: Detection of ambipolar diffusion using N$_2$D$^+$ and para-NH$_2$D
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.22541v1
- **摘要**: 当致密星核中的电离度下降时，磁场与物质可能解耦，导致离子与中性粒子的流速差异（即双极扩散）。我们观测了原恒星核 L1544 中的氘代离子 N2D+ 和中性物质 NH2D，发现了约 0.05 km/s 的速度偏移。这一发现是双极扩散的观测证据，强调了尘埃颗粒生长在调节致密核向原恒星坍缩动力学演化中的作用。
- **PDF**: https://arxiv.org/pdf/2605.22541v1

### Pulsar timing solutions for 17 pulsars at 150~MHz from the Irish LOFAR station
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.22516v1
- **摘要**: 本工作展示了爱尔兰 LOFAR 单站作为独立望远镜对脉冲星进行后续观测和计时的能力。在 2020 年至 2023 年间，我们对 33 颗候选脉冲星进行了监测，成功探测到 22 颗，并为其中的 17 颗提供了 150 MHz 下的相干计时解。其中 7 颗脉冲星是首次报告计时解。这证明了国际 LOFAR 站能有效缓解大型天文台的观测压力，并实现脉冲星的科学潜力。
- **PDF**: https://arxiv.org/pdf/2605.22516v1

### The habitability trade-off: Chemical decoupling and quenching in massive galaxies
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.22510v1
- **摘要**: 使用 IllustrisTNG 模拟研究发现，约 31.5% 的大质量恒星形成星系存在系统性的恒星-气体化学解耦，这通常由近期并合和部分淬灭引起。研究揭示了一个“宜居性权衡”：虽然气体稀释和淬灭降低了未来类地行星的形成效率，但也为现有行星创造了一个辐射危害受抑的短暂宜居窗口。仙女座星系 (M31) 与此类解耦星系表现出相似特征。
- **PDF**: https://arxiv.org/pdf/2605.22510v1

--- 
## 📚 学科: `stat.*`

本周统计学领域在生成式人工智能、不确定性量化及基础理论方面贡献了重要研究。ICML 2026 接收的论文深入探讨了 LLM “超拟合”现象的几何机制，为多样化生成提供了新见解。测试时自适应中的认知不确定性研究引入了 MMD 球与信念集理论，为模型可靠性提供了 PAC-Bayesian 保证。此外，有关神经过程摊销高斯过程推理的成本分析，以及贝叶斯非参数化历史的回顾，也为该领域的理论建设和实践应用提供了深度指导。

### Beyond Temperature: Hyperfitting as a Late-Stage Geometric Expansion
- **分数**: 6
- **链接**: https://arxiv.org/abs/2605.22579v1
- **备注**: Accepted at ICML 2026.
- **摘要**: 最近的研究发现，将 LLM 在小数据集上微调至近零训练损失（超拟合）能增强生成多样性。我们证明该现象并非简单的温度缩放，而是依赖于一种动态的、上下文相关的排序重排机制。层级分析显示，这种效应定位在最后一个 Transformer 块的“终端扩张”中，特征空间发生了显著的几何扩张（约 80.8 维），从而促进了长尾标记的提取。我们还提出了 Late-Stage LoRA，仅更新最后 5 层即可实现稳健生成。
- **PDF**: https://arxiv.org/pdf/2605.22579v1

### MMD-Balls as Credal Sets: A PAC-Bayesian Framework for Epistemic Uncertainty in Test-Time Adaptation
- **分数**: 6
- **链接**: https://arxiv.org/abs/21783v1
- **备注**: Accepted at EIML@ICML 2026.
- **摘要**: 测试时自适应 (TTA) 缺乏连接分布偏移程度与预测可靠性的正式保证。我们开发了一个 PAC-Bayesian 框架，将源分布周围的 MMD 球解释为不精确概率理论中的信念集，从而实现了自然的认知不确定性量化。该理论分离了认知与偶然不确定性，并提供了一个原则性的决策标准，用于确定何时需要进行模型自适应。
- **PDF**: https://arxiv.org/pdf/2605.21783v1

### Bayesian Nonparametrics: Principles and Practice
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.22253v1
- **摘要**: 本文是《贝叶斯非参数化》(Cambridge University Press, 2010) 一书的扩展序言。它解释了为什么贝叶斯非参数化在现代统计中至关重要，回顾了这一相对年轻领域的历史背景，概述了书中的核心内容，并探讨了该领域面临的挑战及未来的发展方向。
- **PDF**: https://arxiv.org/pdf/2605.22253v1

### Three Costs of Amortizing Gaussian Process Inference with Neural Processes
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.21798v1
- **备注**: To appear at ProbNum 2026.
- **摘要**: 神经过程通过学习从上下文集到预测分布的映射来摊销高斯过程 (GP) 推理。我们界定了 GP 与神经过程预测之间的 KL 散度，并将其分解为三个来源：标签污染、信息瓶颈和摊销误差。研究直接将架构尺寸与内核平滑度和输入维度联系起来，并提出了具体的架构建议，如仅从位置预测方差以及使用二阶池化来减小误差。
- **PDF**: https://arxiv.org/pdf/2605.21798v1

### On the Sample Complexity of Discounted Reinforcement Learning with Optimized Certainty Equivalents
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.21763v1
- **备注**: Accepted to RLC 2026.
- **摘要**: 本文研究了具有生成模型的折扣 MDP 中的风险敏感强化学习。我们关注优化确定性等价类 (OCE) 下学习最优价值函数和策略的样本复杂度。研究精确刻画了使 OCE 定义的目标为 PAC 可学习的效用函数特征，并建立了相应的样本复杂度上下界。特别地，对于 CVaR 风险度量，我们改进了其对风险水平参数的依赖项。
- **PDF**: https://arxiv.org/pdf/2605.21763v1

--- 
## 📚 学科: `econ.*`

本周 `econ.*` 领域的关注点主要在于社交网络中的行为传播动力学。通过对在线仇恨内容传播的建模，研究者探讨了复杂网络中的相变现象。研究指出，仇恨内容的扩散不仅取决于单个社区的活动，更取决于社区间的动态链接与平台监管政策的交互。这为数字经济下的内容治理提供了重要的博弈论与动力学参考。

### How hate spreads online and why it returns: Re-entrant phases driven by collective behavior
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.21129v1
- **摘要**: （同 q-bio 摘要）研究利用 SIR 动力学和聚合-断裂模型揭示了在线仇恨内容传播的阈值相位现象。研究特别指出，监管政策可能引发“回返相位”，即减少仇恨社区数量的努力在跨越特定阈值后可能反而导致仇恨传播的卷土重来。
- **PDF**: https://arxiv.org/pdf/2605.21129v1

---