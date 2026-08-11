# 🗓️ 周报 (2026-W31)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-08-02

--- 
## 📚 学科: `eess.*`
本期入选的EESS领域论文涵盖了语义通信、无线定位、多输入多输出（MIMO）系统、控制理论与音频信号处理等前沿方向。研究包括基于大模型的查询导向图像语义编码、利用强化学习优化基站部署、超大MIMO无线能量传输的功率效率优化，以及复杂动力系统的决策数据驱动方法和针对现场音乐源分离的新数据集。

### Generalized Query-Oriented Image Semantic Coding Empowered by Large AI Models and Semantic-Aware Hybrid Beamforming
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28276v1
- **作者**: Sin-Yu Huang, Vincent W. S. Wong
- **备注**: Accepted by IEEE Transactions on Communications (TCOM)
- **摘要**: 语义通信是一种新兴范式，可以在传输过程中保留数据的含义。然而，人类用户往往对基于其意图的特定语义内容感兴趣，而当前语义编码设计中往往未考虑用户的意图。此外，大多数现有语义模型都是使用特定数据集进行微调的，这限制了它们的泛化能力。再者，如何在超大规模多输入多输出正交频分复用（MIMO-OFDM）系统中优先考虑语义上重要的特征仍有待探索。为了解决上述挑战，在本文中，我们提出了一个通用的面向查询的图像语义编码（QO-ISC）框架。在所提框架中，发送端提取与用户查询相关的特征，接收端基于这些特征重建图像。我们使用预训练的大型人工智能模型（LAM）来增强通用的特征表示。我们开发了一种语义感知的混合波束赋形（SA-HBF）算法，以在超大规模MIMO-OFDM系统中优先考虑语义重要的特征。在数据集内未见过的物体类别上进行评估时，仿真结果表明，我们提出的通用QO-ISC框架比传统编解码器和两种最先进的语义编码方案实现了更好的性能。
- **PDF**: https://arxiv.org/pdf/2607.28276v1

### Multi-Agent Reinforcement Learning for Base Station Placement in TDOA-Based Localization
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28002v1
- **作者**: Bastian Perner, Pratik Gajanan Raut, Maximilian Lübke, Norman Franchi
- **备注**: to be published in conference proceedings of IEEE PIMRC 2026
- **摘要**: 设备的精确定位是新兴5G和6G网络的关键能力，并且取决于有效的基站（BS）部署。传统的基于几何的方法，如几何精度因子（GDOP），忽略了实际的传播效应，例如由建筑物引起的非视距（NLOS）阴影和多径诱发的到达时间（TOA）偏差。本文提出了一种射线追踪辅助的多智能体强化学习（MARL）框架，用于时差定位（TDOA）系统中环境感知的基站部署。近端策略优化（PPO）智能体在根据大学校园详细3D模型生成的信道冲击响应（CIR）上进行训练。每个智能体协同部署一个基站，同时优化兼顾定位精度和覆盖范围的共享奖励。该方法在具有不同传播特性的五个校园区域进行了评估。结果表明，学习到的策略实现了与传统基于GDOP的部署相当的定位精度，相较于较强的（均值优化）几何基线，平均定位平均绝对误差（MAE）降低了约3%。其表现具有区域依赖性，在某些特定区域有明显提升（最高约14%），而在其他区域误差相当或略高。这些发现表明，将特定地点的传播数据纳入部署过程可以达到并选择性地改善纯几何策略，这为进一步推动实现持续增益的研究提供了动力。
- **PDF**: https://arxiv.org/pdf/2607.28002v1

### Power-Efficient XL-MIMO Design for Mixed Near- and Far-Field SWIPT Systems
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.27992v1
- **作者**: Muhammad Zeeshan Mumtaz, Mohammadali Mohammadi, Hien Quoc Ngo, Hyundong Shin, Michail Matthaiou
- **备注**: This paper has been accepted for future issue of IEEE Transactions on Communications
- **摘要**: 本文研究了基于混合波束赋形（HB）的模块化超大规模多输入多输出（XL-MIMO）天线阵列支撑的、近场与远场混合（MF）同时无线信息与能量传输（SWIPT）系统的功耗（PC）效率。多个信息解码（ID）和能量收集（EH）用户由位于发射天线阵列近场（NF）和远场（FF）区域的多个组成子阵列提供服务。提出了一种新颖的决策方法，利用基于Frobenius范数的最小二乘（LS）信道估计的频率相关性，对不同的近远场用户进行准确分类。近场空间非平稳（SnS）效应会产生独特的电磁（EM）可见区域（VR），可以通过定制这些区域来实施组成XL-MIMO子阵列的策略性激活。我们构建了一个两级联合优化问题，以在考虑ID and EH用户功率分配（PA）以及子阵列激活（SA）的情况下，最小化整体功耗。这一极具挑战性的混合整数问题被转化为计算上可行的公式，并开发了高度优化的算法。仿真结果表明，相比于全阵列（FA）等功率分配方案，我们提出的PA-SA-HB方案可降低高达93%的整体功耗；相比于PA-FA-HB方案，可降低高达18%的功耗。
- **PDF**: https://arxiv.org/pdf/2607.27992v1

### Data-Driven Formal Methods for Complex Dynamical Systems: A Survey
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.27908v1
- **作者**: Behrad Samari, Alessandro Abate, Antoine Girard, Majid Zamani, Amy Nejati, Abolfazl Lavaei
- **备注**: The proposal for this survey paper has been accepted at Automatica
- **摘要**: 近年来，具有形式化保证的数据驱动方法已成为复杂动力系统验证和控制器合成的强大手段。由于在实际中往往无法获得系统模型，且非线性行为、不确定性和维度灾难等挑战通常导致精确建模不可行，人们对这些方法的兴趣正在迅速增长。这些困难激发了利用从系统收集的有限数据，同时仍对系统的整体行为提供形式化保证的研究。因此，学术界已发表了数百篇关于开发数据驱动框架的论文，这些框架能够在没有显式模型的情况下实现动力系统的形式化验证和合成，解决了超越稳定性之外的复杂规范。尽管增长迅速，但现有的研究成果仍显分散且缺乏系统的组织，限制了对其原理、区别和实用潜力的清晰理解。本综述通过全面概述确定性和随机动力系统的这些数据驱动方法来填补这一空白。我们围绕形式化方法中的三个主要方法论支柱来构建文献结构：基于（无限/有限）抽象的技术、功能证书方法（如控制屏障证书）以及组合方法。对于每种方法，我们系统地将产生的数据驱动保证分为三大类：（i）基于概率近似正确（PAC）和基于场景框架的统计保证，（ii）源自Lipschitz连续性的保证，以及（iii）利用结构性质的保证。虽然关于确定性系统的文献要丰富得多，但我们也特别关注了随机系统，强调了与确定性情况相比所产生的内在差异和挑战。
- **PDF**: https://arxiv.org/pdf/2607.27908v1

### CrowdioSet and PaRIRset: Two Datasets Towards Live Music Source Separation
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.27828v1
- **作者**: Enric Gusó, Xavier Serra
- **备注**: Accepted to ISMIR26. See : https://enricguso.github.io/crowdioset_parirset
- **摘要**: 大多数音乐源分离（MSS）模型在现场音乐录音上的泛化效果不佳，因为它们仅在录音室录音上进行训练，忽略了场馆声学、扬声器系统响应和观众噪声。我们建议通过提供并在两个新型数据集上训练模型来弥补这一差距。首先，我们展示了 CrowdioSet：一个噪声数据集，包含来自 Freesound 的 4800 个真实环境音轨，以及为 MUSDB18 和 MOISESDB 数据集中的人声生成的、基于零样本歌声音色转换的合成合唱。CrowdioSet 能够对现场录音进行有效的音频去噪，从而在客观和主观评估中均实现优异的分离效果。其次，我们介绍了 PaRIRset：这是一个立体声脉冲响应数据集，使用麦克风阵列在 40 个专业音乐会场馆中采集。我们的结果表明，与仅使用语音增强任务中的真实 RIR 相比，添加 PaRIRset RIR 可以提高 MSS 模型的性能。我们向公众免费开放了示例、代码、模型权重、PaRIRset 和 CrowdioSet。
- **PDF**: https://arxiv.org/pdf/2607.27828v1

--- 
## 📚 学科: `q-bio.*`
本期生物学领域的研究论文主要探讨了生态系统和生物医疗人工智能管线的优化。一篇文章引入了非确定性对齐框架，用于识别跨生态系统的食物网交互骨架，帮助预测生态重组；另一篇文章构建了敏感度知觉的诊断基准，评估深度表示学习在单细胞RNA测序聚类中的实际价值与超参数敏感度。

### Identifying common backbones of interactions underlying food webs via non-deterministic alignments
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.27496v1
- **作者**: Yifan Xu, Carlos Taveras, Lydia Beaudrot, César A. Uribe
- **备注**: Published as a conference paper at ICASSP 2026
- **摘要**: 气候变化通过改变物种分布和相互作用重新塑造了食物网，因此识别跨生态系统持续存在的相互作用结构骨架至关重要。确定性对齐方法计算速度慢，且局限于一对一的对应关系。我们引入了一种受最优传输启发的可扩展、非确定性对齐框架，通过多对多映射捕捉重叠的物种角色。该方法通过基元-角色剖面（motif-role profiles）将其构建为 Gromov-Wasserstein 传输问题，既高效又具可解释性。我们将所提方法应用于包含撒哈拉以南非洲地区 129 个哺乳动物食物网的大型大陆级数据集。识别出了成对对齐，并发现了与虚无模型相比具有更强连通性和传递性的稳健骨架。所提方法为预测生态系统重组和保护工作提供了一个正式且可复制的工具。
- **PDF**: https://arxiv.org/pdf/2607.27496v1

### When Does Deep Representation Learning Help Single-Cell Clustering? A Sensitivity-Aware Diagnostic Benchmark for Biomedical AI Pipelines
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.25288v1
- **作者**: Nguyen Thanh Phong, Truong Viet Vu, Nguyen Ha Thu, Tran An Ky, Tran Hoang Thong, Le Pham Thuy Hien, Nguyen Thai Anh
- **备注**: 13 pages, 6 figures. Accepted at ISRSD 2026
- **摘要**: 单细胞核糖核酸测序（scRNA-seq）是精准医学工作流的基础技术，有助于实现联合国关于良好健康与福祉的可持续发展目标3，而无监督聚类是将原始表达矩阵转化为可解释细胞群的关键分析步骤。因此，从业者面临着一个周期性的工程决策：额外的深度表示阶段是否值得其计算和调参成本，还是经典的算法（如主成分分析 PCA 管线）就已经足够？我们通过在十个真实数据集（包含90-5,685个细胞、19,046-41,480个基因、4-11种细胞类型）上对九个聚类管线进行诊断基准测试来回答这个问题，并辅以在七个数据集上针对部分 scVI V2 专门进行的对比。该方案集成了 Optuna 超参数搜索、重复运行鲁棒性测试、Friedman/Wilcoxon-Holm/TOST 检验以及 Sobol 全阶敏感性分析。对比自编码器实现了最高平均调整兰德指数（0.7872），但经过 Holm 校正的检验并未确立其相对于最强基线的绝对优势。单数据集分析揭示了三种可复现的模式：概率变分自编码器（VAE）变体在极小数据集上有所帮助；深度自编码器在具有多批次或多种类型的多尺度数据上胜出；而当线性投影已能捕获主导方差时，经典 PCA 管线仍具有竞争力。Sobol 指数确定学习率（$S_T=0.70$）和隐空间维度（$S_T=0.56$）是主导方差的主要贡献者，指明了有限调参预算应分配在何处。因此，本文的贡献在于为支持可持续医疗分析的生物医学 AI 管线提供了一个兼顾数据集特性和计算成本的决策框架，而非提出一个普适性的优越性声明。
- **PDF**: https://arxiv.org/pdf/2607.25288v1

--- 
## 📚 学科: `cs.*`
本期计算机科学领域的论文涵盖了算法博弈论、软件工程自动化、人机交互与虚拟现实、多模态检索增强生成（RAG）以及量子计算系统评估。具体研究包括：Thiele投票规则下的委员会选举算法、检测SWE-bench等基准中PR与Issue失配的智能体系统、评估跨现实协作中的空间投影技术、解耦宏观推理与微观匹配的双层图多模态RAG框架，以及提出衡量量子计算性价比的全新度量指标。

### Algorithms for Structured Elections under Thiele Voting Rules
- **分数**: 4
- **链接**  https://arxiv.org/abs/2607.28575v1
- **作者**: Alexandra Lassota, Krzysztof Sornat
- **备注**: 18 pages. A conference version of this work appeared in AAAI 2026
- **摘要**: 我们研究了基于批准的委员会选举中，在 Thiele 投票规则下确定赢家问题的计算复杂度。这是一类由固定权重向量参数化的规则，该向量指定了选民的满意度如何取决于选出的其所批准的候选人数量。我们首先根据批准每个候选人的选民集合（即选民的批准选票如何引发候选人之间的依赖关系）分析了最优解的结构，揭示了在任何固定的 Thiele 投票规则下获胜委员会的约束条件。利用这一点，我们在一个被称为“选民区间（VI）”的自然受限领域上，为比例批准投票（PAV）和其他 Thiele 规则设计了固定参数可解（FPT）算法——即在对选民进行适当排序后，每个候选人均被连续区间内的选民所批准。特别地，我们展示了在 VI 上的每个 Thiele 规则对于某个参数都是 FPT 的，而该问题在一般实例上是 NP-难的，即使该参数取常数值时也是如此。我们的结果推进了对选民区间实例上 PAV 计算复杂度的理解，这仍是该领域的核心开放问题之一。我们通过提供一个针对每个候选人最多被两名选民批准的实例的多项式时间算法，以及一个以获胜委员会总得分为参数的 FPT 算法，进一步解决了两项来自关于 PAV（及其他 Thiele 投票规则）文献的开放问题。
- **PDF**: https://arxiv.org/pdf/2607.28575v1

### PAIChecker: Uncovering and Checking PR-Issue Misalignment in SWE-Bench-Like Benchmarks
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28587v1
- **作者**: Manyi Wang, Junjielong Xu, Pinjia He
- **备注**: Accepted at the 41st IEEE/ACM International Conference on Automated Software Engineering (ASE 2026)
- **摘要**: 类似于 SWE-bench 的基准测试被广泛用于评估大语言模型（LLM）解决软件问题的能力。它们通常遵循一个通用的构建流程：通过从拉取请求（PR）描述中提取 Issue 引用，将每个 PR 与其关联的 Issue 进行配对；将 Issue 描述作为问题陈述，并将 PR 补丁作为测试基准（oracle）。然而，由于开发和维护大型代码库的固有复杂性，此类 PR-Issue 配对在实践中经常出现失配（misalignment）。在这项工作中，我们系统地研究了 SWE-bench Verified 实例，发现在 11 个细粒度场景的 5 种模式中，有 13.6% 的实例存在失配。为了在未来实现这些基准测试可靠且可扩展的构建，我们提出了 PAIChecker，这是一个用于检测类 SWE-bench 基准中 PR-Issue 错配的多智能体系统。具体而言，PAIChecker 采用了结合特定模式识别、跨智能体标签合成和代码级验证的三阶段设计，从而实现了更准确、可推广且逐步验证的检测。在 SWE-Gym 和 SWE-bench Multilingual 上的实验表明，PAIchecker 在四种 LLM 骨干网络中均取得了最佳性能，二分类准确率分别达到 92.12% 和 91.67%。
- **PDF**: https://arxiv.org/pdf/2607.28587v1

### CrossAtlas: Evaluating Projection Techniques for Spatial Referencing in Cross-Reality Collaboration
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28583v1
- **作者**: Haoyang Yang, Chenyang Zhang, Elliott H. Faa, Weijian Liu, Lily Seika Chisholm, Benjamin Lee, David Saffo, Feiyu Lu, Blair MacIntyre, Yalong Yang
- **备注**: 11 pages, 8 figures, Accepted to IEEE ISMAR 2026 (TVCG journal track)
- **摘要**: 跨现实（Cross-Reality）协同越来越多地将沉浸式用户与桌面端用户在同步工作空间中连接起来，然而，对于沉浸式 3D 布局与桌面端 2D 视图之间的双向投影技术如何影响沟通，人们仍知之甚少。空间参照依赖于共享的空间理解，但不同的映射方式会以不同的形式保持或扭曲几何关系，从而改变协作者视图中感知到的邻近性、方向和覆盖范围。我们展示了 CrossAtlas，这是一个同步的 PC-VR 协作平台，它在不同弯曲度的布局中集成了多种双向投影技术，包括三种平面投影变体和等距柱状（一种球面投影变体）。在对 24 对协同小组进行的对照研究中，协作者在不同的投影-布局条件下完成了空间参照任务，同时我们收集了绩效和主观评估指标。我们的结果表明，投影方式的选择极大地塑造了协作，其中球面变体通常优于平面投影，并且在不同的物体布局中保持了稳健性。
- **PDF**: https://arxiv.org/pdf/2607.28583v1

### DualG-MRAG: Decoupling Macro-Reasoning and Micro-Matching for Multimodal Retrieval-Augmented Generation
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28580v1
- **作者**: Jiacheng Tao, Qingyun Sun, Haonan Yuan, Ziwei Zhang, Jianxin Li
- **备注**: Accepted to the 34th ACM International Conference on Multimedia (ACM MM 2026). 12 pages
- **摘要**: 尽管多模态检索增强生成（MM-RAG）已取得了令人振奋的成果，但在处理复杂的跨步（multi-hop）推理任务时仍显吃力。现有方法主要集中在独立的实例级匹配上，往往无法捕获跨模态和跨文档的显式关系。尽管图增强方法引入了结构建模，但在多模态场景中面临着根本性的挑战：融入细粒度的视觉特征会导致图规模迅速膨胀并引入检索噪声，而粗粒度的表示则会导致关键局部证据的丢失。为了解决这一两难境地，我们提出了 DualG-MRAG，这是一个为多模态 RAG 引入了解耦架构的双层框架，包含宏观推理（Macro-reasoning）和微观匹配（Micro-matching）图。具体而言，为了通过将全局结构推理与细粒度证据匹配隔离开来以抑制检索噪声，我们构建了用于全局拓扑路由的宏观图和用于精确局部验证的微观图。随后，为了使跨异构证据源的动态相关性得以传播，我们通过 GNN 检索器将检索公式化为查询驱动的消息传递过程。此外，为了给生成模型提供连贯的结构引导，我们引入了一种动态规划解码机制，直接从 GNN 的前向传播中提取显式推理路径，从而替代了独立的文档块的常规输入。广泛的实验表明，DualG-MRAG 在证据召回率和复杂问答准确率上均优于基线方法。
- **PDF**: https://arxiv.org/pdf/2607.28580v1

### Quantum Fidelity-per-Cost: A Metric for Evaluation of Quantum Computing Systems
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28572v1
- **作者**: Siddarth Shinde, Jakub Szefer
- **备注**: 7 pages, 4 figures, 3 tables. Accepted at IEEE International Conference on Quantum Computing and Engineering (QCE) 2026
- **摘要**: 云端可访问的量子计算使得硬件对比不仅是物理基准测试，也成为了实际的购买决策。考虑到各大云端量子计算服务商提供的异构计费模式，兼顾成本的量子计算机对比研究仍未得到充分探索，且十分困难。本文做出了两个主要贡献，以实现兼顾价格的量子计算机对比。首先，本工作提出了一项跨服务商的量子线路执行保真度测量研究，涵盖了四个云端访问路径上的 14 个云 QPU 访问通道（12 个不同的物理 QPU）：亚马逊云服务（AWS）、IBM Quantum Runtime (IBM) 云、IQM Resonance (IQM) 云和 Oxford Quantum Circuits (OQC) 云。其次，本工作提出并分析了一种兼顾成本的评分指标——性价比保真度（Quantum Fidelity-per-Cost, QFC），它在已记录的计费模型下，将与理想输出分布的 Kullback-Leibler (KL) 散度、采样数（shot count）和货币成本融合为一个度量指标。本工作的主要实证观察结果是，兼顾成本的排名可能与纯粹基于保真度的量子计算机评估有所不同，并且当用户在选择中考虑价格时，与仅基于保真度进行选择相比，可能会选择不同的量子计算后端。本工作表明，该排名在指标重新赋权下是稳定的，并且设备的计费模型（而非其硬件本身）决定了其得分如何随采样数进行缩放。随着新机器的上线或服务商调整价格，报告的 QFC 值也会发生变化。
- **PDF**: https://arxiv.org/pdf/2607.28572v1

--- 
## 📚 学科: `math.*`
本期数学领域选择的论文聚焦于科学计算中大型稀疏线性方程组的高效求解。研究提出了一种图神经网络多级预处理器（GMP），将代数多网格（AMG）层次结构作为结构先验，并在统一框架内学习平滑、限制和插值算子。这一数据驱动的预处理器可作为标准Krylov求解器的即插即用组件，有效改善了其收敛性能。

### Graph Neural Multilevel Preconditioners for Iterative Solvers
- **分数**: 5
- **链接**  https://arxiv.org/abs/2607.28456v1
- **作者**: Zechen Zhang, Rui Peng Li, Yousef Saad
- **备注**: Accepted at KDD 2026
- **摘要**: 求解大型稀疏线性系统是科学计算的核心任务，而高效的迭代求解器关键取决于有效且稳健的预处理方法。虽然代数多网格（AMG）等经典方法具有高度的可扩展性，但在不定或非对称系统上，其稳健性可能会下降，因为最初为椭圆偏微分方程（PDE）开发的启发式方法在这些系统上不那么可靠。最近，图神经网络（GNN）已作为数据驱动的预处理器出现；然而，对于一般的稀疏矩阵，施加 AMG 样式的层次结构所带来的实际影响仍未得到充分探索。在这项工作中，我们提出了一种图神经网络多级预处理器（GMP），该处理器采用 AMG 层次结构作为结构先验，并在一个统一的框架中学习平滑、限制和插值算子。我们的方法针对通用稀疏系统，并被实例化为标准 Krylov 求解器的即插即用预处理器。在包含 800 多个稀疏矩阵的基准测试中，我们与经典 AMG、单级 ILUT 以及最先进 of GNN 预处理器进行了对比，并刻画了多级图神经网络预处理在何种情况下能改善收敛，或者相反地，相比于强大的单级基准引入了额外开销。这些结果既展示了在用于大规模科学模拟的学习预处理器中实施 AMG 样式多级结构的潜力，也揭示了其局限性。
- **PDF**: https://arxiv.org/pdf/2607.28456v1

--- 
## 📚 学科: `astro-ph.*`
本期天体物理学领域的选文涵盖了天文观测设备升级、历史物理学验证、多信使天文学统计分析、太阳物理现象模拟以及太阳系外围天体表征等。具体研究包括：LBTI/NOMIC仪器的双重升级以用于宜居带系外行星成像、基于现代历元和历史数据对罗默光速测定方法的重现、多信使天文警报对应体搜索的统计学方法对比、太阳色球层中部分电离流体磁重联过程的数值模拟，以及对一公里级木星不规则卫星Kallichore的物理与轨道特性的精确测定。

### Upgrading LBTI/NOMIC with a quadruple annular groove phase mask and GeoSnap detector for imaging nearby, habitable-zone exoplanets
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28562v1
- **作者**: Kevin Wagner, Manny Montoya, Steve Ertel, Jarron Leisenring, Pontus Forsberg, Samuel Ronayette, Andre Wong, Mikael Karlsson, Olivier Absil, Denis Defrère, Markus Kasper, Jordan Stone, Dániel Apai, Laird Close, Jamie Dietrich, Ewan Douglas, Jamie Drew, Olivier Durney, Marina Fetisova, Kyran Grattan, Olivier Guyon, Jacob Isbell, Sebastián Jorquera, Petri Karvinen, Markku Kuittinen, Hervé Le Coroller, Jared Males, Brittany Miles, Dillon O'Reilly, Eric Pantin, Sascha P. Quanz, Eckhart Spalding, Vivek Vijayakumar, Zach Werber, S. Pete Worden
- **备注**: To be published as Proc. SPIE 14154-340
- **摘要**: 大双筒望远镜干涉仪（LBTI）的零点优化中红外相机（NOMIC）是目前最优秀的热红外成像系统之一，适用于高对比度、高角分辨率的天文观测。在这里，我们介绍了 LBTI/NOMIC 正在进行的两次升级：（1）设计、制造和安装四重环形沟槽相位掩模（Q-AGPM）星冕仪，以及（2）安装 13 微米截止波段的 Teledyne GeoSnap 探测器阵列。Q-AGPM 是首个安装在 NOMIC 内部的星冕仪，也是首批针对 N 波段（约11微米）观测进行优化的星冕仪之一。它在单个钻石衬底上放置了四个环形沟槽相位掩模，使得在 LBTI 双孔径成像模式下，可以在不损失观测效率的情况下在两掩模对之间切换两个望远镜光束。GeoSnap 阵列将取代 NOMIC 原有的 AQUARIUS 阵列，提供更高的量子效率、更大的满阱容量、更快且更线性的读出，并免受需要剧烈斩波的过量低频噪声的干扰。这些升级共同大幅提高了在小角距离处可实现的对比度和灵敏度。我们还展示了使用 LBTI 的新型 FFTCam 条纹跟踪器获得的高对比度 Fizeau 成像序列，该序列通过注入/恢复测试证实了干涉测量相比于单孔径的增益：相对于等时间单孔径曝光，在 0.2-1 角秒范围内，跨越对比度限制和背景限制区域，S/N = 3 的对比度加深了约 2-4 倍。最后，我们阐述了升级后的 LBTI/NOMIC 仪器在亚利桑那大学 Breakthrough Watch 项目中的作用，该项目旨在对最近的单颗类日恒星的宜居带进行迄今为止最深入的观测。
- **PDF**: https://arxiv.org/pdf/2607.28562v1

### De mora luminis: Roemer's discovery 350 years later
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28512v1
- **作者**: Fabio Falchi, Riccardo Furgoni, Paolo Gattillo, Maurizio Francesio
- **备注**: 11 pages, 4 figures, 6 tables. Author-formatted version of the article published in European Journal of Physics 47 (2026) 025802
- **摘要**: 在 1676 年罗默宣布发现光以有限速度传播 350 年之际，我们展示了使用分辨率与 17 世纪晚期望远镜类似的望远镜进行的人眼观测。我们证实了罗默的方法是有效的，即使使用最简单的建模技术（即均匀圆周运动），在我们的测量中，也能得出合理的光速 $c$ 值（在现代值的 10% 误差范围内）。我们发现，由于其他扰动的影响，增加模型的复杂性（例如考虑木星的椭圆轨道）并不一定会使结果更接近 $c$ 的真实值。使用现代星历表可以产生非常精确的结果，即 $c = (298200 \pm 1900)$ km/s。这一体验具有巨大的教学价值，展示了假设的提出与随之而来的预测、进行观测、数据处理以及为同一现象寻找替代解释之间的相互关联。最后，我们在罗默与惠更斯的往来书信中还发现，罗默在 1677 年曾试图通过对木星大红斑子午线中天的数据进行观测和处理，来寻找其前几年观测木卫一（Io）掩食所获发现的独立验证。
- **PDF**: https://arxiv.org/pdf/2607.28512v1

### Statistical treatment of searches for counterparts of positionally-uncertain astrophysical sources: from flux upper limits to detection
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28473v1
- **作者**: Julian Sitarek, Abelardo Moralejo, Juan Jiménez Quiles, Giacomo D'Amico, Andrea Simongini, Antonio Stamerra
- **备注**: 13 pages, 15 figures, accepted for publication in JHEAP
- **摘要**: 多信使和多波长天体物理学的快速发展，导致使用具有不同点扩散函数的仪器对相同事件进行观测的次数不断增加。特别是具有良好角分辨率的指向性仪器，被用来精确锁定定位较差的警报源。在未探测到明确的源对应体的情况下，结果的解释需要统计分析。我们研究了使用警报概率密度函数的两种方法：频率派和贝叶斯派，以及不使用此信息的不可知（agnostic）方法。我们讨论了所有方法的优缺点，并比较了它们的可靠性和性能。我们既考虑了简单的一维玩具模拟，也考虑了使用伽马射线望远镜跟踪引力波事件完整模拟的真实使用案例。频率派和贝叶斯派方法在弱信号情况下的性能相当，且明显优于不可知方法。
- **PDF**: https://arxiv.org/pdf/2607.28473v1

### Magnetic Reconnection Process in Partially Ionized Fluids: Insights from the Solar Chromosphere
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28447v1
- **作者**: Adrian R. Montañez-Lobo, Fabio D. Lora-Clavijo
- **备注**: 34 pages, 14 figures. Accepted for publication in Solar Physics
- **摘要**: 磁重联将储存的磁能转化为动能、热量和辐射。虽然在完全电离的等离子体中已得到广泛研究，但观测表明，电离和重组也通过改变局部等离子体电阻率并启用额外的加热通道来发挥作用。本研究探讨了部分电离的太阳色球层中的磁重联，分析了其形态和能量释放，并重点关注了弹性碰撞、电离和重组。原本为欧姆电阻和热传递设计的 MAGNUS 代码经过修改，以处理弹性裂和非弹性碰撞。模拟为具有双流体效应（带电+中性）的 2.5 维电阻性 MHD，适应通过这些碰撞项进行的相互作用。实施了混合显式-隐式格式以处理这些项的刚性。针对三种磁场强度进行了模拟：100 G、110 G 和 120 G。这些值对应于静宁太阳条件下色球层的中低部。我们发现磁重联使等离子体组分加热了 18% 至 110%。虽然等离子体贝塔（beta）值仅略有上升，但能量释放增长要多得多，这表明带电-中性碰撞（而非仅仅是贝塔值或可用磁能）驱动了增强的重联。此外，电离和重组在温度峰值区域（特别是在粒子加速的地方）变得最为显著。时间分析得出的最大重联率分别为 0.226、0.253 和 0.279。最后，在能量方面，我们的结果表明，在 $0.4 \times 0.01 \times 0.4 \text{ Mm}^3$ 的色球层体积中，释放的能量范围在 $10^{22}$ 到 $10^{23}$ 尔格（ergs）之间。
- **PDF**: https://arxiv.org/pdf/2607.28447v1

### Kilometre-scale Jovian moon characterized for a potential JUICE flyby
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28357v1
- **作者**: Juan Luis Rizos, Jose Maria Gomez-Limon, Yucel Kilic, Altair R. Gomes-Junior, Jose Luis Ortiz, Nicolas Morales, Alvaro Alvarez-Candal, Pasquale Palumbo, Luisa M. Lara, Simon Porter, Benjamin Proudfoot, Evelyn Christiny M. Prais, Jean Marc Christille, Stefano Sartor, Antonio Cabrera, Stefan Geier, Alessia Spolon, Alice Lucchetti, Andrea Soffiantini, Anne Verbiscer, Armin Behrend, Elena Mazzotta Epifani, Jean-Louis Dumont, Luca Zampieri, Mike Skrutskie, Maurizio Pajola, Michel Boutet, Michele Fiori, Raoul Behrend, Stefano Sposetti, Vadim Nikitin, Fabien Cavaille, Jocelyn Serot, Laurent Miralabe, Marc Buie, Mehmed Naim Bagiran, Metin Altan, Mohammad Niaei, Noel Robichon, Orhan Erece, Pierre-Louis Phan, Raphael Lallemand, Suleyman Fisek, Valentin Etienne, Valery Lainey, Yavuz Guney, Yusuf Avcioglu, Francois Poulet, Paul Hartogh, Oliver Witasse, Pablo Santos-Sanz, Julia de Leon, Flavia L. Rommel, Fernando Tinaut-Ruano
- **备注**: Published in Nature Astronomy on 24 July 2026
- **摘要**: 木星的不规则卫星被认为是早期太阳系微行星的遗迹。然而，它们体积小、距离地球远，且在角距离上紧邻木星，这使得远程对其进行表征变得非常困难。在此，我们报告了对公里级卫星 Kallichore 的多仪器观测，这是唯一一颗适合欧空局“木星冰卫探测器”（JUICE）进行近距离飞越的木星不规则卫星，其天体测量和物理特性此前仍鲜有约束。我们使用了哈勃望远镜的光度测量和天体测量，随后进行了地面多站点恒星掩星观测，并利用 10.4 米的大加那利望远镜（Gran Telescopio Canarias）进行了天体测量和光度观测。我们将 Kallichore 的轨道不确定性降低了高达约 80%，并确定了其形状：一个拉长的天体，其最小半轴比为 $a/b = 1.53 \pm 0.10$，面积等效直径为 $3.8 \; (+2.3/-0.3)$ km，具有几何反照率为 $3.7\% \; (+0.7/-2.2)$ 的暗表面。未探测到近距离伴星。这些新的约束条件为航天器在 2031 年抵达木星系统后飞越 Kallichore提供了一条可行的路径。
- **PDF**: https://arxiv.org/pdf/2607.28357v1

--- 
## 📚 学科: `stat.*`
本期统计学领域选择的论文关注大规模高斯过程回归（GPR）的计算瓶颈。研究提出了一种自适应 Nyström 方法，通过贪婪地选择地标点（landmark points）来最小化核近似误差的迹残差，并将地标点扩展与超参数优化交织进行。该方法显著提升了精度和稳定性，为大规模计算机实验提供了一种线性扩展的高效框架。

### Adaptive Nyström for Gaussian Process Regression
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.27427v1
- **作者**: Lulu Kang
- **备注**: 13 pages, 1 figure. Accepted by 2026 Winter Simulation Conference
- **摘要**: 高斯过程回归（GPR）是用于不确定性量化的强大框架，但其 $O(n^3)$ 的复杂度限制了其可扩展性。低秩 Nyström 近似可以将此计算负担降低到 $O(nm^2)$，但其精度在很大程度上取决于地标点（landmark points）的选择。我们提出了一种自适应 Nyström 方法，该方法贪婪地选择地标点以最小化核近似误差的迹残差。与静态近似不同，我们的方法将地标点扩展与超参数优化交织在一起，使得选择过程能够随着协方差结构的改进而进行自适应。在五个基准函数上的数值实验表明，该方法在准确性和稳定性上都显著优于随机地标点选择。它实现了与精确高斯过程推理相当的预测性能，同时保持了相对于样本量的线性扩展，从而为大规模计算机实验提供了一个有原则且高效的框架。
- **PDF**: https://arxiv.org/pdf/2607.27427v1

--- 
## 📚 学科: `econ.*`
本期经济学/社会科学领域选择的论文聚焦于负责任AI的政治经济学与合规博弈。文章构建了一个序贯政治经济学模型，探讨AI供应商、部署者和监管者在审计、合规及责任等方面的博弈。研究深入剖析了为何标准化的文档和评估无法消除部署后的实际危害，并为制定有效的监管和责任机制提供了理论洞见。

### Scaling, Lock-In, and Proxy Compliance: A Political Economy of Responsible AI
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.28023v1
- **作者**: Florian A. D. Burnat, Brittany I. Davidson
- **备注**: Accepted at AAAI/ACM Conference on AI, Ethics, and Society (AIES '26)
- **摘要**: 大规模的 AI 问责制是一个制度性问题：即谁能够观察、验证和改变已部署的系统。我们开发了一个序贯政治经济学模型。在模型中，AI 供应商选择审计可行性和实质性缓解措施，部署者在采用后进行监控同时面临切换成本，而执法则依赖于可验证的证据。预见到部署者的监控反应，供应商可能会止步于可观察的采购门槛，同时将缓解措施控制在社会最优水平之下，从而产生“代理合规（proxy-compliance）”均衡。我们表征了独特的内部均衡以及伤害被完全缓解的边界情况。独立的审计权直接提高了执法的暴露度；可移植性恢复了部署者的杠杆作用；事件报告增加了一条监管者可见的证据渠道；而与结果挂钩的责任则创造了不依赖于供应商控制的检测机制。这些结果解释了为什么文件记录和标准化评估能够与持续存在的部署后危害共存，并为监控、缓解措施以及正式合规与运营结果之间的差距提供了可测试的启示。
- **PDF**: https://arxiv.org/pdf/2607.28023v1

---