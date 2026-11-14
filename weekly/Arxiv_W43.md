# 🗓️ 周报 (2026-W43)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-10-25

--- 
## 📚 学科: `eess.*`

**学科总结**：
本周 EESS 领域的精选论文集中在图像压缩、数据聚类与伪造检测等前沿方向。研究涵盖了基于约束优化的高效渐进式图像压缩算法（NeurIPS 2026）、结合打乱匿名的单轮联邦密度峰值聚类方法，以及专注于唇部细节的音视频一致性伪造检测技术。这些研究体现了深度学习与经典信号/控制理论融合的趋势，在大幅降低参数量与计算开销的同时，显著提升了传输效率、隐私安全与伪造鉴别能力。

### Bound-Conditioned Latent Inference for Progressive Image Compression
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.30966v1
- **作者**: Jaeseok Jang, Seungmin Jeon, Kwang Pyo Choi, Chang-Su Kim
- **备注**: Accepted to NeurIPS 2026
- **摘要**: 渐进式图像压缩通过单比特流的前缀重构图像，涉及局部观测下的序列隐变量推断。针对现有三进制平面编码未充分利用解码三进制作为连续隐变量区间约束的问题，本文提出边界条件隐变量推断（BLI）框架，将渐进编码重构为收缩区间约束下的序列推断。在每个编码步骤中，至今已解码的三进制定义了每个隐元素的上下界。BLI结合界限中心与宽度以及编解码器共享的超先验信息，共同优化用于熵建模的高斯参数 $(μ, σ)$ 和重建隐估计 $\hat{y}$。在 Kodak、CLIC 和 JPEG-AI 数据集上的实验表明，BLI 在渐进式图像编解码器中取得了 SOTA 的率失真性能，且参数量较 CTC 减少约 5.3 倍，延迟也更低。
- **PDF**: https://arxiv.org/pdf/2610.30966v1

### Evolving Federated Density Peak Clustering with Shuffler-Based Anonymization
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.31211v1
- **作者**: Miha Ožbot, Seiichi Ozawa, Igor Škrjanc
- **备注**: Published open access (CC BY 4.0) in Evolving Systems 17, 123 (2026)
- **摘要**: 本文提出了一种基于演化模糊数据流聚类和基于打乱器（Shuffler）匿名的单轮联邦聚类方法（eFDPC）。在联邦聚类中，即使不直接共享原始数据，多轮交互也会增加推断本地数据集属性的风险。每个客户端通过聚类添加与合并从私有微批次数据中独立演化微聚类，随后仅传输选定的密度峰值而非完整模型。客户端与服务器之间引入打乱层，在全局峰值选择前对贡献进行匿名化。实验结果表明，eFDPC 在单轮设置下优于现有联邦聚类基线，并能有效拓展至高维、非独立同分布（non-IID）数据。
- **PDF**: https://arxiv.org/pdf/2610.31211v1

### Lip-Focused Audio-Visual Consistency Detects Speech Content Manipulation beyond Coarse Synchronization
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.30872v1
- **作者**: Jian Zong, Chenghan Lin, Meng Liu, Zhao Xu, Junyu Wang, Siyuan Zhang, Peiyuan Jiang, Longbiao Wang, Jianwu Dang
- **备注**: Accepted by NCMMSC 2026
- **摘要**: 语音内容篡改通过替换音频甚至重新生成嘴部动作改变发言人表述，因现代唇形同步模型高度优化了音视频同步性而难以通过纹理瑕疵检测。本文验证了一个假设：即便控制了说话人身份或粗粒度同步，语音替换仍会扰动声学动态与嘴部动作之间的局部关系。为此，本文构建了 SyncSpeech 基准，并设计了专注于唇部区域的检测器 C-MIND，该检测器在帧级别对齐音频和嘴部动作表征，无需文本转录、ASR 特征或未经篡改的参考视频即可对一致性建模。在 SyncSpeech 和 FakeAVCeleb 数据集上的实验表明，该方法展现出优异的伪造检测精度与泛化能力。
- **PDF**: https://arxiv.org/pdf/2610.30872v1

--- 
## 📚 学科: `q-bio.*`

**学科总结**：
本周定量生物学领域的精选论文涵盖了计算神经科学中的方法论反思、空间转录组学中的几何表征学习以及骨科生物力学实验应用。具体包括：揭示脑电图（EEG）机理模型推断中门控特征重要性评估的潜在陷阱（NeurIPS Workshop）、结合几何先验与方向敏感性的空间转录组表征模型 Tessera，以及关于振荡锯轨迹优化对骨科手术中骨表面的力学完整性保护研究。

### Gate-Based Feature Importance in Simulation-Based Inference for EEG: A Cautionary Tale
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.30364v1
- **作者**: Shrivatsa Deshmukh, Sasha Brenner, Thomas R. Knösche, Nico Scherf
- **备注**: Accepted at NeurIPS 2026 workshops (Sim2Science & Interp4Discovery)
- **摘要**: 基于模拟的推断（SBI）为将机理模型拟合到数据提供了强大工具，但难以明确数据中哪些特征主导了推断参数。本文在计算神经科学背景下探讨了基于学习门控权重（gate weights）特征重要性评估方法的可靠性。研究发现在 Jansen-Rit 神经群模型中，门控权重与基于消融（Ablation）的标准评估结果呈显著负相关（Spearman系数约 -0.61 与 -0.56）。消融表明最重要的特征（总信号功率）在门控机制中却被大幅降权。该结果提醒科研人员在科学机器学习管线中将学习到的门控权重解释为因果特征重要性时应保持谨慎。
- **PDF**: https://arxiv.org/pdf/2610.30364v1

### Spatially Informed and Direction Sensitive Representation Learning for Spatial Transcriptomics
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.28579v1
- **作者**: Azim Dehghani Amirabad, Ali Khodabandeh Yalabadi, Artem Moskalev, Yun-Ching Chen, Mehdi Pirooznia, Scott Oloff, Rui Liao
- **备注**: Accepted at NeurIPS 2026 Workshop (AI4DD)
- **摘要**: 细胞状态受固有基因表达与空间微环境共同塑造。本文提出 Tessera 空间表征学习框架，结合了空间信息基因选择与几何归纳偏置。通过对相对细胞间关系建模，Tessera 具备平移不变性同时保留方向信息，使邻近细胞能够根据其空间上下文与细胞状态做出不同贡献。实验表明，Tessera 在表征质量上超越了现有的空间基础模型，并在未经训练的大规模（达训练集16倍）组织上下文中实现了优秀的零样本泛化能力。
- **PDF**: https://arxiv.org/pdf/2610.28579v1

### Turning-Point Impact Compromises the Biomechanical Integrity of Cortical Bone during Oscillating Sawing
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.28234v1
- **作者**: Han Wang, Urara Satake, Toshiyuki Enomoto
- **备注**: Published in Annals of Biomedical Engineering
- **摘要**: 在全膝关节置换等骨科手术中广泛使用振荡骨锯，保留骨表面的力学完整性对植入物稳定性至关重要。本文研究了振荡锯切过程中轨迹转向点冲击载荷的生物力学后果。通过对比传统轨迹与优化后抑制转向点冲击的轨迹，结果表明传统轨迹产生周期性应力峰值并导致广泛表面裂纹，削弱局部抗压强度；而优化轨迹显著抑制了峰值冲击力，使得加工表面更为平滑，局部与全局抗压强度均显著提升。
- **PDF**: https://arxiv.org/pdf/2610.28234v1

--- 
## 📚 学科: `cs.*`

**学科总结**：
本周计算机科学领域的论文涵盖了 3D 视觉生成、类级别 3D 姿态估计、数据预训练语料审计以及文生图（T2I）版权水印保护等热门方向。亮点工作包括：支持任意可变粒度几何条件的图像到 3D 部件生成模型 FlexPart（NeurIPS 2026）、高精度实时 RGB-D 类级别姿态估计与形状补全模型 F2G-Pose（NeurIPS 2026）、利用具身智能体对大语言模型预训练语料进行质量调试的 Agentic 框架，以及低频水印技术 SpectralCanary。

### A Unified Framework for Image-to-3D Part Generation via Variable Granularity
- **分数**: 7
- **链接**: https://arxiv.org/abs/2610.31671v1
- **作者**: Qiwen Gu, Xin Zhou, Xiwu Chen, Zhongyang Zhu, Zhuo Zhang, Junqiao Zhao
- **备注**: Accepted at NeurIPS 2026
- **摘要**: 可控 3D 部件生成对数字资产创作至关重要，但现有方法缺乏适应多粒度控制的需求。本文提出了 FlexPart，一个统一的图像到 3D 部件生成框架，支持在单一模型中处理从稀疏点到密集包围盒与掩码等异构几何条件。此外，本文提出了非对称几何引导机制，利用强空间先验在不同粒度间对齐表征。在 PartVerseXL 数据集上，FlexPart 在掩码条件下的 Part CD 比现有方法降低了 10.5% 至 16.6%，同时保持了出色的整体网格生成质量。
- **PDF**: https://arxiv.org/pdf/2610.31671v1

### F2G-Pose: Geometry-Aware Foundation Feature Lifting for Direct RGB-D Category-Level Object Pose Estimation
- **分数**: 7
- **链接**: https://arxiv.org/abs/2610.31623v1
- **作者**: Jinyu Zhang, Haitao Lin, Jiashu Hou, Xiangyang Xue, Yanwei Fu
- **备注**: Accepted at NeurIPS 2026
- **摘要**: 本文研究类别级 RGB-D 物体姿态估计。为了平衡可靠性与效率，本文提出 F2G-Pose，这是一个实时、单前向传播的直接预测框架，能从单张 RGB-D 观测中一次性预测类别级姿态、度量尺寸和相机坐标系下的补全形状。F2G-Pose 将密集视觉基础特征提升至局部点云，使用 DGCNN 标记化编码局部几何，并结合 Mixture-of-Experts Transformer 融合物体级结构。在仅使用合成数据训练的情况下，F2G-Pose 在 SOPE 和 ROPE 数据集上达到了 SOTA 精度，并在姿态推断中达到 28 FPS 的实时速度。
- **PDF**: https://arxiv.org/pdf/2610.31623v1

### Can an Agent Debug a Web Corpus? Agentic Auditing of Slovak FineWeb2
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.31636v1
- **作者**: Marek Šuppa, Ivan Vykopal, Jaroslav Kopčan
- **备注**: Accepted to WaC Workshop at EMNLP 2026
- **摘要**: 跨语言数据管线（如 FineWeb2）在处理具体语言时常遗留未预期的失效模式。本文探索将 LLM 作为语料库调试智能体：具身智能体通过受限 API 探索语料库，将发现的问题编译为可执行测试，并由母语者验证。在 FineWeb2 的斯洛伐克语部分（2650万文档），仅花费少量 API 成本的智能体成功定位了7个重要缺陷现象，包括一个包含 140 余万篇文档的机器生成垃圾内容农场。编译后的测试套件能在 0.7 秒内完成全量语料库扫描，极大降低了全面重新分类的成本。
- **PDF**: https://arxiv.org/pdf/2610.31636v1

### SpectralCanary: Embarrassingly Simple Low-Frequency Traces for T2I Dataset-Use Auditing
- **分数**: 4
- **链接**: https://arxiv.org/abs/2610.31659v1
- **作者**: Sy-Tuyen Ho, Anirudh Satheesh, Soham Chawathe, Huy Nghiem, Yongkyun Lee, Andrew Adams Schoen, Furong Huang
- **备注**: NeurIPS 2026 Workshop (Attributing Model Behavior at Scale)
- **摘要**: 审计文本到图像（T2I）模型是否在特定图像集上微调非常困难。主动式数据集审计通常在数据发布前植入共享信号。本文提出 SpectralCanary，利用平滑低通掩码将固定金丝雀图像融合至数据集图像中，无需修改文本或进行逐图优化。轻量级验证器即可在怀疑模型的生成结果中提取信号。实验表明，低频视觉信号比中高频信号能更稳定可靠地迁移至生成模型中，且该水印方法对图像画质损伤极小，能有效抵抗对抗性擦除攻击。
- **PDF**: https://arxiv.org/pdf/2610.31659v1

--- 
## 📚 学科: `math.*`
_本周缺少高价值论文_

---

## 📚 学科: `astro-ph.*`

**学科总结**：
本周天体物理学精选论文涵盖了自监督多模态 AI 在 JWST 数据分析中的应用、康普顿极化仪响应快速计算框架、系外行星大气流失观测（TOI-3884b）、QUIJOTE 巡天的银河系同步辐射偏振功率谱测量，以及太阳色球层莫顿波局部增强机制的首次观测发现。论文展示了从数据科学赋能天文学到恒星与太阳物理微观机制探索的丰富成果。

### Self-Supervised Representation Learning for JWST Galaxy Images and Low Resolution Spectra
- **分数**: 7
- **链接**: https://arxiv.org/abs/2610.31078v1
- **作者**: Yang Cheng, Morgan Fouesneau, Ivelina G. Momcheva, Tobias Buck, Shengxiu Sun
- **备注**: Accepted for the NeurIPS 2026 RPS Workshop
- **摘要**: 本文提出了一种自监督多模态模型，可从缺乏传统 SED 拟合所需多波段覆盖的稀疏 JWST 数据中恢复星系恒星质量。模型在单波段 F150W 图像与观测帧 1-2 $μ$m PRISM 光谱配对上进行训练，获得的联合图谱表征在 $1<z\le3$ 红移范围内恢复恒星质量达到了 $R^2 \sim 0.9$ 的精度；CLIP 跨模态对齐进一步提升了单模态的推理性能。
- **PDF**: https://arxiv.org/pdf/2610.31078v1

### A Generalized Framework for Rapid Polarization Response Generation in Wide Field-of-View Compton Polarimeters
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.31559v1
- **作者**: Mohamed Gamal Zaid, Merlin Kole, Mark McConnell, Fabio Muleri, Hancheng Li
- **备注**: Accepted for publication in ApJ
- **摘要**: 伽马射线暴（GRB）前体辐射的偏振测量是探测其辐射机制和磁场结构的最直接手段。针对大视场平面康普顿极化仪，GRB 轴外入射会引入 Klein-Nishina 投影调谐。本文对全前体辐射能量波段及任意入射/偏振角进行了无近似的数值求解，并推出了包含极化响应的开源快速计算框架，在减少 95% 以上蒙特卡洛模拟工作量的同时精准再现偏振响应。
- **PDF**: https://arxiv.org/pdf/2610.31559v1

### A Headwind-like Helium Outflow from TOI-3884b
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.31492v1
- **作者**: Joe P. Ninan, Jessica Libby-Roberts, Suvrath Mahadevan, Oleg Kochukhov, Daniel M. Krolikowski, Gudmundur Stefansson, Shubham Kanodia, Jaume Orell-Miquel, Caroline V. Morley, Kevin France, Girish Duvvuri, Chad F. Bender, William D. Cochran, Megan Delamer, Scott A. Diddams, Samuel Halverson, Fred Hearty, Leslie Hebb, Andrew Monson, Paul Robertson, Arpita Roy, Christian Schwab
- **备注**: Accepted for publication in Astronomical Journal (AJ)
- **摘要**: 本文报道了围绕 M4 型矮星公转的极地轨道超级海王星 TOI-3884b 大气层蒸发的观测发现。通过分析 He I 10830 Å 吸收线，观测到高达 6.8% 的过量凌星深度。大气流失在光度凌星前 5 小时即已显现，但没有显著的凌星后尾巴。这种类似于“迎风”的外流形态支持辐射驱动的质量损失机制，为检验恒星-行星相互作用及行星磁场理论提供了新窗口。
- **PDF**: https://arxiv.org/pdf/2610.31492v1

### QUIJOTE scientific results - XII. Characterization of the polarized synchrotron emission at the power spectrum level in the QUIJOTE-MFI wide survey
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.31469v1
- **作者**: F. Vansyngel, J. A. Rubino-Martin, P. de Ferra, R. B. Barreiro, R. T. Genova-Santos, B. Casaponsa, M. Fernandez-Torreiro, D. Adak, K. Aryan, M. Ashdown, J. M. Casas, F. J. Casas, R. Cepeda-Arroita, A. Fasano, D. Herranz, E. Martinez-Gonzalez, F. Poidevin, R. Rebolo, B. Ruiz-Granados, D. Tramonte, P. Vielva, R. A. Watson
- **备注**: Accepted for publication in MNRAS
- **摘要**: 本文利用 QUIJOTE-MFI 巡天（10-20GHz）联合 Planck 和 WMAP 数据，分析了多极矩范围 $30 < \ell < 130$ 内的偏振同步辐射功率谱。EE 和 BB 功率谱均可由简单幂律模型良好描述（最佳拟合斜率分别为 $α_{EE} = -3.24$ 和 $α_{BB} = -3.81$）。研究给出了同步辐射与尘埃的关联度及对未来前景 CMB B 模态偏振测量中同步辐射污染程度的精细估计。
- **PDF**: https://arxiv.org/pdf/2610.31469v1

### Unexpected Local Enhancement of Chromospheric Moreton Waves on the Sun
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.31457v1
- **作者**: Y. W. Ni, J. H. Guo, C. Li, Y. K. Wang, G. Y. Chen, C. Xia, C. Fang, P. F. Chen
- **备注**: Accepted for publication in ApJ Letters
- **摘要**: 太阳爆发常驱动激波并在色球层留下莫顿波（Moreton waves）印记，莫顿波通常随传播衰减。本文利用中国首颗太阳探测卫星“夸父一号”（CHASE）的高精度光谱观测，首次报道了莫顿波在传播中途发生显著局部增强的现象。结合 SDO 磁场测量发现，增强位置对应日冕约 70 Mm 高度的磁零点。研究证实该增强系由磁零点附近的波模式转换所致（快模式波转化为被局部捕获的慢模式波）。
- **PDF**: https://arxiv.org/pdf/2610.31457v1

--- 
## 📚 学科: `stat.*`

**学科总结**：
本周统计学领域的精选论文集中在 AI 模型评估指标的反思、可解释性概率推断与概率校准（Calibration）机制的深入探究。研究涉及 AI 天气预报在极值评估中的评价指标敏感性分析、基于神经符号规则的统计序列预测模型 RUNES（NeurIPS 2026）、基于特征空间局部细化的残差校准框架 LAPE，以及对单调分布回归（IDR）中托马阶梯现象失准缺陷的理论解释与改进。

### Can We Trust Evaluations of AI Weather Forecasts for Extremes? How Evaluation Protocols Shape Model Rankings
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.31237v1
- **作者**: Tobias Biegert, Sam Allen, Zhongwei Zhang, Sebastian Lerch
- **备注**: Accepted paper at NeurIPS 2026 Workshop (TAE)
- **摘要**: AI 气象模型在计算成本极低的情况下表现出与传统物理模型相当的竞争性能，但关于其预测极端天气能力的结论尚存争议。本文研究了评估协议如何影响模型排名。结果发现排名对评估指标非常敏感：当评估局限于已观测到的极值事件时物理模型表现最好，而使用加权评分函数时 AI 模型得分更高。分析表明 AI 模型普遍低估极值频率（遗漏为主），而物理模型预测更频繁（虚警为主），得分差异主要来自分布失准而非判别能力差异。
- **PDF**: https://arxiv.org/pdf/2610.31237v1

### What Comes Next and Why: Interpretable Next-Event Prediction with Neuro-Symbolic Rules
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.31114v1
- **作者**: Tim Nico Bauerschmidt, Isabel Valera, Jilles Vreeken
- **备注**: Accepted at NeurIPS 2026
- **摘要**: 在现实序列预测应用中，解释预测原因与提高准确率同等重要。本文提出 RULES，一种直接从数据中学习时序符号规则的神经符号模型，并将其与残差网络结合构成 RUNES。RUNES 将符号规则与残差网络加性结合，在保持极高预测准确率的同时，提供了对激活规则以及残差如何调整预测的透明访问视角。
- **PDF**: https://arxiv.org/pdf/2610.31114v1

### Residual Calibration via Local Feature-Space Refinement
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.30652v1
- **作者**: Xihao Wang, Chengyao Yu, Ruixing Ming
- **备注**: Accepted at NeurIPS 2026
- **摘要**: 深度神经网络常难以提供可靠的置信度估计。现有的事后校准方法多依赖基于分数的全局变换，无法捕获特征空间局部区域中变化的置信度失准。本文提出局部自适应概率估计（LAPE）事后残差校准框架，将全局校准器输出作为稳定锚点，利用特征空间邻域校准样本的非参数局部信息来细化个体预测，有效提升了现有基线模型的置信度校准质量。
- **PDF**: https://arxiv.org/pdf/2610.30652v1

### On the Calibration of Isotonic Distributional Regression
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.31258v1
- **作者**: Tobias Biegert, Johannes Resin, Alexander Jordan, Sebastian Lerch
- **备注**: Accepted at AISTATS 2026 - Workshop on Calibration for Modern AI
- **摘要**: 单调分布回归（IDR）是一种用于概率预测的非线性非参数技术。本文揭示并记录了 IDR 的一个奇特样本外缺陷：其概率积分变换（PIT）值呈现为类似于托马阶梯函数（Thomae's function）的分数频率尖峰分布。本文从理论上解释了该尖峰行为与单调拟合离散结构的关系，并探讨了如何通过平滑方法消除此人工瑕疵。
- **PDF**: https://arxiv.org/pdf/2610.31258v1

--- 
## 📚 学科: `econ.*`
_本周缺少高价值论文_