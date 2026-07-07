# 🗓️ 周报 (2026-W27)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-07-05

--- 
## 📚 学科: `eess.*`
### Cross Domain Few-Shot Class-Incremental Audio Classification Via Adversarial Contrastive Learning
- **分数**: 4
- **链接**  https://arxiv.org/abs/2607.02254v1
- **作者**: Yongjie Si, Yanxiong Li, Sen Huang, Beibei Liu
- **备注**: 5 pages, 3 figures, 4 tables, accepted for publication in Interspeech 2026
- **摘要**: 当前的少样本类增量音频分类（FCAC）方法假设基类和增量类的样本处于同一领域（遵循相同的分布）。然而，上述两类样本之间通常存在领域偏移。在本文中，我们探索了基类和增量类样本存在领域偏移的跨领域 FCAC 问题。我们提出了一种对抗对比训练策略，使模型能够有效地对来自未见领域的不同类别的样本进行分类。该模型由一个编码器和一个分类器组成。编码器在基阶段进行训练，但在增量阶段被冻结，而分类器在所有阶段都进行训练。在六对跨领域数据集上进行了实验。结果表明，我们的方法在平均准确率上超过了最先进的方法。代码位于 https://github.com/YongjieSi/ACL 。
- **PDF**: https://arxiv.org/pdf/2607.02254v1

### QuadRocket: An Aerial Robotic Testbed for Adaptive Thrust-Vector Control of Rocket-Like Vehicles
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.02474v1
- **作者**: Pedro Santos, Joel Reis, Paulo Oliveira, Carlos Silvestre
- **备注**: Paper accepted for publication in IEEE Transactions on Aerospace and Electronic Systems
- **摘要**: 本文介绍了 QuadRocket，这是一个基于四旋翼的火箭原型，为验证类运载火箭系统的先进推力矢量控制策略提供了一个低成本、低风险的平台。该原型由一个通过万向节安装在四旋翼顶部的圆柱形主体组成，形成了一个具有不可忽略惯性的飞行倒立摆。在控制设计中，耦合系统被建模为单个轴对称刚体，由沿其纵轴施加的矢量力驱动。采用二维球面上的缩减姿态表示，以显式利用车辆的轴向对称性，并将偏航角与推力矢量方向解耦。在此模型上，我们推导出了一个自适应反步控制器，在存在未知恒定干扰的情况下实现几乎全局的轨迹跟踪，同时控制点变换减轻了非最小相位行为。然后将四旋翼视为推力矢量执行器，并设计了基于动态表面的姿态控制器来跟踪所需的推力矢量，同时考虑了执行器动力学并避免了虚拟控制信号的显式微分。整个架构在仿真中进行了评估，并在室内动作捕捉场地进行了实验验证。结果表明，该系统具有精确的轨迹跟踪和有效的干扰补偿能力，并证实了 QuadRocket 作为推力矢量控制机器人车辆多功能测试平台的适用性。
- **PDF**: https://arxiv.org/pdf/2607.02474v1

### Audio-Based Understanding of Audiobook Narration Appeal
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.02473v1
- **作者**: Shahar Elisha, Mariano Beguerisse-Díaz, Emmanouil Benetos
- **备注**: Accepted to Interspeech 2026
- **摘要**: 朗读是听书体验的核心，塑造了听众如何与内容产生共鸣和理解。本研究探讨了朗读特质如何影响有声书的吸引力，并指出其效果因流派、书名和受众而异。我们使用预训练的音频模型从 LibriVox 中提取人声和声学特征（例如音调、语速、响度），并分析它们与消费数据（具体为收视率/收听率）的关系以及它们与流派和书名的相互作用。尽管消费数据有限，我们发现即使在考虑了书名效应之后，仅声学信息就与吸引力存在强大的关联。我们使用更细致的专有参与度指标进一步验证了这些发现。据我们所知，这是首个将朗读质量、流派、书名和有声书消费联系起来的系统性计算研究，突显了数据驱动的洞察力在改善有声书个性化和朗读者选角方面的潜力。
- **PDF**: https://arxiv.org/pdf/2607.02473v1

### Fourier Preconditioning for Neural Feature Learning
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.02199v1
- **作者**: Preston Pitzer, Anish Pradhan, Harpreet S. Dhillon
- **备注**: Accepted for publication in IEEE Signal Processing Letters
- **摘要**: 受互信息（MI）启发的特征学习技术能够生成保留非线性依赖结构的低维嵌入，但直接估计互信息在低数据机制下会受到噪声概率分布估计的影响。基于二阶统计量计算的 H-Score 指标为训练特征提取网络提供了一个实用的代理度量。我们证明了 H-Score 在无约束函数设置下对可逆变换具有不变性，但在受约束的逼近类下对输入基旋转变得敏感。因此，我们研究了 H-Score 网络的酉预处理，并表明选择合适的基旋转可以通过将预测依赖性集中到更少的优势模式中来减少有限宽度截断误差。我们确定快速傅里叶变换（FFT）是近似平稳过程的一种有效的、独立于数据的、低成本的预处理方法，其中谱结构诱导了互协方差奇异值谱的集中。我们引入了基于谱熵和累积依赖能量的免训练指标，以量化基的适用性并在网络训练之前预测下游推理收益。在八个多变量数据集上的实验表明，FFT 预处理在资源受限的环境中特别有用，实现了高达 50% 的归一化均方误差（NMSE）降低，而所提出的指标与观察到的性能提升相关，并正确识别了谱预处理不利的情况。
- **PDF**: https://arxiv.org/pdf/2607.02199v1

### LMPAN: A Lightweight Multi-Path Alignment Network for Joint Full-Duplex Acoustic Echo Cancellation and Noise Suppression
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.02062v1
- **作者**: Chengwei Liu, Shaofei Xue, Haoyin Yan, Xiaotao Liang, Zheng Xue
- **备注**: Accepted by Interspeech 2026
- **摘要**: 我们提出了一种轻量级多路径对齐网络（LMPAN），用于全双工语音对话系统中的设备端联合回声消除（AEC）和噪声抑制（NS）。为了解决硬件引起的失真和动态声学环境，我们引入了三个核心创新：（1）多路径对齐阶段，用于纠正参考信号、线性 AEC（LAEC）输出和麦克风信号之间的时间和能量失配；（2）基于注意力机制的动态融合方法，在变化的声学场景下动态融合增强的 LAEC 和麦克风特征；（3）具有下游任务（ASR、VAD）动态目标生成策略的后滤波模块。此外，我们采用了一个利用自监督学习表征的两阶段训练框架，以提高感知质量。实验表明，LMPAN 仅包含 480K 参数和 126 MACs，实现了与最先进的轻量级模型 DeepVQE-S 相当的性能，同时确保了实时推理能力。
- **PDF**: https://arxiv.org/pdf/2607.02062v1

#### 学科总结 (`eess.*`)
本期选录的 `eess.*` 学科论文共 5 篇，主要涵盖音频处理、机器人控制和统计特征学习等领域。研究涉及：基于对抗对比学习解决少样本类增量音频分类中的领域偏移；利用四旋翼无人机设计低成本火箭原型测试平台（QuadRocket），并实现自适应推力矢量控制；采用自监督音频模型分析有声书声学特征与听众吸引力之间的系统性关联；提出一种通用的傅里叶预处理（FFT）方法以显著提升受约束 H-Score 网络特征提取的精度；以及针对移动设备设计的超轻量级多路径对齐网络（LMPAN），在回声消除和噪声抑制任务中实现了兼顾实时性与感知质量的突破。

--- 
## 📚 学科: `q-bio.*`
### Affinage: genome-scale mechanistic gene annotation from the published literature
- **分数**: 6
- **链接**  https://arxiv.org/abs/2607.02217v1
- **作者**: Matteo Di Bernardo, Iain M. Cheeseman
- **备注**: 12 pages, 6 figures. Accepted to the Workshop on Generative and Agentic AI for Biology at ICML 2026
- **摘要**: 理解基因的机制功能是生物学的关键起点。然而，对于人类蛋白质组的大部分，这些知识散落在数以千计的原始论文中，或者仍未确立，而生物学家依赖的策划数据库可能会落后于最新文献数年。大语言模型现在可以根据需要阅读和合成这些文献，但对许多基因忠实地进行这一过程是一项昂贵、不可重复的检索过程，且无法在用户间扩展。在这里，我们介绍了 Affinage，一个 LLM 管道，它仅从原始文献中针对每个基因执行一次检索和机制推理，并将结果存储为可重用的结构化注释。由生物学家设计的阅读步骤仅提取直接的实验证据，而合成步骤仅对这些发现进行推理。应用于整个基因组，Affinage 注释了 19,293 个编码人类蛋白质的基因。该分析为数千个在 UniProt 中功能为空白或仅有存根（stub）的基因提供了机制解释，在一项由跨家族 LLM 评委评分的直接对比中，其表现优于精心策划的参考库，在 99.1% 的基因上胜出。Affinage 还描绘了蛋白质组中仍未有机制表征的 10% 的部分，并将作为一个持续更新、立足于文献的基因功能普查工具。所有记录均在 https://affinage.wi.mit.edu 公开释放。更广泛地说，Affinage 展示了领域专家如何将其专业知识编码到可扩展的 LLM 管道中，以改善指导生物学假设和实验的公开可用数据。
- **PDF**: https://arxiv.org/pdf/2607.02217v1

### SF-Cluster: Frustration-Guided MSA Subsampling for Alternative Protein Conformation Recovery
- **分数**: 6
- **链接**  https://arxiv.org/abs/2607.00180v1
- **作者**: Hanqun Cao, Zijun Gao, Chunbin Gu, Ge Liu, Pheng Ann Heng, Pranam Chatterjee
- **备注**: Accepted at the AI4Science Workshop at ICML 2026 (Oral)
- **摘要**: 深度学习结构预测器对其多序列比对（MSA）输入高度敏感，这使得 MSA 子采样成为恢复交替构象的实用途径。现有方法（如 AF-Cluster）在序列空间中运行，对采样哪个构象盆地的控制有限。我们引入了 SF-Cluster，它利用预测的局部能量挫折（energetic frustration）模式对 MSA 进行子采样，这是一种在很大程度上独立于序列相似性的表征。在跨越折叠切换、变构、寡聚化偶联和内在无序系统的 48 个案例的基准测试中，并使用 AF-Cluster 风格的双参考 RMSD 标准，SF-Cluster 在双状态类别中提高了交替构象的目标状态恢复率，其中在变构系统上观察到的改进最大（提高了 15.5 个百分点）。所选的 MSA 可以转移到架构不同的预测器上，表明构象信号存在于 MSA 组成中。从机制上讲，匹配深度的对照表明，这种恢复优势主要归因于所选子集的有效深度，而挫折模式选择可靠地达到了这一深度。同时，高度受挫的残基在深度突变扫描和 NMR 双状态交换支持的位点富集，并且挫折协变在状态转换接触处富集，同时保持与协同进化耦合的区别。总之，这些结果将挫折模式确定为构象预测的可转移表征，并将 MSA 子采样定位为表征引导的重加权问题。
- **PDF**: https://arxiv.org/pdf/2607.00180v1

### MERLIN-SUITE: Probabilistic modular GRN inference from multi-omics data integrating regulatory priors and transcription factor activity
- **分数**: 4
- **链接**  https://arxiv.org/abs/2607.01791v1
- **作者**: Suvojit Hazra, Marina Kotvanova, Kirstan Gimse, Sushmita Roy
- **备注**: 27 pages, 7 figures, This book chapter is scheduled to appear in the lab protocol series Methods in Molecular Biology
- **摘要**: 准确重建基因调控网络（GRNs）对于理解发育和疾病中的转录过程至关重要。MERLIN-SUITE（https://github.com/Roy-lab/MERLIN-SUITE）代表了一系列基于 MERLIN（利用单基因信息进行模块化调控网络学习）的算法扩展，MERLIN 是一个概率框架，它推断共调控模块的基因特异性和模块特异性调控程序，捕捉转录网络的详细和模块化特征。虽然基于表达的推理是有效的，但它往往与实验验证的调控相互作用不一致。MERLIN-P 通过整合外部调控先验（如基序、ChIP 和微扰数据）来解决这一问题，从而提高生物学相关性和预测准确性。MERLIN-P-TFA 通过引入潜在转录因子活性（TFA）的正则化估计进一步推进了该框架，克服了 TF mRNA 水平可能无法代表蛋白质活性的局限性。通过整合表达数据、先验知识和活性感知建模，这种统一的方法支持在体（bulk）和单细胞数据集中进行鲁棒的 GRN 重建。本章介绍了 MERLIN-SUITE，重点是 MERLIN-P-TFA，并展示了其在小鼠细胞重编程的单细胞、多模态数据集上的应用，以推断 GRN 并识别关键调控因子。
- **PDF**: https://arxiv.org/pdf/2607.01791v1

### scMTNI: Leveraging cellular trajectory and context to infer dynamic GRNs from single-cell multi-omics data
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.01508v1
- **作者**: Suvojit Hazra, Chandrani Kumari, Sushmita Roy
- **备注**: 24 pages, 5 figures, This book chapter is scheduled to appear in the lab protocol series Methods in Molecular Biology
- **摘要**: 转录基因调控网络（GRNs）描述了调控因子与靶基因之间的定向关系，以细胞类型特异性的方式决定基因表达模式。单细胞多组学技术，如单细胞 RNA 测序（scRNA-seq）和单细胞转座酶可接近染色质测序（scATAC-seq），能够以前所未有的高分辨率测量细胞类型特异性的基因表达和调控。然而，用于推断细胞类型特异性 GRN 并建模其动态变化的工具仍然匮乏。为了促进在细胞发育或疾病进展等需要考虑细胞谱系结构和动力学的背景下推断和分析细胞类型特异性 GRN，我们开发了一个多任务学习框架：单细胞多任务网络推理（scMTNI）。scMTNI 及其相关的网络分析工具提供了一个全面的方案来定义细胞类型特异性的 GRN 并研究其动态。本章介绍了 scMTNI 工具，并展示了其在现有的细胞重编程单细胞多模态数据集上的应用，以推断细胞类型特异性 GRN 并识别细胞重编程过程中细胞命运转变的关键调控因子。
- **PDF**: https://arxiv.org/pdf/2607.01508v1

#### 学科总结 (`q-bio.*`)
本期选录的 `q-bio.*`（定量生物学）学科论文共 4 篇，紧扣 AI 在生物信息学中的应用这一前沿方向。研究包含：利用 LLM 检索原始文献并完成全基因组规模人类机制性基因注释的 Affinage 系统；通过局部能量挫折模式指导 MSA 抽样、大幅提高蛋白质替代构象预测精度的 SF-Cluster 模型；以及两种用于单细胞多组学数据重建基因调控网络（GRN）的先进概率计算框架，分别是集成转录因子活性的 MERLIN-SUITE 和融合细胞轨迹信息的 scMTNI。

--- 
## 📚 学科: `cs.*`
### Reasoning LLM Improves Speaker Recognition in Long-form TV Dramas
- **分数**: 7
- **链接**  https://arxiv.org/abs/2607.02504v1
- **作者**: Yuxuan Li, Lingxi Xie, Xinyue Huo, Jihao Qiu, Jiacheng Shao, Pengfei Chen, Jiannan Ge, Kaiwen Duan, Qi Tian
- **备注**: Accepted to ICML 2026
- **摘要**: 长篇电视剧对全面的视频理解提出了严峻的挑战，其中解读复杂的故事情节往往依赖于**说话人识别**，即准确将每一句口头表达归因于其相应角色的任务。在本文中，我们通过两项主要贡献推进了该领域的研究。（1）我们引入了 **DramaSR-532K**，这是一个大规模基准数据集，包含超过 900 个独特角色的 53.2 万条标注对话行，需要集成听觉、语言和视觉线索进行说话人识别。（2）我们提出了 **DramaSR-LRM**，这是一种基于大推理模型（LRM）的鲁棒方法。DramaSR-LRM 旨在通过多模态工具调用自动聚合上下文证据，合成各种输入以实现高保真度的角色归属。实验结果表明，DramaSR-LRM 显著优于现有基线方法，特别是在声学特征本身不可靠的短语音上。所有数据和代码将在项目页面公开：https://www.github.com/198808xc/DramaSR-LRM 。
- **PDF**: https://arxiv.org/pdf/2607.02504v1

### Learning to Move Before Learning to Do: Task-Agnostic pretraining for VLAs
- **分数**: 6
- **链接**  https://arxiv.org/abs/2607.02466v1
- **作者**: Junhao Shi, Siyin Wang, Xiaopeng Yu, Li Ji, Jingjing Gong, Xipeng Qiu
- **备注**: Accepted to ICML 2026, 21 pages,6 figures
- **摘要**: 视觉-语言-动作（VLA）模型从根本上受到专家演示（即观察、指令和动作三元组）稀缺性的瓶颈限制，因为大规模收集这些数据的成本极高。我们认为，这一瓶颈源于将两个截然不同的学习目标混为一谈：获取物理能力（如何移动）和获取语义对齐（做什么）。至关重要的是，只有后者才需要语言监督。基于这一“分解假设”，我们提出了任务无关预训练（TAP），这是一个两阶段框架。该框架首先通过自监督的逆动力学目标，从廉价、无标注的交互数据（包括丢弃的非任务轨迹和自主机器人探索）中学习可迁移的运动先验。随后，在轻量级的第二阶段中，使用极少的专家数据将这些先验与语言进行对齐。在 SIMPLER 基准测试中，TAP 仅使用少几个数量级的标注数据，就能达到在超过 100 万条专家轨迹上训练的模型的水平，在标准行为克隆上实现了 10% 的绝对提升。在真实的 WidowX 平台上，在互联网规模的基准模型由于摄像头扰动而崩溃至 0% 的情况下，TAP 仍能保持 25% 的成功率，这表明任务无关预训练产生了解耦、可迁移的物理表征，并为具身智能提供了一条可扩展的进路。
- **PDF**: https://arxiv.org/pdf/2607.02466v1

### Language Models as Measurement Apparatus for Culture
- **分数**: 6
- **链接**  https://arxiv.org/abs/2607.02459v1
- **作者**: Kent K. Chang
- **备注**: Accepted to the Big Picture workshop co-located with ACL 2026. This version expands the camera-ready (adding Fig. 3 and section 6.3, as well as correcting minor typos) in Proceedings of The Big Picture v2: Crafting a Research Narrative, pp. 131--143, San Diego, CA, USA. Association for Computational Linguistics
- **摘要**: 语言模型越来越多地被用于量化文化现象，但究竟是什么使得这种测量具有独特的文化性？本文认为，NLP 在文化方面的研究是一种物质-话语实践：测量仪器——包括模型、数据、标注、评估——参与了它所测量的文化现实的建构，而不是被动地记录它。借鉴凯伦·巴拉德（Karen Barad）关于“能动性划分”（agential cut）的概念——即现象与仪器之间的权宜边界——我表明，仪器的实质性设计选择画出了这样的边界，并且该边界从一开始就纠缠在一起，因为语言模型已经内化了它们所测量的大部分文化材料。我通过三个关于电视和电影对话的案例研究（测量结构、互动和偏离）以及对仪器本身的三个检验（文化标记的抹去、对历史材料的调谐以及在能动工作流中的能动性）来说明这一点。这一宏观分析提出了一个理论驱动、实证严谨且带有文化权宜性的研究计划，将每一次能动性划分都视为一次自觉的承诺，既是方法论上的，也是伦理上的。
- **PDF**: https://arxiv.org/pdf/2607.02459v1

### Understanding the Robustness of Distributed Self-Supervised Learning Frameworks Against Non-IID Data
- **分数**: 5
- **链接**  https://arxiv.org/abs/2607.02447v1
- **作者**: Xuanyu Chen, Nan Yang, Shuai Wang, Dong Yuan
- **备注**: Accepted at ICLR2026
- **摘要**: 最近的研究引入了分布式自监督学习（D-SSL）方法，以利用海量的无标记去中心化数据。然而，D-SSL 面临着数据异构性的关键挑战，且目前对于不同 D-SSL 框架如何应对这一挑战的理论理解十分有限。为了填补这一空白，我们对非独立同分布（non-IID）设置下 D-SSL 框架的鲁棒性进行了严格的理论分析。我们的结果表明，使用掩码图像建模（MIM）进行预训练天然比对比学习（CL）对异构数据更具鲁棒性，并且去中心化 SSL 的鲁棒性随着平均网络连通性的增加而提高，这意味着联邦学习（FL）的鲁棒性不亚于去中心化学习（DecL）。这些发现为指导未来 D-SSL 算法的设计提供了坚实的理论基础。为了进一步说明我们理论的实际应用，我们引入了 MAR 损失，这是对具有局部到全局对齐正则化的 MIM 目标的改进。在不同模型架构和分布式设置下的广泛实验验证了我们的理论见解，并进一步证实了 MAR 损失作为我们分析应用的效果。
- **PDF**: https://arxiv.org/pdf/2607.02447v1

### PointDiT: Pixel-Space Diffusion for Monocular Geometry Estimation
- **分数**: 4
- **链接**  https://arxiv.org/abs/2607.02515v1
- **作者**: Haofei Xu, Rundi Wu, Philipp Henzler, Nikolai Kalischek, Michael Oechsle, Fabian Manhardt, Marc Pollefeys, Andreas Geiger, Federico Tombari, Michael Niemeyer
- **备注**: ICML 2026. Project page: https://haofeixu.github.io/pointdit/
- **摘要**: 最先进的单张图像 3D 重建方法通常依赖于复杂的混合架构和损失函数，或者将几何压缩到潜在空间中以利用预训练的潜在扩散模型。在这项工作中，我们展示了这种架构开销和复杂的损失公式是不必要的。我们引入了一种简约的像素空间扩散 Transformer（PointDiT），它构建在普通的 ViT 之上，直接在原始 3D 点图斑块上运行，并以来自预训练 DINOv3 的图像标记为条件。与现有的潜在扩散方法不同，我们完全从头开始训练我们的扩散骨干，消除了对点图分词器的需求。尽管设计简单，我们的方法超越了复杂的基于潜在空间的扩散模型，同时比混合替代方案显著更简单。值得注意的是，它能产生更锐利的几何结构，并且在高度模糊的区域（如透明物体）中更加鲁棒。
- **PDF**: https://arxiv.org/pdf/2607.02515v1

#### 学科总结 (`cs.*`)
本期选录的 `cs.*` 学科均为发表在 ICML、ICLR、ACL 等计算机顶会和研讨会的高质量研究成果。研究覆盖面极广：多模态推理模型 DramaSR-LRM 通过海量对话数据大幅提升了电视剧长视频中的角色说话人归属精度；具身智能模型 TAP 引入“任务无关预训练”概念，将物理运动能力和语义对齐学习解耦，利用无标数据构建强大的机器人运动先验；探讨了大语言模型作为文化量化工具时的设计边界与伦理反思；提供了分布式自监督学习在非同分布（non-IID）数据下理论鲁棒性的严格分析并提出改进的 MAR 损失；此外，PointDiT 设计了一种直接在像素空间 3D 点图斑块上运行的扩散 Transformer 模型，为单图 3D 重建提供了一种高精度且极简的骨干选择。

--- 
## 📚 学科: `math.*`
_本周在该学科下未筛选出符合学术质量要求的推荐论文。_

--- 
## 📚 学科: `astro-ph.*`
### The Road to Identifying the Earliest Radio-Powerful AGN with the SKA
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.02366v1
- **作者**: Jose Afonso, Stergios Amarantidis, Stas Shabala, Ross J. Turner, Luca Ighina, Mojtaba Raouf, Nuno Covas, Pedro Martins, Nick Seymour, Alessandro Caccianiga, Alexander Hedge, Jess W. Broderick, Davi Barbosa, Isabella Prandoni, Sabyasachi Pal, Bruno Arsioli, Luis Barroso, Rodrigo Carvajal, João Tiago, Andrew Hopkins, Manuela Magliocchetti, Israel Matute, Ciro Pappalardo
- **备注**: Published in Advancing Astrophysics with the SKA II (AASKAII), 2026 (arXiv:2606.20366). Report-no:AASKAII/Afonso01. Advancing Astrophysics with the SKA II (AASKAII) outlines the transformative scientific advances that will be enabled by the SKA telescopes
- **摘要**: 再电离时代（EoR）是现代天体物理学最关键的前沿之一，标志着第一批星系、恒星和超重质量黑洞（SMBH）的出现。尽管有来自阿塔卡马大型毫米/亚毫米阵列和詹姆斯·韦伯空间望远镜的见解，我们仍然难以解释为什么在 $z\sim7$ 时就已经存在驱动发光活动星系核（AGN）的 $\sim10^{9}$ M$_\odot$ SMBH。最近在一些早期 AGN 中发现的强射电辐射是令人瞩目的，它为早期黑洞吸积提供了新的约束，并且随着平方千米阵列天文台（SKAO）的建立，有望通过 21 厘米吸收研究直接探测中性氢。然而，研究进展依然缓慢：在 $z>6$ 处仅已知少数几个强射电 AGN，远低于理论预测，这引发了关于这是反映了其内在属性还是选择效应及不完整光谱信息的问题。在本章中，我们综合了最先进的流体动力学和半解析模拟的预测，以及来自 SKAO 先导设施的观测约束。这些模型表明，在再电离时代存在大量、尚未被探测到的强射电 AGN 群，但同时也表明目前的巡天受到选择偏误和不完整射电光谱信息的限制。我们讨论了一种基于宽带射电能谱分布、光谱弯曲、动力学喷流演化以及仅射电红移估计来识别高红移射电 AGN 的物理驱动策略，为传统的经验方法提供了一种具有变革性的替代方案。最后，我们论证了 SKAO 的灵敏度和光谱覆盖范围将如何允许在 50 MHz - 15 GHz 范围内进行精细频率采样，从而彻底改变我们识别最早强射电 AGN 和探测最早 SMBH 的能力。
- **PDF**: https://arxiv.org/pdf/2607.02366v1

### Tracing grain growth in the forming prestellar core L1506C with 3D modeling of Herschel, IRAM, and CFHT observations
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.02353v1
- **作者**: E. Zhu, I. Ristorcelli, K. Demyk, M. Juvela, N. Ysard, D. Paradis, H. Roussel, W. Kiviaho
- **备注**: 21 pages, accepted for publication in A&A
- **摘要**: 在恒星形成的早期阶段，原恒星核的性质通常是从热尘埃辐射的观测中推断出来的，因此取决于尘埃的性质，这些性质必须经过仔细表征。我们的目标天体 L1506C 是金牛座分子云中 L1506 纤维状结构的一部分。利用 Herschel PACS、SPIRE 以及 IRAM-NIKA2 的数据，构建了覆盖整个光谱范围（从 160 μm 到 2 mm）的能量分布（SED），并使用修改后的黑体（MBB）进行了拟合。这些数据还使用了 3D 辐射转移代码 SOC 和最新的 THEMIS 2 尘埃模型进行建模，并利用来自 CFHT 上的 WIRCam 和 Spitzer 的消光观测作为附加约束。MBB 建模表明 L1506C 分裂成两个质量小于其金斯质量的低密度核。尘埃色温和发射率光谱指数表现出明显的反相关性，并伴随着尘粒性质的变化。为了对最致密的部分进行建模，需要比弥散星际介质更演化的尘粒，这表明在恒星形成的极早期阶段（甚至在重力塌缩开始之前），尘埃颗粒的生长就已经发生了。
- **PDF**: https://arxiv.org/pdf/2607.02353v1

### Indicatives of Early Stages of Star Formation in the Universe
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.02351v1
- **作者**: Irina Acharova, Margarita Sharina
- **备注**: 13 pages, 4 figures, published in Astrofizicheskii Byulleten
- **摘要**: 本文分析了环星系云中球状星团（GC）的形成条件。详细证实了邻近宇宙中球状星团与红移在 0.2 到 5.9 之间的环星系云在金属丰度分布上的相似性。环星系云和球状星团数量的分布在金属丰度值 $[\rm{X/H}]\simeq -2.6, -2.0, -1.4,-0.5$ 处均包含四个局部极大值的序列。计算了质量为 $10^{8}\,M_{\odot}$ 的环星系云从极低金属丰度 $ [\rm{X/H}] <-2.3$ 开始，接着经历 $-2.3 \le [\rm{X/H}]<-1.7$ 和 $-1.7 \le [\rm{X/H}] < -0.9$ 阶段，最终达到高金属丰度 $[\rm{X/H}] \ge -0.9$ 的序列富集过程，其中这些区间的边界与分布中天体数量的局部极小值相一致。结果表明，为了重现此类分布，只需在云的一部分被金属富集的每个阶段，形成一个或多个总质量为 $3 \times 10^{6}\,M_{\odot}$ 的球状星团即可。研究表明，能够引发超新星爆发的恒星的最大质量会随着金属丰度的增加而增加。针对对应于星系云和球状星团分布极大值的金属丰度，计算了该质量的可能数值。
- **PDF**: https://arxiv.org/pdf/2607.02351v1

### Analyses on Christoph Clavius' Reports of Total Solar Eclipses in 1560 and 1567: Key References for the Centennial Variations of the Earth's Rotation Speed and the Solar Radius
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.02347v1
- **作者**: Hisashi Hayakawa, Mitsuru Sôma, Jean-Pierre Rozelot, Koji Murata, Alexei A. Pevtsov, Stanislav Gunár, Lucie M. Green
- **备注**: 20 pages, 5 figures, and accepted for publications in the Astrophysical Journal Letters
- **摘要**: 太阳半径（以下简称 R_Sun）的变化是太阳磁活动随时间演变的关键参考。过去的太阳辐射量可能随着 R_Sun 的变化而变化，并对地球的气候产生过影响。在现代直接观测之前，日食观测提供了测量绝对 R_Sun 值的独特机会。科学界讨论了自 1715 年起可能存在的长期 R_Sun 变率。在此覆盖范围之前，克拉维斯（Clavius）的日食报告曾引发关于局部日食可见度以及可能存在的长期 R_Sun 趋势的定性争论。本研究利用近期月球地形数据和历表数据的巨大进展，为解决这一争论提供了有效的方案。克拉维斯的日食报告描述了 1560 年在科英布拉（Coimbra）发生的显式全食，以及 1567 年在罗马发生的遮掩月球周围的“细环”。在考虑月球边缘轮廓并假设 Auwers 的经典 R_Sun 的情况下，我们的研究修正了 1560 年的 ΔT 约束（-492 s =< ΔT =< 200 s）和 1567 年的 ΔT 约束（140 s =< ΔT =< 151 s），以符合克拉维斯的描述。本研究利用三种方案来解释克拉维斯的记述，约束了 1567 年的 R_Sun 范围。局部全食要求 1567 年的 R_Sun 上限在绝对尺寸上为 R_Sun =< 696200 km（角尺寸为 959.92"），这表明不存在线性的长期 R_Sun 收缩，但在百年尺度上可能存在 R_Sun 振荡。相反，环食方案被认为是不大可能的，因为它需要 R_Sun 在 3 个世纪内减少 7.5"，这甚至超出了极端“太阳收缩”假说的能力范围。
- **PDF**: https://arxiv.org/pdf/2607.02347v1

### The VLA-COSMOS 3 GHz Large Project: Polarised source counts and catalogue
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.02342v1
- **作者**: S. Ranchod, S. A. Mao, R. P. Deane, V. Smolčić, J. D. Wagenveld, M. Bondi, K. Mooley, E. Schinnerer
- **备注**: 13 pages, 10 figures (main text). Accepted for publication in Astronomy and Astrophysics (A&A)
- **摘要**: 探测微弱偏振射电源群体对于解释星系中磁场的性质 and 演化至关重要。虽然最近的研究为 1.4 GHz 下的微央级（$μ$Jy）偏振源数量提供了深入见解，但更高频率的巡天可能对由于内部或外部退偏振效应而在较低频率下发生退偏振的新源群体更加敏感。我们展示了迄今为止在 3 GHz 下最深的偏振源计数，其角分辨率为 $1.5''$。通过这些相对较高频率的观测，我们旨在探测微弱的偏振星暴星系（SFG）群体。此外，通过光谱建模，我们旨在为偏振源计数随频率演化提供进一步的见解。我们处理了 VLA-COSMOS 3 GHz 大型项目的偏振数据，该项目是最深的高分辨率射电连续谱巡天之一。我们制作了 Stokes Q 和 U 拼接通道图。在选择全强度下的已知源后，我们执行了 3D 旋转测度合成，并使用经验确定的阈值搜索偏振辐射。在法拉第深度灵敏度为 2.6 $μ$Jy/beam 时，我们在阈值以上检测到了 65 个偏振源（51 deg$^{-2}$）。我们发现，我们在 3 GHz 下的累积和欧几里得归一化源计数与文献中 1.4 GHz 的结果一致，我们将其归因于所探测源的光谱指数和退偏振的结合效应。我们在样本中没有检测到恒星形成星系（SFGs），并导出了偏振 SFG 密度的 2$σ$ 上限为 $<2.0~\mathrm{deg}^{-2}$。这意味着在 SKA 时代，要想轻易检测到这一群体，将需要更深得多的观测。
- **PDF**: https://arxiv.org/pdf/2607.02342v1

#### 学科总结 (`astro-ph.*`)
本期精选的 `astro-ph.*` 学科论文共 5 篇，展现了对观测、数值模拟以及历史文献在天物理学交叉应用的多维度解析。研究包含：综合半解析和流体模型探索如何通过 SKAO 检测高红移超大质量黑洞驱动的早期射电 AGN；利用 3D 辐射转移对原恒星核 L1506C 进行建模并追溯尘粒在塌缩前的极早期生长机制；研究早期宇宙中环星系云金属丰度演化与球状星团形成的关系；借助最新高精度月球地形与历表数据重新校准 16 世纪 Clavius 的日食报告以约束百年尺度太阳半径波动和地球自转偏角；以及基于 VLA-COSMOS 3 GHz 的微弱射电偏振源计数与分类，为 SKA 时代探测星系磁场和微弱恒星形成星系奠定了基础。

--- 
## 📚 学科: `stat.*`
### Online Safety Monitoring for LLMs
- **分数**: 4
- **链接**  https://arxiv.org/abs/2607.02510v1
- **作者**: Mona Schirmer, Metod Jazbec, Alexander Timans, Christian Naesseth, Maja Waldron, Eric Nalisnick
- **备注**: ICML 2026 Hypothesis Testing Workshop
- **摘要**: 尽管进行了对齐训练，大语言模型在部署时仍容易生成不安全的内容。因此，实时在线监控输出并在无法保证安全时发出警报至关重要。我们研究了一种简单的实时监控器，它通过阈值化将来自外部模型的验证信号转化为警报决策，并通过风险控制来校准该阈值。在数学推理和红队数据测试集的实验中，我们表明这种简单设计与基于序列假设检验的更高级监控器相比具有很强的竞争力。
- **PDF**: https://arxiv.org/pdf/2607.02510v1

#### 学科总结 (`stat.*`)
本期选录的 `stat.*` 学科论文专注于大语言模型（LLM）的实时安全监控。通过巧妙融合统计学中的风险控制原理，研究人员开发了一种高效便捷的在线监测机制。该方法通过引入外部模型的验证信号并对自适应校准的阈值进行硬分割，在部署阶段实现实时异常预警。研究证实该轻量化策略在面对逻辑推理和对抗红队测试等高风险场景时，能取得与高度复杂的序列假设检验相媲美的表现，推动了统计边界控制在 AI 安全对齐领域中的落地。

--- 
## 📚 学科: `econ.*`
### Estimating Supply Incrementality in Two-sided Marketplaces: A Causal Machine Learning Approach
- **分数**: 6
- **链接**  https://arxiv.org/abs/2606.30999v1
- **作者**: Yufei Wu, Daniel Schmierer, Dan Zylberglejd
- **备注**: 5 pages, 3 figures. Accepted at the KDD 2025 Workshop on Causal Inference and Machine Learning in Practice (not presented)
- **摘要**: 在具有异构产品的双边市场中，了解额外供应与市场产出（例如市场中的总交易量或交易价值）之间的因果关系至关重要。本文研究了一种用于估计跨产品细分市场的这种因果关系的因果机器学习方法。我们以 Airbnb 市场为例，重点关注额外房源供应对总预订量的影响，但该方法同样适用于其他双边市场。我们的方法将双重/去偏机器学习与利用预先存在的知识作为先验的层次贝叶斯框架相结合。我们利用地理空间文献中产品细分相似性的度量，为模型构建了易于处理且具有信息量的特征。我们发现，这样的模型能够对额外供应带来的市场回报提供合理的估计，并具有很强的样本外表现。
- **PDF**: https://arxiv.org/pdf/2606.30999v1

### Understanding Guest Preferences and Optimizing Two-sided Marketplaces: Airbnb as an Example
- **分数**: 4
- **链接**  https://arxiv.org/abs/2607.00280v1
- **作者**: Yufei Wu, Daniel Schmierer
- **备注**: 5 pages, 3 figures. Presented at the KDD 2024 Workshop on Two-Sided Marketplace Optimization, Barcelona, Spain
- **摘要**: Airbnb 是一个基于连接和归属感的社区——Airbnb 上的许多房东都是普通人，他们分享自己的世界，为房客提供连接和宾至如归的感觉；Airbnb 致力于连接人和地方。在我们连接房客和房东的努力中，我们提供工具使房东能够制定具有竞争力的价格，这有助于提高房客的负担能力，同时帮助房东获得更多预订。我们还个性化房客体验，向他们展示符合其需求的房源。为了指导这些工作，我们结合了经济学建模和因果推断技术，以了解房客如何根据房东设定的价格等因素预订住宿，以及这种偏好在不同房客和房源之间如何变化。这种理解有助于我们确定 Airbnb 支持市场并更好连接房客与房东的机会。例如，了解房客对不同价格的反应程度有助于优化我们提供给房东的工具，从而使房东能够选择和设定竞争性价格，进一步平衡供需。作为另一个例子，了解房客偏好的异质性有助于我们个性化房客体验，并根据他们对不同价格和其他因素的反应程度，将他们与符合其需求的房源进行更好的匹配。
- **PDF**: https://arxiv.org/pdf/2607.00280v1

### A condition for the identification of multivariate models with binary instruments -- with Corrigendum and Addendum
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.01429v1
- **作者**: Florian Gunsilius
- **备注**: Original paper published in the Journal of Econometrics including corrigendum and addendum
- **摘要**: 本文引入了一个利用二元工具变量对具有连续内生变量的多变量工具变量模型进行非参数点识别的实证条件。在传统方法不适用的环境中，验证这一条件可以确认点识别。特别是，它表明仅使用二元工具变量即可点识别具有一般异质性的非线性工具变量模型。这推广了现有的识别结果，这些结果要么大幅限制了未观察到的异质性，要么要求工具变量具有大支撑集。该工具变量模型的主要假设是其第一阶段的循环单调性，这是单变量模型经典秩不变性假设的多变量推广。推导了经验可观测分布的渐近收敛结果，以便在实践中检查该条件。该识别基于拟凹函数之间循环单调映射的固定集收敛结果。勘误修正了引理 1 的证明。其中给出的证明错误地将分布水平集的保留与通过 Brenier 映射保留底层概率测度等同起来。我们用基于逆 Brenier 映射（它起到了多变量秩的作用）的论点替换了该论点。修正后的论点适用于比原论文中考虑的拟凹类更灵活、但明显不同的分布类。特别是，它允许在紧支撑上存在光滑的非拟凹和多峰密度，前提是相关的秩固定集满足非退化条件。此外，对于光滑参数分布类，它通常是满足的。
- **PDF**: https://arxiv.org/pdf/2607.01429v1

#### 学科总结 (`econ.*`)
本期选录的 `econ.*` 学科论文共 3 篇，聚焦于双边平台优化与微观计量经济学的方法论突破。研究包括：结合双重/去偏机器学习与层次贝叶斯框架（引入地理相似特征先验），以评估 Airbnb 房源供给增长对预订量的因果增量效应；利用因果推断探讨供求弹性及用户偏好的异质性，以支撑更好的平台定价工具设计与搜索匹配个性化；以及微观计量理论领域的进展，该研究给出了非参数化、含一般异质性的多维内生工具变量模型在仅持有二元工具变量时的识别条件，并利用基于逆 Brenier 映射的循环单调性对其关键的分布测度等同引理进行了理论勘误。