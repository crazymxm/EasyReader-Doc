# 🗓️ 周报 (2026-W32)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-08-09

--- 
## 📚 学科: `eess.*`
本周 `eess.*`（电气工程与系统科学）领域精选了5篇高质量论文，涵盖了高光谱图像处理、音频处理、视频压缩、交通定位和控制理论。论文分别探讨了基于无监督光谱校准的高光谱变化检测方法、结合扩散模型与可微分调音台的音乐混音系统、实现超低码率实时视频编码的GVC-RT模型、结合几何感知和深度学习的路侧单目摄像头车辆精确定位，以及利用无源性理论对一阶动量优化算法进行的收敛性分析。这些研究不仅在理论上有重要突破，还在多媒体、智能交通等实际场景中展示了强大的应用价值。

### Hyperspectral Calibration Detection: A Novel Concept For Change Detection With Unsupervised Incremental Safe Pseudo-Labeling Implementation
- **分数**: 4
- **链接**  https://arxiv.org/abs/2608.06028v1
- **作者**: Chia-Hsiang Lin, Shih-Min Hsu, Ching-Yun Liang, Jocelyn Chanussot, Jhih-Yan Chen
- **备注**: 16 pages, 21 figures, 3 tables. Accepted for publication in IEEE Transactions on Image Processing
- **摘要**: 高光谱变化检测 (HCD) 在土地覆盖监测等领域有许多关键应用。大多数基准 HCD 算法是半监督方法，有些甚至能实现极低的样本标注率。然而在一些实际场景中（例如需要机载边缘计算进行即时检测响应），由于无法为新获取的图像获取地面真实标注，我们必须满足零标注的要求。在这项工作中，我们提出了一种完全无监督的 HCD 算法，并结合了一个轻量级模型，非常适用于机载检测任务。基于安全收集一些未变化像素样本的迭代增强训练集，我们学习了一个迭代精细化的光谱校准函数，最终补偿了获取条件的变化（这在双时相图像中经常观察到），从而通过分析校准后的光谱使变化的像素易于被检测。所提出的高光谱循环无监督校准和增量检测 (HyperLUCID) 算法不仅计算效率高（比大多数基准 HCD 方法快 1 到 2 个数量级），而且在几个真实基准 HCD 数据集上达到了最先进的结果（整体准确率约为 93.6% 至 97.9%）。开源代码：https://github.com/IHCLab/HyperLUCID。
- **PDF**: https://arxiv.org/pdf/2608.06028v1

### Diff2Mix: Controllable Music Mixing via Diffusion Models and Differentiable Audio Effects
- **分数**: 4
- **链接**  https://arxiv.org/abs/2608.05442v1
- **作者**: Yisu Zong, Jinjie Shi, Joshua Reiss
- **备注**: Accepted to ISMIR 2026
- **摘要**: 自动音乐混音旨在将多轨录音组合成平衡且连贯的音乐作品。由于不同歌曲的内容以及混音师的主观偏好共同塑造了最终结果，一个实用的系统应该在提供平衡混音的同时，允许可控的风格变化。然而，大多数现有方法将自动混音和混音风格控制视为两个独立的任务，这使得单一系统难以在保持可编辑性和风格感知的同时产生高质量的混音。为了解决这一局限性，本文提出了 Diff2Mix，这是一个基于扩散模型和可微分调音台的生成式自动混音系统。该系统提供了两个级别的可选用户控制：参考音频实现了整体制作风格的控制，而可微分调音台则提供了明确的音频效果参数，以实现可解释性和细粒度的优化。我们通过在混音质量和控制能力方面的客观和主观评估，展示了我们系统的竞争性能。我们在项目主页 https://zys711.github.io/Diff2Mix 上提供了代码和音频示例。
- **PDF**: https://arxiv.org/pdf/2608.05442v1

### GVC-RT: Towards Real-Time Generative Video Compression at Ultra-Low Bitrates
- **分数**: 4
- **链接**  https://arxiv.org/abs/2608.04891v1
- **作者**: Tianjian Dang, Sixian Wang, Lei Luo, Guo Lu, Jincheng Dai
- **备注**: Accepted to appear in the Proceedings of the 34th ACM International Conference on Multimedia (MM '26). 10 pages, 9 figures, and 2 tables. Code: https://github.com/semcomm/GVC-RT
- **摘要**: 最近的生成式视频编解码器 (GVC) 通过压缩生成式分词器的 token，在超低比特率（每个像素小于 0.02 比特）下实现了令人瞩目的重建保真度。然而，现有的 GVC 通常需要大量的计算时间和模型复杂度，这阻碍了它们在计算受限设备和实时应用中的部署。为了弥补这一差距，我们系统地识别了计算瓶颈，并提出了 GVC-RT。该方法重新设计了生成式隐式编码框架，以在不牺牲压缩性能的情况下实现实时视频编码。具体而言，GVC-RT 基于预训练的免查找量化 (LFQ) 分词器，采用了一种非对称架构，直接学习匹配 LFQ 隐空间分布，而生成空间对齐仅在训练期间通过正则化损失项进行强制约束。通过这种方式，我们在推理阶段绕过了繁重的分词过程，并完全移除了复杂的特征对齐过程。此外，我们还引入了一种轻量级的反分词器架构，以解决解码过程中的最终延迟瓶颈。实验结果表明，GVC-RT 的性能超越了之前的 SOTA 模型 GLC-Video，在 DISTS 和 LPIPS 方面分别实现了平均 12.4% 和 48.8% 的 BD-rate 节省，同时在 1080p 视频上实现了 123.1/55.1 fps 的编码/解码速度。代码见 https://github.com/semcomm/GVC-RT。
- **PDF**: https://arxiv.org/pdf/2608.04891v1

### Accurate Localization of Road Traffic Objects on the Road Plane Using Surveillance Camera Imagery
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.05840v1
- **作者**: Jan Gawroński, Witold Czajewski
- **备注**: 8 pages, 7 figures. Accepted for publication in the proceedings of the 2026 Progress in Applied Electrical Engineering (PAEE) conference
- **摘要**: 利用单目路侧监控摄像头进行精确的车辆定位对于智能交通系统、交通监控和交通冲突分析至关重要。标准方法通常根据检测器边界框的中心来估计车辆位置，由于透视畸变和视差，这可能会产生很大的误差，特别是对于高位摄像头和大型车辆。本文提出了一种两阶段几何感知定位管线，用于估计车辆接地面投影到道路平面上的形状。首先，使用基于 YOLO 的检测器检测车辆。其次，专用的 ResNet34 回归网络预测对应于投影车辆底面的四个角点。最终位置计算为预测四边形的几何中心。该方法在 CARLA 中生成的合成数据上进行了训练，并在来自 DAIR-V2X 的真实路侧图像上进行了微调。在合成和真实数据上的实验表明，相比于幼稚的边界框中心定位，该方法有明显的改进。在 DAIR-V2X 数据集上，图像空间定位平均误差从 31.77 像素降至 15.30 像素（提升 51.8%），中值误差降至 4.29 像素。中等距离车辆的地平面中值误差从 5.52 米降至 0.90 米，远距离车辆从 8.67 米降至 1.84 米。结果还表明，检测器边界框周围的上下文信息对几何定位至关重要。在受到强烈透视畸变和视差影响的远距离车辆和几何上具有挑战性的情况下，效果提升最为显著。
- **PDF**: https://arxiv.org/pdf/2608.05840v1

### A Passivity-Based Analysis of First-Order Momentum-Based Methods
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.05492v1
- **作者**: Sepehr Moalemi, James Richard Forbes
- **备注**: 6 pages, 4 figures, 1 table. Accepted to the 65th IEEE Conference on Decision and Control (CDC)
- **摘要**: 本文针对一类其梯度分别具有 0 和 L 下上扇区边界的函数，提出了基于一阶动量的算法的离散时间无源性分析方法。通过循环变换，表明动量法可以表示为与输出严格无源（OSP）系统呈负反馈的无源控制器。然后利用弱无源性定理推导出了显式的超参数条件，在这些条件下，偏移梯度渐近消失。在要求存在唯一平稳点并排除远离该点但梯度任意小的附加假设下，建立了迭代步收敛到全局极小值的结论。
- **PDF**: https://arxiv.org/pdf/2608.05492v1

--- 
## 📚 学科: `q-bio.*`
本周 `q-bio.*`（定量生物学）领域精选了3篇具有重要临床及理论价值的论文。这些论文探讨了生物医学和认知科学中的关键问题，包括：通过分析细胞因子基因中的单核苷酸多态性（SNP）来预测炎症性肠病（IBD）患者接受靶向治疗后的生化缓解情况；利用信息论框架和熵最小化原理对自闭症患者“坚持一致性”的行为特征进行定量化解释；以及在临床预后建模中，指出将生存结局（事件发生时间数据）强行进行二值化处理所带来的信息丢失代价，并提出了生存感知贝叶斯网络作为改进方案。

### IL-10 rs1800896 polymorphism predicts biochemical remission in IBD patients undergoing biologic therapy
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.05345v1
- **作者**: Michela Helga Falzone, Davide Giuseppe Ribaldone, Martina Buglione, Irene Cottone, Marta Vernero, Demis Pitoni, Angelo Armandi, Francesca Saba, Eleonora Dileo, Alfredo Santovito, Gian Paolo Caviglia
- **备注**: 22 pages; 2 main tables and 1 main figure; supplementary tables and figure included. Pre-peer-reviewed author manuscript. The final article was published in Immunology, 2026, volume 177, issue 2, pages 432-438
- **摘要**: 背景：包括单核苷酸多态性（SNP）在内的遗传因素可能会调节炎症性肠病（IBD）患者的病程和治疗效果。目的：我们研究了细胞因子基因中的四个 SNP 与 IBD 患者临床表型及分子靶向药物治疗反应之间的关联。材料与方法：共纳入 197 例接受靶向治疗的 IBD 患者（142 例克罗恩病 [CD]，55 例溃疡性结肠炎 [UC]）。分析的 SNP 包括 TNF-alpha rs1800629（-308 G>A）、TGF-beta rs1800471（密码子 10 C>T）、IL-6 rs1800795（-174 G>C）和 IL-10 rs1800896（-1082 G>A）。12 个月（T12）时的生化缓解定义为在无持续皮质类固醇治疗的情况下，T12 时的 CRP <5.0 mg/L 且粪便钙卫蛋白 <250 microg/g。结果：IL-6 rs1800795 C 等位基因与较年轻的诊断年龄显著相关（p=0.049），而 TNF-alpha rs1800629 A 等位基因在 CD 患者中的观察频率高于 UC 患者（p=0.036）。在纳入符合方案分析的 134 例患者中，41.0% 在 T12 时达到生化缓解。IL-10 rs1800896 变异等位基因与缓解相关（OR 2.15，95% CI 1.03-4.44；p=0.041），且该关联在多变量分析中保持显著（调整后 OR 4.15，95% CI 1.49-11.56；p=0.007）。结论：细胞因子相关 SNP 的基因分型可能有助于识别具有独特疾病表型的患者，并支持 IBD 的个体化治疗策略。
- **PDF**: https://arxiv.org/pdf/2608.05345v1

### An entropic explanation of insistence on sameness in autism
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.04616v1
- **作者**: Przemysław Śliwiński
- **备注**: 11 pages, 2 figures, a preprint of the accepted article
- **摘要**: 本文提出了一个基于信息论的框架，旨在将自闭症中对“保持一致性”的坚持解释为个体试图减少惊讶和不确定性的一种通用行为模式。它提供了一种对自闭症的新定义，即一种将认知功能限制在辨别、记忆和预测环境中具体属性的障碍。通过在一组描述自闭症患者认知局限性的假设下进行研究，观察到了坚持一致性与受约束的信息熵指标最小化之间的类比。该指标由公式 $D_H(R, M) = H(R|M) + H(M|R)$ 给出，其中 $R$ 代表随机刺激序列，$M$ 是存储和检索这些刺激的记忆，而 $H(.|.)$ 表示它们的条件熵，分别被解释为惊讶和不确定性。首先推导出，为了使该指标最小化，个体可以学习 $R$（并将该知识存储在 $M$ 中），或者可以将 $R$ 限制在已知的 $M$ 中。随后得出结论，对保持一致性的坚持是后者的体现。此外，研究表明，所提出的框架：（1）有助于量化惊讶、不确定性、感官超载与剥夺、焦虑、舒适区、失望、迷失方向、拘泥细节、刻板、遵守规则或异常精确度等概念。（2）为学习疗法和日常护理流程提供了一系列指导方针，并允许将它们定义为优化算法，并实现为机器人住家护理员的程序。（3）可以借助类似于图灵测试的方法进行验证，无需涉及自闭症个体的实验。如果该框架得到积极验证，将为旨在提高自闭症患者在基本日常生活活动中自理能力的疗法提供正式的理论基础和设计指南。
- **PDF**: https://arxiv.org/pdf/2608.04616v1

### The Cost of Binarizing Survival Outcomes in Clinical Prognostic Modeling
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.04046v1
- **作者**: Shashank Yadav, David M. Routman, Andrew Y. K. Foong
- **备注**: Accepted to Machine Learning for Healthcare (MLHC) Conference 2026
- **摘要**: 生存分析是分析事件发生时间数据的成熟框架，然而许多临床机器学习研究在模型训练前仍会将结局进行二值化。这种做法排除了删失（censored）患者，将时间信息压缩为单一阈值，并可能影响哪些特征被筛选为具有预后相关性。我们在贝叶斯网络（BN）特征选择的背景下检验了这种二值化的代价，并以最近的两篇发表论文作为案例研究：一篇将基于 BN 的特征选择应用于头颈癌队列，另一篇是外科队列研究，后者虽然不基于 BN，但同样对其生存终点进行了二值化。我们用针对特征到结局边缘的 Cox 偏对数似然代替了二值评分函数，并将这一修改命名为“生存感知贝叶斯网络（Survival-Aware Bayesian network）”，从而恢复了二值化所遗漏的预后特征。我们的消融实验证实，这种改进是由事件发生时间评分公式驱动的，而不是由于保留了更多患者。结果在头颈癌的五种终点-队列组合中得到了推广，并延伸到另外三种癌症类型（乳腺癌、结直肠癌和肾癌）。我们建议，具有生存结局的临床研究应默认使用事件发生时间（time-to-event）方法，因为二值化会丢弃生存分析所保留的预后信号。
- **PDF**: https://arxiv.org/pdf/2608.04046v1

--- 
## 📚 学科: `cs.*`
本周 `cs.*`（计算机科学）领域精选了1篇针对医学图像处理的高质量应用论文。该研究深入探讨了医学影像超分辨率（SR）技术在脑白质高信号（WMH）分割中的实际影响，揭示了超分辨率算法对微小病变的主要副作用是“抹除”真实病变而非“幻觉”虚假病变，并系统评估了多种重建算法与分割方法在此任务上的表现，为临床神经影像预处理提供了重要的实证依据。

### Does FLAIR super-resolution erase or hallucinate small white-matter lesions?
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.06311v1
- **作者**: Zahra Khodakarami, Yue Li, Pulkit Khandelwal, John Detre, Sandhitsu Das, Christopher Brown, David Wolk, Paul Yushkevich
- **备注**: 10 pages, 2 figures, 3 tables. Accepted at the 11th International Workshop on Simulation and Synthesis in Medical Imaging (SASHIMI 2026), held in conjunction with MICCAI 2026. This is the version submitted for review; the final authenticated version will appear in the Springer LNCS proceedings
- **摘要**: 脑白质高信号（WMH）是液体衰减反转恢复（FLAIR）扫描中的明亮区域，与脑血管病变和神经退行性变有关。在临床设置中，FLAIR 通常是以较厚的切片获取的，从而导致其面外（through-plane）分辨率较差。超分辨率（SR）是一种广泛用于从各向异性扫描中恢复各向同性体积的方法。然而，在进行 WMH 分割之前应用超分辨率是否能保留病变内容仍是未知的：模型可能会抹去微小的真实病变，或者幻觉出不存在的病变。我们使用了 ADNI 队列中 29 名受试者的 1 mm 各向同性高分辨率（HR）FLAIR 扫描图像，每张图像均由专家手动进行了 WMH 分割。然后，我们将每张图像降级为模拟的 3 mm 和 5 mm 面外获取图像。利用多对比度隐式神经表示（INR）、单对比度自监督模型（ECLARE）和三次插值将其上采样到 HR 网格上。基于模拟厚切片和原始 HR FLAIR 的 WMH 分割分别设定了每个病变分析的下限和上限。在四种 WMH 分割方法（WMH-SynthSeg、segcsvd、MARS-WMH、TrUE-Net）中，我们在对 HR 上的微小病变最敏感的方法（MARS-WMH）下进行了分析，评估指标包括检测敏感性、抹除率（重建后丢失的 HR 检测病变）和幻觉率（在手动和 HR 分割中均不存在的预测成分）。超分辨率的主要影响是抹去微小的真实病变，而不是产生幻觉，并且这种影响随着切片厚度的增加而增加，尽管相比于原始的厚切片，每种重建方法仍然提高了病变检测能力。在两种厚度下，ECLARE 恢复微小病变信号的效果最好，而 INR 的表现并不优于三次插值。
- **PDF**: https://arxiv.org/pdf/2608.06311v1

--- 
## 📚 学科: `math.*`
_本周缺少高价值论文_

--- 
## 📚 学科: `astro-ph.*`
本周 `astro-ph.*`（天体物理学）领域精选了5篇极具科研价值的高水平论文。研究内容广泛，从恒星演化到宇宙学尺度均有涉及。具体成果包括：首次探测到碳星V420 Vul周围延伸达20秒差距的星际中性氢（H I）包层；通过三维数值模拟揭示了核状态方程（EoS）对磁旋转超新星爆发多信使辐射的深远影响；基于SDSS和DESI海量光谱数据构建了红移在1.0到3.5之间、迄今最完备的1型类星体光度函数（QLF）；通过SDO卫星数据证实了热非平衡（TNE）循环在太阳伪流线及开放磁场中的存在；以及利用SUNRISE-III气球空间望远镜的高分辨率红外光谱观测，首次揭示了太阳黑子本影内耀斑核在色球层中的千米级精细动力学结构。

### HI envelope around the carbon star V420 Vul
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.06245v1
- **作者**: Xu-Jia Ouyang, Yong Zhang, Chuan-Peng Zhang, Li-Yun Zhang
- **备注**: 8 pages, 5 figures, 1 table. Accepted for publication in A&A Letters
- **摘要**: 我们报告了利用阿雷西博星系 L 波段馈源阵列（ALFA）的历史巡天数据，在米拉变星 V420 Vul 方向上探测到一个延伸的 21 厘米秒差距级中性氢（H I）结构。该辐射表现出空间相干但强度不对称的形貌，但仍保留了以 $v_{\mathrm{LSR}} \sim 47.6\,\mathrm{km\,s^{-1}}$ 为中心的全局对称运动学轮廓。在采用的约 1.9 kpc 距离下，该结构延伸超过约 20 pc，这意味着其动力学时间尺度在 $10^6$ 年的数量级。尽管总中性氢质量（约 70 M_sun）表明原子气体储层主要由周围的星际介质主导，而非原始的恒星抛射物，但空间分辨率光谱和位置-速度图揭示了一个以该恒星为中心的潜在对称速度框架。我们将此解释为恒星风优先穿过多孔周围星云的动力学印记，表明尽管存在主导性的星际学耦合，但恒星晚期质量流失的凝聚运动学记录仍可以在秒差距尺度和百万年时间尺度上得以保留。
- **PDF**: https://arxiv.org/pdf/2608.06245v1

### The impact of nuclear equations of state on the dynamics and multi-messenger emission of magnetorotational stellar explosions
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.06017v1
- **作者**: Andrea Celati, Matteo Bugli, Luca Del Zanna, Marco Cusinato, Martin Obergaulinger
- **备注**: Accepted for publication in Astronomy & Astrophysics. 21 pages, 17 figures
- **摘要**: 大质量恒星在生命终结时的引力塌缩会导致强大的超新星爆发，从而产生致密天体，调节宿主星系的动力学，并对宇宙化学演化做出贡献。在快速自转和强磁场存在的情况下，这类爆发可以达到极高能量，从而解释了超亮超新星（hypernovae）和长伽马射线暴等源。我们研究了核状态方程（EoS）的变化对磁旋转爆发及其多信使辐射（包括中微子和引力波）的影响。EoS 在硬度、成分和有限温度行为上的差异会影响塌缩、反弹和喷流发射阶段。使用包含相对论磁流体力学、双矩中微子输运、中微子-物质相互作用和广义相对论修正的 Aenus-Alcar 代码，我们对不同的 EoS 进行了轴对称模拟。所有模型都始于同一个具有太阳金属丰度、零龄主序质量为 20 倍太阳质量、偶极磁场和壳层自转剖面的前超新星前身星。不同的 EoS 在爆炸动力学、原中子星性质、抛射物质量和多信使信号方面产生了显著差异。我们的结果表明，磁旋转塌缩核心超新星的特征不仅取决于 EoS 的冷硬度，还取决于其热和成分特性，这强调了结合引力波和中微子观测来约束高密物质物理和爆炸机制的重要性。
- **PDF**: https://arxiv.org/pdf/2608.06017v1

### Luminosity function of quasars at $1.0<z<3.5$ from SDSS and DESI
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.06000v1
- **作者**: Gaocheng Yin, Linhua Jiang, Zhiwei Pan, Paul Martini, Wei-Jian Guo, Siwei Zou, Shengxiu Sun, Swayamtrupta Panda, Abhijeet Anand, Benjamin Alan Weaver, Aaron Meisner, Andrei Cuceu, Arjun Dey, Axel de la Macorra, Christophe Magneville, David Brooks, David Kirkby, David Schlegel, David Sprayberry, Davide Bianchi, Dick Joyce, Enrique Gaztañaga, Eusebio Sanchez, Francisco Javier Castander, Francisco Prada, Gaston Gutierrez, Graziano Rossi, Gregory Tarlé, Hiram K. Herrera-Alcantar, Hu Zou, Ignasi Pérez-Ràfols, Jaime E. Forero-Romero, Jessica Nicole Aguilar, John Moustakas, Joseph Harry Silber, Klaus Honscheid, Laurent Le Guillou, Marc Manera, Martin Landriau, Michael Schubnell, Mustapha Ishak, Nathalie Palanque-Delabrouille, Peter Doel, Ramon Miquel, Robert Kehoe, Satya Gontcho A Gontcho, Seshadri Nadathur, Simone Ferraro, Stephanie Juneau, Steven Ahlen, Theodore Kisner, Todd Claybaugh, Will Percival, Anthony Kremin, Claire Lamman, Claire Poppett, Rongpu Zhou
- **备注**: 16 pages, 6 figures. Accepted for publication in The Astrophysical Journal
- **摘要**: 我们展示了一项关于红移在 $1.0<z<3.5$ 之间的 1 型类星体演化的研究，该阶段覆盖了类星体活动的巅峰时期。以往的诸多工作已对类星体的演化进行了广泛探索，但推导出的类星体光度函数（QLFs）彼此并不十分一致，这可能是由于不同类星体挑选技术及相关完整度修正所引入的复杂性。我们采用了一种基于所有已知类星体库构建 QLF 的新策略。我们重点关注了一个约 1700 平方度的宽区域和一个约 265 平方度的深空区，这些区域拥有主要来自 SDSS 和 DESI 的丰富光谱数据。然后，我们在静止波段的紫外/光学波段中应用传统的颜色切割来选择候选类星体，并利用类星体库对其进行识别。我们最终的样本包含 62,426 个红移在 $1.0<z<3.5$ 之间的类星体，在颜色选择中具有极高的完整度（约 96%）和纯度（约 93%）。简单的颜色切割可以潜在地减少研究类星体演化时的选择偏差。我们推导了分箱 QLF，并使用双幂律模型对其进行表征。样本的不完整性和污染被计入计算的不确定性中。与先前的结果相比，我们的 QLF 在暗端略高，在 $2.5<z<3.5$ 时的亮端也更高。该 QLF 表明，在 $1.0 < z < 2.5$ 时的类星体演化可以很好地由纯光度演化模型描述，而在 $2.5 < z < 3.5$ 时，则可以由纯光度演化或纯密度演化模型来描述。
- **PDF**: https://arxiv.org/pdf/2608.06000v1

### Thermal Non-equilibrium Cycles in a Non-eruptive Pseudo-Streamer
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.05986v1
- **作者**: Clara Froment, Sophie Masson
- **备注**: 32 pages, 11 figures, published in Solar Physics. Truncated abstract to match arXiv requirements
- **摘要**: 热非平衡（TNE）是一种著名的热力学机制，通常在日冕环中进行研究。这些蒸发和冷凝循环是由准稳态和分层的加热诱导的。长周期极紫外（EUV）脉动和日冕雨是 TNE 的两种表现形式。循环的准周期性是 TNE 的一个显著特征，因为系统在一个无法达到的平衡位置周围动态演化。最近有关于在开放-封闭边界（如扇形-脊形拓扑和伪流线）处出现日冕雨的报道。然而，关于驱动这些日冕雨事件的物理机制尚无明确结论。我们报告了利用 SDO 上的 AIA 观测到的非爆发性伪流线中检测到的长周期 EUV 脉动和共空间循环日冕雨。结合 PFSS 模型和 EUV 动力学，详细研究了该伪流线的磁拓扑和演化。这个持续 2.5 天的事件展示了先前在日冕环中报道的 TNE 事件的所有特征：在不同通道中依次出现的周期性 EUV 脉冲（遵循其温度响应峰值的顺序），以及在这些循环结束时出现的日冕雨。我们进一步表明，伪流线中的 TNE 循环不仅发生在闭合磁场中，也发生在开放磁场中。我们的观测支持了最近数值研究的发现，即 TNE 也可以发生在开放磁场区域和开放-封闭边界处。与此同时，在 EUV 中观察到，互换重联在整个开放-封闭边界上持续且非爆发性地发生。在未来的工作中，应详细研究 TNE 与互换重联之间的相互作用。这一观测为理解太阳大气中的 TNE 及其对太阳风的潜在影响开拓了进一步的前景。
- **PDF**: https://arxiv.org/pdf/2608.05986v1

### Chromospheric Dynamics of an Umbral Flare Kernel - Based on Coordinated SUNRISE III SCIP and Domeless Solar Telescope Observations
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.05977v1
- **作者**: Ayumi Asai, Satoru UeNo, Takuma Matsumoto, Takayoshi Oba, Yukio Katsukawa, Masahito Kubo, Ryohtaroh T. Ishikawa, Yusuke Kawabata, Hirohisa Hara, Yoshihiro Naito, Toshifumi Shimizu, Sami K. Solanki, Andreas Lagg, Achim Gandorfer, Jose Carlos del Toro Iniesta, Pietro Bernasconi, Thomas Berkefeld, Alex Feller, Tino L. Riethmuller, Alberto Alvarez-Herrero, H. N. Smitha, David Orozco Suarez, Bianca Grauf, Michael Carpenter, Alexander Bell, Valentin Martinez Pillet, Laurent Gizon, Francisco Javier Bailen, Julian Blanco Rodriguez, Juan Sebastian Castellanos Duran, Edvarda Harnes, Johannes Hoelken, Francisco A. Iglesias, Azaymi L. Siu-Tapia, Hanna Strecker, Dusan Vukadinovic, SUNRISE-III team
- **备注**: 11 pages, 5 figures, Accepted for publication in ApJL (a part of the Focus Issue on Sunrise III)
- **摘要**: 我们报告了在 SUNRISE-III 气球任务搭载的红外光谱偏振仪 SCIP 与京都大学飞驒天文台无圆顶太阳望远镜（DST）联合观测期间，获得的一次 M1.4 级太阳耀斑的成像光谱观测结果。该耀斑于 2024 年 7 月 13 日发生在 NOAA 活动区 13738 中，表现出位于太阳黑子本影内的一个紧凑的耀斑核。SCIP 在本影周围 58" x 58" 的视场内进行了快速狭缝扫描观测，时间分辨率为 40 秒，覆盖了包括 Ca II 8498/8542 A 和 K I D1 在内的红外色球层和上光球层谱线。与此同时，DST 以 25 秒的时间分辨率在 H-alpha、Ca II 8542 A 和 Na I D1/D2 谱线中观测了更广泛的周边区域。在 SCIP 和 DST 观测的所有色球谱线中均检测到明显的耀斑相关增亮，而在光球谱线中未发现显著增强。SCIP 的高空间分辨率揭示了耀斑核内尺度在 1000 千米量级的精细子结构，而这些结构在地面观测中显得模糊。光谱剖面展现了随时间和空间变化的多普勒频移和谱线展宽，表明色球层中存在复杂的精细尺度等离子体运动。这些结果表明，正如 SCIP 所揭示的那样，观测到的红色不对称性源于多个精细尺度耀斑核在时间上的相继演变，而不是源于单一的连续过程。
- **PDF**: https://arxiv.org/pdf/2608.05977v1

--- 
## 📚 学科: `stat.*`
本周 `stat.*`（统计学）领域推荐了1篇关于个性化医疗决策的理论与应用并重的论文。该研究针对传统动态治疗方案（DTR）仅关注平均疗效和二元决策的局限，提出了“风险感知分位数动态治疗方案（RQDTR）”框架。该方法不仅能优化结局分布的临床尾部特征，还能显式引入治疗风险并支持多类别决策。在建立严格统计一致性和有限样本误差理论的同时，在重度抑郁症和脓毒症真实临床数据集上验证了该方法出色的效益-风险权衡表现。

### Risk-Aware Quantile Learning for Personalized Dynamic Treatment Regimes
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.05434v1
- **作者**: Chunyin Lei, Annie Qu
- **备注**: An earlier version of this work was accepted at STAI-X 2026
- **摘要**: 顺序临床决策通常不仅涉及最大化平均疗效。临床医生可能需要同时优化结果分布中具有临床相关性的尾部、控制治疗相关风险，并在多种治疗方案中进行选择。现有的分位数动态治疗方案（DTR）方法捕捉了治疗结局的分布特征，但很大程度上仍局限于仅关注疗效的目标和二元治疗。为了解决这些局限性，我们提出了风险感知分位数动态治疗方案（RQDTR），这是一个统一的框架，旨在优化累积潜在结果的预设分位数，同时显式地引入治疗相关风险。我们还开发了一种基于角度的公式，用于联合学习多个治疗类别的决策规则。我们的框架包括三个具有可解释性的子类：仅疗效的分位数学习、具有人群级别风险控制的基于约束的学习，以及通过复合效益-风险效用进行的基于效用的学习。在理论上，我们建立了识别性和 oracle 等价性、平滑替代函数的 Fisher 一致性、估计方案的一致性以及有限样本性能误差率。广泛的模拟研究以及在 All of Us 重度抑郁症和 MIMIC-III 脓毒症数据上的应用表明，与现有的分位数 DTR 方法相比，RQDTR 改善了面向尾部的疗效，并实现了更优的效益-风险权衡。
- **PDF**: https://arxiv.org/pdf/2608.05434v1

--- 
## 📚 学科: `econ.*`
本周 `econ.*`（经济学）领域推荐了1篇发表于《法律与经济学杂志》的高质量实证论文。该研究采用基于设计的双重机器学习（Double Machine Learning）方法，结合澳大利亚新南威尔士州的全新行政数据集，深入探讨了拒绝法律援助对贫困被告法庭判决结果的因果影响。研究发现，未通过资助审查而被迫雇佣私人律师的被告，其监禁率显著降低了10个百分点，但在被监禁的情况下刑期反而可能更长。这一发现为评估政府法律援助资源分配的效率及公平性提供了微观计量经济学证据。

### Legal aid eligibility and court outcomes: a design-based double-machine-learning approach
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.05211v1
- **作者**: Fabio Italo Martinenghi
- **备注**: Accepted for publication at the Journal of Law & Economics
- **摘要**: 法律面前人人平等是一项基本人权，而为贫困被告提供高质量的法律援助对于实施这一权利至关重要。在所有被告均能获得律师协助的背景下，我研究了拒绝法律援助对法庭判决结果的影响。我将双重机器学习与一个连接澳大利亚新南威尔士州法律援助与法庭判决的新行政数据集相结合，以学习输入已知的分配函数。我发现，未能通过资产审查并自行聘请私人律师的申请人，其被监禁的可能性比通过审查并依赖法律援助的申请人低 10 个百分点。鉴于平均监禁时间接近四年，这一差距是非常显著的。然而，我发现有证据表明，如果他们被监禁，他们在监狱中度过的时间会更长。政府对广泛提供援助的偏好（而非在每个案件上分配的时间）可能会解释这种模式。
- **PDF**: https://arxiv.org/pdf/2608.05211v1

---