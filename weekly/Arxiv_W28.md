# 🗓️ 周报 (2026-W28)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-07-12

--- 
## 📚 学科: `eess.*`

本次 eess.* 学科精选的 5 篇论文主要聚焦于通信、信号处理及安全监测技术。其中包括利用里德堡原子接收器（Rydberg atomic receiver）提升下一代无线通信性能的两篇前沿研究，分别解决了高速移动场景下的多普勒频移自适应跟踪和高信噪比条件下的统一物理信道建模问题；在安全监控与异常检测方面，有两篇研究针对海上关键基础设施（如海底电缆、船舶轨迹）开发了基于卡尔曼滤波、概率路网等结合几何与物理模型的检测框架；最后，在语义通信领域，提出了一种针对块擦除信道的高鲁棒性神经视频联合源信道编码（JSCC）框架。这些成果在提升现代通信系统鲁棒性与空间监控安全性方面具有重要应用价值。

### Doppler-Resilient Rydberg Atomic Receiver for High-Dynamic Communication Networks via Adaptive Local Oscillator Tracking
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08145v1
- **作者**: Yiyue Xiang, Jianxiong Pan, Qiaolin Ouyang, Bichen Kang, Bin Qi, Neng Ye
- **备注**: Accepted by ISICN 2026
- **摘要**: 里德堡原子接收器因其卓越的灵敏度以及克服传统射频天线物理限制的能力，已成为下一代无线通信非常有前途的候选方案。里德堡原子接收器利用原子能级的共振响应进行信号检测，固有地受限于狭窄的瞬时带宽。然而，在卫星通信等高移动性场景中，严重的多普勒效应会引发载波频率偏移，从而使信号超出瞬时带宽并导致严重失真。在本文中，我们提出了一种自适应局部振荡器（LO）跟踪里德堡原子接收器架构，旨在将高动态信号锁定在有效的原子响应带宽内。通过采用交叉乘积自动频率控制（CPAFC）算法，系统动态估计瞬时频率偏移，生成相应的误差控制信号，并通过反馈回路调节 LO 频率。因此，无论动态变化如何，中频信号都可以始终锁定在靠近原子响应带宽中心的位置。仿真结果表明，所提出的架构显著优于现有的里德堡原子接收器，有效减轻了高动态环境中的性能退化。
- **PDF**: https://arxiv.org/pdf/2607.08145v1

### Unified Analytical Model for Atomic Receivers Under Typical Quantum Interference Paths
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08118v1
- **作者**: Yiyue Xiang, Neng Ye, Qihao Peng, Pei Xiao, Jianping An
- **备注**: Accepted by IEEE ISIT 2026
- **摘要**: 原子接收器利用被称为电磁诱导透明（EIT）的量子相干效应进行射频（RF）到光信号的转换，为下一代无线通信提供了一种革命性的范式。然而，目前的信息论表征主要局限于 Ξ 型 EIT 路径，且严重依赖弱探测近似，这无法预测原子接收器在高信噪比条件下的行为。在本文中，我们为原子接收器建立了一个统一的解析模型，并将该模型应用于三种典型的量子干涉路径，即 V 型、Λ 型和 Ξ 型配置。为了提供通用的表征，我们提出了量子相干转移系数（QCTC），使用基于三能级 EIT 稳态解的微扰框架来对原子接收器引起的等效信道响应进行建模。然后推导出了三种路径下等效信道增益的闭式表达式。我们的研究结果为未来原子无线电通信中的容量分析和波形优化提供了解析基础。
- **PDF**: https://arxiv.org/pdf/2607.08118v1

### Geometry-Informed Maritime Anomaly Detection Using Probabilistic Roadmaps
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08100v1
- **作者**: Gabriele Oliva, Andrea Tomei, Roberto Setola
- **备注**: Accepted for MED2026 conference, to appear
- **摘要**: 海上异常检测对于航行安全和保护关键水下基础设施至关重要。本文提出了一种基于几何信息的监督学习框架，用于使用自动识别系统（AIS）数据检测波罗的海中的异常船舶轨迹。在可航行海洋区域上构建概率路网（PRM），并将其作为结构先验将轨迹投影到可行通道上。这种表示方法能够提取可解释的航程级特征，从而捕获航线效率、偏离标称路径的几何偏差、运动学变异性以及与海底电缆的距离。为了解决标记异常事件稀缺的问题，通过受控的轨迹微扰和感知基础设施的失真生成了合成异常，从而产生用于监督训练的平衡数据集。在此特征集上训练随机森林分类器，并在交叉验证和预留测试集下进行评估。实验结果表明，该方法具有稳定的泛化性能，测试 ROC AUC 达到 0.837，表明将航行可行性约束嵌入异常检测过程中的有效性。所提出的方法为几何复杂环境下的基础设施感知型海上监控提供了一个可解释且具有操作相关性的框架。
- **PDF**: https://arxiv.org/pdf/2607.08100v1

### Model-Based Detection of Anomalous Events in Submarine Cables Using Distributed Deformation Sensing and Kalman Filtering
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08099v1
- **作者**: Camilla Fioravanti, Bianca Mazza, Marta Menci, Gabriele Oliva, Roberto Setola
- **备注**: Accepted for MED2026 conference, to appear
- **摘要**: 海底电力和电信电缆构成了关键的全球基础设施，但它们仍然容易受到海上活动和蓄意破坏造成的机械损伤。因此，对这些资产进行持续监控对于尽早发现异常事件至关重要。本文提出了一个基于模型的框架，用于利用沿电缆的空间分布式变形测量来实时检测海底电缆的异常。电缆被建模为一个受具有固定边界条件的阻尼波动方程控制的受拉结构。通过空间离散化获得有限维状态空间表示，从而能够使用卡尔曼滤波器来估计在随机环境干扰下电缆的动态状态。然后，将异常检测表述为应用于滤波器新息序列的统计假设检验。与纯数据驱动的警报相比，所提出的框架提供了一个可解释的残差信号，其阈值可以与规定的误报概率相关联。数值模拟表明，所提出的框架可以可靠地识别局部干扰，同时对周围环境激发保持鲁棒性。
- **PDF**: https://arxiv.org/pdf/2607.08099v1

### Towards Robust Semantic Video Transmission over Block Erasure Channels
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.07823v1
- **作者**: Nargis Fayaz, Homa Esfahanizadeh, Matin Mortaheb, Jinfeng Du, Harish Viswanathan
- **备注**: accepted and will be presented at IEEE VTC FALL 2026
- **摘要**: 本文研究了在块擦除信道上进行鲁棒视频传输的语义感知神经联合源信道编码（JSCC）。我们提出了一个同时探索空间域和特征域设计的神经视频压缩框架。在空间域中，视频帧被划分为块，通过均匀擦除和两级语义引导的非均匀擦除策略，实现局部的擦除处理和细粒度的鲁棒性控制。在特征域中，潜特征被划分，使缺失特征能够在保持整体空间一致性的同时进行语义恢复。全面的实验量化了在不同均匀和非均匀擦除概率下的重建质量。我们的结果表明，空间域 JSCC 擅长处理随机局部丢失，而特征域 JSCC 对分布式擦除提供了优异的鲁棒性，并在低损耗场景下保持了高保真度。该分析强调了空间连续性与语义冗余之间的权衡，为设计鲁棒的、任务感知的视频视频通信系统提供了见解。
- **PDF**: https://arxiv.org/pdf/2607.07823v1

--- 
## 📚 学科: `q-bio.*`

本次 q-bio.* 学科精选了 1 篇发表于 BIOKDD 2026 的高质量计算生物学论文，探讨在精准肿瘤学中如何预测个性化药物的治疗反应。研究提出了名为 PREDIKTOR 的多视图机器学习框架，创新性地将基于患者个体基因调控网络的“机制图谱视图”与模拟药物诱导转录组改变的“扰动视图”通过对比学习进行对齐。该模型在 TCGA 数据集以及实际临床试验中表现出卓越的泛化与零样本迁移能力，并提供了高可解释性的基因与通路机制分析。

### Predicting Therapeutic Outcome via Aligning Patient-Specific Knowledge Graph and Gene-Level Perturbation Representations
- **分数**: 6
- **链接**  https://arxiv.org/abs/2607.04557v1
- **作者**: Dongmin Bang, Sugyun An, Inyoung Sung, Ilho Yun, Sun Kim, Sangseon Lee
- **备注**: 12 pages, 5 figures, 5 tables. Accepted at BIOKDD 2026, held in conjunction with ACM SIGKDD 2026
- **摘要**: 从治疗前转录组准确预测患者特异性的治疗反应，受限于匹配的临床反应标签和治疗后分子谱的稀缺。临床前迁移学习模型可以模拟药物诱导的表达变化，但通常难以解释且不稳定，而知识图谱方法虽然提供了机制背景，但仍是静态的，无法捕捉药物诱导的转录组扰动动力学。我们提出了 PREDIKTOR，一个以患者为中心的多视图框架，它将个性化网络视图与可迁移的转录组扰动视图相对齐，以预测临床药物反应。对于每位患者，我们利用 DysRegNet 从肿瘤表达中构建个性化的基因调控网络，并使用 DrugBank 的药物-靶点链接进行增强；图神经网络编码器产生一个以药物为中心、具有机制基础的嵌入。与此同时，在 LINCS L1000 上预训练的冻结特定条件基因-基因注意力模型，为同一患者-药物对生成模拟的扰动后转录组谱。我们通过带有药物上下文硬负样本的 CLIP 式对比目标，在共享潜空间中对齐这两个视图，然后拼接这些表征进行端到端反应分类。在 TCGA 数据集上，PREDIKTOR 在患者、药物和组织划分的评估中均一致优于最先进的基线模型，并能零样本迁移到 I-SPY2 临床试验，相比竞争方法将 AUROC 提高了 5.6%。对齐的嵌入产生稳定的基因和通路归因，恢复了已知机制，支持具有可操作性和可解释性的精准肿瘤学。
- **PDF**: https://arxiv.org/pdf/2607.04557v1

--- 
## 📚 学科: `cs.*`

本次 cs.* 学科精选的 3 篇论文涵盖了计算机视觉、大语言模型机理以及多模态教育媒体分析。具体包括：（1）Wat3R 框架：成功解决了在缺乏水下三维标注数据的情况下，进行水下 3D 重建和多视图深度估计的难题；（2）针对大模型“超级权重（Super Weights）”的精细研究：挑战了传统直觉，证明即使有些参数在剪枝时表现得极其重要，对其进行孤立微调反而会导致模型性能崩溃，微调必须依赖于整层上的低秩等结构化分解；（3）多模态社交媒体分析：通过 YouTube 语料研究 ChatGPT 在非正式教育传播中的呈现方式，揭示了“快速输出导向”内容更易获得流量但缺乏教学深度的结构性矛盾，引发了关于 AI 素养教育的深刻思考。

### Wat3R: Underwater 3D Geometry Learning without Annotations
- **分数**: 4
- **链接**  https://arxiv.org/abs/2607.08772v1
- **作者**: Jiangwei Ren, Xingyu Jiang, Zijie Song, Wei Xu, Hongkai Lin, Dingkang Liang, Xiang Bai
- **备注**: Accepted to ECCV 2026. The dataset and code are available at https://github.com/LSXI7/Wat3R
- **摘要**: 由于光线衰减、散射以及缺乏大规模、高质量的三维标注，在水下环境中估计三维几何形状带来了独特的挑战。先前的开拓性方法依赖于在水下环境中极不切实际的大规模密集标注。在本文中，我们提出了 Wat3R，这是一个跨域半监督学习框架，旨在使前馈三维重建模型从空气适应到水下场景。独特的是，我们的方法基于教师-学生架构，不需要任何标注的水下数据，仅在丰富的无标注真实水下视频片段上就能学习到鲁棒的几何表征。我们还设计了一个跨视图一致性损失，利用来自其他视图的几何线索来补偿由于水衰减和散射导致的当前视图中的信息降级。此外，考虑到缺乏全面的评估基准，我们构建了 Water3D，这是一个涵盖各种水体和水下场景的多样化数据集，旨在用于几何任务评估。实验结果表明，Wat3R 在水下多视图深度估计和点云重建中优于当前最先进的方法。
- **PDF**: https://arxiv.org/pdf/2607.08772v1

### Super Weights in LLMs and the Failure of Selective Training
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08733v1
- **作者**: Shreyas Subramanian, Adewale Akinfaderin, Akarsha Sehwag
- **备注**: Accepted at the Conference on Language Modeling (COLM) 2026
- **摘要**: 最近的研究发现了“超级权重（Super Weights）”，即那些一旦移除就会使模型性能下降几个数量级的单个参数。我们表明，这种由于剪枝超级权重引起的性能退化并不普遍适用于所有大语言模型（LLM）。此外，如果这些参数如此重要，那么感知超级权重的训练应该非常有效。但我们展示了相反的结果。在 OLMo-1B 和 OLMo-7B 上，孤立地训练超级权重（100 到 8,192 个参数）会将准确率降低到随机猜测的水平，而将其扩展到多达 36K 个参数的局部邻域也无法带来改善。这种失败是特定于超级权重坐标的：在相同的 down_proj 层中训练相同数量的随机选择位置，反而能比基线有所改善，因此崩溃来自于针对超级权重本身，而不是由于稀疏性。传统的 LoRA 通过低秩结构更新注意力权重矩阵中的每个位置，仅用 0.16% 的参数就取得了成功，并且对 down_proj 应用相同的低秩更新也同样成功。一项 10 个种子的消融实验证实，限制对应于超级权重坐标位置的 LoRA 更新，产生的结果在统计上无法区分。这些发现表明，参数的重要性并不意味着其在孤立状态下的可训练性，有效的微调依赖于整层上的结构化分解，而不是针对单独重要的权重。
- **PDF**: https://arxiv.org/pdf/2607.08733v1

### How YouTube Frames ChatGPT Use in Education: An Epistemic Network Analysis with Supporting Multimodal Metadata
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08698v1
- **作者**: Shayla Sharmin, Mohammad Al-Ratrout, Mohammad Fahim Abrar, Roghayeh Leila Barmaki
- **备注**: This paper has been accepted in ICMI 2026 and will be presented in October
- **摘要**: 我们通过转录文本、标题、缩略图和观众评论等多模态元数据来审查教育类 YouTube 视频，以调查 ChatGPT 在不同创作者群体中是如何被框架化的，以及这些框架化方式如何与观众反应和平台传播度相关联。目前对于在大语言模型是如何呈现给非正式、由创作者主导的公共舆论中的学习者，我们知之甚少。遵循 PRISMA 声明，我们选择了 52 个视频进行分析。我们确定了三个结构上不同的讨论群体：（G1）将 ChatGPT 定位为思考的认知脚手架的视频；（G2）导向检索练习和技能培养的视频；（G3）将 ChatGPT 框架化为内容生成工具的视频。认知网络分析（ENA）揭示了具有大效应量的显著群体差异。多模态元数据在视频文本、标题和缩略图中一致地反映了这些区别。偏向学习内容的视频观众将 ChatGPT 描述为思考伙伴或导师，而偏向输出生成视频的观众则对过度依赖、浅层学习和认知外包表示担忧。G3 获得了与 G2 相当的平台传播度，但其教学原理框架却大打折扣。这可能表明，尽管教学深度较低，输出导向的内容仍在竞争曝光率。这些发现揭示了自主 AI 学习中的结构性紧张关系：优先考虑快速输出的内容比促进深层参与的内容覆盖了多得多的学习者。这一差距引发了关键问题：到底是谁的 AI 素养愿景得到了推广，而学习者最终真正得到了什么。
- **PDF**: https://arxiv.org/pdf/2607.08698v1

--- 
## 📚 学科: `math.*`

本次 math.* 学科精选了 1 篇发表于 UAI 2026 的高水平数理统计与机器学习理论论文。该研究深入探讨了在未知标量仿射变换以及异方差噪声背景下的精确排列恢复（特征匹配）问题。作者提出了一种包含标准化和“对数最小和（LSL）”最小化的两步法，并证明了可以完美恢复排列所需的特征向量最小分离距离的严格非渐近理论边界。该成果为数据对齐、特征配准等统计与机器学习经典算法提供了坚实的数理理论支撑。

### Exact Permutation Recovery Under Unknown Scalar Affine Transformation
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08628v1
- **作者**: Tigran Galstyan, Avetik Karagulyan, Arshak Minasyan
- **备注**: 22 pages, 6 figures, accepted to UAI 2026
- **摘要**: 我们研究了当潜在的真实特征向量受到未知的标量仿射变换影响时，配对两组带噪声的特征向量的问题。我们的方法主要包含两个步骤。首先，我们对特征向量进行标准化以估计未知的标量仿射变换。随后，我们通过使用估计的变换来最小化两组观测值之间的对数最小和（LSL），从而估计排列。我们的主要结果表明，如果真实特征向量的最小分离距离缩放为 $\sqrt{ρ_σ} \vee (d\log n)^{1/4} \vee \sqrt{\log n}$（其中 $d$ 是环境维度，$n$ 是样本量，而 $ρ_σ$ 是噪声幅度的最大比例），则可以完美恢复未知的排列。有趣的是，在温和的异方差条件下，所获得的速度与非仿射设置下的速度一致。我们还进一步表明，存在一些需要更大最小分离距离才能实现完美恢复的配置。从极小极大化（minimax）的角度来看，后者使得配对问题相比于非仿射设置更具挑战性。因此，我们展示了在特征匹配问题中，标准化数据可以隐式地估计标量仿射参数。作为我们分析的一部分，我们证明了在存在异方差噪声幅度的情况下，仿射参数估计量的非渐近收敛边界。
- **PDF**: https://arxiv.org/pdf/2607.08628v1

--- 
## 📚 学科: `astro-ph.*`

本次 astro-ph.* 学科精选的 5 篇论文涵盖了致密天体物理、星际介质、高能天体物理与宇宙学观测等前沿领域。具体研究包括：（1）在全克尔时空中推导翘曲吸积盘方程，揭示了克尔裸奇点相比于黑洞在吸积盘内边缘所特有的“驼峰”偏转结构；（2）在金牛座无星核心 TMC-1 之外的极低光度天体分子云中，首次检测到了三环多环芳烃（PAH）“菲烯”，推进了对恒星形成早期阶段有机分子分布的认知；（3）推出了 VAPOLA —— 基于 ALMA 望远镜对活动星系核（AGN）与银心人马座 A* 进行多频段偏振监测的在线科学就绪级数据库；（4）通过大规模水动力模拟，验证了利用星系团的 X 射线与毫米波联合观测来无偏推导哈勃常数 $H_0$ 的方案可行性；（5）探究了低红移下超新星宿主星系中的活动星系核（AGN）活动，证实其并不会对 Ia 型超新星作为标准烛光的哈勃残差测距造成显著系统性偏差。

### Tilted thin accretion disks in the full Kerr spacetime and their implications
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08728v1
- **作者**: K. S. Sruthy, Chandrachur Chakraborty, Sudip Bhattacharyya
- **备注**: 25 pages, 17 figures, 2 tables, accepted for publication in Phys. Rev. D
- **摘要**: 我们在全克尔时空中推导出一个稳态翘曲盘方程，以研究自转塌缩天体周围薄粘滞吸积盘的倾斜动力学。该公式基于普林格（Pringle）框架，适用于所有克尔参数 $a$ 值，从而既包含了克尔黑洞（BHs；$0 < a \le 1$）也包含了克尔裸奇点（$a > 1$）。通过引入精确的开普勒和冷泽-蒂林（Lense-Thirring）进动频率，我们在不诉诸慢转动或弱场近似的情况下，解析地获得了吸积盘的径向倾斜轮廓。在现实边界条件下获得的所得方程的数值解表明，其与慢转动近似存在显著偏差，特别是在相对论效应占主导地位的内盘区域。在扩散机制中，我们发现对于克尔裸奇点，其倾斜轮廓在特定角动量消失的半径附近表现出独特的内部驼峰特征，而这一特征在克尔黑洞中是不存在的。考虑内盘的倾斜可能会显著影响对观测到的 X 射线光谱、时变和偏振特征的解释，这对于探测强引力场区域以及推断中心天体的自转至关重要。虽然仅凭这种独特的驼峰特征无法唯一地区分克尔黑洞与克尔裸奇点，但结合对吸积盘机制的限制来解释它们，可能会为观测吸积塌缩天体的物理性质提供一种潜在的物理手段。
- **PDF**: https://arxiv.org/pdf/2607.08728v1

### Detection of the Polycyclic Aromatic Hydrocarbon Phenalene (C$_{13}$H$_{10}$) in the Very Low Luminosity Object (VeLLO) MC27/L1521F
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08699v1
- **作者**: Gabi Wenzel, Thomas H. Speak, Ci Xue, Edwin A. Bergin, Andrew M. Burkhardt, Martin A. Cordiner, Miya Duffy, Zachary T. P. Fried, Andrew Lipnicky, Christopher N. Shingledecker, Reace H. J. Willis, Anthony J. Remijan, Michael C. McCarthy, Brett A. McGuire, Ilsa R. Cooke
- **备注**: Accepted for publication in The Astrophysical Journal Letters
- **摘要**: 迄今为止，在金牛座分子云内的无星致密核心 TMC-1 CP 中已检测到 14 种多环芳烃（PAHs），其尺寸从包含 2 到 7 个碳环（包括五元环和六元环）不等。它们的发现引发了关于冷星际介质（ISM）中 PAHs 分布及其在恒星形成过程中演化的疑问。在这里，我们展示了在 TMC-1 CP 之外对三环 PAH 的首次星际探测。我们在致密核心 MC27/L1521F 中检测到了菲烯（Phenalene，C$_{13}$H$_{10}$），这是一种紧凑的、周边稠合的多环芳烃。MC27/L1521F 是金牛座中的一个分子云，包含一个极低光度天体（VeLLO）。我们比较了菲烯在两个源中相对于单环芳香烃苯甲腈的丰度，发现它在 MC27/L1521F 中增强了四倍。我们讨论了两处源中可能形成和破坏路径的意义。这些发现进一步支持了 PAHs 在整个冷星际介质中的广泛丰度，并且与恒星形成最早阶段的存活、遗传或补充机制相一致。
- **PDF**: https://arxiv.org/pdf/2607.08699v1

### VAPOLA -- A multi-year, multi-band polarization survey of AGN and Sgr A* at mm wavelengths with ALMA I. Survey Overview and Science-Ready Archival Products
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08657v1
- **作者**: Alejandro Mus, Ciriaco Goddi, Douglas Carlos, Vincenzo Galluzzi, Ezequiel Albentosa-Ruiz, Ivan Martí-Vidal, Hugo Messias, Kazi L. J. Rygl, Geoffrey B. Crew, Lynn D. Matthews, Elisabetta Liuzzo, Nicola Marchili, Raphael P. Rolim, Mariafelicia De Laurentis, Rocco Lico, Cristiano Urban
- **备注**: Accepted in A&A, 07/06/2026
- **摘要**: 阿塔卡马大型毫米波/亚毫米波阵列（ALMA）是毫米和亚毫米波段最灵敏的干涉测量阵列。通过 ALMA 定相系统（APS），它可以参与全球甚长基线干涉测量（VLBI）阵列，从而提高其灵敏度和分辨率。然而，处理和分析在 VLBI 观测期间以 APS 模式获得的 ALMA 数据仍然是一项复杂的任务，需要专门的专业知识以及耗时的校准和成像步骤。在本文中，我们介绍了 VAPOLA——这是首个在线、多历元、多波段的存储库，包含了全球 VLBI 观测期间对活动星系核（AGN）和人马座 A*（Sgr A*）进行 ALMA 观测的高级数据产品。该存储库建立在自动处理完全校准的 ALMA（QA2）数据管道基础之上，能够在极少用户干预的情况下生成科学就绪的产品。它包括完全校准的干涉可视度、跨单个和合并光谱窗口的全斯托克斯图像、极化和光谱指数图，以及来自可视度域极化拟合的表格化极化参数。通过用户友好的网页门户提供即用型数据，VAPOLA 使非专业用户能够进行先进的科学分析，而无需掌握深奥的 ALMA 步骤。这一资源将促进广泛的科学调查，包括表征吸积流和相对论性喷流中的磁场特性、活动星系核中尘埃和分子星周环的结构和运动学，以及朝向银河系中心星际介质的吸收研究。此外，该数据集提供了源集成参数和校准元数据，这对于优化 VLBI 校准和成像工作流以及对超大质量黑洞及其环境的理论模型引入强有力的观测约束至关重要。
- **PDF**: https://arxiv.org/pdf/2607.08657v1

### The Three Hundred Project: validating $H_0$ inference from mock X-ray and millimetre analyses of galaxy clusters
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08613v1
- **作者**: F. De Luca, H. Bourdin, P. Mazzotta, E. Rasia, A. Kozmanyan, W. Cui, M. De Petris, D. de Andres, G. Yepes
- **备注**: Accepted for publication in A&A
- **摘要**: 星系团中热力学量的测量在不同程度上受到 X 射线和毫米波段中径向平均观测值简化建模的影响。这包括关于宇宙学模型和星系团内介质（ICM）形貌的假设。在从“The Three Hundred”流体动力学模拟中提取的大量星系团样本中，我们评估了由形貌假设引起的系统差异，这些差异预计存在于由 X 射线光谱学或联合 X 射线与毫米波成像推断出的 ICM 温度之间。我们发现这些差异显示出与星系团动力学和形貌指标相关的明确定义的统计行为。然后，我们研究了先验已知这种统计行为的星系团温度分布的联合推断，如何使我们能够约束从表观星系团尺寸推断出的宇宙学参数。假设平坦的 $Λ$CDM 模型以及关于 $Ω_\mathrm{m}$ 和氦丰度的先验，该方法为我们提供了哈勃常数 $H_0$ 的无偏估计。对于 100 和 1000 个星系团的样本，其精度分别约为 $4\%$ 和 $1.5\%$，并最终受限于约 $0.6$--$0.8\, {\rm km\, s^{-1} Mpc^{-1}}$ 的系统不确定性。这项工作突出了星系团样本的联合 X 射线和毫米波观测在对 $H_0$ 施加严密约束方面的巨大潜力。
- **PDF**: https://arxiv.org/pdf/2607.08613v1

### Active galactic nuclei are not responsible for systematics in the empirical properties of type Ia supernovae
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08604v1
- **作者**: Peter Clark
- **备注**: Published in RNAAS - This is an author compiled version. 3 Pages, 1 Figure
- **摘要**: 尽管作为关键的宇宙学基准，Ia 型超新星（SNe Ia）的经验属性仍受到重大系统不确定性的影响，其中最大的是它们的天体物理学及其与环境的联系。随着更大的观测样本降低统计不确定性，这些不确定性的相对重要性将会增加。在这里，我探索了在 Ia 型超新星宿主星系的一部分中存在活动星系核（AGN）是否可能是此类系统不确定性之一。利用 ZTF SNe Ia DR2 样本，我发现在低红移范围（z < 0.15）内，某些 SNe Ia 宿主星系中 AGN 的存在对其测量的哈勃残差并未产生显著的系统性影响。
- **PDF**: https://arxiv.org/pdf/2607.08604v1

--- 
## 📚 学科: `stat.*`

本次 stat.* 学科精选了 1 篇发表于 UAI 2026 的贝叶斯实验设计（BED）论文。该文针对基于策略的贝叶斯实验设计中期望信息增益（EIG）极难计算的“双重不可积性（double intractability）”这一经典计算瓶颈，创新性地提出了一种基于“分数匹配（Score Matching）”的解耦算法。该方法成功将策略优化过程中的乘性计算开销转化为加性开销，大幅减轻了策略训练的计算负担。该成果使得在深度神经网络架构搜索或超参数调优中，进行多次高效、低成本的贝叶斯策略实验设计训练成为可能。

### Bayesian Experimental Design via Score Matching
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.08335v1
- **作者**: Angus Phillips, Gavin Kerrigan, Tom Rainforth
- **备注**: Accepted for the 42nd Conference on Uncertainty in Artificial Intelligence (UAI 2026)
- **摘要**: 基于策略的贝叶斯实验设计（BED）方法允许学习深度策略网络，这些网络能够根据先前收集的数据自适应地做出智能设计决策。然而，此类策略的训练通常受到一个根本性挑战的阻碍：期望信息增益（EIG）的双重不可积性（double intractability）。这需要昂贵或复杂的近似，从而限制了人们在优化策略本身上投入的精力。为了解决这个问题，我们表明，通过首先解决与所用策略无关的分数匹配（score matching）问题，可以将 EIG 的双重不可积性从策略学习中分离开来，然后使用学习到的分数近似以单重不可积（singly intractable）的方式训练策略。这把关键的乘性计算成本转变成加性成本，减轻了策略训练本身的计算负担，使得在需要时多次训练策略的成本要低得多（例如进行架构搜索、超参数微调或避免局部最优）。在实验中，我们训练了多个极具竞争力的策略，而没有在似然评估中引入乘性成本，这允许我们在不进行超参数或架构搜索的情况下选择最佳策略，从而提高了整体性能。
- **PDF**: https://arxiv.org/pdf/2607.08335v1

--- 
## 📚 学科: `econ.*`

本次 econ.* 学科精选了 1 篇跨学科的物理经济学（Econophysics）论文。该研究创新地将物理学中的热平衡动力学引入到全球宏观经济与环境指标的分析中。通过对过去 40-50 年世界各国能源消耗和碳排放数据的实证分析，作者提出了“能源热平衡假设”（ENTH）。该理论证明了统计物理中的瑞利-金斯（Rayleigh-Jeans）凝聚现象可以极为精准地描述和预测不平等的洛伦兹与帕累托分布曲线。这一发现为研究全球资源分配不均与财富不平等提供了一种新颖的、基于统计物理学的微观建模范式。

### Thermodynamic description of worldwide distribution of energy and carbon emission
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.07315v1
- **作者**: Klaus M. Frahm, Dima L. Shepelyansky
- **备注**: 11 pages, 8 figures, may include certain unpublished parts of arXiv:2512.06420, arXiv:2506.17720, arXiv:2606.17965
- **摘要**: 基于公开数据，我们使用洛伦兹曲线和帕累托曲线，分析了过去 40-50 年间世界各国能源和碳排放的分布情况。在重新缩放的格式下，这些曲线在此时间段内保持了显著的稳定性，并以高基尼系数为特征，表明能源分布存在强烈的不平等。为了解释这些分布，我们引入了能源热平衡假设（ENTH），根据该假设，这些分布源于代表不同国家的智能体的瑞利-金斯（Rayleigh-Jeans, RJ）热平衡和凝聚。我们表明，该假设对上述历史时期数据中获得的洛伦兹曲线和帕累托曲线提供了极好的描述。它还为不平等现象提供了自然的依据，将其与低能量状态下的 RJ 凝聚联系起来。此外，我们还将其与世界财富不平等现象进行了类比。
- **PDF**: https://arxiv.org/pdf/2607.07315v1

---