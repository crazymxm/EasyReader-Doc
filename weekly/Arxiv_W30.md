```markdown

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
# 🗓️ 周报 (2026-W30)
> 更新时间: 2026-07-26

--- 
## 📚 学科: `eess.*`
### Designed Vocalizations Dataset: Sound-Designed Human and Animal Voices for Non-human Voice Conversion
- **分数**: 4
- **链接**  https://arxiv.org/abs/2607.20951v1
- **作者**: Seolhee Lee, Minsu Kang, Yangsun Lee, Woosun Min, Choonghyeon Lee, Namhyun Cho
- **备注**: Accepted at InterSpeech 2026
- **摘要**: AI语音转换的进展使得诸如电影、有声书和游戏等各种媒体应用成为可能。然而，大多数研究和公开基准仍集中于自然人类语音，导致诸如怪兽咆哮和机器人声音等“设计过的发音”未得到充分探索，部分原因在于缺乏公开可用的资源。为了填补这一空白，我们推出了“设计发音数据集”（Designed Vocalizations Dataset），通过整理包括语音和动物发音在内的多样化原始声音源，并应用专业的人声效果处理来产生相应的效果修改变体。我们还提供了一个标准化的测试集，其中在源音色组和预设风格上具有明确的“已见/未见”划分，以在受控条件下评估泛化能力。最后，我们报告了基准测试结果，以支持可重复的评估和未来的研究。数据集和演示样本可在以下网址获取：https://ncai-official.github.io/speech/publications/designed-vocalizations-dataset/。
- **PDF**: https://arxiv.org/pdf/2607.20951v1

### When Persistency is not Exciting in Data-Driven Predictive Control
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21280v1
- **作者**: Gianluca Giacomelli, Chuyu Lu, Siep Weiland, Valentina Breschi
- **备注**: Accepted at the 65th IEEE Conference on Decision and Control (invited session)
- **摘要**: 在数据驱动控制中，理解如何收集对控制目的有意义的数据至关重要。虽然现有的方法主要依赖于满足秩条件来评估实验的质量，但我们表明，仅满足该条件并不总是足以获得满意的闭环性能。针对无法使用类白噪声激励进行数据收集的场景，我们研究了线性行为表示的频域含义。分析表明，数据既需要满足秩条件，又需要激发控制目标所关注的频率，从而为针对直接数据驱动方法定制的控制导向实验设计奠定了基础。这些发现得到了数值结果的证实。依赖于满足秩条件但忽略了跟踪控制目标的数据使能预测控制器，会导致闭环系统无法跟踪选定的参考。
- **PDF**: https://arxiv.org/pdf/2607.21280v1

### Certified Stochastic Control via Covariance Steering with Pick-to-Learn
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21086v1
- **作者**: Chun-Wei Kong, Zachary Donovan, Morteza Lahijanian, Jay McMahon
- **备注**: To appear in the 65th IEEE Conference on Decision and Control
- **摘要**: 我们提出了 CS-P2L，这是一个将协方差转向（CS）与 Pick-to-Learn（P2L）元算法相结合的框架，用于在高保真随机模拟器上进行经认证的控制器合成。该方法在模拟器展开（rollouts）上迭代评估策略，利用最坏情况下的违规来收紧代理约束，并在给定置信度水平下提供基于压缩的、关于真实违规概率的概率保证。在具有不确定重力的航天器动力下降问题上，CS-P2L 通过 600 次展开认证了 4.9% 的违规边界，而独立的协方差转向低估了大约两倍的违规率。
- **PDF**: https://arxiv.org/pdf/2607.21086v1

### Robust Asynchronous Q-Learning under Reward and State Corruption via Batching
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.20822v1
- **作者**: Sreejeet Maity, Aritra Mitra
- **备注**: To appear at the 65th IEEE Conference on Decision and Control (CDC) 2026
- **摘要**: 受恶劣环境下强化学习的启发，我们考虑了在反馈受到对抗性损坏的情况下学习最优策略的问题。具体而言，在每个时间步，对手可以根据 Huber 污染模型扰动学习者的奖励和状态观测。为了防御此类数据损坏，我们提出了 BR-Async-Q：一种基于两个核心思想构建的新型、基于纪元（epoch）的鲁棒 Q-学习算法：（i）将在线数据流划分为批次以降低方差，以及（ii）利用此类批次数据构建 Bellman 最优算子的鲁棒估计。我们证明了 BR-Async-Q 的高概率 ℓ_∞ 误差边界，该边界与普通 Q-学习相匹配，仅多出一个随损坏样本比例缩放的微小附加项。据我们所知，这为受到奖励和状态双重损坏的异步 Q-学习提供了首个鲁棒性保证。此外，当仅奖励被损坏时，我们算法的边界对损坏比例的依赖是极小极大最优的。
- **PDF**: https://arxiv.org/pdf/2607.20822v1

### Self-Attention Transformer-Based Detector for Faster-than-Nyquist Signaling
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.20745v1
- **作者**: Nurettin Safak, Osman Tokluoglu, Enver Cavus
- **备注**: Accepted and presented at the 2026 IEEE Signal Processing and Communications Applications Conference (SIU)
- **摘要**: 在本研究中，针对在超奈奎斯特（FTN）信号传输信道（该信道引入了压缩因子为 τ=0.8 的故意符号间干扰（ISI））上发送的 BPSK 信号，提出了一种新型的仅编码器 Transformer 接收机架构。构建并评估了包含 BPSK 调制、RRC 脉冲成形以及由匹配滤波引起的 ISI 系数的完整端到端通信链。该 Transformer 接收机在 Eb/N0 为 0-8 dB 的范围内与最优的 BCJR 检测器进行了基准测试。为了系统地缩小与 BCJR 的误码率（BER）差距，开发了一种结合多 SNR 预训练和每 SNR 课程微调的两阶段训练策略。并与基于 GRU 的接收机对比分析了该 Transformer 接收机的计算复杂度和推理延迟。注意力图可视化表明，在不需要任何先验信道知识的情况下，Transformer 能够自主识别 FTN 引起的 ISI 记忆结构；随着 SNR 的增加，注意力权重显著集中在中心 token 及其最近的邻居周围。
- **PDF**: https://arxiv.org/pdf/2607.20745v1

### 学科总结
本期 `eess.*`（电气工程与系统科学）领域的论文聚焦于语音合成、控制理论以及信号处理。研究内容涵盖了用于非人声转换的创新性“设计发音”数据集，针对数据驱动预测控制中数据收集与实验设计的深入探讨，以及将协方差转向与元算法结合以实现高保真随机模拟控制的框架。此外，还包括在反馈受扰动环境下的鲁棒异步 Q 学习算法理论研究，以及基于自注意力 Transformer 的超奈奎斯特（FTN）信号检测技术。这些论文在理论推导与工程应用上均有突破。

--- 
## 📚 学科: `q-bio.*`
### Is EEG-to-Text Feasible in Real-World Scenarios? An In-Depth Analysis Using a Neuropsychology-Inspired Benchmark
- **分数**: 7
- **链接**  https://arxiv.org/abs/2607.18749v1
- **作者**: Zihan Zhang, Yu Bao, Xiao Ding, Tianyi Jiang, Kai Xiong
- **备注**: 17 pages, 8 figures. Published in Proceedings of ACL 2026 Main Conference
- **摘要**: 将大脑信号翻译成文本可以为重度瘫痪患者恢复沟通，但迄今为止实际可用的系统仍依赖于侵入式皮层脑电图（ECoG）。脑电图（EEG）提供了一种非侵入式的替代方案，而“脑电转文本”（EEG2Text）也得到了广泛的探索。然而有趣的是，现有的 EEG2Text 模型普遍依赖于“教师强制”（teacher-forcing）评估；一旦脱离，它们便无法生成有意义的解码。这种依赖极大地限制了 EEG2Text 在真实、非学术场景中的应用。这引发了关于 EEG2Text 是否是一个有意义的研究方向，以及脑电信号中是否真正包含可解码的语言信息的广泛争论。在本文中，我们采用受神经心理学启发的范式，发现现有的 EEG2Text 基准忽略了脑电信号的不稳定性，而这一缺陷混淆了推断并引发了争论。我们的实验为无需“教师强制”的 EEG2Text 解码可行性提供了关键证据。据此，我们使用 128 通道高密度脑电帽构建了“脑电转文本语料库”（COFETT），提供了一个专门用于评估 EEG2Text 模型的基准。与多个现有基准相比，COFETT 在区分模型性能方面达到了先进水平（SOTA），并实现了鲁棒的、无教师强制的评估，从而为实际的 EEG2Text 应用开辟了道路。代码开源在 https://github.com/baoyudu/COFETT。
- **PDF**: https://arxiv.org/pdf/2607.18749v1

### Graph Learning on Ensembles of Cyclic Peptides: An Investigation of Molecular Ensemble Modeling
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21561v1
- **作者**: Aaron Feller, Kris Deibler, Maxim Secor
- **备注**: Accepted to Graph Foundation Models workshop at ICML '26. Contains 8 pages, 4 figures
- **摘要**: 尽管许多分子在溶液中以构象系综（conformational ensembles）的形式存在，但基于结构进行分子性质预测时，通常只使用单一的代表性构象。我们引入了 EnsembleEGNN，这是一个分子系综基础模型。它首先使用共享的等变图神经网络（EGNN）层编码每个构象体，然后使用集合注意力模块（Set Attention Block）对生成的构象体表示进行池化，从而对整个系综进行编码。我们在环肽系综数据集 CREMP 上预训练了该模型，采用的多任务自监督目标结合了掩码 token 恢复、噪声坐标重构和成对距离重构。在 CREMP-CycPeptMPDB 数据集上，从头开始训练 EnsembleEGNN 完全失败（$R^2=0.005$）。然而，预训练模型达到了 $R^2=0.477$ 和皮尔逊相关系数 $r=0.699$，超越了仅基于序列的 BERT 基线（$R^2=0.439$，皮尔逊 $r=0.667$）。当 EnsembleEGNN 与 BERT 序列编码器进行端到端联合训练时，混合模型进一步提升至 $R^2=0.538$ 和皮尔逊 $r=0.737$。这些结果表明，将构象系综编码为单一的具有热力学信息的嵌入，能有效提高环肽性质预测的准确性。
- **PDF**: https://arxiv.org/pdf/2607.21561v1

### An unsupervised clustering analysis of breast cancer data derived from electronic health records enhanced through UMAP dimensionality reduction
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.19089v1
- **作者**: Davide Chicco, Nicoletta Benvenuto
- **备注**: Accepted at the CIBB 2026 conference ( https://cibb2026.teralab.ai/ )
- **摘要**: 乳腺癌是最广泛的癌症类型之一，影响着全球约 800 万女性。被诊断患有此病的患者的电子健康记录（EHR）可以作为计算分析的宝贵数据集，从而有助于发现关于该病理的新见解。尤其是无监督聚类，可以识别具有医学显着特征的患者群体，揭示医生可能忽略的数据趋势。在本研究中，我们首先将基于密度的 DBSCAN 聚类方法应用于源自乳腺癌患者电子病历的三个独立数据集。随后，为了提升我们的聚类效果，我们在应用 DBSCAN 之前引入了使用 UMAP 的降维阶段。我们利用三个统计指标（DBCV、DCSI 和 DISCO）评估了聚类结果。结果证实了将 UMAP 与 DBSCAN 结合处理电子健康记录数据的有效性，为医学上解释由该方法识别的患者群体奠定了基础。
- **PDF**: https://arxiv.org/pdf/2607.19089v1

### Subject-Conditioned Glucose Forecasting in Type-1 Diabetes
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.19006v1
- **作者**: Giorgia Rigamonti, Mirko Paolo Barbato, Davide Marelli, Paolo Napoletano
- **备注**: Accepted at the IEEE EMBC 2026 Conference
- **摘要**: 准确预测血糖浓度是 1 型糖尿病管理的关键，有利于及早发现不良血糖事件并支持及时的治疗干预。尽管最近在血糖预测方面取得了进展，但现有的大多数方法都依赖于群体层面的表示或隐式个性化策略，无法提供有效的个体特异性预测。在这项工作中，我们提出了受试者条件血糖预测（SCGP），这是一种专为个性化血糖预测而设计的新型多模态深度学习架构。SCGP 根据观察到的血糖数据和从上下文信息中学习到的紧凑的受试者特异性表示来对血糖预测进行条件约束。通过将受试者特征刻画与血糖动力学建模显式分离，并避免异构输入的早期融合，该框架有效地捕捉了受试者间的变异性，同时保留了鲁棒且可靠的时间建模。在两个前沿基准数据集上的实验表明，SCGP 一致地提高了预测性能，能够在多个预测视野内可靠地检测不良血糖事件，突出了显式受试者条件约束在个性化糖尿病管理中的优势。
- **PDF**: https://arxiv.org/pdf/2607.19006v1

### 学科总结
本期 `q-bio.*`（定量生物学）领域精选了计算生物学与智慧医疗交叉的前沿成果。重点关注了非侵入式脑电图转文本（EEG-to-Text）在现实应用中的可行性，并推出了高质量的 COFETT 基准。此外，研究还涵盖了利用图神经网络进行环肽分子构象系综预测的基础模型，结合 UMAP 与 DBSCAN 进行乳腺癌电子健康病历的无监督聚类分析，以及用于 1 型糖尿病个性化血糖预测的多模态深度学习架构（SCGP）。这些工作有力推动了生物信息学与临床辅助决策系统的发展。

--- 
## 📚 学科: `cs.*`
### 3D-Aware VLMs with Implicit and Explicit Geometries
- **分数**: 4
- **链接**  https://arxiv.org/abs/2607.21595v1
- **作者**: Wenhao Li, Xueying Jiang, Quanhao Qian, Deli Zhao, Ran Xu, Shijian Lu, Gongjie Zhang
- **备注**: Accepted by ECCV 2026, Open Sourced
- **摘要**: 尽管取得了快速进展，但大多数基于 2D 视觉输入的现有视觉语言模型（VLM）在处理需要精细空间理解和推理的各种 3D 任务时，往往表现得十分挣扎。为了弥补这一差距，我们提出了 VLM-IE3D，这是一个统一的框架，通过为 VLM 配备从 RGB 视频中学习到的隐式和显式 3D 几何结构，来增强其 3D 空间感知能力。我们的 VLM-IE3D 引入了“隐式几何 Token”（IGT）来从输入视频中捕获高层的几何先验，以及互补的“显式几何 Token”（EGT）来从重建的 3D 属性中编码详细的几何结构。在此基础上，VLM-IE3D 配备了一个 3D 感知适配器，能有效将这两种类型的几何表示与 2D 视觉线索进行融合。这种仅依靠 RGB 的设计注入了强大的 3D 归纳偏置，用于精细的空间理解和推理，而无需任何额外的 3D 输入。广泛的实验表明，VLM-IE3D 在 3D 视频检测、3D 视觉定位（grounding）、3D 密集字幕生成以及空间推理等各种 3D 任务中，始终表现出优异的性能。代码和模型见：https://github.com/Vegetebird/VLM-IE3D。
- **PDF**: https://arxiv.org/pdf/2607.21595v1

### Beyond Episodic Evaluation: Memory Architectural Bottlenecks in Sequential Embodied Question Answering
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21571v1
- **作者**: Zikui Cai, Kaushal Janga, Tan Dat Dao, Seungjae Lee, Shivin Dass, Mingyo Seo, Kaiyu Yue, Mintong Kang, Nandhu Pillai, Monte Hoover, Aadi Palnitkar, Ruchit Rawal, Ruijie Zheng, Bo Li, Yuke Zhu, Roberto Martín-Martín, Tom Goldstein, Furong Huang
- **备注**: Accepted to IROS 2026
- **摘要**: 具身问答（EQA）传统上是在单回合（episodic）公式下进行评估的，即智能体独立解决每个任务，并在回合之间重置内部状态。然而，现实世界中的机器人是持续运行的，必须积累、留存并选择性地重用从先前的交互中获得的信息。尽管有这一实际需求，但在 EQA 中支持序列记忆所需的架构机制仍未得到充分探索。在这项工作中，我们研究了当 EQA 智能体在序列化评估下（即在同一场景中回答多个问题，且记忆在不同查询之间传递）不同记忆架构的表现。我们发现，仅仅保留现有记忆通常是不够的。仅保留可通行性信息（如 2D 占用网格图）的智能体能记住机器人探索过的位置，但无法记住后续问题所需的视觉语义证据。在短程单回合数据上训练的智能体面临着不同的挑战：当暴露于连续、多查询的历史记录中时，其继承的上下文会遭受严重的时间失配，而不是形成可重用的场景表示。为了克服这一架构瓶颈，我们强调了结构化、空间定位记忆的必要性：将持久的视觉观测映射到度量 3D 几何上的架构，能在连贯的场景表示中保留视觉语义证据。在模拟环境中的广泛实验表明，这种记忆形式打破了序列设置中的“准确性-效率”权衡，同时实现了更高的回答准确率和更低的导航成本。我们进一步在真实世界的移动机器人上验证了这些发现，证明了空间定位的视觉记忆对于在物理环境中实现持续、智能的运行至关重要。
- **PDF**: https://arxiv.org/pdf/2607.21571v1

### Graph Learning on Ensembles of Cyclic Peptides: An Investigation of Molecular Ensemble Modeling
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21561v1
- **作者**: Aaron Feller, Kris Deibler, Maxim Secor
- **备注**: Accepted to Graph Foundation Models workshop at ICML '26. Contains 8 pages, 4 figures
- **摘要**: 尽管许多分子在溶液中以构象系综（conformational ensembles）的形式存在，但基于结构进行分子性质预测时，通常只使用单一的代表性构象。我们引入了 EnsembleEGNN，这是一个分子系综基础模型。它首先使用共享的等变图神经网络（EGNN）层编码每个构象体，然后使用集合注意力模块（Set Attention Block）对生成的构象体表示进行池化，从而对整个系综进行编码。我们在环肽系综数据集 CREMP 上预训练了该模型，采用的多任务自监督目标结合了掩码 token 恢复、噪声坐标重构和成对距离重构。在 CREMP-CycPeptMPDB 数据集上，从头开始训练 EnsembleEGNN 完全失败（$R^2=0.005$）。然而，预训练模型达到了 $R^2=0.477$ 和皮尔逊相关系数 $r=0.699$，超越了仅基于序列的 BERT 基线（$R^2=0.439$，皮尔逊 $r=0.667$）。当 EnsembleEGNN 与 BERT 序列编码器进行端到端联合训练时，混合模型进一步提升至 $R^2=0.538$ 和皮尔逊 $r=0.737$。这些结果表明，将构象系综编码为单一的具有热力学信息的嵌入，能有效提高环肽性质预测的准确性。
- **PDF**: https://arxiv.org/pdf/2607.21561v1

### Towards Robust Iris Recognition Through Occlusion Identification and Conditional Diffusion-Based Reconstruction
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21545v1
- **作者**: Kamrul Hasan, Mylene C. Q. Farias, Oleg V. Komogortsev
- **备注**: Accepted by IEEE International Joint Conference on Biometrics (IJCB) 2026
- **摘要**: 虹膜识别是一种利用虹膜独特且稳定的纹理来识别个人的可靠生物特征识别方法。然而，当具有区分度的虹膜纹理被眼睑、睫毛、镜面反射或其他采集伪影部分遮挡时，识别性能可能会下降。现有的方法通常直接在退化的样本上进行识别，或仅依赖于剩余的可见虹膜区域，而当大量纹理被损坏时，这可能是不够的。为了解决这一局限性，我们提出了一个遮挡感知的虹膜识别框架，包含三个顺序模块：遮挡类型识别、基于扩散的重构和基于深度学习的识别。首先，一个基于残差 2D CNN 的网络用于确定虹膜图像是未遮挡的还是属于受控的遮挡类别之一。其次，将遮挡图像、二值掩膜和预测的遮挡类型作为条件，输入到一个去噪扩散概率模型（DDPM）中，以重建损坏的区域。最后，采用 VGG19-HPMNet（一种具有水平金字塔映射的改进型 VGG19 模型）提取具有区分度的全局和局部虹膜特征用于识别。在 CASIA-Iris-Thousand 数据集上进行的受控合成遮挡协议下的实验表明，该框架通过识别遮挡类型、重构掩膜区域并重新评估恢复后的虹膜样本，显著提高了虹膜识别的性能。
- **PDF**: https://arxiv.org/pdf/2607.21545v1

### Sources of Inequity and Fairness Risks inWellbeing Sensing
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21527v1
- **作者**: Han Zhang, Vedant Das Swain, Koustuv Saha, Anind K. Dey, Jennifer Mankoff
- **备注**: 16 pages, 1 figure, 2 tables. Accepted to AIES 2026
- **摘要**: 用于身心健康的被动感知技术通过智能手机和可穿戴设备持续收集人类行为数据，并应用机器学习/人工智能模型来推断心理状态和行为（例如，抑郁症、认知负荷）。这些系统正越来越多地被应用于高风险环境（如医院、大学），但其公平性研究仍十分有限，且主要局限于对模型性能的事后、基于身份的对比。然而，被动感知结合了异构的传感基础设施、间接的行为推断以及长期的部署——这些特征虽然并非该领域独有，但在该领域表现得尤为明显，并引发了两个尚未得到充分探讨的问题：（1）这些特征会带来哪些额外的非公平性来源？（2）这些不公平性是如何在算法审计之外、贯穿系统生命周期进行传播的？为了填补这一空白，我们对来自五个国家的 14 名研究人员和从业人员进行了半结构化访谈，调查公平性风险是如何在整个被动感知生命周期中产生和应对的。我们的研究结果在实证上刻画了五个具体的非公平性来源（例如，对监测的接受度、行为规律性），这些来源在基于身份的属性之外系统性地塑造了公平性风险。我们进一步总结了在系统生命周期中（从研究设计到部署）的 15 种公平性风险及相应的缓解策略。最后，我们指出了在现实中限制公平实践的结构性障碍，并提出要实现公平的被动感知，既需要研究人员个人的努力，也需要来自资助者、出版机构和部署机构在生态系统层面上的治理支持。
- **PDF**: https://arxiv.org/pdf/2607.21527v1

### 学科总结
本期 `cs.*`（计算机科学）领域的论文涵盖了计算机视觉、具身智能、生物化学交叉、生物特征识别及人工智能伦理等多个前沿课题。研究包括通过隐式和显式几何结构增强视觉语言模型（VLM）3D空间感知能力的 VLM-IE3D，探讨具身问答（EQA）在持续运行场景下序列记忆架构瓶颈的具身机器人研究，以及利用等变图神经网络进行环肽分子系综属性预测的基础模型。此外，还提出了利用扩散模型进行遮挡重构的鲁棒虹膜识别框架，并对身心健康被动感知系统中的公平性风险进行了全生命周期的实证研究与伦理探讨。

--- 
## 📚 学科: `math.*`
_本周缺少高价值论文_

--- 
## 📚 学科: `astro-ph.*`
### ALMA CO-CAVITY II. Resolved Scaling Relations in Void Galaxies
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21464v1
- **作者**: S. B. De Daniloff, D. Espada, S. Duarte Puertas, Y. K. González-Koda, G. Torres-Ríos, S. F. Sánchez, R. García-Benito, S. Verley, I. Pérez, M. Argudo-Fernández, A. Bongiovanni, M. Sánchez-Portal, U. Lisenfeld, M. I. Rodríguez, A. Conrado, A. Jiménez, B. Bidaran, L. Sánchez-Menguiano, T. Ruiz-Lara, A. Zurita, P. Vásquez-Bustos, M. Alcázar-Laynez, P. Villalba-González, E. Florido, R. E. Miura
- **备注**: 21 pages, 14 figures. Accepted for publication in A&A
- **摘要**: 涉及恒星形成率（SFR）、分子气体质量和恒星质量的标度关系是理解星系演化的关键，此前已在解析尺度上进行了探索。然而，这些关系尚未在特别强调大尺度环境（LSE）的情况下进行检验。在这项工作中，我们研究了居住在宇宙最稀疏区域的 41 个空洞星系（VG）样本的解析 Schmidt-Kennicutt 关系（rSK）、分子气体主序关系（rMGMS）和恒星形成主序关系（rSFMS）。利用来自 ALMA CO-CAVITY 和 CAVITY 巡天在 2.5角秒（0.8-2.1 kpc）尺度上的高分辨率干涉 CO(1-0) 数据和光学 IFU 数据，我们研究了全样本以及空洞中单个星系的这些关系。我们对这些关系进行了拟合，发现其参数化形式与用于所有大尺度环境中星系的参数化形式相似。然而，与其他样本不同，rMGMS 是这三个关系中结合最紧密的（$σ_{rMGMS}=0.16$ dex，$σ_{rSK}=0.21$ dex，$σ_{rSFMS}=0.24$ dex）。我们发现，标度关系偏差的一个主要来源是星系间的个体差异。然而，rMGMS 受这些差异的影响较小。有学者曾提出，rMGMS 源于分子气体在恒星含量和暗物质设定的引力势内的集中。我们假设，rMGMS 的偏差追踪了在较长时间尺度上发生的引力势变化，而 rSK 和 rSFMS 的偏差则是由恒星形成率更快速的变化驱动的。这种区别对于我们的空洞星系样本尤为重要，因为这 41 个 ALMA CO-CAVITY 空洞星系比其他大尺度环境中的星系更加孤立，因此较少受到能够显著改变气体分布或在短时间尺度上触发恒星形成事件的影响。从这个意义上说，随着时间的推移，rMGMS 可能是这些关系中最稳定的。
- **PDF**: https://arxiv.org/pdf/2607.21464v1

### Experimental Measurements of Benzene Ice Critical Saturation Ratios on Titan Tholins and Impact on the Microphysical Modeling of Titan's South Polar Benzene Cloud
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21415v1
- **作者**: David Dubois, Erika Barth, Laura T. Iraci, Ella Sciamma-O'Brien, Farid Salama, Sandrine Vinatier
- **备注**: 33 pages, 7 figures, 3 tables, accepted for publication in the Planetary Science Journal
- **摘要**: 卡西尼号复合红外光谱仪（CIRS）在 2009 年 8 月北半球春分之后，探测到了土卫六（Titan）秋季南极平流层中存在苯（C6H6）冰云。这一事件增加了苯的混合比并提高了云顶高度。我们在此展示了在低温（从 138 K 的 13.8 到 157 K 的 3.3，代表土卫六的大气温度）下，纯 C6H6 冰沉积到 NASA Ames 宇宙模拟室（COSmIC）中产生的土卫六气溶胶模拟物（tholins）上时的临界饱和度（Scrit）的新实验测量结果。通过对比在空白基底和土卫六 tholins 上获得的苯蒸气沉积的 Scrit 值，揭示了气溶胶作为凝结核所起的极佳促进作用。我们将这些新的 Scrit 测量结果引入到社区气溶胶和辐射大气模型（CARMA）中，用以计算核化接触参数（由 m = 2.6e-4 T + 0.9494 给出），从而研究在土卫六南极 87 S 大气中，C6H6 云颗粒的大小和数量密度随高度的变化。我们讨论了这些新测得的温度相关数据对微物理建模的影响，这导致模拟的苯云形成高度比之前的观测结果低了约 20 km。对这一差异的一种可能解释是，该云系可能受到了多种挥发性气体组分共凝结的影响。
- **PDF**: https://arxiv.org/pdf/2607.21415v1

### Ultra-High-Energy Particle Production in Binary Mergers Endowed with Magnetic Fields
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21385v1
- **作者**: Carlos H. Coimbra-Araujo, Rita C. Anjos, Jonas P. Pereira, Jaziel G. Coelho
- **备注**: 16 pages, 4 figures. Accepted for publication in Physical Review D
- **摘要**: 我们研究了在 LIGO-Virgo-KAGRA 探测到的双星系统合并前阶段，通过 Bañados-Silk-West（BSW）机制产生超高能粒子的过程。通过求解在磁化 Kerr 时空（磁场强度 $B \sim 10^{12}$--$10^{14}$ G）中带电粒子的测地线方程，我们证明了在视界附近的碰撞可以达到 $E_{\mathrm{cm}} \sim 10^{18}$-- $10^{20}$ eV 的质心能量，使其牢牢处于超高能宇宙线（UHECR）的能量范围内。我们系统地探索了合并遗迹的参数空间，改变了黑洞质量（$M \sim 20$--$150\,M_\odot$，这是双黑洞群体的特征值）、无量纲自旋（$χ_f \sim 0.7$--$0.9$）、磁场强度和粒子角动量。我们的分析揭示了三种不同的加速机制：引力主导机制（$B < 10^{12}$ G），此时磁场增强作用可以忽略；过渡机制（$10^{12}~\text{G} \lesssim B \lesssim 10^{13}~\text{G}$），此时引力效应和磁效应相互竞争；以及磁场主导机制（$B > 10^{13}$ G），此时磁场将碰撞能量放大了将近一个数量级。对于 34 个具有高遗迹自旋（$χ_f > 0.7$）的引力波事件，我们计算了可达到的最大能量，发现具有 $χ_f \gtrsim 0.85$ 和 $M \gtrsim 100\,M_\odot$ 的系统可以达到 $E_{\mathrm{max}} \sim 10^{20}$ eV。我们的结果确立了磁化双星合并，特别是双中子星并合中形成的黑洞-中子星系统和并合后的黑洞遗迹，是极具前景的超高能宇宙线源，并提供了将引力波观测值与粒子加速效率联系起来的定量预测。
- **PDF**: https://arxiv.org/pdf/2607.21385v1

### Magnetohydrodynamical opening of dust traps in protoplanetary disks
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21350v1
- **作者**: Sergey Khaibrakhmanov, Vitaly Akimkin
- **备注**: 17 pages, 8 figures, 2 tables, accepted to ApJ
- **摘要**: 在原行星盘中观测到的环状结构通常被解释为局部压力极大值，这会诱发高效的尘埃聚集。我们重新审视了这一范式，考虑了大尺度磁场应力对气体旋转速度的影响。我们的模拟表明，在具有粒径 $> 1\,μ$m 尘埃颗粒的典型湍流原行星盘外围，磁场可以在动力学上表现得非常强，并导致与开普勒旋转产生 $1-2$% 的偏差。在我们的模拟中，这种效应使得 Stokes 数为 $0.01-0.1$ 的大颗粒的向内漂移速度提高了多达两倍。重要的一点是，这种磁流体力学（MHD）与开普勒旋转的偏差并不依赖于局部气体压力梯度，而仅导致向恒星方向的漂移。由该效应引起的快速漂移可以抵消在环内边缘由于正压力梯度引起的向外漂移，从而打开尘埃陷阱。对于湍流参数 $α=10^{-3}$ 的原行星盘，该效应出现在半宽为 $10$ au 且密度对比度高达 $60$%（对于 $α=10^{-2}$ 则为 $200$%）的环中。因此，原行星盘中大尺度磁场的存在，要么完全阻止了尘埃在密度环中的积累以及流体不稳定性（streaming instability）的发生，要么为其施加了更严格的条件。
- **PDF**: https://arxiv.org/pdf/2607.21350v1

### Comparative 3D Asymmetric Expansion and Angular Widths Evolution of Fast and Slow Coronal Mass Ejections
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21236v1
- **作者**: Anjali Agarwal, Wageesh Mishra, Jie Zhang, Soumyaranjan Khuntia, Manuela Temmer
- **备注**: 23 pages, 7 figures, 3 tables; Accepted for publication in ApJ
- **摘要**: 日冕物质抛射（CME）的径向和横向尺寸影响着它们在地球的持续时间和相撞概率。这些性质与 CME 在不同径向和横向上的膨胀速度有关；然而，以往的大多数研究都是使用投影的全冰淇淋锥体（full ice-cream cone）几何来模拟 CME 的演化，这种几何无法区分径向和横向的膨胀。我们的研究利用分级圆柱壳（Graduated Cylindrical Shell）模型，调查了在日冕仪高度内，七个快速 CME 和七个慢速 CME 的非对称膨胀（相对径向和横向分量）及运动学特征。我们的研究证实，CME 呈非对称膨胀，且在这两个 CME 群体中，横向膨胀均超过了径向膨胀。这种非对称性限制了全冰淇淋锥模型的准确性。对于快速和慢速 CME，较高的前沿速度都与较高的膨胀速度相关。在 10 个太阳半径（Rs）的高度，膨胀速度（横向和径向）较大的慢速 CME 具有较大的角宽度（正面和侧面），而快速 CME 则在横向膨胀速度与正面角宽度之间表现出负相关。我们发现慢速 CME 的膨胀和传播速度表现出两阶段演化，而快速 CME 则表现出更多样化的趋势。总的来说，这项研究表明快速和慢速 CME 的演化方式不同，在对其物理参数进行统计估计时不应将其视为单一群体。我们的研究强调了估算不同方向上、以及标准日冕仪高度之外的 CME 角宽度和膨胀速度的重要性，以便捕捉它们完整的物理演化。
- **PDF**: https://arxiv.org/pdf/2607.21236v1

### 学科总结
本期 `astro-ph.*`（天体物理学）领域的研究涉及星系演化、行星科学、高能天体物理以及太阳物理学。研究包括利用 ALMA 观测数据探讨稀疏空洞星系中三种关键标度关系（rSK、rMGMS、rSFMS）的解析表现；针对土卫六（Titan）大气中苯冰云微物理建模的低温实验测量；在强磁场双星合并系统前阶段通过 BSW 机制产生超高能宇宙线（UHECR）的理论推导；大尺度磁场应力对原行星盘中尘埃陷阱开启与流体不稳定性抑制的影响；以及利用 3D 模型对比分析快速与慢速日冕物质抛射（CME）的非对称膨胀与运动学演化。这些工作深化了我们对从宇宙尺度到太阳系天体的物理过程的理解。

--- 
## 📚 学科: `stat.*`
### Risk-Limiting Audits for Parliamentary Majorities
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.21082v1
- **作者**: Jack Freestone, Dennis Leung, Damjan Vukcevic
- **备注**: 22 pages, 7 figures, accepted for E-Vote-ID 2026
- **摘要**: 现有的风险限制审计（RLA）方法通常专注于对单场选举竞争进行认证。然而，在议会选举中，政治上相关的结果往往是某个政党是否赢得了足够多的席位以组建政府，而不是每个报告的席位结果是否都准确无误。延续 Mohanty 等人（2019）的研究，我们将议会多数席位的认证表述为一个“部分结合检验”（partial conjunction testing）问题：只要验证报告的获胜政党确实赢得了至少其报告席位的多数即可。基于 SHANGRLA 审计框架，我们通过结合席位层面的统计量，构建了用于多数席位结果的序列审计统计量。接着，我们提出了在席位之间分配审计工作量的自适应采样策略，包括能够学会避免在似乎不太可能真正获胜的席位上耗费过多精力的变体。通过基于 2014 年印度人民院（Lok Sabha）选举的合成与真实数据的模拟，我们表明，与认证每个报告的获胜席位相比，对议会多数席位进行审计可以显著减少需要检查的选票数量（减少近千倍）。
- **PDF**: https://arxiv.org/pdf/2607.21082v1

### 学科总结
本期 `stat.*`（统计学）领域精选了一篇将统计检验应用于民主选举安全审计的创新研究。文章提出了一种针对议会多数席位认证的风险限制审计（RLA）方法，将其转化为“部分结合检验”问题。通过自适应采样策略在不同席位间动态分配审计工作量，显著提升了审计效率，在模拟实验中成功减少了近千倍的选票核对量，为现代电子投票和民主选举的统计审计提供了切实可行的解决方案。

--- 
## 📚 学科: `econ.*`
_本周缺少高价值论文_

---
```