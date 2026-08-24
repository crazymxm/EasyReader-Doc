# 🗓️ 周报 (2026-W34)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-08-23

--- 
## 📚 学科: `eess.*`
> **本期学科总结**：本期在电气工程与系统科学领域（eess.*）共筛选出 5 篇高质量论文。研究主题广泛且兼具理论深度与实用性，涵盖了电动垂直起降（eVTOL）飞机的统一飞行员控制系统设计、利用多音正弦调频波形进行宽带 MIMO 发射波束图合成的优化方法、具有功率方向性约束的随机控制在智能防洪系统中的应用、线性时不变系统中探索与利用平衡的双重控制理论综述，以及关于深度伪造语音对人类欺骗性趋势的量化评估（如 ElevenLabs 等最新工具带来的安全挑战）。这些研究展示了系统控制、信号处理与人机交互领域的前沿进展。

### Taming the Tilt: A Unified Pilot Control Concept for Transformational eVTOL Aircraft
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.20300v1
- **作者**: Daniel Milz, Marc May, Andreas Seefried, Tobias Bellmann
- **备注**: Accepted for publication in "Aerospace Systems", 31 pages, 16 figures
- **摘要**: 在过去的十年中，变革性电动垂直起降（eVTOL）飞行器因其高效的机翼巡航能力以及对地面基础设施的较低依赖而受到了极大的关注。然而，这些飞行器的控制系统设计仍然具有挑战性，因为它们必须在多个飞行阶段运行，而每个阶段都具有截然不同的主导动力学特征。如果不加以解决，这种复杂性将显著增加飞行员的工作量，从而推动了针对多阶段飞行操作的飞行员控制系统的发展。“简化车辆操作”概念为减轻飞行员工作量提供了一种极具前景的策略。本研究展示了一种新型 eVTOL 飞机飞行员控制概念的设计与实现，并通过在配备有源力反馈侧杆的全动模拟器上进行串联倾转翼飞机的仿真进行了验证。该系统在特定飞行阶段向飞行员提供触觉反馈，以支持直观控制。所提出的方法通过利用可用的自由度，实现了无缝过渡和多阶段飞行机动。此外，还提出了一种基于最优控制的方法，作为评估指令滤波器引起的性能损失和操纵器件活动的指标。结果表明，与闭环系统相比，所提出的指令滤波器并未显著增加任务执行时间，而有源侧杆有助于减少操纵器件的活动。
- **PDF**: https://arxiv.org/pdf/2608.20300v1

### Wideband MIMO Beampattern Synthesis using Adaptive Frequency Modulated Waveforms
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.20214v1
- **作者**: David A. Hague
- **备注**: Accepted for publication at 2026 EUSIPCO Conference
- **摘要**: 多输入多输出（MIMO）天线阵列在其每个阵元上发射独特的波形，从而增加了合成新型发射波束图的可调自由度。宽带 MIMO 波束图的形状由 MIMO 交叉谱密度矩阵（CSDM）的结构决定，该矩阵的元素是波形集中每个波形之间的交叉光谱，是频率的函数。本文展示了一种使用多音正弦调频（MTSFM）波形集来合成宽带 MIMO 波束图的模型。MTSFM 波形的瞬时相位是一个有限傅里叶级数。通过修改傅里叶系数来合成恒包络和频谱紧凑的波形，其 CSDM 能够紧密逼近所需的宽带 MIMO 发射波束图。本文构建了一种优化算法，用于合成具有必要 CSDM 结构的 MTSFM 波形集，并结合一个说明性的设计示例进行了演示。
- **PDF**: https://arxiv.org/pdf/2608.20214v1

### Performance-Guaranteed Reference Tracking With Power Directionality Constraints: Application to Controlled Stochastic Watersheds
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.20120v1
- **作者**: Jonathan Shell, Sepehr Moalemi, Branko Kerkez, Jeff Scruggs
- **备注**: 6 pages, 6 figures. Accepted to the 65th IEEE Conference on Decision and Control (CDC)
- **摘要**: 现代雨水基础设施面临着不断增加的需求，这需要相应地提升其调蓄能力。传统上，这些需求是通过建设新的基础设施资产来满足的，而这是一项成本高昂的举措。近年来，许多系统运营商通过采用反馈控制技术来提高系统性能，并取得了巨大成功。然而，由此产生的闭环系统表现出功率方向性约束，这在反馈合成中引入了非线性约束。在这项工作中，我们针对一类存在功率方向性约束的通用问题，开发了一种具有可证明均方参考跟踪性能边界的随机控制合成方法。随后，该方法被应用于一个使用真实世界智能水务系统数值模型的防洪减灾案例中。其核心成果是将原本设计用于干扰抑制的性能保证控制（PGC）框架，扩展到能够适应参考跟踪控制目标。
- **PDF**: https://arxiv.org/pdf/2608.20120v1

### Dual Control: On Exploration-Exploitation in Linear Systems
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.20073v1
- **作者**: Tomas J. Meijer, Anders Rantzer
- **备注**: To be published in Annual Review of Control, Robotics, and Autonomous Systems Vol. 10 (2027)
- **摘要**: “双重控制”一词是指同时平衡探索（exploration）和利用（exploitation）的双重目标。这类问题已经被研究了将近一个世纪。本文致力于对线性时不变系统的最优控制相关的理论和方法进行综述，这些系统的参数最初是未知的，必须通过主动探测来学习。我们回顾了支撑四个主要研究方向的核心思想：多臂老虎机、自适应调节器、遗憾率极小化控制器以及极小极大最优双重控制器。前三个方向有着悠久的历史和丰富的文献积累，而第四个方向则为鲁棒双重控制提供了一个极具前景的框架。
- **PDF**: https://arxiv.org/pdf/2608.20073v1

### Tracking the Trend in How Speech Synthesizers Deceive People
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.19959v1
- **作者**: Milan Šalko, Anton Firc, Kamil Malinka, Vojtěch Staněk, Martin Perešini, Filip Pleško, Jakub Reš
- **备注**: Accepted at the 6th Symposium on Security and Privacy in Speech Communication (SPSC 2026)
- **摘要**: 语音合成技术的进展使得深度伪造（deepfake）音频变得高度逼真。早期的研究报告称人类的检测准确率在 70-80% 之间，但这些研究主要依赖于较旧的合成器。我们在一项包含 82 名 IT 专业人员的测试中，对比了人类对 2019 年、2022 年和 2024 年发布的三个代表性语音合成工具的检测能力，并在相同材料上将人类与六个预训练检测器进行了基准测试。对于完全合成的语音（全伪造），尽管听众被明确告知存在深度伪造，但 F1 分数从 RTVC 和 YourTTS 的约 90% 骤降至 ElevenLabs 的 48%。对于局部伪造（即一段话中仅修改了一个句子），严格准确率降至 9%，听众在 77% 的情况下会将合成的句子分类为真实语音。人类和检测器在不同的方面表现出互补的失败模式，且两者都无法可靠地定位短时间的篡改。此外，听众越来越多地将真实的语音误标为伪造，从而侵蚀了对未篡改音频的信任。这些发现表明，在选定的现代和局部伪造条件下，仅凭人类听觉感知是不可靠的，这促使了程序性验证、来源追踪、水印技术以及分段级检测的发展。
- **PDF**: https://arxiv.org/pdf/2608.19959v1

--- 
## 📚 学科: `q-bio.*`
> **本期学科总结**：本期定量生物学领域（q-bio.*）收录了 3 篇将计算技术应用于生物医学的研究。首先，探讨了利用量子-经典混合机器学习（量子核方法）处理无细胞 DNA 碎片及甲基化数据，以提升早期肺癌检测率；其次，针对基于子宫肌电图（EHG）预测早产的任务，明确了片段级与患者独立验证的区别，建立了一个防止数据泄漏的患者独立基准并结合了共形选择性预测；最后，利用图神经网络（GNN）基于稀疏的心脏内测量信号来准确高效地表征心脏组织电生理特性，助力心律失常消融治疗。这些工作展现了 AI 和量子计算在现代医学精准诊断和治疗中的巨大潜力。

### Quantum Kernel Estimation for the Discovery of Early Lung Cancer Detection
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.19304v1
- **作者**: Hamed Javidi, Alex Zajichek, Hakan Doga, Laxmi Parida, Filippo Utro, Peter J. Mazzone
- **备注**: Accepted at the CIBB 2026 conference (https://cibb2026.teralab.ai/)
- **摘要**: 使用低剂量胸部计算机断层扫描进行肺癌筛查可降低死亡率，但其效果受到普及率、依从性以及管理挑战的限制。基于血液的游离 DNA（cfDNA）生物标志物提供了一种补充方法，但由于肺癌的异质性以及高维、非线性的分子信号，早期检测仍然非常困难。我们评估了基于 DNA 碎片组学和 DNA 甲基化的量子-经典混合机器学习在肺癌检测中的应用。在特征选择之后，使用 20 和 40 个特征子集对模型进行了训练。通过使用具有多种纠缠策略的角度和密实角度特征映射，将特征编码到量子希尔伯特空间中。使用精确的状态向量模拟计算了基于保真度的量子核，并将其与预计算核 SVM 和核 PCA 逻辑回归相结合，同时与在原始特征上训练的 SVM 模型进行了对比。该框架能够系统地评估编码和纠缠设计如何影响分类。在重复的留出集评估中，量子核模型在两个数据集上都取得了具有竞争力的表现。对于碎片组学，几种 20 特征的配置相比于经典 SVM 基线提高了 AUC，这表明其有效捕捉了非线性的 cfDNA 碎片结构。对于甲基化，经典 SVM 取得了最高的 AUC，尽管选定的量子模型仍具有竞争力，并在某些情况下提高了特异性。将特征从 20 个增加到 40 个并不能持续提高性能，且往往会增加变异性。总体而言，这些结果支持将量子核方法作为基于 cfDNA 的肺癌检测的一种极具前景的方法。
- **PDF**: https://arxiv.org/pdf/2608.19304v1

### A Leakage-Proof Benchmark and Conformal Selective Triage for Electrohysterogram-Based Preterm Birth Prediction
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.17712v1
- **作者**: Sunday A. Adetunji, Rhoda O. Oyewusi
- **备注**: Accepted for publication in the Proceedings of the 48th Annual International Conference of the IEEE Engineering in Medicine and Biology Society (EMBC 2026), Toronto, Canada. Paper ID 4188
- **摘要**: 早产仍是全球新生儿发病和死亡的主要原因。子宫肌电图（EHG）作为一种对子宫肌电活动的无创测量方法已被用于早产预测，但当来自同一母亲记录的片段被拆分到训练和验证数据中时，性能评估可能会出现偏差。我们正式明确了片段级验证与患者独立记录分组验证之间的区别，在足月-早产子宫肌电图数据库（TPEHGD）上建立了一个患者独立的基准，并评估了类条件共形选择性预测。研究对所有 300 条记录（其中 38 条为早产）在三种预设方案下进行了分析。使用记录分组嵌套交叉验证对含有 92 个特征的弹性网逻辑模型进行了评估；数据预处理、模型拟合、Platt 校准和共形估计均仅限于训练数据，而性能指标则是通过对严格袋外记录级预测进行 1000 次自助法重采样计算得出的。在患者独立的评估下，AUROC 为 0.493（95% CI 0.467-0.520），AUPRC 为 0.122（0.095-0.152），Brier 分数为 0.115（0.094-0.137）。在 26 周或之前 AUROC 为 0.514，之后为 0.469。在错误覆盖率 alpha=0.10 时，边际覆盖率为 0.897，弃权率为 72.7%，单标签预测准确率为 0.624。这些发现为 EHG预测建立了一个记录分离的参考基准，并为分段生理数据提供了一个更广泛的验证原则：重采样的单位应当与预测性能意图泛化的单位相一致。共形预测进一步量化了现有信息何时支持单标签分类，以及何时由于不确定性而需要延迟决策。
- **PDF**: https://arxiv.org/pdf/2608.17712v1

### Characterising cardiac tissue properties with graph neural networks
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.15843v1
- **作者**: Ching-En Chiu, Yoo Ri Kim, Magdi Saba, Danilo Mandic, Marta Varela
- **备注**: Accepted at The Statistical Atlases and Computational Modeling of the Heart (STACOM) workshop 2026
- **摘要**: 从空间稀疏的心脏内测量中高效且准确地表征心脏组织的电生理特性，对于定位消融靶点和改善心律失常治疗具有重要的临床意义。我们开发了一个基于图神经网络的框架，该框架在二维平面上的合成心电图信号上进行训练，以识别与室性早搏（PVCs）心脏消融相关的关键区域。我们的方法在检测单片纤维化、快速去极化和高兴奋性区域时，分别达到了 0.96、0.97 和 0.95 的平均精度。训练好的模型随后可以通过少样本微调应用到二维弯曲表面上，展示了其泛化能力。未来的工作将进一步开发该框架以用于 PVC 消融的临床应用。
- **PDF**: https://arxiv.org/pdf/2608.15843v1

--- 
## 📚 学科: `cs.*`
> **本期学科总结**：本期计算机科学领域（cs.*）精选了 3 篇在机器学习理论及应用方向有重要突破的论文。理论方面，一篇 ICML 2026 论文研究了在深度 ReLU 网络下多组非参数回归的迁移学习框架，证明了其克服维度灾难的能力及快速收敛率；应用方面，一篇提出了 BERT-LER 模型，统一了结构化电子健康记录（EHR）中检验结果的表示与基于集成梯度的模型可解释性；另一篇则针对航海安全，利用机器学习模型实现了电子海图（ENC）变更的自动化分类，提升了地理空间数据在维护过程中的自动化水平。这些研究反映了深度学习从基础理论到跨学科交叉落地应用的成熟度。

### Transfer Learning in Nonparametric Regression with Deep ReLU Networks
- **分数**: 6
- **链接**  https://arxiv.org/abs/2608.20255v1
- **作者**: Junpeng Ren, Carlos Misael Madrid Padilla, Yanzhen Chen, Oscar Hernan Madrid Padilla
- **备注**: Accepted at the 43rd International Conference on Machine Learning (ICML 2026)
- **摘要**: 本文为包含多个组的数据开发了一个通用的非参数回归迁移学习框架。在各组共享公共结构以及具有加性形式的组特异性偏差的假设下，所提出的方法采用了一种两阶段的偏移量学习程序：第一阶段汇总所有组的数据以估计一个总体的均值函数，第二阶段估计每组的偏移量，通过加性组合得到最终的组级估计量。本文为该框架确立了 $\mathcal L_2$ 误差的上界，涵盖了在温和的复杂度和噪声条件下的一大类非参数估计量。当具体应用到深度 ReLU 网络时，在层次组合模型下推导出了显式的收敛速度，展示了克服维度灾难的能力。文章还考虑了能够实现具有更快收敛速度的正迁移的条件，包括使用更简单的函数进行学习以及通过跨组汇集样本进行数据增强。各种仿真和真实数据实验进一步验证了所提方法的有效性。
- **PDF**: https://arxiv.org/pdf/2608.20255v1

### Explainable Transformer Models for Clinical Prediction Tasks on Structured Electronic Health Records
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.20315v1
- **作者**: Jun Ni Du, Lukas Adamek, Maxim Kryukov, Flavio Dormont, Ziv Bar-Joseph, Sven Jager, Brandon Rufino
- **备注**: Accepted at MLHC 2026; to appear in Proceedings of Machine Learning Research (PMLR)
- **摘要**: 针对结构化电子健康档案（EHR）的预测模型在医疗机器学习中仍然居于核心地位，但极少有模型能同时强调定量实验室信息以及对输入医疗事件的可解释性。我们提出了 BERT-LER，这是一种针对编码 EHR 时间线的 BERT 风格模型，在包含 7500 万患者去隐私数据的 EHR 数据集上进行了预训练和微调。该模型将实验室检测结果编码为离散 Token，同时通过基于百分位数的离散化保留分级信息，并结合集成梯度（Integrated Gradients）实现基于输入 EHR 序列的 Token 级归因。我们在公共的 EHRShot 基准套件以及一个基于真实世界数据的哮喘严重程度进展研究中对我们的方法进行了基准测试。这通过在单一框架中统一实验室数值表示和可解释性，填补了 EHR 基座式模型的方法学空白，同时评估了预测性能和解释是否能泛化到标准临床预测任务之外。在 EHRShot 和哮喘任务中，BERT-LER 的预测性能与公开可用的基准模型相比极具竞争力，且在与实验室相关的任务中通常表现更优，并提供了与临床已知风险因素相一致的归因。我们的架构和可解释性方法可以应用于使用结构化 EHR 训练的语言模型的许多治疗领域和预测任务。
- **PDF**: https://arxiv.org/pdf/2608.20315v1

### Electronic Navigational Chart Change Classification
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.20218v1
- **作者**: Jacob Arndt, Abhishek Potnis, Alexandre Sorokine
- **备注**: Accepted at 34th ACM SIGSPATIAL 2026
- **摘要**: 电子海图（ENCs）是用于航海导航系统的地理空间矢量数据集，代表了水深、助航设施、交通计划和危险物等水文和导航信息。航道局面临的一个主要挑战是确定给定的海图变更对航海安全构成的是关键风险还是非关键风险。现有的工作流程严重依赖人工审查和验证，这不仅劳动强度大、难以随海图更新量的增加而扩展，还会引入分析师之间的不一致性。为了解决这一挑战，我们提出了一种用于 ENC 变更自动分类的方法。我们建立了一个基线编码方案，将复杂的矢量数据变更转化为用于分类模型的结构化表格格式。该编码方案的两个关键组成部分包括：空间上下文编码器，用周围的地理特征丰富变更表示；以及 ENC 属性编码器，用以表示修改对象的细微属性值描述。我们在两个不同的业务数据集上对所提方法进行了评估，这两个数据集包含 1,308 对海图，其中包含超过 100,000 个独立的海图修改。利用所提编码方案的调优梯度提升树（GBDT）在两个数据集上分别达到了 90% 和 94% 的准确率，比在没有空间上下文和属性嵌入的编码上训练的默认超参数模型提高了 5-7%。这些结果证明了将机器学习集成到业务地理空间管线中以改进 ENC 维护并提高航海安全的可行性。最后，我们的实验证明了简单的位置和空间聚合方法的有效性，为评估该应用中更复杂的空间表示学习技术奠定了基础。
- **PDF**: https://arxiv.org/pdf/2608.20218v1

--- 
## 📚 学科: `math.*`
> **本期学科总结**：本期数学领域（math.*）选录了 1 篇应用数学与控制理论相关的交叉学科论文。该研究聚焦于变革性 eVTOL 飞机的控制系统设计，提出了一种基于最优控制（Optimal Control）的严格数学方法，用以量化评估由指令滤波器引入的性能惩罚以及操纵器件有源力反馈側杆的活动状态。这不仅为复杂动力学系统的多阶段飞行控制提供了创新的工程设计概念，也展示了控制科学与应用数学方法的深度结合。

### Taming the Tilt: A Unified Pilot Control Concept for Transformational eVTOL Aircraft
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.20300v1
- **作者**: Daniel Milz, Marc May, Andreas Seefried, Tobias Bellmann
- **备注**: Accepted for publication in "Aerospace Systems", 31 pages, 16 figures
- **摘要**: 在过去的十年中，变革性电动垂直起降（eVTOL）飞行器因其高效的机翼巡航能力以及对地面基础设施的较低依赖而受到了极大的关注。然而，这些飞行器的控制系统设计仍然具有挑战性，因为它们必须在多个飞行阶段运行，而每个阶段都具有截然不同的主导动力学特征。如果不加以解决，这种复杂性将显著增加飞行员的工作量，从而推动了针对多阶段飞行操作的飞行员控制系统的发展。“简化车辆操作”概念为减轻飞行员工作量提供了一种极具前景的策略。本研究展示了一种新型 eVTOL 飞机飞行员控制概念的设计与实现，并通过在配备有源力反馈侧杆的全动模拟器上进行串联倾转翼飞机的仿真进行了验证。该系统在特定飞行阶段向飞行员提供触觉反馈，以支持直观控制。所提出的方法通过利用可用的自由度，实现了无缝过渡和多阶段飞行机动。此外，还提出了一种基于最优控制的方法，作为评估指令滤波器引起的性能损失和操纵器件活动的指标。结果表明，与闭环系统相比，所提出的指令滤波器并未显著增加任务执行时间，而有源侧杆有助于减少操纵器件的活动。
- **PDF**: https://arxiv.org/pdf/2608.20300v1

--- 
## 📚 学科: `astro-ph.*`
> **本期学科总结**：本期天体物理学领域（astro-ph.*）共选入 5 篇优质论文，涵盖了星系化学演化、大质量恒星形成、超新星观测、紧凑射电源性质及太阳系早期演化等关键方向。研究内容包括：利用自洽金属丰度标定重新评估空间分辨和积分的质量-金属丰度关系，探究恒星形成率的作用；通过 ALOHA JCMT 大型项目对暗星云（IRDCs）团块进行分子线观测，揭示多阶段气体演化过程；对正常 Ia 型超新星 SN 2021pfs 进行对比分析，揭示前身星金属丰度对光度曲线及宇宙学测距的影响；利用 VLBA 进行多频观测，研究紧凑射电源 J0011+3443 的物理本源；以及通过陨石中 Ti、Cr、Mo 的非质量相关同位素异常分析，重建早期原行星盘内盘的尘埃混合与演化机制。

### Re-evaluating the resolved mass-metallicity relation with a self-consistent metallicity calibration
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.20239v1
- **作者**: Ziming Peng, Renbin Yan, Zesen Lin, Xihan Ji
- **备注**: 13 pages, 9 figures, accepted by A&A. Comments are welcome
- **摘要**: 研究目的：质量-金属丰度关系（MZR）对于理解星系的化学演化至关重要。恒星形成率（SFR）是否在设定金属丰度方面发挥作用长期以来一直存在争议。使用不同的金属丰度标定可能会对这一基本但尚未解决的问题得出不同的结论。方法：我们应用基于光致电离模型的自洽金属丰度标定来重新评估空间分辨和积分的 MZR。我们利用了来自 SDSS-IV/MaNGA 的积分视场单元数据，包含约 $3.5\times10^6$ 个时空元（spaxels）和约 4550 个星系。我们将我们首选的金属丰度标定与文献中的几种强线标定以及直接法金属丰度进行了比较。我们分析了 MZR 的金属丰度残差以评估 SFR 的影响，并应用偏相关系数来量化这些影响。结果：我们使用的金属丰度标定显示出与直接法最好的自洽性。我们为空间分辨的 MZR 提供了 3 个方程，并证实了局域 SFR 与金属丰度没有显著的相关性。考虑到积分性质，(s)SFR 与金属丰度残差不呈现相关性。结果表明，流入和流出的平衡更受青睐，并且质量-金属丰度关系不依赖于 SFR 作为其次要因素。
- **PDF**: https://arxiv.org/pdf/2608.20239v1

### ALOHA IRDCs Molecular Line Follow-up: I. Gas properties and kinematics
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.20238v1
- **作者**: Jinjin Xie, Yaoting Yan, Zhiyuan Ren, Jarken Esimbek, Di Li, Yan Duan, Gary A. Fuller, Nicolas Peretto, Jingwen Wu, Wenjin Yang, Christian Henkel, Xuepeng Chen, Qianru He, Yongxiong Wang, Keping Qiu, Ningyu Tang, Sijia Peng, Chao-Wei Tsai, Pham Ngoc Diep, Hauyu Baobab Liu, Busaba Kramer, Kee-Tae Kim, Ken'ichi Tatematsu, Mark G. Rawlings, Maria Jesus Jimenez Donaire, Gan Luo, Xin Lyu, Jiawei Liu, Yuchen Xing, Sheng-yuan Liu, Koichiro Sugiyama, Ram K. Yadav, Willem A. Baan, Gordon Macleod, Patricio Sanhueza, Long-Fei Chen, Chang Won Lee, Yang Su, Chen Wang, Ruili Wang, Ruilin Xia, Andrej Sobolev, Dmitry A. Ladeyschikov, David Eden, Woojin Kwon, Fengwei Xu, Hongjun Ma, Daniel Harsono, Sihan Jiao, Rowan Smith, Ke Wang, Tie Liu, Guangxing Li, Xin Guan, Yuxin He, Dalei Li, Xindi Tang, Chunsheng Luo, Jianjun Zhou, Kitiyanee Asanok, Dan Bintley, Huei-Ru Vivien Chen, En Chen, Chakali Eswaraiah, Ana Duarte-Cabral, Siyi Feng, Ray S. Furuya, Tomoya Hirota, Ernar Imanaly, Xue-Jian Jiang, Qaynar Jandaolet, Abay Jengis, Weiguang Ji, Yi-Jehng Kuan, Min-Young Lee, Chong Li, Cuihuan Li, Guodong Li, Hua-bai Li, Jiasheng Li, Yujie Li, Mengting Liu, Kuan-Yu Liu, Shu Liu, Rong Liu, Yongquan Luo, Yingxiu Ma, Steve Mairs, Fumitaka Nakamura, Harriet Parsons, Jaime Pineda, Hailiang Shen, Mingke Sun, Serikbek Sailanbek, Nurzhan Shaimoldin, Ya-Wen Tang, Antneh Gashaye Tegegne, Kadirya Tursun, Glenn J. White, Gang Wu, Jifeng Xia, Yuanzhen Xiong, Naiping Yu, Nannan Yue, Xinyu Yang, Yuebin Yang, Miaomiao Zhang, Chao Zhang, Shiyu Zhang, Dongdong Zhou, Qiao Zhao, Xiang Zhao
- **备注**: 11 pages, 3 figures, accepted for publication on A&A
- **摘要**: 红外暗星云（IRDCs）是研究大质量恒星和星团形成初始条件的理想场所。ALOHA IRDCs 是詹姆斯·克拉克·麦克斯韦望远镜（JCMT）的一项大型计划，已使用 SCUBA-2 绘制了邻近的 IRDCs。需要互补的分子线观测来表征致密气体的物理、运动学和化学性质。我们的目标是确定在 ALOHA IRDCs 中识别出的团块的热学、运动学和化学性质，并评估它们的演化状态和恒星形成活动水平。我们使用 Effelsberg 100 米和 Yebes 40 米望远镜，分别对 56 个 ALOHA IRDCs 团块进行了单点 K 波段和 W 波段观测。我们使用超精细组比（HFGR）方法导出了 $NH_3$ 动能温度，并从 $HCO^+$、$H^{13}CO^+$、$SiO$ 和 $HNCO$ 剖面中识别了塌缩和激波特征。水超脉泽（water masers）和 $NH_2D$ 发射被用作化学演化和恒星形成的互补示踪剂。这些团块的动能温度在 15-29 K 之间。我们在 18 个源中探测到了 $NH_2D$ 发射，其质心速度与 $NH_3$ 一致，表明这两种分子示踪了相同的致密气体成分。超过一半的团块表现出蓝色不对称的 $HCO^+$ 剖面，将它们识别为塌缩候选体。在 22 个源中探测到了水超脉泽，具有显著的速度范围和变异性。宽 $SiO$ 发射（>~20 km/s）表明存在强激波，而较窄的范围（<~6 km/s）可能示踪了大尺度相互作用或低速激波。广泛存在的塌缩特征、激波示踪剂、超脉泽和 $NH_2D$ 发射表明，相对平静、化学性质年轻的物质可以与受到早期原恒星反馈影响的动力学活跃气体共存，这为大质量 IRDC 团块的物理和化学协同演化提供了见解。
- **PDF**: https://arxiv.org/pdf/2608.20238v1

### SN 2021pfs: A Type Ia Supernova Likely Affected by Progenitor Metallicity, as Revealed by Comparison with Its Twin Counterpart
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.19929v1
- **作者**: Abdusamatjan Iskandar, Xiaofeng Wang, Ali Esamdin, Wenxiong Li, Xiangyun Zeng, Ruifeng Huang, Guoliang Lu, D. Andrew Howell, Curtis McCully, Samuel Wyatt, Daichi Hiramatsu, Estefania Padilla Gonzalez, Craig Pellegrino, Megan Newsome, Lluis Galbany, David J. Sand, Nathan Smith, Huei Sears
- **备注**: 35 pages, 14 figures, published in SCIENCE CHINA Physics, Mechanics & Astronomy,DOI: 10.1007/s11433-026-2999-3
- **摘要**: 我们展示了对正常 Ia 型超新星（SN Ia）2021pfs 的详细光度和光谱观测，该超新星发生在红移为 0.009 的 Seyfert 2 星系 NGC 5427 中。SN 2021pfs 达到的绝对 B 波段峰值星等为 $M_{\rm max}(B)=$-19.28 $\pm$ 0.40 等，峰值后的衰减率为 $Δm_{15}(B)=$1.13 $\pm$ 0.06 等。这颗邻近的 SN Ia 观测到的性质与 SN 2011fe 非常相似，包括主要的等离子光谱特征和光度演化。尽管它们的衰减率相似，但在极早期阶段，与 SN 2011fe 相比，SN 2021pfs 在 U 波段上升得更快，但在 r 和 i 波段上升得更慢。这种光度差异，尤其是在短波长波段，可能会在距离估计中引入高达约 12% 的系统不确定性。对宿主星系局部和全局环境的分析表明，与 SN 2011fe 的环境相比，产生 SN 2021pfs 的前身星具有更高的金属丰度。这种较高前身星金属丰度可能解释了观测到的光度差异以及由此产生的 SN 2021pfs 和 SN 2011fe 之间的距离差异，尽管需要更多此类“孪生” SN Ia 样本来确认这一趋势并评估其对宇宙学测量的影响。
- **PDF**: https://arxiv.org/pdf/2608.19929v1

### J0011+3443: a GPS compact symmetric object, gravitational lens, or dual AGN?
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.19928v1
- **作者**: Efthalia Traianou, Tingting Liu, Roman Gold, Richard Mushotzky
- **备注**: 8 pages, 3 figures, 3 tables. Accepted for publication in A&A
- **摘要**: 我们展示了对 J0011+3443 (TXS 0008+344, z=0.89) 在 2.3、4.9、8.5 以及首次在 23.6 GHz 下进行的全新多频甚长基线阵列（VLBA）观测。该源由两个紧凑成分 A 和 B 组成，投影间距为 $314\pm2$ pc，外加在 23.6 GHz 下探测到的第三个特征 C，距离 A 约 0.6 mas。存档的低分辨率射电测量证实了其具有整体的吉赫兹峰值光谱（GPS），在观测框架下的峰值频率为 $ν_\mathrm{peak}=0.73\pm0.08$ GHz，峰值通量密度为 $S_\mathrm{peak}=879\pm125$ mJy。与几乎频率匹配的低分辨率测量进行对比显示，VLBA 恢复了 4.85 GHz 通量密度的 $0.85\pm0.11$ 以及 8.46 GHz 通量密度的 $0.50\pm0.06$。在 8.5 GHz 下较低的恢复比例表明低表面亮度发射已被解析掉或低于 VLBA 的表面亮度灵敏度。因此，我们将 VLBA 成分光谱解释为仅代表紧凑的可恢复发射的光谱。23.6 GHz 的形貌、未探测到平谱核心、A 和 B 相似的紧凑光谱以及陡峭的整体 GHz 光谱，更倾向于将 J0011+3443 解释为 GPS 类紧凑对称源（可能处于短寿命或残骸阶段），尽管在没有多历元天体测量的情况下不能排除双 AGN 起源。
- **PDF**: https://arxiv.org/pdf/2608.19928v1

### Origin of nucleosynthetic isotope variability in the NC reservoir: Evidence from Ti, Cr, and Mo isotopes
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.19786v1
- **作者**: Elias Wölfer, Christoph Burkhardt, Gerrit Budde, Christian A. Jansen, Jonas Pape, Thorsten Kleine
- **备注**: Accepted for publication in Geochimica et Cosmochimica Acta (https://doi.org/10.1016/j.gca.2026.08.021)
- **摘要**: 核合成同位素异常允许区分非碳质（NC）和碳质（CC）类型的陨石，并揭示了特别是在 NC 天体中相关的同位素变化。理解这一 NC 趋势的起源对于识别产生 NC 同位素非均质性的过程，以及利用这些同位素异常重建太阳原行星盘的早期演化至关重要。我们报告了一组全面、此前未研究或研究较少的陨石的非质量相关 Ti、Cr 和 Mo 同位素组成，以及通过对原始普通球粒陨石进行顺序消化获得的酸浸出液。本研究中调查的一些样品填补了此前确定的 NC 趋势中明显的空白，这表明这些空白反映的是更连续同位素趋势的不具代表性的采样。整体陨石和浸出液表现出截然不同的同位素系统学，这表明 NC 同位素的变异性并不反映星周盘中前太阳载体的选择性热处理。NC 趋势也不能反映 CC 尘埃从外盘向内盘的持续添加，因为早期和晚期形成的 NC 陨石显示出很大程度上重叠的同位素组成。相反，我们发现 NC 同位素的非均质性最好通过化学和同位素不同的尘埃组分之间的分馏和混合来解释，这类似于产生碳质球粒陨石同位素变异性的过程。在此基础上，我们论证了内盘中存在子结构，这些子结构促进了不同尘埃组分之间的分馏和混合，并有助于保留一个长寿命的尘埃储库，NC 微行星在很长一段时间内从中吸积。
- **PDF**: https://arxiv.org/pdf/2608.19786v1

--- 
## 📚 学科: `stat.*`
> **本期学科总结**：本期统计学领域（stat.*）选录了 1 篇发表于机器学习顶级会议 ICML 2026 的杰出工作。该研究探讨了使用深度 ReLU 网络进行多组非参数回归的迁移学习框架。在共享公共结构与组特异性加性偏差的假设下，该算法设计了创新的两阶段偏移量估计方法。不仅在数学上确立了在层次组合模型下克服“维度灾难”的极佳 $\mathcal L_2$ 误差收敛速度，还推导出了实现更快“正迁移”的统计条件，对高维非参数统计推断与迁移学习理论的发展具有重要科学价值。

### Transfer Learning in Nonparametric Regression with Deep ReLU Networks
- **分数**: 6
- **链接**  https://arxiv.org/abs/2608.20255v1
- **作者**: Junpeng Ren, Carlos Misael Madrid Padilla, Yanzhen Chen, Oscar Hernan Madrid Padilla
- **备注**: Accepted at the 43rd International Conference on Machine Learning (ICML 2026)
- **摘要**: 本文为包含多个组的数据开发了一个通用的非参数回归迁移学习框架。在各组共享公共结构以及具有加性形式的组特异性偏差的假设下，所提出的方法采用了一种两阶段的偏移量学习程序：第一阶段汇总所有组的数据以估计一个总体的均值函数，第二阶段估计每组的偏移量，通过加性组合得到最终的组级估计量。本文为该框架确立了 $\mathcal L_2$ 误差的上界，涵盖了在温和的复杂度和噪声条件下的一大类非参数估计量。当具体应用到深度 ReLU 网络时，在层次组合模型下推导出了显式的收敛速度，展示了克服维度灾难的能力。文章还考虑了能够实现具有更快收敛速度的正迁移的条件，包括使用更简单的函数进行学习以及通过跨组汇集样本进行数据增强。各种仿真和真实数据实验进一步验证了所提方法的有效性。
- **PDF**: https://arxiv.org/pdf/2608.20255v1

--- 
## 📚 学科: `econ.*`
> **本期学科总结**：本期经济学与社会科学计算领域（econ.*）选录了 1 篇探讨现代民主制度数学模型的综述性工作。该文通过三个前沿案例——投票理论、参与式预算以及协商民主，深入阐释了如何利用严谨的数学模型，并融合真实世界中的制度约束、运行成本、数据反馈以及实现可行性，从而优化并解决社会选择与经济决策中的核心挑战。这展现了应用数学、公共经济学与机制设计领域的交叉结合。

### The New Mathematics of Democracy
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.16869v1
- **作者**: Bailey Flanigan, Ismar Volic
- **备注**: To appear in Notices of the American Mathematical Society, December 2026
- **摘要**: 本文调查了民主数学中新兴的研究方向。它通过三个案例研究——投票理论、参与式预算和协商民主——来突出当今的挑战如何推动结合了真实世界数据、制度约束和实施可行性的严谨数学研究。在每个案例中，我们都强调了活跃且有前景的研究前沿、真实世界影响的证据、实际应用以及参与其中的机会。
- **PDF**: https://arxiv.org/pdf/2608.16869v1

---