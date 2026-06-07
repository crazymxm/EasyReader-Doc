# 🗓️ 周报 (2026-W23)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-06-07

--- 
## 📚 学科: `eess.*`
本次选择的论文涵盖了机器人硬件设计、多语言语音识别（ASR）、通用音频编码器以及复杂环境下的定位技术。重点关注了柔性机器人生长中的摩擦力优化、ASR模型在未见语种对上的泛化能力，以及针对病理语音识别的个性化适配技术。这些研究展示了电子与电气工程在感知与控制领域的最新进展。

### Gotta Grow Fast: Design and Benchmarking of a Tip Mount for High-Speed Vine Robots
- **分数**: 4
- **链接**: https://arxiv.org/abs/2606.06040v1
- **作者**: Antonio Alvarez Valdivia, Robert Reeve, Ankush Dhawan, et al.
- **备注**: Accepted to IEEE Robotics & Automation Letters
- **摘要**: 柔性生长型藤蔓机器人通过尖端外翻延伸，能够穿过杂乱环境。然而，在尖端集成摄像头和传感器具有挑战性，因为随着机器人生长，尖端材料不断更新。本研究提出了一种三角形滚轮尖端支架，通过滚动而非滑动来减少生长过程中的内部阻力，首次实现了在TPU涂层尼龙材料上的稳定外翻。实验表明，该设计具有最低的尾部张力和最佳的重复性，并为该领域提供了开源的基准测试框架和CAD设计。
- **PDF**: https://arxiv.org/pdf/2606.06040v1

### Towards Truly Multilingual ASR: Generalizing Code-Switching ASR to Unseen Language Pairs
- **分数**: 4
- **链接**: https://arxiv.org/abs/2606.05846v1
- **作者**: Gio Paik, Hyunseo Shin, Soungmin Lee
- **备注**: ICML 2026 Workshop on Machine Learning for Audio
- **摘要**: 语码混合（Code-switching）语音识别因多语言资源匮乏而极具挑战。现有方法多依赖合成数据或特定语种对的微调，扩展性有限。本研究探讨了从有限的已知语种对中学到的语码混合能力是否能通过模型合并和领域泛化方法迁移到未见语种对。实验结果显示，合并后的双语模型在未见语种对上表现出适度的泛化能力，表明语码混合能力的跨语种对迁移仍存在局限。
- **PDF**: https://arxiv.org/pdf/2606.05846v1

### USAD 2.0: Scaling Representation Distillation for Universal Audio Understanding
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06444v1
- **作者**: Heng-Jui Chang, Alexander H. Liu, Saurabhchand Bhati, et al.
- **备注**: Accepted to Interspeech 2026
- **摘要**: 我们提出了 USAD 2.0，这是一个整合了自监督学习（SSL）和有监督基础模型知识的通用音频编码器。该模型通过领域感知蒸馏解决了教师模型不匹配问题，扩展到了音乐领域，并增加了第二阶段的有监督蒸馏。通过深度缩放，我们将模型扩展到了10亿参数。实验表明，USAD 2.0 在探测任务和基于大语言模型的评估中均达到了顶尖性能。
- **PDF**: https://arxiv.org/pdf/2606.06444v1

### Impact of RTK Augmentation and INS Integration on GNSS Positioning Accuracy and Continuity: A Benchmarking Study on Inland Waterways
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06358v1
- **作者**: Yan-Yun Zhang, Jef Billet, Jan Swevers, Peter Slaets
- **备注**: 8 pages. Accepted to CCTA 2026
- **摘要**: 在内河航道中，桥梁等结构会影响GNSS信号和RTK改正数的可用性。本研究对集成RTK和INS的GNSS接收机进行了基准测试。结果表明，桥下改正数丢失会导致定位精度下降和状态跳变。虽然INS能支持短期连续性，但会引入漂移。研究强调了在内河航道应用中，需要更高级的状态估计来实现空间连续且不确定性一致的定位。
- **PDF**: https://arxiv.org/pdf/2606.06358v1

### FiLM-Based Speaker Conditioning of a SpeechLLM for Pathological Speech Recognition
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06211v1
- **作者**: Fernando López, Santosh Kesiraju, Jordi Luque
- **备注**: Accepted in Odyssey 2026
- **摘要**: 针对神经系统疾病导致的病理语音识别难题，本研究采用特征线性调制（FiLM）进行说话人条件化。通过在冻结的ASR编码器层中注入x-vector信息，无需修改基础模型权重即可使模型适配个体患者。在西班牙语和英语数据集上的实验表明，该方法在病理语音识别上具有竞争力，同时保留了模型处理正常语音及回答语音相关问题的能力。
- **PDF**: https://arxiv.org/pdf/2606.06211v1

--- 
## 📚 学科: `q-bio.*`
本周论文集中在生物信息学与人工智能的交叉领域，涉及视觉表征中的特征绑定问题、AI辅助药物靶点发现、生物分子序列与结构的协同设计，以及利用强化学习模拟人工视觉修复。这些研究利用了Transformer、扩散模型和流匹配等前沿技术解决生物学核心问题。

### Formalizing the Binding Problem
- **分数**: 6
- **链接**: https://arxiv.org/abs/2606.03976v1
- **作者**: Lianghuan Huang, Yihao Li, Saeed Salehi, et al.
- **备注**: Accepted to ICML 2026
- **摘要**: “绑定问题”（Binding Problem）探讨系统如何识别哪些特征属于同一物体。本文通过信息论方法形式化了该问题，并引入了一种探测方法来测量深度学习模型（如ViT）表征中的绑定信息。实验显示，绑定信息是实现强大视觉识别和推理的关键。研究揭示了现有架构在处理具有共享特征或遮挡的场景时如何整合物体属性。
- **PDF**: https://arxiv.org/pdf/2606.03976v1

### Site4Drug: Predicting Drug-Binding Target Sites with an AI Agent
- **分数**: 6
- **链接**: https://arxiv.org/abs/2606.01816v1
- **作者**: Taehan Kim, Sarrah Rose Mikhail Leung, Bharat Mekala, et al.
- **备注**: Accepted to ICML 2026 Workshop on GenBio
- **摘要**: 选择蛋白质上的干预位点往往是药物研发的瓶颈。Site4Drug 是一个模态感知型位点发现智能体，它能输出带约束、证据摘要和风险标志的候选区域排名列表。该智能体能够根据拓扑结构、PTM倾向等证据推荐结合模态（如抗体 vs 小分子），避免选择化学上可行但在生物学上被遮蔽的位点。
- **PDF**: https://arxiv.org/pdf/2606.01816v1

### Demystifying Multimodal Biomolecular Co-design With Intrinsic Geodesic Coupling
- **分数**: 6
- **链接**: https://arxiv.org/abs/2606.01628v1
- **作者**: Keyue Qiu, Xintong Wang, Zhilong Zhang, et al.
- **备注**: Accepted to ICML 2026
- **摘要**: 蛋白质和小分子等生物分子的序列与三维结构紧密相关。现有的生成模型往往假设固定的同步耦合。本文提出 GeoCoupling 框架，通过优化异构模态之间的时间耦合来提高生成质量。在基于结构的药物设计和非条件蛋白质设计中的实验证明，学习到的耦合优于同步耦合，生成的分子具有更好的物理有效性和多样性。
- **PDF**: https://arxiv.org/pdf/2606.01628v1

### Multimarginal flow matching with optimal transport potentials
- **分数**: 4
- **链接**: https://arxiv.org/abs/2606.05327v1
- **作者**: Raghav Kansal, David Crair, Nghia Nguyen, et al.
- **备注**: Accepted to ICML 2026
- **摘要**: 流匹配（Flow matching）是学习两个分布间动态传输图的有力工具。本文针对具有中间观测边缘分布的“多边缘”场景，提出了一种利用动态最优传输（OT）势能项的方法。通过扩展条件流匹配目标，推导出一种高效的免模拟算法，并在单细胞RNA测序、海洋学和气象学数据集上展示了领先的性能和训练效率。
- **PDF**: https://arxiv.org/pdf/2606.05327v1

### Learning to See via Epiretinal Implant Stimulation in silico with Model-Based Deep Reinforcement Learning
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.03118v1
- **作者**: Jacob Lavoie, Marwan Besrour, William Lemaire, et al.
- **备注**: Published in Biomed. Phys. Eng. Express
- **摘要**: 本研究探讨利用深度强化学习（RL）优化视网膜植入物的电刺激方案，以恢复患者视觉。由于电刺激会产生拉长的各向异性形状，RL智能体被训练用于组装这些形状以形成清晰的图像。通过在虚拟病人环境 rlretina 中训练，智能体生成的图像比传统方法更易识别，为提高人工视力中的视锐度迈出了第一步。
- **PDF**: https://arxiv.org/pdf/2606.03118v1

--- 
## 📚 学科: `cs.*`
计算机科学领域的精选论文探讨了离散扩散语言模型的检索增强技术、人类与大模型在科学探索中的行为差异、高性能FPGA架构设计以及将工程CAD特征引入深度学习的表示方法。整体反映了AI技术在自然语言处理、系统架构及工程设计自动化中的深度融合。

### Self-Augmenting Retrieval for Diffusion Language Models
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06474v1
- **作者**: Paul Jünger, Justin Lovelace, Linxi Zhao, et al.
- **备注**: ICML 2026
- **摘要**: 离散扩散语言模型通过并行去噪生成文本。本研究发现，去噪过程中丢弃的低置信度Token实际上是很有用的检索信号。我们提出了 SARDI 框架，在去噪过程中利用这些预判 Token 引导检索。SARDI 无需训练且适用于任何具有推理能力的离散扩散模型，在多步问答基准测试中优于现有的检索基线，且吞吐量提高了8倍。
- **PDF**: https://arxiv.org/pdf/2606.06474v1

### Human Adults and LLMs as Scientists: Who Benefits from Active Exploration?
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06464v1
- **作者**: Mandana Samiei, Eunice Yiu, Anthony GX-Chen, et al.
- **备注**: Accepted at CogSci 2026
- **摘要**: 在因果学习中，成年人通常难以识别合取因果规则。本研究通过主动探索任务发现，当赋予人类自主权时，其推理能力显著提升。研究还对比了大语言模型，发现顶级模型虽然在推理准确度上接近人类，但在探索效率上较低，且同样存在合取-析取性能差距。
- **PDF**: https://arxiv.org/pdf/2606.06464v1

### Modeling, Optimizing and Exploring Multi-Die FPGA Routing Architectures
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06421v1
- **作者**: Amirhossein Poolad, Soheil Gholami Shahrouz, Andrew Boutros, Vaughn Betz
- **备注**: Accepted to FPL 2026
- **摘要**: 本文增强了开源FPGA CAD工具VTR，以建模2.5D和3D多芯片FPGA的路由架构。通过基于HSPICE的电路建模，研究了芯片间连接密度、延迟和布线能力。结果显示，优化的3D FPGA相比2D设备可减少14%的线长并提升6%的频率。所有扩展均已开源并集成至VTR主分支。
- **PDF**: https://arxiv.org/pdf/2606.06421v1

### Bridging CAD and Data-Driven Design: Attributed Feature Graphs for Engineering Design
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06405v1
- **作者**: Abhishek Indupally, Ibraheem Alawadhi, Satchit Ramnath, Jami J. Shah
- **备注**: Accepted to ASME IDETC-CIE 2026
- **摘要**: 传统数据驱动设计往往丢弃参数化语义。本研究引入了属性特征图（AFG），将CAD特征（如拉伸、加强肋）编码为节点及其关系为边。AFG保留了设计意图并兼容图神经网络。案例研究显示，该模型能准确预测性能指标，并允许工程师将预测结果直接映射回特定的CAD特征进行修改。
- **PDF**: https://arxiv.org/pdf/2606.06405v1

--- 
## 📚 学科: `math.*`
_本周缺少高价值论文_

--- 
## 📚 学科: `astro-ph.*`
天文学领域的精选论文涉及猎户座星团的演化规律、太阳光谱线的物理建模、系外行星系统中的动力学共振以及遥远类星体中的相对论性流。这些研究利用了Gaia卫星的高精度天文测量数据、高分辨率光谱分析以及复杂的N体模拟技术。

### Dynamical evolution and dissolution timescale of young stellar clusters in the Orion star-forming complex
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06457v1
- **作者**: Sergio Sánchez-Sanjuán, Ángeles Pérez-Villegas, et al.
- **备注**: Accepted for publication in MNRAS
- **摘要**: 本文结合Gaia DR3数据分析了猎户座恒星形成区的13个年轻星团。通过N体模拟，发现这些星团分为两类：一类演化受银河系势场调节，可作为疏散星团长期存在；另一类则受内部动力学主导，将在1.2亿年内解散并填充银河系恒星场。研究展示了初始条件的异质性如何产生不同的演化路径。
- **PDF**: https://arxiv.org/pdf/2606.06457v1

### Depolarization and Polarization-Transfer Rates for Solar He I Lines due to Collisions with Neutral Hydrogen
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06433v1
- **作者**: Moncef Derouich, Saleh Qutub
- **备注**: Accepted for publication in Astronomy & Astrophysics
- **摘要**: 中性氦（He I）谱线广泛用于太阳诊断。本研究计算了He I原子与中性氢碰撞导致的消偏振和极化转移率，涵盖了主要的太阳He I诊断线（如10830 Å）。这些精确的碰撞参数对于太阳光谱极化建模和磁场诊断具有重要意义。
- **PDF**: https://arxiv.org/pdf/2606.06433v1

### gr8stars II : judgement day for spectroscopic parameter model systematics
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06234v1
- **作者**: Alix Violet Freckelton, Annelies Mortier, et al.
- **备注**: Accepted for publication in MNRAS
- **摘要**: 精确的恒星参数对系外行星研究至关重要。本研究利用5种光谱分析方法处理了585颗类太阳恒星。研究发现不同方法得到的温度和金属丰度差异显著大于随机误差。这种系统误差会传播到行星质量和半径的测量中，研究给出了行星平衡温度不确定性的下限约为4%。
- **PDF**: https://arxiv.org/pdf/2606.06234v1

### Peas and USPs: Can Stellar Spindown and Peas in a Pod Replicate Ultra-Short-Period Planet Characteristics?
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06230v1
- **作者**: Adam Distler, Juliette Becker
- **备注**: Accepted in ApJ
- **摘要**: “豆荚里的豌豆”（PIAP）系统具有规律的行星间距。本文研究了恒星自转减慢产生的动力学共振如何影响这些系统。研究发现，仅靠恒星自转减慢不足以解耦规律间距的PIAP系统，必须伴随最内侧行星的向内迁移。这一框架可用于测试行星迁移路径和初始恒星倾角。
- **PDF**: https://arxiv.org/pdf/2606.06230v1

### A New Member of the Fast and Furious Family: A Relativistic and Time-Variable UV Outflow in a Luminous Quasar
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.06226v1
- **作者**: Lucas M. Seaton, Patrick B. Hall, et al.
- **备注**: Published in the Astrophysical Journal
- **摘要**: 我们报告了一个极高速度的类星体流，其速度高达光速的30%（约90,000 km/s）。该流在二十年的光度观测中表现出明显的变率。这种超高速流的存在挑战了现有的加速模型，且其动能释放足以对宿主星系产生显著的反馈影响。
- **PDF**: https://arxiv.org/pdf/2606.06226v1

--- 
## 📚 学科: `stat.*`
本周统计学领域的论文关注了高维数据的因果影响评估、表格数据的基石模型构建、网络模型选择的方法论综述以及金融高频数据的流式分析。这些工作将传统的统计推断理论与现代高效计算架构结合，解决了如大数据集子集影响分析和高维小样本预测等实际难题。

### Finding Most Influential Sets
- **分数**: 6
- **链接**: https://arxiv.org/abs/2606.05919v1
- **作者**: Lucas D. Konrad, Nikolas Kuschnig
- **备注**: Published as a conference paper at ICML 2026
- **摘要**: 识别对估算结果影响最大的大小为 $k$ 的子集（MIS）通常因搜索空间巨大而难以实现。本文证明对于线性分式效应，MIS选择可以简化为一系列Top-k问题，并提出了一种 $\mathcal{O}(n)$ 复杂度的算法。实验表明，该方法能找回以前在计算上无法触及的全局最优影响子集。
- **PDF**: https://arxiv.org/pdf/2606.05919v1

### GOTabPFN: From Feature Ordering to Compact Tokenization for Tabular Foundation Models on High-Dimensional Data
- **分数**: 6
- **链接**: https://arxiv.org/abs/2606.05441v1
- **作者**: Al Zadid Sultan Bin Habib, Md Younus Ahamed, et al.
- **备注**: Accepted to ICML 2026
- **摘要**: 本研究探讨如何使小型表格基石模型在“高维小样本”（HDLSS）场景下有效。我们提出了图引导排序（GO-LR）和神经启发亚基压缩（NSC）单元，将相邻的特征压缩为元特征，实现了紧凑的表征。该方法在有限的Token预算下显著提高了TabPFN类模型的预测精度和稳定性。
- **PDF**: https://arxiv.org/pdf/2606.05441v1

### Network model selection: A review of methods
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.05954v1
- **作者**: Zoran Levnajić
- **备注**: Book chapter version (Springer 2026)
- **摘要**: 理解复杂网络的演化机制是网络科学的核心。本书系统回顾了网络模型选择的方法，将其分为四大类，并提供了软件可用性信息和未来方向探讨。它是首个全面梳理该领域最前沿方法的学术资源，对网络科学领域的研究者具有重要价值。
- **PDF**: https://arxiv.org/pdf/2606.05954v1

### Zero-Copy Semantic Contagion: An In-Memory Streaming Architecture for Evolving Attention Graphs
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.05733v1
- **作者**: Kabir Murjani
- **备注**: Accepted to SIGMOD Workshop (FinDS 2026)
- **摘要**: 本文引入了一种基于Rust和Python的混合流处理架构，通过新闻文本实时构建跨公司注意力图。利用零拷贝解析和神经霍克斯过程，系统能以毫秒级延迟捕捉供应链波动引发的股价传导信号。实验证明，相比于单资产模型，该架构能大幅提升收益率预测的精准度。
- **PDF**: https://arxiv.org/pdf/2606.05733v1

--- 
## 📚 学科: `econ.*`
经济学领域在本周探讨了数据子集影响力的算法优化、算法定价中的策略选择以及去中心化金融（DeFi）中价格预言机的鲁棒性。研究反映了计量经济学与算法博弈论的交汇，特别是在应对算法共谋和链上资产操作安全性方面的理论创新。

### Finding Most Influential Sets
- **分数**: 6
- **链接**: https://arxiv.org/abs/2606.05919v1
- **作者**: Lucas D. Konrad, Nikolas Kuschnig
- **备注**: ICML 2026
- **摘要**: 本文提出了一种高效算法来识别对目标估计值（如因果效应）影响最大的样本观测子集。通过将搜索问题转化为Top-k优化，该方法解决了大样本下的计算瓶颈。这在经济学研究中对验证结果的鲁棒性和识别异常点具有重要意义。
- **PDF**: https://arxiv.org/pdf/2606.05919v1

### Should Demand Models Incorporate Competitor Prices? Oblivious Learning and Algorithmic Collusion
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.05363v1
- **作者**: Yuhang Wu, Assaf Zeevi
- **备注**: Preliminary version accepted at EC 2026
- **摘要**: 在多卖方平台上，定价算法是否应考虑竞争对手的价格？尽管“刻意忽略”可能促进短期获利，但研究表明这种做法并不稳健。通过刻画市场动态，我们发现纳入竞争信息并辅以充分的价格探索才是唯一纳什均衡。总体而言，长期共谋模式难以通过简单的忽略模型来维持。
- **PDF**: https://arxiv.org/pdf/2606.05363v1

### Cost of Manipulation in AMM-Based Oracles
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.03548v1
- **作者**: Sebastian Müller, Nordine Moumeni, Adel Messaoudi
- **备注**: Published at DeFi Workshop of FC'26
- **摘要**: 本文研究了基于自动做市商（AMM）的链上预言机的抗操纵能力。通过定义“操纵成本”，研究推导了单池和多池架构下的操作公式。结果表明，使用流动性权重的中位数聚合方式能最大限度地提高攻击成本。该工作为DeFi协议提供了定量化评估安全风险的准则。
- **PDF**: https://arxiv.org/pdf/2606.03548v1

---