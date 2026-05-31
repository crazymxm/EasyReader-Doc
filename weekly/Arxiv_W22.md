# 🗓️ 周报 (2026-W22)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-05-31

--- 
## 📚 学科: `eess.*`
本次选择的论文展示了电子工程与系统科学在多个前沿领域的应用：从提升大模型合并效率的 MergePipe 框架，到增强临床 MRI 自动化流程可靠性的 BCER 智能体；在多模态生成方面，提出了关注物理一致性的视听生成基准。此外，还涵盖了针对脑部应用的简化电学模型，以及在“月船3号”探月任务中得到实证的实时重定位导航策略。这些研究体现了从算法优化到航天工程应用的广泛跨度，重点关注系统的可扩展性、可靠性与实时性。

### Access Sets Matter: Budgeting Expert Reads for Scalable Weight-Space Model Merging
- **分数**: 4
- **链接**  https://arxiv.org/abs/2605.29489v1
- **作者**: Yuanyi Wang, Yanggan Gu, Su Lu, Yifan Yang, Zhaoyi Yan, Congkai Xie, Jianmin Wu, Hongxia Yang
- **备注**: ICML 2026 Workshop on Weight-Space Symmetries: from Foundations to Practical Applications
- **摘要**: 权重空间模型合并通常被表述为对 Checkpoint 的代数运算，但在大语言模型（LLM）规模下，资源瓶颈通常在于必须读取的专家权重集。我们引入了 MergePipe，这是一个预算感知型的执行层，它将 LLM 合并抽象为一个“专家访问集”问题：在给定的合并算子和共享权重坐标系下的 Checkpoint 系列中，在显式 I/O 预算内选择要访问的专家 delta 块。MergePipe 对参数块进行索引，构建确定性访问计划，并使用可回放的清单执行带预算的合并。该计划在构建上是预算完备的，并在全额预算下恢复完整合并；对于固定系数加法算子，忽略更新的误差受限于被忽略 delta 的范数。在 Qwen 和 Llama 合并工作负载中，MergePipe 将专家读取 I/O 减少了高达一个数量级，并实现了高达 11 倍的加速。代表性的预算扫描显示，其参数偏差与全额合并相比仅为 $O(10^{-3})$，且在下游基准测试中没有单调退化。
- **PDF**: https://arxiv.org/pdf/2605.29489v1

### BCER Agent: Reliable Long-Horizon MRI Workflow Execution via Compilation, Artifact Binding, and Bounded Local Recovery
- **分数**: 4
- **链接**  https://arxiv.org/abs/2605.29163v1
- **作者**: Ziyang Long, Xinqi Li, Junzhou Chen, Yifan Gao, Debiao Li, Hsin-Jung Yang
- **备注**: Pre-review submitted version of a paper accepted to MICCAI 2026. The final authenticated version will be available on SpringerLink
- **摘要**: 近期许多医疗视觉语言模型（VLM）和智能体研究主要在 2D 图像或较短的工具调用交换上进行基准测试，而真实的 MRI 分析通常需要操作 3D/4D 体数据的长程、相互依赖的流水线。在这些条件下，反应式工具调用智能体容易因中间引用错误、工具参数不匹配以及对跨步骤依赖性的控制有限而导致级联崩溃。为此，我们引入了 BCER（Brain-Cerebellum-Extremity-Reflector），这是一种旨在实现可靠长程 MRI 工作流执行的控制器架构。BCER 将高级规划与执行解耦，并提供有界的局部恢复。我们在涵盖大脑、前列腺和心脏任务的多器官 MRI 基准上评估了 BCER，使用了短链和长链工作流。相对于反应式基线，BCER 在端到端执行方面取得了持续改进，在长链工作流中增益最为显著。此外，BCER 通过维护最终输出与中间构件、测量值之间的显式链接，实现了可审计性。
- **PDF**: https://arxiv.org/pdf/2605.29163v1

### Benchmarking Single-Factor Physical Video-to-Audio Generation
- **分数**: 3
- **链接**  https://arxiv.org/abs/2605.30339v1
- **作者**: Tingle Li, Siddharth Gururani, Kevin J. Shih, Gantavya Bhatt, Sang-gil Lee, Zhifeng Kong, Arushi Goel, Gopala Anumanchipalli, Ming-Yu Liu
- **备注**: CVPR 2026
- **摘要**: 生成式视频转音频（V2A）模型能够产生极具真实感的配音，但其是否捕捉到了潜在的物理过程仍不清楚。现有的评估侧重于感知真实感，忽略了受控干预下的物理正确性。在本文中，我们引入了 FlatSounds，这是一个通过以下方式审计 V2A 模型物理推理能力的基准：1) 受控的反事实对，其中改变单个物理因素；2) 单视频模式测试，探测内部一致性和方向趋势。这些设置测试生成的音频是否正确反映了特定的物理属性和时序。我们对最先进模型的评估揭示了一个持续的权衡：模型更多地依赖文本提示词而非视觉流来推断物理和语义。提示词通常能提高物理和语义准确性，但矛盾地降低了时间对齐性。我们的结果强调，有必要从追求音频质量转向直接从像素学习物理过程。
- **PDF**: https://arxiv.org/pdf/2605.30339v1

### A Lumped-Element Electrical Model of the Human Head for Brain-Oriented Applications
- **分数**: 3
- **链接**  https://arxiv.org/abs/2605.30172v1
- **作者**: Angelo Faccia, Ermanno Citraro, Francesco P. Andriulli
- **备注**: 4 pages, 4 figures. To appear in the proceedings of the APS March Meeting 2026, Detroit, Michigan
- **摘要**: 在这项工作中，我们提出了一种用于电准静态（EQS）头部建模的紧凑替代电路。考虑了三层壳几何结构（大脑、颅骨、头皮），每一层通过径向和切向路径建模，实现为 RC 分支。频率相关的组织电导率和介电常数被映射为色散电阻和电容元件。该模型在多种几何配置和工作频率下通过半解析球谐函数参考解进行了验证，展示了良好的一致性。忽略色散和电容路径可能导致在所考虑的频率范围内高估头皮电位，这突显了进行色散 RC 电路建模的必要性。
- **PDF**: https://arxiv.org/pdf/2605.30172v1

### Real-Time Retargeting Using Controllability Boundary for Chandrayaan-3 Lunar Landing
- **分数**: 3
- **链接**  https://arxiv.org/abs/2605.29412v1
- **作者**: Suraj Kumar, Debjyoti Chakrabarti, Aditya Rallapalli, Bharat Kumar GVP, Ashok Kumar Kakula
- **备注**: 8 pages, 6 figures, Accepted for publication in American Control Conference 2026
- **摘要**: 本文介绍了为“月船 3 号”（Chandrayaan-3）月球着陆任务开发的实时重定位导航策略。基准导航生成近似燃料最优的下降轨迹，而高级策略在名义着陆点变得不可行时，能够安全地重定位到替代站点。该重定位策略利用可控边界的凸表示，实现了快速可行性检查和实时目标更新。据作者所知，这代表了数据驱动重定位框架在实际月球着陆任务中的首次应用。飞行前模拟和“月船 3 号”的飞行结果验证了该方法的有效性。
- **PDF**: https://arxiv.org/pdf/2605.29412v1

--- 
## 📚 学科: `q-bio.*`
本期生物学领域关注空间转录组学的计算创新。GEARS 框架通过几何优先的方法解决了单细胞 RNA 测序空间信息丢失的问题，实现了无标签的单细胞空间重建；而 FPLIER 则通过联邦学习技术，在保护隐私的前提下，使分布式机构能够共同训练基因通路信息提取模型。这些工作共同推动了高精度、隐私受保护的生物大数据分析方法的发展。

### Geometry-First Generative Spatial Single-Cell Reconstruction
- **分数**: 4
- **链接**  https://arxiv.org/abs/2605.28200v1
- **作者**: Ehtesamul Azim, Muhtasim Noor Alif, Tae Hyun Hwang, Yanjie Fu, Wei Zhang
- **备注**: 32nd SIGKDD Conference on Knowledge Discovery and Data Mining (KDD 2026)
- **摘要**: 单细胞 RNA 测序（scRNA-seq）能分析大量细胞但会丢失空间背景，而空间转录组学（ST）在较低分辨率下保留了部分空间结构。大多数现有的集成方法要么反卷积点混合物，要么将细胞映射到测量的点晶格上，这使得重建受限于固定网格和切片特定的坐标系。我们提出了 GEARS，一个几何优先的框架，在 ST 的指导下重建内在的单细胞空间几何，而不依赖于细胞类型标签、组织学图像或细胞到点的分配。GEARS 首先学习一个域不变的表达编码器来对齐 ST 点和解离细胞，然后训练一个带有基于扩散的精炼器（采用 EDM 风格预处理）的置换等变生成器，在源自 ST 坐标的姿态不变监督下生成局部空间几何。广泛的实验表明，与强大的空间映射和反卷积基线相比，GEARS 持续改进了全局距离保持、局部邻域保真度和空间分布对齐。
- **PDF**: https://arxiv.org/pdf/2605.28200v1

### FPLIER: Federated Pathway-Level Information Extractor
- **分数**: 3
- **链接**  https://arxiv.org/abs/2605.29587v1
- **作者**: Daniele Malpetti, Christian Berchtold, Francesco Gualdi, Marco Scutari, Laura Azzimonti, Francesca Mangili
- **备注**: Accepted for publication at the ACM BCB '26 conference
- **摘要**: 在转录组学中，通路级信息提取器（PLIER）等基因集感知因子分解方法在大型异构表达图谱上训练时最有效。然而，许多临床相关的队列由于隐私和治理限制无法合并。我们提出了 FPLIER，这是 PLIER 的联邦扩展，它允许在多个数据持有者之间进行分布式训练，同时纳入公开数据集。通过安全聚合，FPLIER 产生的训练更新在代数上等同于集中式汇总数据方法，同时保持表达数据本地化。我们在两个模拟联盟中评估了 FPLIER 并证明了其稳定的收敛性。我们进一步对针对训练统计数据和发布模型的成员推理攻击进行了系统分析，结果表明隐私风险受训练表达矩阵秩的控制。
- **PDF**: https://arxiv.org/pdf/2605.29587v1

--- 
## 📚 学科: `cs.*`
计算机科学领域本周的研究焦点集中在多模态生成与智能体可靠性上。Archon 模型实现了数字人生成的全模态统一；Veda 框架通过蒸馏稀疏注意力显著加速了视频扩散模型。针对智能体，研究者探讨了多组件 LLM 的全局不一致性问题及其修正方法。此外，GAVIS 提升了 3D 高斯泼溅的主动制图精度，而一份量化的案例研究探讨了物理学家监督 AI 智能体开发科学软件的现实局限。

### Archon: A Unified Multimodal Model for Holistic Digital Human Generation
- **分数**: 7
- **链接**  https://arxiv.org/abs/2605.30311v1
- **作者**: Chong Bao, Shichen Liu, Lijun Yu, David Futschik, Stylianos Moschoglou, Shefali Srivastava, Ziqian Bai, Feitong Tan, Guofeng Zhang, Zhaopeng Cui, Sean Fanello, Yinda Zhang
- **备注**: Accepted to CVPR 2026. Project Page: https://zju3dv.github.io/archon/
- **摘要**: 数字人是沉浸式交互的基础，但创建一个包含文本、音频、动作和视觉内容的统一模型仍是挑战。我们提出了 Archon，一个全预训练的以人为中心的多模态模型。Archon 通过特定模态的分词器统一了七种模态，并使用在同步模态和 72 个任务上预训练的原生自回归统一多模态模型来建模联合分布。为解决高保真说话视频中的 Token 爆炸问题，我们引入了内存高效的语义视频重参数化，在保持微观动态的同时实现了 4 倍的 Token 减少，并配合语义驱动的视频扩散解码器。我们还提出了“模态思考”（Thinking in Modality），将复杂的跨模态任务分解为分步思维链，逐步增强保真度和可控性。实验证明 Archon 在各种数字人生成任务中达到了优越性能。
- **PDF**: https://arxiv.org/pdf/2605.30311v1

### Physics Is All You Need? A Case Study in Physicist-Supervised AI Development of Scientific Software
- **分数**: 6
- **链接**  https://arxiv.org/abs/2605.30353v1
- **作者**: Nhat-Minh Nguyen
- **备注**: 10 pages, 2 figures, 2 tables, 1 physicist and a few AI agents. Accepted by ICML 2026 AI for Science Workshop
- **摘要**: AI 智能体是工具、共同作者还是研究员？我们呈现了一个量化的案例研究：一位物理学家在 12 个工作日内监督一个 AI 编码智能体（Claude Code, Sonnet, Opus）构建 JAX 中的微分摄动理论模块 CLAX-PT。我们记录并分类了 15 次监督事件。智能体自主解决了其中 10 个，但有 3 个避开了自动化测试。这三个失败都有共同点：智能体将缓解症状误认为解决了根本原因，在不符合物理定律的代码架构中调整参数。研究发现，只有注入物理概念（如各向异性 BAO 阻尼）才能触发架构重新设计。结果表明，监督设计而非模型能力决定了智能体输出的可信度。
- **PDF**: https://arxiv.org/pdf/2605.30353v1

### Uncertainty-driven 3D Gaussian Splatting Active Mapping via Anisotropic Visibility Field
- **分数**: 6
- **链接**  https://arxiv.org/abs/2605.30342v1
- **作者**: Shangjie Xue, Jesse Dill, Dhruv Ahuja, Frank Dellaert, Panagiotis Tsiotras, Danfei Xu
- **备注**: Accepted to CVPR 2026
- **摘要**: 我们提出了 GAVIS，一个用于 3D 高斯泼溅（3DGS）中不确定性量化和主动制图的框架。我们的核心见解是：训练视图未覆盖的区域会导致 3DGS 产生不可靠预测。为此，我们引入了一种高效的方法来量化 3DGS 中的可见性场，定义为每个粒子相对于训练视图的各向异性可见性，并使用球谐函数表示。该可见性场被集成到基于贝叶斯网络的不确定性感知 3DGS 光栅化器中，实现了合成视图的实时（200 FPS）不确定性量化。实验证明 GAVIS 在精度和效率上均显著优于前人方法。
- **PDF**: https://arxiv.org/pdf/2605.30342v1

### Locally Coherent, Globally Incoherent: Bounding Compositional Incoherence in Multi-Component LLM Agents
- **分数**: 6
- **链接**  https://arxiv.org/abs/2605.30335v1
- **作者**: Anany Kotawala
- **备注**: 25 pages, 7 figures, 24 tables. ICML 2026 Workshops
- **摘要**: 多组件 LLM 智能体通过仅看到部分问题的组件来组装概率主张；即使每个组件在局部是连贯的，这种组合也可能违反基本的概率公理。我们将这种“局部连贯、全局不连贯”的失败正式化为组合残差 eps*。我们量化了这种现象，并发现在实验中 33-94% 的集群存在 eps* > 0 的情况。我们提出了一种分层 Boyle-Dykstra 投影来确定性地修复组合，并提供了一种顺序连贯性监控方法。研究还发现，检索、分区感知提示等直观的 LLM 侧缓解措施往往会失效或产生退化。
- **PDF**: https://arxiv.org/pdf/2605.30335v1

### Veda: Scalable Video Diffusion via Distilled Sparse Attention
- **分数**: 6
- **链接**  https://arxiv.org/abs/2605.30325v1
- **作者**: Shihao Han, Hao Yang, Xinting Hu, Xiaofeng Mei, Yi Jiang, Xiaojuan Qi
- **备注**: Accepted to ICML 2026
- **摘要**: 将扩散 Transformer 扩展到生成高分辨率长视频受限于自注意力的平方成本。我们通过实证展示，生成质量并非取决于稀疏率本身，而是取决于稀疏掩码与全注意力的块几何结构的对齐程度。基于此，我们提出了 Veda，一个蒸馏稀疏注意力框架。Veda 将块选择表述为从全注意力中显式重建的问题，集成了统计感知评分和头感知分块。一个硬件高效的跳块内核将理论稀疏度转化为实际加速。在 Waver 和 Wan2.1 等大模型上的实验表明，Veda 实现了 5.1 倍的端到端加速，且生成质量无明显下降。
- **PDF**: https://arxiv.org/pdf/2605.30325v1

--- 
## 📚 学科: `math.*`
数学领域本周贡献了扩散模型在统计最优性方面的深度理论证明，证明了其在学习低维多峰分布时能克服维度灾难。此外，还收录了一篇关于核密度估计中乘性偏差修正的经典统计研究，探讨了半参数密度估计在理论与实践中的表现。

### Diffusion Models Are Statistically Optimal for Learning Low-Dimensional Multi-Modal Distributions
- **分数**: 6
- **链接**  https://arxiv.org/abs/2605.30153v1
- **作者**: Jingda Wu, Changxiao Cai
- **备注**: accepted to ICML 2026
- **摘要**: 基于得分的扩散模型在学习高维分布（尤其是具有低维和多峰结构的分布）方面取得了巨大成功。然而，对其统计效率的理论理解仍然有限。在这项工作中，我们研究了扩散模型学习支撑在低维子集并集上的分布的样本复杂度。我们证明了扩散模型仅需 $\widetilde{O}(\varepsilon^{-k \vee 2})$ 个样本即可在 1-Wasserstein 距离上达到 $\varepsilon$ 误差，其中 $k$ 是内在维度。这一近乎最优的收敛率显著优于先前受维度灾难困扰的理论保证，为扩散模型在复杂高维任务中的成功提供了严谨的理论依据。
- **PDF**: https://arxiv.org/pdf/2605.30153v1

### On multiplicative bias correction in kernel density estimation
- **分数**: 3
- **链接**  https://arxiv.org/abs/2605.30071v1
- **作者**: M. C. Jones, D. F. Signorini, Nils Lid Hjort
- **摘要**: 本文结合了 Hjort 和 Glad (1995) 以及 Jones 等人 (1995) 的方法，研究了核密度估计中的乘性偏差修正。该技术在参数化分布拟合数据时表现优异，而在其他情况下也能保持良好水平。我们证明了新估计器在理论上实现了通用高阶偏差修正，并能针对适当的媒介模型表现更好。模拟实验表明，对于小到中等规模的样本，新估计器在实践中能实现部分理论潜力。
- **PDF**: https://arxiv.org/pdf/2605.30071v1

--- 
## 📚 学科: `astro-ph.*`
天体物理学本周涵盖了从观测数据库到理论模拟的丰富内容。包括了意大利“北十字”射电干涉仪的 INCART 公开数据库发布；关于海王星及亚海王星内部对流混合与热导率的演化模型；弱电离等离子体中非线性阿尔芬波的传播研究；以及对 SN 1987A 超新星外环长达 30 年的跨波段多仪器监测分析。

### The Northern Cross Fast Radio Burst project: VI. The INCART public database
- **分数**: 3
- **链接**  https://arxiv.org/abs/2605.30192v1
- **作者**: L. Bruno, G. Bernardi, M. Pilia, D. Pelliciari, A. Geminardi, F. Fiori, V. Galluzzi, G. Naldi, M. Trudu, A. Zanichelli
- **摘要**: 快速射电暴（FRB）是来自河外的明亮且极短促的闪烁。本文介绍了意大利“北十字”（NC）射电干涉仪的公开平台 INCART，用于分发 NC 的 FRB 观测数据产品。INCART 向社区提供频率-时间序列数据集和物理参数编目，其设计保证了科学再分析的可能性并优化了长期存储，有助于促进跨研究组的协作。
- **PDF**: https://arxiv.org/pdf/2605.30192v1

### The evolution and internal structure of Neptunes and sub-Neptunes II. Convective mixing and thermal conductivity
- **分数**: 3
- **链接**  https://arxiv.org/abs/2605.30078v1
- **作者**: Mark Eberlein, Ravit Helled
- **摘要**: 本文研究了海王星和亚海王星类行星的成分梯度如何抑制对流，并对比了三种热导率模型对行星演化的影响。利用修改后的 MESA 模型，我们发现对流混合对热形成且具有大成分梯度的行星半径演化有显著影响。对于冷形成或成分梯度窄的行星，热导率变得至关重要，决定了稳定梯度下能捕获多少能量。
- **PDF**: https://arxiv.org/pdf/2605.30078v1

### Propagation of waves in weakly ionized two-fluid plasmas. II. Nonlinear Alfvénic waves
- **分数**: 3
- **链接**  https://arxiv.org/abs/2605.30057v1
- **作者**: David Martínez-Gómez
- **摘要**: 本文利用双流体模型研究了霍尔电流和离子-中性粒子碰撞对弱电离等离子体中非线性阿尔芬波传播的影响。推导了阻尼和加热率的解析表达式，并通过数值模拟研究了由有源力引起的非线性密度摄动和整体流。发现圆偏振特征模态的非线性扰动不显示典型的振荡运动，但保留了整体流。
- **PDF**: https://arxiv.org/pdf/2605.30057v1

### The outer rings of SN 1987A from year 1994 to 2024: morphology, light curves, and optical to mid-infrared spectra
- **分数**: 3
- **链接**  https://arxiv.org/abs/2605.30043v1
- **作者**: Sophie Rosu, et al.
- **摘要**: SN 1987A 的外环（ORs）在爆炸前约 2 万年喷出。我们分析了从 1994 年到 2024 年跨越光学到中红外的多波段数据（来自 HST, VLT, JWST）。结果显示外环的光学光变曲线在过去 30 年中稳步下降，符合电离后逐渐消散的预期，目前尚未观察到超新星抛射物与外环相互作用的迹象。
- **PDF**: https://arxiv.org/pdf/2605.30043v1

--- 
## 📚 学科: `stat.*`
统计学领域本周亮点包括：利用边缘似然实现模型与数据的同步稀疏化；基于概念瓶颈模型的解释性错误切片发现方法 CB-SLICE；以及一种旨在让模型学会向新任务外推的关系方法。此外，还提出了一种基于 Jensen-Shannon 散度的非参数 $k$-NN 算法，用于处理成分数据的缺失值填充，展现了在稳健性和解释性方面的进步。

### Joint Model and Data Sparsification via the Marginal Likelihood
- **分数**: 6
- **链接**  https://arxiv.org/abs/2605.29908v1
- **作者**: Alexander Timans, Thomas Möllenhoff, Christian A. Naesseth, Mohammad Emtiyaz Khan, Eric Nalisnick
- **备注**: ICML 2026
- **摘要**: 线性系统中的稀疏恢复是高维回归的基础。我们提出通过优化单个边缘似然目标，同时学习特征相关性和样本相关性，从而实现模型和数据的对称剪枝。这种方法保留了共轭性，允许闭式更新，并提升了模型对离群值或噪声错配的鲁棒性。实验证明，该联合自动相关性确定（ARD）方法能持续产生既稀疏又鲁棒的预测模型。
- **PDF**: https://arxiv.org/pdf/2605.29908v1

### CB-SLICE: Concept-Based Interpretable Error Slice Discovery
- **分数**: 6
- **链接**  https://arxiv.org/abs/2605.29836v1
- **作者**: Yael Konforti, Mateo Espinosa Zarlenga, Elaf Almahmoud, Mateja Jamnik
- **备注**: ICML 2026
- **摘要**: 识别深度学习模型在特定人群组上的系统性错误（错误切片）对于调试至关重要。我们利用概念瓶颈模型（CBM）的特性，提出了 CB-SLICE。由于 CBM 的预测直接依赖于人类可理解的语义概念，我们通过分组具有共同概念预测失败的样本来识别错误源头。CB-SLICE 在揭示已知偏差方面优于现有方法，并提供了更丰富、更忠实于模型推理过程的解释。
- **PDF**: https://arxiv.org/pdf/2605.29836v1

### Learning to Extrapolate to New Tasks: A Relational Approach to Task Extrapolation
- **分数**: 3
- **链接**  https://arxiv.org/abs/2605.30132v1
- **作者**: Adam Ousherovitch, Yixin Wang
- **备注**: ICML 2026
- **摘要**: 现代学习系统擅长插值，但在训练分布之外的任务外推上表现不佳。我们开发了关系任务外推器（RTE），其核心在于学习任务之间的转换关系。通过将目标任务分解为已知锚点任务和转换算子，RTE 能将已知任务的知识迁移到未见任务。在函数预测和序列预测的多种外推场景中，RTE 均显著优于现有方法。
- **PDF**: https://arxiv.org/pdf/2605.30132v1

### A Jensen-Shannon divergence based $k$--$NN$ algorithm for missing value imputation in compositional data
- **分数**: 3
- **链接**  https://arxiv.org/abs/2605.29702v1
- **作者**: Michail Tsagris, Connie Stewart, Abdulaziz Alenazi
- **摘要**: 本文开发了一种新的非参数方法来填补成分数据中的缺失值。该方法基于 $k$-NN 算法，利用 Jensen-Shannon 散度和 Fréchet 均值以增强估计灵活性。与受限的参数模型不同，该方法不假设数据结构，且适用于包含零值的成分数据。模拟研究显示，该算法在准确性和计算效率上均优于竞争算法。
- **PDF**: https://arxiv.org/pdf/2605.29702v1

--- 
## 📚 学科: `econ.*`
经济学领域本周关注表格基础模型在离散选择任务中的“经济有效性”。研究指出，虽然这些模型精度高，但常违反需求单调性等经济逻辑。提出的两阶段适配器通过效用最大化框架约束模型预测，既保留了基础模型的高精度，又确保了经济一致性和可解释的政策分析能力。

### Auditing and Fixing Economic Validity in Tabular Foundation Models for Discrete Choice
- **分数**: 6
- **链接**  https://arxiv.org/abs/2605.26559v1
- **作者**: Yingshuo Wang, Xian Sun, Yanhang Li, Zhichao Fan, Zexin Zhuang
- **备注**: ICML 2026 Workshop
- **摘要**: 表格基础模型在选择预测任务上精度很高，但其预测常违反经济逻辑：例如价格上涨反而导致需求增加。我们提出了一个两阶段适配器，将基础模型预测嵌入效用最大化框架。第一阶段估计受经济理论约束的标准选择模型，第二阶段训练一个修正项来引入基础模型的预测信息。在交通数据集上的实验显示，该方法在保持完美经济一致性的同时，比标准 Logit 模型提升了高达 13% 的准确率。
- **PDF**: https://arxiv.org/pdf/2605.26559v1