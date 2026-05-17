# 🗓️ 周报 (2026-W20)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-05-17

--- 
## 📚 学科: `eess.*`

本周 eess 领域论文涵盖了控制理论、无线通信、视频编码和多机器人系统。重点探讨了离散时间系统连续嵌入的理论限制，针对 6G 网络的混合专家网络（MoE）资源优化，以及低复杂度的视频编码次级变换方法。此外，还涉及多机器人系统的分布式控制原型框架和化工装置硬件架构的启发式优化。整体展现了控制与通信技术在工业与智能系统中的深度融合。

### On the Nonexistence of Continuous Immersions for Discrete-time Systems
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.15161v1
- **作者**: Eron Ristich, Eduardo Sontag, Necmiye Ozay
- **摘要**: 了解非线性动力系统何时存在线性嵌入至关重要，因为这类嵌入允许我们利用丰富的线性系统理论工具来分析非线性动力学。最近，Liu 等人 (2023) 表明，对于允许可数个但多于一个 omega 极限集的连续时间动力系统，无法通过一一连续映射将其嵌入到有限维线性系统中。本文将这些结果扩展到离散时间动力学，并证明离散时间中也存在类似的障碍。我们进一步考虑了涉及 alpha 极限集的推广。文中提供了几个示例来演示这些结果。
- **PDF**: https://arxiv.org/pdf/2605.15161v1

### Deep Mixture of Experts Network for Resource Optimization in Aerial-Terrestrial CF-mMIMO Systems under URLLC
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.15135v1
- **作者**: Donggen Li, Chong Huang, Jingfu Li, Pei Xiao, Wenjiang Feng, Dusit Niyato, Zhu Han
- **摘要**: 超可靠低延迟通信 (URLLC) 作为第六代 (6G) 无线网络的关键组成部分，有望支持低空环境中的实时可靠信息交换。然而，实现 URLLC 通常会带来巨大的资源开销，包括带宽消耗增加、发射功率提高以及接入点 (AP) 部署更密集，这对比谱效率 (SE) 和能量效率 (EE) 提出了巨大挑战。此外，现有的迭代优化算法计算密集，难以满足 URLLC 的延迟要求。为了应对这些挑战，我们提出了一种混合空地无小区大规模 MIMO (CF-mMIMO) 网络来支持多样化服务，并开发了频道预测网络和深度混合专家 (MoE) 网络进行上行链路优化。首先，我们设计了信道预测网络 (CP-Net) 以减轻高移动性用户设备 (UE) 造成的信道老化。随后基于预测的 CSI，开发了用于功率分配的深度 MoE 网络。实验结果证明了该方法的有效性。
- **PDF**: https://arxiv.org/pdf/2605.15135v1

### FaSST: Fast Sparsifying Secondary Transform
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.15086v1
- **作者**: Darukeesan Pakiyarajah, Samuel Fernández-Menduiña, Eduardo Pavez, Antonio Ortega, Debargha Mukherjee
- **摘要**: 数据相关的次级变换旨在解耦可分初级变换的系数，可以提高残差编码效率；然而，其部署往往受限于计算复杂度。最近的视频编解码器使用低频非可分变换 (LFNST) 的变体，它丢弃了一些高频次级变换系数，限制了编码增益。此外，现有的数据相关次级变换缺乏明确的率失真 (RD) 优化设计准则。在这项工作中，我们提出了一种设计低复杂度数据相关次级变换的框架，称为快速稀疏化次级变换 (FaSST)。我们的方法通过将数据驱动的稀疏正交变换 (SOT) 分解为一系列 Givens 旋转来对其进行近似。实验结果表明，模式自适应的 FaSST 在匹配 LFNST 的 RD 性能的同时，减少了 83.67% 的计算量。
- **PDF**: https://arxiv.org/pdf/2605.15086v1

### A Prototyping Framework for Distributed Control of Multi-Robot Systems
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.15049v1
- **作者**: Junaid Ahmed Memon, Allan Andre Do Nascimento, Kostas Margellos, Antonis Papachristodoulou
- **摘要**: 本文介绍了一种用于多机器人系统分布式控制的原型框架，旨在弥合理论与分布式优化算法实际测试之间的差距。该框架使用单程序多数据 (SPMD) 范式，在单台计算机上模拟分布式控制，每个核心运行相同的算法，并利用局部状态和邻居间的通信。我们在四旋翼无人机位置交换任务中演示了该框架，使用了非合作博弈论分布式算法。结果表明，该框架为验证分布式算法提供了一种低成本且易于获取的方法。
- **PDF**: https://arxiv.org/pdf/2605.15049v1

### Hybrid Metaheuristic Optimization of Distributed Control System Hardware Architecture with Model-Based Verification
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.14788v1
- **作者**: Ruslan Zakirzyanov
- **摘要**: 大型化工厂依赖于分布式过程控制系统 (PCS)，这些系统由通过工业网络互连的众多处理单元、通信模块和 I/O 设备组成。在工厂参数部分不确定的情况下，设计成本效益高且可靠的硬件架构仍然是一个具有挑战性的组合优化问题。本文提出了一种用于分布式控制系统硬件架构合成的形式化模型。开发了一个基于混合蚁群的元启发式框架来构建可行的分层架构。该方法在大型硫酸厂控制系统的案例研究中得到了验证。结果证实，所获得的架构满足结构和动态性能要求。
- **PDF**: https://arxiv.org/pdf/2605.14788v1

--- 
## 📚 学科: `q-bio.*`

本周 q-bio 领域专注于神经群体活动的建模预测及其在行为解码中的应用。两篇论文均投稿至 NeurIPS 2026，展示了该方向的前沿趋势：一是利用 Mamba 模型在 Neuropixels 尺度上实现隐式行为解码，其表现优于传统线性分类器；二是推出了 SpikeProphecy 大型基准测试集，旨在标准化因果自回归脉冲序列预测的评估流程，并提出了多维度的群体指标分解方法，为解析大脑区域的可预测性提供了新工具。

### Implicit Behavioral Decoding from Next-Step Spike Forecasts at Population Scale
- **分数**: 4
- **链接**: https://arxiv.org/abs/2605.12999v1
- **作者**: John R. Minnick, Jesus Gonzalez-Ferrer, Kamran Hussain, Jinghui Geng, Ash Robbins, Mohammed A. Mostajo-Radji, David Haussler, Jason Eshraghian, Mircea Teodorescu
- **摘要**: 闭环脑机接口通常需要预测即将发生的神经群体活动并读取动物的行为状态。一个仅在 Neuropixels 尺度上针对下一步脉冲计数进行训练的 Mamba 预测器，可以在一次前向传递中同时完成这两项任务。在相同的时间背景下，读取该模型预测速率的轻量级线性头比读取原始脉冲计数的相同线性分类器能更好地解码行为。我们在 Steinmetz 视觉辨别基准上进行了测试，结果显示 Mamba 预测的速率对小鼠选择的解码准确率达到 75.7%，约为随机水平的 2.3 倍。整个流水线在工作站级 GPU 上运行时间在 50 毫秒 bin 预算内。
- **PDF**: https://arxiv.org/pdf/2605.12999v1

### SpikeProphecy: A Large-Scale Benchmark for Autoregressive Neural Population Forecasting
- **分数**: 4
- **链接**: https://arxiv.org/abs/2605.12992v1
- **作者**: John R. Minnick, Jinghui Geng, Kamran Hussain, Jesus Gonzalez-Ferrer, Ash Robbins, Mohammed A. Mostajo-Radji, David Haussler, Jason K. Eshraghian, Mircea Teodorescu
- **摘要**: 神经群体模型通常通过预测和实际脉冲计数之间的单一聚合皮尔逊相关系数 $r$ 来评估，但这掩盖了关键结构。我们引入了 SpikeProphecy，这是第一个针对真实电生理记录的因果自回归脉冲计数预测的大规模基准。我们的核心贡献是一个群体指标分解方法，将性能分为时间保真度、空间模式准确性和幅度无关的对齐度。我们将此协议应用于包含约 89,800 个神经元的 105 个 Neuropixels 会话，并对比了 7 种基准架构（包括 SSM、Transformer、LSTM 和脉冲网络）。该基准揭示了跨模型的一致的大脑区域可预测性排名。
- **PDF**: https://arxiv.org/pdf/2605.12992v1

--- 
## 📚 学科: `cs.*`

本周 cs 领域涵盖了计算机视觉、医疗 AI 与通信优化等多个子方向。重点论文包括 CVPR 2026 Oral 入选的 VGGT-Ω，展示了大规模前馈重建模型的卓越扩展性；ICML 2026 的 EviScreen 框架通过引入证据推理提升了疾病筛查的可解释性。此外，还包括应用于 6G 通信优化的 MoE 网络研究。这些研究共同体现了深度学习在处理复杂物理世界任务（如三维重建、医疗诊断和无线资源调度）时的性能提升与解释性增强。

### VGGT-$\Omega$
- **分数**: 4
- **链接**: https://arxiv.org/abs/2605.15195v1
- **作者**: Jianyuan Wang, Minghao Chen, Shangzhan Zhang, Nikita Karaev, Johannes Schönberger, Patrick Labatut, Piotr Bojanowski, David Novotny, Andrea Vedaldi, Christian Rupprecht
- **摘要**: 最近的前馈重建模型（如 VGGT）已证明在竞争传统基于优化的重建器的同时，能提供有用的几何感知特征。我们通过引入 VGGT-$\Omega$ 表明，这些模型的质量会随着模型和数据规模的增加而可预测地扩展，它显著提高了静态和动态场景的重建精度和效率。我们引入了架构改进以提升训练效率，建立支持动态场景的高质量数据标注流水线，并采用自监督学习协议。VGGT-$\Omega$ 的 GPU 显存占用仅为前作的 30%，允许使用 15 倍的监督数据进行训练。在多个基准测试中，该模型表现强劲，例如在 Sintel 上的相机估计精度提高了 77%。
- **PDF**: https://arxiv.org/pdf/2605.15195v1

### Evidential Reasoning Advances Interpretable Real-World Disease Screening
- **分数**: 4
- **链接**: https://arxiv.org/abs/2605.15171v1
- **作者**: Chenyu Lian, Hong-Yu Zhou, Jing Qin
- **摘要**: 疾病筛查在临床实践中的早期发现和及时干预中至关重要。然而，目前的医疗图像筛查模型往往缺乏解释性，且性能尚不理想。为解决这些挑战，我们提出了 EviScreen，这是一个利用历史病例区域级证据的疾病筛查证据推理框架。EviScreen 通过双知识库检索区域证据来提供追溯可解释性。随后的证据感知推理模块结合当前病例和历史证据进行预测，增强了筛查性能。此外，EviScreen 通过对比检索衍生的异常图增强了定位可解释性。实验表明，该方法在多个真实世界疾病筛查基准上达到了优异性能。
- **PDF**: https://arxiv.org/pdf/2605.15171v1

### Deep Mixture of Experts Network for Resource Optimization in Aerial-Terrestrial CF-mMIMO Systems under URLLC
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.15135v1
- **作者**: Donggen Li, Chong Huang, Jingfu Li, Pei Xiao, Wenjiang Feng, Dusit Niyato, Zhu Han
- **摘要**: [注：此篇论文在 eess.* 与 cs.* 重复出现，详见上文翻译。本文提出了一种基于 MoE 的 6G 网络资源优化框架，旨在满足 URLLC 约束下的超可靠低延迟通信需求。]
- **PDF**: https://arxiv.org/pdf/2605.15135v1

--- 
## 📚 学科: `math.*`

本周数学领域（动力系统与控制论方向）主要探讨了非线性动力系统线性嵌入的拓扑障碍。论文证明了对于具有多个 omega 极限集的离散时间系统，无法通过连续的一一映射将其嵌入有限维线性系统，并进一步探讨了 alpha 极限集的推广。该成果为利用线性化工具（如 Koopman 算子理论）分析复杂非线性系统划定了明确的理论边界。

### On the Nonexistence of Continuous Immersions for Discrete-time Systems
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.15161v1
- **作者**: Eron Ristich, Eduardo Sontag, Necmiye Ozay
- **摘要**: [注：此篇论文在 eess.* 与 math.* 重复出现，详见上文翻译。该研究扩展了关于连续时间动力系统线性嵌入不存在性的现有结论，并将其应用到了离散时间动力系统及其极限集特性上。]
- **PDF**: https://arxiv.org/pdf/2605.15161v1

--- 
## 📚 学科: `astro-ph.*`

本周 astro-ph 领域研究覆盖面广，从引力透镜理论到高能天体物理现象均有涉及。重点包括：JWST 在强引力透镜观测中的前沿应用综述；半人马座 A 中新发现的瞬变脉冲超亮 X 射线源（PULX）及其数据处理挑战；利用贝叶斯分层模型优化 KiDS+VIKING-450 宇宙学分析，缓解 $S_8$ 张力；以及磁重联在日球层电流片（HCS）离子加速中作用的模拟研究和恒星形成区电子温度关系的系统性观测。

### Strong Gravitational Lensing with the James Webb Space Telescope
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.15189v1
- **作者**: Adi Zitrin
- **摘要**: 广义相对论预言大质量天体会弯曲时空，使背景光源的光线偏折，即“引力透镜”现象。随着哈勃空间望远镜等设施的出现，透镜已成为现代天文学的主要工具，用于研究星系及星系团中的暗物质分布。强引力透镜效应能放大背景光源，使我们能观察到极遥远、微弱的天体。结合詹姆斯·韦伯空间望远镜 (JWST) 前所未有的性能，引力透镜让我们能以前所未有的深度观测宇宙。本文总结了强透镜应用的最新进展及 JWST 的未来前景。
- **PDF**: https://arxiv.org/pdf/2605.15189v1

### Significant or Not? The Impact of Randomisation During Data Reduction on Confirming a New Pulsating Ultraluminous X-ray Source Candidate in Centaurus A
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.15137v1
- **作者**: Amy H. Knight, Timothy P. Roberts, Callum Potter, Alistair T. Pagan, Dominic J. Walton
- **摘要**: 我们报告了在 NGC 5128 (半人马座 A) 中发现的一个新的候选脉冲超亮 X 射线源 (PULX) 4XMM J132542.2-425943。该源是瞬变的，仅在 2014 年的一次重大爆发期间可见，其 X 射线光谱较软，与典型的硬光谱 PULX 不同。我们对 XMM-Newton 的观测数据进行了搜索，发现了一个频率为 1.27 Hz 的相干正弦脉冲信号，但显著性较低。研究发现，数据缩减过程中的随机化会显著影响边缘信号的强度，可能导致误报或漏报，这在 PULX 搜索中需引起重视。
- **PDF**: https://arxiv.org/pdf/2605.15137v1

### KiDS+VIKING-450 cosmology with Bayesian hierarchical model redshift distributions
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.15078v1
- **作者**: George T. Kyriacou, Arrykrishna Mootoovaloo, Alan F. Heavens, Andrew H. Jaffe, Florent Leclercq, Konrad Kuijken
- **摘要**: 来自测光数据的层析红移分布是宇宙剪切分析的关键。在本文中，我们开发了一个基于模板的贝叶斯分层模型框架，并将其应用于 KiDS+VIKING-450 弱透镜数据。通过边缘化推断出的红移分布，我们发现贝叶斯方法与之前的研究相比增加了聚类参数，从而缓解了与 Planck 卫星观测结果之间的 $S_8$ 张力。在本调查中，与 Planck 的张力从 $2.3\sigma$ 降至 $1.9\sigma$。
- **PDF**: https://arxiv.org/pdf/2605.15078v1

### The Role of Magnetic Reconnection in Energizing Protons and Heavier Ions at the Heliospheric Current Sheet
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.15068v1
- **作者**: Giulia Murtas, Xiaocan Li, Fan Guo, Giuseppe Arrò, Jeongbhin Seo, Colby Haggerty
- **摘要**: 帕克太阳探测器 (PSP) 在日球层电流片 (HCS) 附近观察到了高能质子和重离子群体。我们通过求解耦合到大规模二维 MHD 磁重联模拟的帕克输运方程，研究了 HCS 处的离子加速。研究发现，多种离子形成了幂律分布，其能谱指数和高能截止能量 $E_{\text{max}}$ 与原位观测数据一致。结果进一步证实了磁重联在 HCS 产生高能重离子中的关键作用。
- **PDF**: https://arxiv.org/pdf/2605.15068v1

### The DESIRED electron temperature relations in star-forming regions of the local Universe
- **分数**: 3
- **链接**: https://arxiv.org/abs/2605.15048v1
- **作者**: M. Orte-García, C. Esteban, J. García-Rojas, J. E. Méndez-Delgado, K. Z. Arellano-Córdova, A. Z. Lugo-Aranda, L. Toribio San Cipriano, F. F. Rosales-Ortega, I. R. Martínez-Hernández, E. Reyes-Rodríguez
- **摘要**: 本研究利用 DESIRED 数据库中 699 条银河系和河外 H II 区域及恒星形成星系的光谱，对离子物种间的电子温度 ($T_{\rm e}$) 关系进行了同质性观测研究。我们重新计算了电子密度和温度，并分析了不同诊断指标间的关系。结果显示涉及低电离诊断（如 [O II] 和 [S II]）的关系具有较大的固有分散，而 [N II] 相关关系的分散较小，更具可靠性。这些结果为在诊断指标有限的情况下估计电子温度提供了稳健的经验基础。
- **PDF**: https://arxiv.org/pdf/2605.15048v1

--- 
## 📚 学科: `stat.*`

本周统计学领域（偏向机器学习理论）重点关注协变量偏移下的无监督领域自适应。NeurIPS 2026 投稿论文 TILT 提出了一种创新的损失倾斜机制，它通过在目标域施加惩罚项，隐式地在总体水平上诱导出相对重要性权重，且该权重对于源-目标分布的重合度要求较低。该研究为分布偏移环境下的模型泛化提供了新的损失函数设计思路和理论保障。

### TILT: Target-induced loss tilting under covariate shift
- **分数**: 4
- **链接**: https://arxiv.org/abs/2605.14280v1
- **作者**: Kakei Yamamoto, Martin J. Wainwright
- **摘要**: 我们引入并分析了用于协变量偏移下无监督领域自适应的目标诱导损失倾斜 (TILT) 框架。它基于一种新型目标函数，将源预测器分解为 $f+b$，在带标签的源数据上拟合 $f+b$，同时在无标签的目标输入上惩罚辅助分量 $b$。在总体水平上，这种目标端惩罚隐式诱导了相对重要性权重，即使源-目标对的支撑集不相交，该权重依然一致有界。我们证明了超额风险的泛化 oracle 不等式，并提供了稀疏 ReLU 网络训练的端到端保证。实验显示 TILT 在多个回归和分类任务中均优于传统的密度比估计基准。
- **PDF**: https://arxiv.org/pdf/2605.14280v1

--- 
## 📚 学科: `econ.*`
_本周缺少高价值论文_