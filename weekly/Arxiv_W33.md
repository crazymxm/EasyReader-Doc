# 🗓️ 周报 (2026-W33)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-08-16

--- 
## 📚 学科: `eess.*`
### The Impact of Temporal Context Length and Encoding Strategies on Self-Supervised ECG Representation Learning
- **分数**: 4
- **链接**  https://arxiv.org/abs/2608.12695v1
- **作者**: Ahmed Sameh, Ramzi Al-Sharawi, Yogatheesan Varatharajah
- **备注**: Accepted at the 48th Annual International Conference of the IEEE Engineering in Medicine and Biology Society (EMBC 2026). 6 pages, 2 figures, 1 table
- **摘要**: 自监督心电图（ECG）模型通常在几秒钟的ECG信号上进行训练，且越来越多地使用离散化的标记序列。目前尚不清楚这些选择是否牺牲了在现实世界动态记录中进行心律推断和纵向一致性所需的信息。我们在Icentia11k单导联数据集上进行了一项对照研究，改变了（i）输入时序长度（16秒、1分钟、5分钟和10分钟）和（ii）前端表示（连续卷积块嵌入 vs. 固定矢量量化标记），同时保持Transformer骨干网络和训练协议不变。我们通过下游异常心律检测和探究跨记录稳定性的患者级检索来评估学到的表示。结果表明，将时序上下文扩展到16秒片段以上可实现更强的迁移能力和更高的检索准确性，其中5分钟和10分钟的模型表现最佳，表明其能更好地捕捉缓慢变化的心律动态和个体特异性结构。在所有评估的时序长度中，连续块嵌入的性能均优于离散化标记，这表明量化可能会丢弃临床相关的波形细节。这些发现推动了在临床预测和基于相似性的应用中，强调扩展上下文和连续编码器的ECG基础模型的发展。我们的代码和预训练模型公开在 https://github.com/muha-0/ecg-ssl-representation-learning。
- **PDF**: https://arxiv.org/pdf/2608.12695v1

### Joint Communication-Control Strategy Optimization with Partially Nested Information Structures: The Linear-Quadratic Case
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13535v1
- **作者**: Haoyi You, Kaiqing Zhang
- **备注**: Preliminary version accepted to IEEE CDC 2026
- **摘要**: 本文在分散式随机控制的公共信息（CIB）框架下，公式化了具有二次成本的多智能体线性系统中的联合通信-控制策略优化（JCCO）问题。为了计算的可行性，我们重点关注具有部分嵌套（PN）信息结构（IS）的此类JCCO问题。特别地，在导致PN IS的基准通信协议下，我们建立了一系列条件，在这些条件下，待优化的（附加）通信策略可以保持部分嵌套性，而违反这些条件通常会导致开环通信策略中最佳策略的非线性。然后，我们开发了一种基于动态规划的方法，用以计算具有开环通信策略的JCCO的最优控制策略，从而产生了一组闭式Riccati方程。作为具有独立研究价值的副产品，该方法还提供了一种在CIB框架下解决具有PN IS和输出反馈的分散式线性二次控制的方法。最后，我们将该方法扩展到具有闭环通信策略的JCCO中，从而产生了一个比基于无限维CIB信念的动态规划更易于处理的动态规划。
- **PDF**: https://arxiv.org/pdf/2608.13535v1

### On the global feature importance for interpretable and trustworthy heat demand forecasting
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13039v1
- **作者**: Milan Zdravković
- **备注**: 9 pages, 5 figures. This preprint corresponds to the paper published in Thermal Science 2025 Volume 29, Issue 5 Part A, Pages: 3355-3365
- **摘要**: 本文引入了事前（ante-hoc）可解释人工智能（XAI）方法，以评估用于区域供热系统智能控制中热量需求预测的机器学习模型的全局特征重要性，旨在提高其可解释性和可信度，从而应对与遵守社区标准、客户满意度和责任风险相关的挑战。该方法包括使用四种不同的方法，即梯度提升法的固有可解释性以及选定的事后（post-hoc）方法，即部分依赖（Partial Dependence）、累积局部效应（Accumulated Local Effects）和SHAP。所选方法均不涉及特征排列或扰动，从而避免了因引入随机不切实际的数据实例值而导致的偏差。本文对结果进行了讨论，包括在适用情况下对互补性的评估，并在区域供热过程的背景下给出了具体的解释。
- **PDF**: https://arxiv.org/pdf/2608.13039v1

### Analysis of Motor Signatures of Social Adaptation in Autism for Efficient Human-Centric Systems
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.12548v1
- **作者**: Lara Pereira, Teresa Sousa, Miguel Castelo-Branco, João Ruivo Paulo
- **备注**: Accepted at IEEE SMC2026
- **摘要**: 舞蹈模仿融合了运动规划、感觉运动集成和社交认知，为表征自闭症患者的运动行为提供了一个敏感的框架。在这项工作中，我们探索了一个计算分析框架，以识别有助于设计和开发改进的医疗及人机系统的潜在生物标志物。我们分析了自闭症患者和神经典型（发育正常）成年人在单人以及社交框架下的双人条件下进行舞蹈模仿时的3D运动捕捉数据。在方法上，我们使用动态时间规整（DTW）量化了运动一致性，并提出了社交上下文敏感性指数（SCSI）来衡量社交框架对变异性的调节。然后，这些特征被用于分类器，以区分自闭症患者或神经典型组。结果表明，神经典型成年人在社交框架下的模仿中表现出更高的运动变异性，尤其是在上下肢，而自闭症成年人在不同情境下保持了运动的一致性。分类在区分组别方面达到了79.2%的均衡准确率。这些发现表明，运动模仿中的社交上下文敏感性构成了自闭症相关运动行为的强大生物标志物，强调了社交调节在运动评估中的重要性，并为包容性以人为本技术的发展提供了信息。
- **PDF**: https://arxiv.org/pdf/2608.12548v1

#### 📝 学科总结
本周 `eess.*` 学科挑选的论文主要聚焦于信号处理、智能控制和生物医学工程在医疗及工业系统中的应用。研究内容包括：利用自监督学习优化心电图（ECG）表征，探讨时序上下文长度与编码策略对诊断的影响；在多智能体系统中优化联合通信与控制策略，特别是在部分嵌套信息结构下的线性二次控制；引入可解释人工智能（XAI）方法来评估区域供热系统热需求预测模型的全局特征重要性，以提升系统可信度；以及通过3D运动捕捉数据和动态时间规整算法，分析自闭症患者在社交舞蹈模仿中的运动特征，为开发以人为本的辅助医疗系统提供客观的生物标志物。这些研究展示了控制理论与机器学习在解决实际物理和生理系统问题中的深度融合。

--- 
## 📚 学科: `q-bio.*`
### The Rosetta Stone and Levels of Principled Inference to the Experience of Another Mind
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.12030v1
- **作者**: Kallum Robinson, Giulio Tononi, Naotsugu Tsuchiya, Matteo Grasso
- **备注**: To appear in Qualia Structure. Springer Nature (forthcoming)
- **摘要**: 经典的“他心”（Other Minds）问题困扰了哲学家数千年：我们是否有办法真正理解另一个心灵的体验？我们通过亲身体验了解自己内在的经验，但对他人经验的认识只能通过外在描述，这两者之间存在着一道“熟识鸿沟”（acquaintance gap）。结构性方法旨在用数学结构来表征体验，并承诺提供一块“罗塞塔石碑”，即一种将体验内容转化为数学结构的系统方法。在本章中，我们研究了两种这样的方法——质感结构范式（Qstr）和整合信息理论（IIT），以探讨如果它们拥有所寻求的罗塞塔石碑，能让我们对另一个心灵做出何种推断。Qstr是现象间的（inter-phenomenally）方法，旨在通过一种体验与所有其他体验的关系来详尽地表征它，并为体验的同一性提供必要条件。IIT则是现象内部的（intra-phenomenally）方法，认为单一体验是由处于某种状态的基质所展开的因果效应结构所解释的，这是一种解释性同一性，对于体验的同一性而言既是必要条件也是充分条件。虽然这两种方法都无法跨越通往另一个心灵的“熟识鸿沟”，但它们提供了一个通用的形式化媒介，通过该媒介可以对不同的心灵进行比较，从而缩小了这一鸿沟。我们用范畴论中的结构对应层级来确定推断的强度。这些层级从同构、强伴随和弱伴随，一直递降到推断失效的系统极限。我们的结论是，这些结构性方法及其各自罗塞塔石碑的存在并不能解决他心问题，而是对我们可能做出的推断提供了一套有原则的约束系统，这远比以前能够证成的推断要多得多。
- **PDF**: https://arxiv.org/pdf/2608.12030v1

### Beyond Local Power: Functional Connectivity Analysis for Subject-Independent Learning Style Recognition
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.12000v1
- **作者**: Wiga Maulana Baihaqi, Indriana Hidayah, Sri Kusrohmaniah, Noor Akhmad Setiawan
- **备注**: 7 pages, 5 figures. Accepted for publication at 4th IEEE International Conference on Artificial Intelligence and Mechatronics Systems 2026
- **摘要**: 识别个人学习风格能够优化教学效果。传统的问卷调查是结构化的，而行为追踪方法则需要长期积累交互日志。为了克服这些时间限制，本文提出了一种客观的脑电图（EEG）方法，通过评估相位锁定值（PLV）连接性与局部特征，来识别主动-反思型（AR）和言语-视觉型（VV）Felder-Silverman维度的学习风格。在参与者进行瑞文高级推理测验任务期间，记录了28名参与者的脑电信号。支持向量机分类采用了留一法交叉验证（LOSO-CV）以及70:30的受试者内划分。由于明显的额枕极化，VV维度实现了70.00%的受试者级准确率。相反，AR维度的跨受试者泛化能力较低（55.56%），这是由于重叠的执行网络和“系统性神经逆转”现象，即稳定的个人连接特征与全局边界完全对立（投票差距高达20-0）。最终，这些结果表明，一刀切的固定分类器受到生物多样性的限制，强调了未来需要自适应特征转换技术来弥合跨受试者泛化差距。
- **PDF**: https://arxiv.org/pdf/2608.12000v1

### $\texttt{DisMorph}$: learning to disentangle technical distortions from true biological change
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.08173v1
- **作者**: Jingru Fu, Kathleen E. Larson, Douglas N. Greve, Bruce Fischl, Malte Hoffmann
- **备注**: 11 pages, 6 figures, longitudinal morphometry, deformable registration, neuroimaging, domain randomization, gradient non-linearity distortion, accepted by the SASHIMI Workshop at MICCAI 2026
- **摘要**: 纵向核磁共振成像（MRI）能够敏感地测量脑结构变化，用于研究衰老和神经退行性疾病。形变图像配准是通过计算捕捉纵向扫描之间几何差异的密集变形来估计此类变化的关键工具。然而，MRI扫描仪会引入因采集系统和协议而异的几何畸变，例如梯度非线性（GNL）畸变。现有的配准方法估计的单一变形场混淆了生物和技术效应，如果畸变未得到（部分）校正，可能会使下游形态测量产生偏差。我们提出了$\texttt{DisMorph}$，这是一个完全在合成数据上训练的配准框架，它显式地将纵向变形分解为技术和解剖变换。它预测两个密集的变形，每个变形编码一种效应。在训练期间，一种新型生成模型分别合成这两种效应以提供解耦监督，而领域随机化则促进了跨成像协议的泛化。我们在三种互补的设置中评估了我们的方法。在已知地面真值的模拟数据上，我们的方法比传统配准更准确、更一致地检测解剖变化。在仅因GNL畸变而异的真实图像对上，我们的方法将大部分几何变化归因于畸变场，证明了在没有解剖变化时的特异性。在纵向阿尔茨海默病（AD）图像对上，我们的方法检测到了AD相关脑结构的解剖变化，同时识别出了标准校正后残留的畸变。通过在纵向变形中将MRI诱导的畸变与生物学变化分离开来，我们的方法为临床环境中（保持采集一致性具有挑战性）更准确的纵向形态测量奠定了基础。
- **PDF**: https://arxiv.org/pdf/2608.08173v1

#### 📝 学科总结
本周 `q-bio.*` 学科挑选的论文涵盖了理论神经科学、认知科学以及神经影像计算的前沿进展。第一篇论文探讨了通过质感结构（Qstr）和整合信息理论（IIT）等数学结构方法来推断和理解“他心”体验哲学难题的可行性。第二篇研究了基于脑电图（EEG）功能连接性（PLV）客观识别个人学习风格的方法，指出了脑网络重叠与个体生物多样性对跨受试者分类泛化性的挑战。第三篇提出了一种名为 `DisMorph` 的解耦配准框架，该框架能够从纵向MRI形变中分离出设备产生的梯度非线性几何畸变与真实的脑结构解剖病理变化，从而显著提升阿尔茨海默病等病症形态测量的精确度。这些论文展示了计算方法与定量模型在解析复杂大脑功能、认知状态及临床神经影像分析中的强大潜力。

--- 
## 📚 学科: `cs.*`
### HumanTracker: Towards Comprehensive and Human-Aligned Motion Tracking Benchmark
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13555v1
- **作者**: Dairu Liu, Zekun Qi, Jiayu Zeng, Ruixi Yu, Yu Guan, Yintianrun Zhang, Xuchuan Chen, Sikai Liang, Zekai Li, Chenghuai Lin, Xinqiang Yu, Wenyao Zhang, He Wang, Li Yi
- **备注**: Accepted to ECCV 2026
- **摘要**: 仿人运动跟踪对于远程操作和全身模仿至关重要，但评估结果往往与人们在视频中感知到的不一致。运动学误差虽然能计算每帧姿态的平均差异，但遗漏了最关键的物理伪影，特别是支撑不稳定以及不正确的接触（如脚部滑动和触地时机不对）。同时，广泛使用的测试套件规模较小，缺乏挑战接触丰富、长时程行为所需的多样性。我们引入了 HumanTracker，使仿人跟踪评估既符合人类感知又具备可扩展性。HumanTracker 基准包含来自多位专业表演者的约153小时光学运动轨迹，分为四个运动大类，并配有文本标签以便进行细粒度诊断。我们还提出了 HumanScore，这是一种与偏好相一致的评估指标，基于包含2.4万个运动的1.2万个运动对进行训练。在具有代表性的先进跟踪器上，HumanScore 能更好地预测人类偏好，并揭示了运动学指标经常遗漏的接触和稳定性失效问题。
- **PDF**: https://arxiv.org/pdf/2608.13555v1

### Joint Communication-Control Strategy Optimization with Partially Nested Information Structures: The Linear-Quadratic Case
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13535v1
- **作者**: Haoyi You, Kaiqing Zhang
- **备注**: Preliminary version accepted to IEEE CDC 2026
- **摘要**: 本文在分散式随机控制的公共信息（CIB）框架下，公式化了具有二次成本的多智能体线性系统中的联合通信-控制策略优化（JCCO）问题。为了计算的可行性，我们重点关注具有部分嵌套（PN）信息结构（IS）的此类JCCO问题。特别地，在导致PN IS的基准通信协议下，我们建立了一系列条件，在这些条件下，待优化的（附加）通信策略可以保持部分嵌套性，而违反这些条件通常会导致开环通信策略中最佳策略的非线性。然后，我们开发了一种基于动态规划的方法，用以计算具有开环通信策略的JCCO的最优控制策略，从而产生了一组闭式Riccati方程。作为具有独立研究价值的副产品，该方法还提供了一种在CIB框架下解决具有PN IS和输出反馈的分散式线性二次控制的方法。最后，我们将该方法扩展到具有闭环通信策略的JCCO中，从而产生了一个比基于无限维CIB信念的动态规划更易于处理的动态规划。
- **PDF**: https://arxiv.org/pdf/2608.13535v1

### Measuring Task-Agnostic Training Data Influence Across Language Model Pretraining
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13515v1
- **作者**: Yuto Nishida, Hirokazu Kiyomaru, Yusuke Oda, Takashi Kodama, Chaoran Liu, Daisuke Kawahara, Yusuke Miyao, Max Müller-Eberstein, Masaru Isonuma
- **备注**: Accepted to COLM 2026
- **摘要**: 在语言模型预训练过程中，一致地测量训练数据的影响极具挑战性。很难选择能够代表模型通用能力的下游任务或验证集，且在中间检查点对任务性能的依赖使跨训练阶段的比较变得复杂。我们提出了一种不需要选择下游任务或验证集作为归因目标的训练数据影响测量方法。具体而言，我们通过一个样本的梯度更新在多大程度上缩短了与给定预训练运行的最终参数之间的平方距离，来定义该样本的影响，并在无需重新训练的情况下从中间检查点估计该数值。将该方法应用于 Pythia 和 PolyPythia 套件的18种配置中，我们发现了有影响力数据的系统性时间变化。在训练早期，与文献相关的数据与走向最终参数的轨迹契合度更强；而在训练后期，STEM（科学、技术、工程、数学）数据的契合度则变得更强。这种定性的交叉趋势在不同的模型配置中基本一致。我们的研究结果提供了一个易于处理的轨迹级视角，展示了有影响力的数据在整个预训练过程中的变化情况，对针对特定下游任务或验证集定义的传统影响分析进行了补充。
- **PDF**: https://arxiv.org/pdf/2608.13515v1

### Runtime Monitoring of Distributed Cyber-Physical Systems Without a Global Clock
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13486v1
- **作者**: Charles Koll, Houssam Abbas
- **备注**: Accepted to Runtime Verification 2026
- **摘要**: 我们首次针对无全局时钟的分布式信息物理系统（CPS），给出了基于密集时间时序逻辑规范进行连续运行监控的理论表征和算法。分布式CPS由多个智能体组成，每个智能体都有一个局部时钟；这些时钟彼此漂移，因此没有定义明确的全局时间。在根据时序逻辑规范监控这种系统的输出信号时，如何解释公式的时间约束以及满足性意味着什么，目前尚不明确。然而，像控制工程师这样的CPS设计人员通常会根据全局时间来思考其系统的运行。大多数现有的分布式系统监控技术都采用不适用于CPS的离散时间规范，和/或需要将时间约束显式映射到局部时钟。我们提出了一种算法，为包含所有时间算子的信号时序逻辑（STL）子集解决了上述挑战。它依赖于将满足信号推广到这种部分同步的设置（即时钟漂移），并对多维部分同步时间的几何结构进行分析。该算法返回满足规范的所有可能全局时刻的集合。了解这些可能的全局时刻对于调试分布式混合控制系统（如无人机机群和电网）至关重要。我们推导了该算法的最坏情况复杂度，并实现了其一种合理近似，实验表明，即使在多达50个智能体的场景中，也能进行有效的监控。
- **PDF**: https://arxiv.org/pdf/2608.13486v1

### MapRoute++: Surrogate-Guided Semantic Routing for Visual Concept Unlearning
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13478v1
- **作者**: Ashok Urlana, L. D. M. S. Sai Teja, Vivek Hruday Kavuri, Ponnurangam Kumaraguru
- **备注**: Accepted at Unlearning and Model Editing Workshop, ECCV 2026
- **摘要**: 我们展示了我们在 Gen$\mu$ 2.0 挑战赛任务 3（视觉概念擦除/遗忘）中的参赛方案。在 MapRoute 的基础上，我们引入了特定任务的训练目标、更丰富的概念表征以及用于特定概念映射器选择的语义路由。我们的方法提高了鲁棒的概念移除能力，同时保留了不相关和语义邻近的概念。在官方基准测试中，使用 Stable Diffusion v1.4 的“擦除-保留-鲁棒性”（ERR）指标进行评估，我们的方法在五个概念类别中平均超越了最先进的基准方法 12.1%，取得了实质性的提升。
- **PDF**: https://arxiv.org/pdf/2608.13478v1

#### 📝 学科总结
本周 `cs.*` 学科挑选的论文展示了计算机科学在三维运动捕捉、语言模型训练、分布式系统以及安全隐私和控制优化领域的多元化突破。研究包括：推出了更符合人类直觉感知的仿人运动跟踪基准 `HumanTracker` 及其评估指标；探讨了在多智能体系统中兼顾通信与控制成本的联合优化方法；提出了一种无需依赖特定下游任务、仅通过梯度平方距离变化来动态衡量大语言模型预训练阶段数据影响力的全新轨迹方法；设计了首个针对无全局时钟、存在时钟漂移的分布式信息物理系统（CPS）的实时监控算法；以及在多模态大模型安全方面，基于语义路由开发了能够精准、鲁棒地擦除特定视觉概念的 `MapRoute++` 框架。这些成果展现了系统安全、可解释性及人机协同等方向的技术演进。

--- 
## 📚 学科: `math.*`
### Equi-dependence implying independence
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13559v1
- **作者**: Iosif Pinelis
- **备注**: 5 pages. To appear in The American Mathematical Monthly
- **摘要**: 本文证明了如果一个事件 $A$ 在无限伯努利试验序列的每次试验中具有相同的条件概率，那么 $A$ 独立于每次试验。实际上，文中建立了一些更为普遍的结论。
- **PDF**: https://arxiv.org/pdf/2608.13559v1

### Joint Communication-Control Strategy Optimization with Partially Nested Information Structures: The Linear-Quadratic Case
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13535v1
- **作者**: Haoyi You, Kaiqing Zhang
- **备注**: Preliminary version accepted to IEEE CDC 2026
- **摘要**: 本文在分散式随机控制的公共信息（CIB）框架下，公式化了具有二次成本的多智能体线性系统中的联合通信-控制策略优化（JCCO）问题。为了计算的可行性，我们重点关注具有部分嵌套（PN）信息结构（IS）的此类JCCO问题。特别地，在导致PN IS的基准通信协议下，我们建立了一系列条件，在这些条件下，待优化的（附加）通信策略可以保持部分嵌套性，而违反这些条件通常会导致开环通信策略中最佳策略的非线性。然后，我们开发了一种基于动态规划的方法，用以计算具有开环通信策略的JCCO的最优控制策略，从而产生了一组闭式Riccati方程。作为具有独立研究价值的副产品，该方法还提供了一种在CIB框架下解决具有PN IS和输出反馈的分散式线性二次控制的方法。最后，我们将该方法扩展到具有闭环通信策略的JCCO中，从而产生了一个比基于无限维CIB信念的动态规划更易于处理的动态规划。
- **PDF**: https://arxiv.org/pdf/2608.13535v1

#### 📝 学科总结
本周 `math.*` 学科精选的论文在概率论和随机控制理论方面提供了新颖的数学见解。其中一篇简短而深刻的论文证明了“等相关性隐含独立性”的命题，指出在无限伯努利试验序列中，如果某事件在每次试验中的条件概率均相同，则该事件独立于每次试验，并将其推广至更一般的情形。另一篇论文则针对多智能体随机控制中的联合通信-控制优化问题，在数学上证明了保持部分嵌套信息结构（PN IS）的边界条件，并利用动态规划和闭式黎卡提（Riccati）方程组，推导出了去中心化线性二次控制问题的精确解法。这些工作从基础数学定理和应用数学优化的角度推动了相关领域的发展。

--- 
## 📚 学科: `astro-ph.*`
### JWST MIRI Medium Resolution Spectrometer Point Fixed Pattern Corrections: Cleaner and Higher Signal-to-Noise Spectra of Point Sources
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13464v1
- **作者**: Karl D. Gordon, David R. Law
- **备注**: 12 pages, 6 figures, accepted to AJ
- **摘要**: 詹姆斯·韦伯空间望远镜（JWST）的中红外仪器中分辨率光谱仪（MIRI MRS）提供了获取 5-28 微米光谱的能力。JWST 数据处理管线（pipeline）可以消除大部分仪器伪影，但并非全部，所得光谱的信噪比（S/N）仍受限于固定图案噪声。在先前工作的基础上，我们利用对 O、A 和 G 型矮星流量标准星以及小行星的观测（采用默认的四点抖动模式），构建了点源固定图案修正（PFPCs）。PFPCs 可以应用于采用目标捕获和相同抖动模式获取的点源光谱。根据源的光谱特性，它们可以单独使用，也可以与管线残留条纹修正结合使用。PFPCs 能够消除窄带和宽带伪影，从而在各种信噪比下改善光谱。对于较高信噪比的观测，PFPCs 显著提高了信噪比，增幅高达数倍，使信噪比数值达到 1000 或更高。我们提供了 `MRS-PFPC` python 软件包，以便任何人都能在自己的数据中应用此项修正。
- **PDF**: https://arxiv.org/pdf/2608.13464v1

### Widefield Arecibo Virgo Extragalactic Survey: II. Characterizing the HI properties and environment of the WAVES South region
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13411v1
- **作者**: V. Partík, R. Taylor, R. Minchin
- **备注**: 16 pages + 4 pages of appendices, accepted in A&A, 14 figures, 4 tables
- **摘要**: **背景**：星系团是极端环境，在此处与热星系团介质的相互作用推动了星系的快速演化。这些过程可能导致光学暗气体的云团形成，正如先前在室女座（Virgo）及其他星系团中所观测到的那样。
**目的**：我们调查了室女座星系团两个相邻大区域中中性氢（HI）的分布和性质，以理解星系团环境如何影响星系转化。具体而言，我们检查了恒星形成和静息星系群的含气量，并寻找气损驱动演化的证据。
**方法**：我们使用视觉和自动源提取方法对 21cm HI 阿雷西博室女座河外宽场巡天（WAVES）南部数据进行了编目。通过将这些结果与光学选择的样本相结合，我们比较了 WAVES 南部与此前研究过的 VC1 区域的 HI 特性。为了探测低于标称探测极限的气体储量，我们对 WAVES 南部、VC1 和 VC2 覆盖范围内的无线电光谱进行了叠加分析。
**结果**：我们探测到了 56 个 HI 源，中位均方根（rms）噪声为 0.8 mJy，其中包括 50 个星系、两个星系云（其中一个是光学暗星系云）以及 ALFALFA Virgo 7 复合体。我们的结果显示，与 VC1 区域相比，WAVES 南部的探测比例显著较低。叠加分析表明，在 WAVES 南部、VC1 和 VC2 的最多 157 个叠加天体中，在 0.080 mJy rms 下未发现新的 HI 探测。
**结论**：较低的 HI 探测比例表明，与 VC1 区域相比，WAVES 南部是一个在动力学上更为松弛和成熟的演化环境。在一小部分早期型星系中存在残留的 HI，支持了通过环境剥离使矮不规则星系向矮椭圆星系转化的模型。最后，我们指出光学暗星系云与最近发现的“蓝色斑块”（blue blobs）之间可能存在演化联系。
- **PDF**: https://arxiv.org/pdf/2608.13411v1

### Differential Reddening and Extinction Law Analyses of Galactic Open Clusters
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13313v1
- **作者**: Xiaohan Chen, Shu Wang, Xiaodian Chen
- **备注**: 15 pages, 9 figures, 1 table, Accepted for publication in AJ
- **摘要**: 消光显著影响着疏散星团参数及其在银河系结构研究中的应用，然而，对疏散星团消光特性的均匀大样本测量仍然有限。利用盖亚（Gaia）时代的疏散星团成员星样本，结合多波段光度测量和恒星参数，我们推导出了成员星的色余，并在星团尺度上提供了平均红化、差异红化和色余比（CER）的均匀表征。差异红化随平均红化系统性增加，银道面附近的高红化星团表现出更强的消光变化。逐星红化校正使 435 个具有可靠 CMD 宽度测量的星团中的 369 个（85%）的颜色-星等图（CMD）序列变窄，星团色余图揭示了小尺度的消光结构。中值 CER 与标准弥散星际介质消光曲线相符，而宽泛的 CER 分布及其在银盘上的大尺度变化，可能反映了沿不同银河视线采样的主要尘埃环境的差异。
- **PDF**: https://arxiv.org/pdf/2608.13313v1

### Radio Properties of Narrow-Line and Broad-Line Seyfert 1 Galaxies
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13303v1
- **作者**: K. É. Gabányi, S. Komossa, A. Mezősi, E. Forgács-Dajka, S. Frey
- **备注**: 33 pages, 13 figures, 11 tables. Published in Galaxies
- **摘要**: 窄线塞弗特 1 (NLS1) 星系宿主着活动星系核（AGN），其宽发射线区具有较窄的光学发射线。这通常被解释为中心超大质量黑洞质量相对较低以及超爱丁顿吸积。我们对比了从斯隆数字巡天（SDSS）中整理的大样本 NLS1 和宽线塞弗特 1 (BLS1) 星系的无线电属性。我们将 NLS1 和 BLS1 样本与 1.4 GHz 的“Faint Images of the Radio Sky at Twenty-Centimeters”（FIRST）巡天，以及 3 GHz 的甚大天线阵大天区巡天（VLASS）第一和第二纪元数据进行了交叉匹配。我们计算了无线电谱指数、1.4 GHz 无线电功率和无线电嘈杂度（radio loudness）。我们发现 NLS1 星系的 1.4 GHz 无线电探测率较低。NLS1 样本的中位无线电嘈杂度、无线电噪（radio-loud）AGN 的比例以及中位 1.4 GHz 无线电功率也较低。中位谱指数意味着 NLS1 样本的无线电光谱比 BLS1 样本略陡。将根据无线电数据估计的恒星形成率与广域红外巡天探测器（WISE）卫星的红外测量数据进行对比表明，被 FIRST 和 VLASS 探测到的 NLS1 和 BLS1 星系中，超过一半包含发射无线电的 AGN。
- **PDF**: https://arxiv.org/pdf/2608.13303v1

### X-ray Flaring and Variability in NGC 1275, the Heart of the Perseus Cluster
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.13281v1
- **作者**: Sarah Ketchum, Jon M. Miller, S. W. Allen, Doyee Byun, Tianyin Hu, Missagh Mehdipour, Veronica Tananko, Xin Xiang, Irina Zhuravleva
- **备注**: Accepted for publication in ApJ Letters
- **摘要**: NGC 1275 是英仙座星系团（Perseus Cluster）的中心星系。其内部的活动星系核（AGN）以强且多变的无线电活动而闻名，这与射流的产生密切相关，这些射流在热星系团介质（ICM）中吹出了巨大的气泡。高空间分辨率的 X 射线成像可以将 AGN 与明亮的 ICM 区分开来，但要监测流入黑洞的物质吸积率并确定 NGC 1275 中的吸积盘-射流关联，需要高频次的观测。在此，我们报告了使用雨燕卫星（Neil Gehrels Swift Observatory）20 多年来获取的数据对 NGC 1275 进行的 X 射线监测。通过对每次观测中时间恒定的 ICM 进行建模，可以可靠地追踪黑洞吸积产生的 X 射线辐射，典型流量误差仅为约 3%。在 MJD 59956（2023年2月21日）开始，检测到了在短短几天内流量增加约2倍的 X 射线耀斑。该耀斑暗示辐射区域大小符合 $r \leq 870~(10^{8}~M_{\odot}/M_{BH})~ GM/c^{2}$。耀斑的轮廓与潮汐瓦解事件（TDE）的简单预测不符。在大约 300 天后的 43 GHz 无线电监测数据中也出现了一个耀斑。总体而言，我们的结果表明，协调的中等分辨率 X 射线成像和无线电监测有可能追踪对大尺度结构影响最显著的 AGN 中的吸积盘-射流关联，并可推广到其他影响其宿主星系的源中。
- **PDF**: https://arxiv.org/pdf/2608.13281v1

#### 📝 学科总结
本周 `astro-ph.*` 学科挑选的论文涵盖了从高精度数据校准、星系环境演化、星际红化到活动星系核（AGN）高能物理等多个天体物理学前沿领域。具体成果包括：开发了针对詹姆斯·韦伯空间望远镜 MIRI MRS 光谱仪的固定图案噪声校正包 `MRS-PFPC`，大幅提升了点源光谱信噪比；利用 WAVES 巡天数据解析了室女座星系团南部中性氢（HI）的分布，为矮星系演化与气体剥离机制提供了证据；通过 Gaia 时代的海量数据对银河系疏散星团的差异红化和消光规律进行了精细测定；对比了窄线与宽线塞弗特1型星系的射电特征，极大地揭示了其星系核物理机制的差异；以及通过对英仙座星系团核心 NGC 1275 进行长达20年的 X 射线监测，捕捉到了黑洞吸积盘-射流关联的多波段耀斑信号。这些成果极大丰富了我们对宇宙大尺度结构和高能天体演化的理解。

--- 
## 📚 学科: `stat.*`
_本周缺少高价值论文_

## 📚 学科: `econ.*`
_本周缺少高价值论文_