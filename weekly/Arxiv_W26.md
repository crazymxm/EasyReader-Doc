# 🗓️ 周报 (2026-W26)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-06-28

--- 
## 📚 学科: `eess.*`

本期 `eess.*`（电气工程与系统科学）学科精选了5篇高质量论文，涵盖了医学图像超分辨率、机器人动力学控制以及语音信号处理等前沿方向。在医学影像方面，ECCV 2026 录用论文提出了一种双先验零空间学习框架，在严格保持测量一致性的前提下提升了切片超分辨率效果。在机器人领域，AVEC 2026 论文针对轮式四足机器人自主竞速，结合 MPC 与 RL 实现了出色的主动侧倾控制。在语音领域，三篇 Interspeech 2026 录用论文分别针对端到端语音质量评估（基于对比学习优化 DNSMOS）、示例查询口语词检测（提出可扩展的语音分词器 wav2tok 2.0）以及跨领域语音表示（结合 Whisper 与 Qwen 的双编码器融合框架）提出了创新的解决方案。

### Dual-Prior Guided Null-Space Learning with Mixture-of-Splines for Arbitrary Medical Slice Super-Resolution
- **分数**: 4
- **链接**  https://arxiv.org/abs/2606.26716v1
- **作者**: Haofei Song, Siyuan Xu, Xintian Mao, Shaojie Guo, Qingli Li, Yan Wang
- **备注**: Accepted to ECCV 2026! Project page: https://github.com/DeepMed-Lab-ECNU/Medical-Image-Reconstruction
- **摘要**: 任意切片超分辨率通过在任意尺度上合成中间切片，从各向异性的临床采集数据中重建各向同性的体数据。然而，将这种病态逆问题视为无约束的基于残差的回归，存在产生解剖学上不合理结构或改变原始观测数据的风险。为了解决这两个问题，本文提出了双先验零空间学习（DP-NSL）框架，将其重构为受两个互补先验引导的约束恢复过程。测量一致性投影（MCP）强制执行“确定性观测先验”：重建经历精确的正交投影，从而以零误差再现每个采集的切片，将所有学习到的细节限制在不可观测的零空间中。在这个零空间内，样条混合（MoS）模块通过动态混合不同解析阶数的B样条专家来引入“几何连续性先验”，从而允许每个解剖区域以内容感知的连续性水平进行建模。为了促进空间相干性，局部空间一致性解码器（LSCD）进一步注入了局部归纳偏置。在三个CT和一个MRI基准数据集上的实验表明，DP-NSL在严格保持测量一致性的同时，表现优于现有方法。代码可在 https://github.com/DeepMed-Lab-ECNU/Medical-Image-Reconstruction 获取。
- **PDF**: https://arxiv.org/pdf/2606.26716v1

### Racing a Wheeled Quadruped: Active Load Transfer Mitigation via Model Predictive Control
- **分数**: 4
- **链接**  https://arxiv.org/abs/2606.26313v1
- **作者**: Marla Eisman, Brian Lam, Samuel Sonnino, Francesco Borrelli
- **备注**: Accepted to the 17th International Symposium on Advanced Vehicle Control (AVEC 2026), 7-11 September 2026, Tsukuba, Japan
- **摘要**: 本文提出了一种使用模型预测控制（MPC）和强化学习（RL）的分层控制框架，用于主动侧倾控制，以在轮式四足机器人自主竞速过程中管理侧向载荷转移。该框架集成了线下时间最优赛道生成、主动最小化侧向载荷转移率（LTR）的在线MPC规划器，以及直接部署在机器人16个执行器上的底层全身RL策略。MPC基于Unitree Go2-W平台的车辆动力学自行车模型。机器人的腿部执行器充当主动悬架，其中膝关节产生防侧倾力迹以向弯道内侧倾斜。物理赛道实验表明，主动侧倾控制使平均 LTR 降低了高达 44%，最快单圈时间缩短了 8.7%，并将峰值侧向加速度能力提升了 21.3% 至 1.98 $m/s^2$，在超出非倾斜基线控制器范围的情况下仍能保持强健的高速稳定性。补充代码和视频可在 https://github.com/meisman-ucb/go2w-roll-control-mpc 获取。
- **PDF**: https://arxiv.org/pdf/2606.26313v1

### DNSMOS-C: Improving End-to-end Speech Quality Models via Contrastive Learning
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.26903v1
- **作者**: Xinyu Liang, Fredrik Cumlin, Victor Ungureanu, Chandan K. A. Reddy, Christian Schuldt, Saikat Chatterjee
- **备注**: Accepted at Interspeech 2026
- **摘要**: 我们推出了 DNSMOS-C，这是一个紧凑的端到端语音质量评估模型，它通过整合基于 MOS 引导的三元组对比损失，扩展了 DNSMOS Pro 框架。该对比监督直接应用于中间嵌入，鼓励隐空间在感知质量方面得到更好的组织，同时保留了 DNSMOS Pro 的简单性和高效性。与依赖于大型预训练自我监督学习（SSL）编码器和多阶段训练的先前方法不同，DNSMOS-C 在单个统一框架内联合学习语音表示和 MOS 回归。在多个数据集上的实验表明，DNSMOS-C 在相关性指标上一致优于 DNSMOS Pro，并在具有挑战性的域外测试集上实现了更好的泛化。此外，隐空间分析表明，我们的方法学习到的表示展现出一种涌现的低维质量排序，这增强了可解释性并提高了训练稳定性。这些发现表明，基于 MOS 引导的对比学习能够实现更稳健、更准确的质量预测，而不会产生额外的计算开销。
- **PDF**: https://arxiv.org/pdf/2606.26903v1

### wav2tok 2.0: Scalable Audio Tokenization Maintaining Explicit Pairwise Token Alignment for Efficient Audio Retrieval
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.26824v1
- **作者**: Adhiraj Banerjee, Vipul Arora
- **备注**: Accepted at INTERSPEECH 2026
- **摘要**: 学习能够保留跨变长语音相似性的离散语音表示是示例查询口语词检测（QbE-STD）的核心。虽然 wav2tok 引入了基于 CTC 的序列对齐来强制实现 token 一致性，但其紧密耦合的聚类和对齐训练方案限制了其可扩展性。我们提出了 wav2tok 2.0，这是一个基于 BEST-STD 骨干网构建的可扩展、对齐感知型语音分词器。wav2tok 2.0 采用阶段式训练，首先通过对比学习和向量量化来学习具有判别性且与说话人无关的表示，然后使用 CTC 对齐损失和具有自适应权重的、新型基于 DTW 对齐的帧级预测目标来强制实现成对的 token 一致性。实验表明，wav2tok 2.0 在 QbE-STD 上一致优于 BEST-STD 和通用分词器，同时保持了高效性和可扩展性。
- **PDF**: https://arxiv.org/pdf/2606.26824v1

### WQ-Fusion: Dynamic Gated Attention for Cross-Domain Audio Representation
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.26556v1
- **作者**: Mingda Lin, Lei Ding, Xinyue Zhou, Tiantian Xiong, Hanchen Pei, Gongping Huang, Hao Zhang, Jingdong Chen, Jacob Benesty
- **备注**: Accepted by INTERSPEECH 2026
- **摘要**: 尽管预训练模型在特定任务中表现出色，但在不同的声学领域中学习通用表示仍然极具挑战性。为了解决这个问题，我们提出了 WQ-Fusion，这是一个用于跨领域语音表示学习的强健双编码器框架。为了克服静态拼接的局限性，WQ-Fusion 通过自适应特征调制模块和一种新型的元素级门控注意力机制将 Whisper 和 Qwen 进行了融合。这种设计能够实现动态特征选择，从而使模型可以有选择地强调相关的声学和语义维度。在 Interspeech 2026 语音编码器能力挑战赛（Track A）基准上的广泛实验表明，通过有效路由异构信息，WQ-Fusion 实现了 0.836 的优异综合评分，显著优于最强的单编码器基准模型。
- **PDF**: https://arxiv.org/pdf/2606.26556v1

--- 
## 📚 学科: `q-bio.*`

本期 `q-bio.*`（定量生物学）学科精选了3篇在顶尖计算机体系结构、人工智能和医学影像会议上发表的论文。研究内容高度跨界：ISCA 2026 的论文针对大规模基因组图谱分析，提出了一种创新的存内计算系统（GRAINS），大幅降低了传统架构的访存瓶颈；ALIFE 2026 论文从认知科学角度，将单细胞藻类的趋光性重构为基于生化反应网络（CRN-ODE）实现的强化学习与信息获取过程；MICCAI 2026 论文则探讨了三维荧光显微镜下的自监督学习，证明了原生 3D 掩码自编码器（MAE-3D）结合蛋白质语言模型（ESM2）在单细胞表示学习中的巨大优势。

### GRAINS: Storage-Aware Algorithm-Architecture Co-Design Enabling High-Performance and Low-Cost Graph-Based Genome Analysis
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.26468v1
- **作者**: Nika Mansouri Ghiasi, Harun Mustafa, Talu Güloglu, Rakesh Nadig, Konstantina Koliogeorgi, Susana Rebolledo Ruiz, Marc Rautmann, Furkan Eris, Mohammad Sadrosadati, Jisung Park, Onur Mutlu
- **备注**: To appear in ISCA 2026
- **摘要**: 基因组序列的图形表示已成为一种能够高效、富有表现力地表示海量基因组数据库的强大方法。尽管有这些优势，但由于需要访问大量低重用率的数据，在大大规模基因组图谱上进行分析会导致来自存储系统的重大数据移动开销。直接在存储设备内部处理数据是减轻这种开销的根本解决方案。然而，由于现代固态硬盘（SSD）内部硬件资源有限，现有的图形基因组分析工具均无法在存储系统内高效使用。同时，先前针对（i）传统的、线性的非图形基因组分析或（ii）常规的、非基因组图形分析开发的以存储为中心的系统，并不适用于图形基因组分析独特的特殊数据结构和访问模式。我们提出了 GRAINS，这是第一个用于在存储器中进行大规模基因组图谱分析的系统。通过对在基因组图谱上运行的典型分析管线的详细剖析，我们进行了存储感知的算法-架构协同设计，以（i）使这些管线对存储更友好，并（ii）通过在存储器和闪存中进行处理进一步提高性能、能源效率和成本效益。GRAINS 的协同设计基于三个关键方面。首先，基于基因组图谱的独特特征，我们提出了一种新的批处理和执行流。其次，通过在闪存内和存储器内处理，我们避免了传输低重用率的闪存页面。第三，为了充分利用闪存颗粒的并行性，我们通过重新规划现有 SSD 结构设计了一种有效且轻量级的调度技术。相比于最先进的软件基准，GRAINS 提供了 2.7 倍至 47.8 倍的加速（能耗降低 4.4 倍至 31.6 倍），相比于硬件加速基准提供了 1.5 倍至 17.0 倍的加速（能耗降低 3.1 倍至 20.7 倍）。
- **PDF**: https://arxiv.org/pdf/2606.26468v1

### Implementation of reinforcement learning in chemical reaction networks: application to phototaxis as curiosity-driven exploration
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.26168v1
- **作者**: Ruyi Tang, Grégoire Sergeant-Perthuis, David Colliaux
- **备注**: This paper is accepted as talk at ALIFE 2026 (Waterloo, Canada)
- **摘要**: 生命系统使用嘈杂且不完整的感官信号在环境中进行导航。在单细胞藻类中，趋光性通常被建模为由刺激-反应规则驱动的机械性“运行-翻滚”（run-tumble）过程。然而，这种描述忽略了生物体如何主动采样其环境以减少感官歧义。从极简认知的角度出发，我们将这种导航重构为一个主观的、信息驱动的感觉运动过程。为此，我们提出了一个将部分可观测马尔可夫决策过程（POMDP）与生化反应动力学联系起来的框架。环境变量是隐藏的，而细胞通过无记忆的贝叶斯步骤，从每次观测中更新极简的内部状态。这些内部动力学在向光定位与探索性重新定位之间取得平衡，并且可以通过化学反应网络常微分方程（CRN-ODE）来实现。我们的模型包括一个用于光感受的生物物理观测过程，以及一个在化学上可计算的关于信息增益的多项式界。通过对 30 个实验记录的衣藻（Chlamydomonas）轨迹使用逆强化学习（IRL），我们推断出了与观测到的趋光运动一致的行为目标，并使用标准的随机模拟算法（SSA）基准对所得动力学进行了基准测试。我们的模型重现了经验性的对光对齐分布，在此数据集上与客观的 SSA 基准相当。在这一框架下，“运行-翻滚”交替作为一种信息获取策略自然涌现：翻滚使细胞重新定位以采集新的感官配置并解决感官歧义，展示了细胞内生化网络如何支持细胞导航中的自适应信息寻求行为。
- **PDF**: https://arxiv.org/pdf/2606.26168v1

### 3D Masked Autoencoders are Robust Learners of Volumetric and Multimodal Cellular Representations for Microscopy
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.23964v1
- **作者**: Amirhossein Kardoost, Lion Gleiter, Tingying Peng, Carsten Marr
- **备注**: Accepted at MICCAI 2026. Code available at: https://github.com/marrlab/mae3d-opencell
- **摘要**: 尽管细胞本质上具有三维特性，但荧光显微镜中的自我监督学习通常依赖于 2D 投影。我们在三维体积显微镜数据上对 2D 和 3D 掩码自编码器（MAE-2D 与 MAE-3D）进行了系统性的比较。在匹配架构和训练协议的情况下，MAE-3D 在下游单细胞任务上的表现一致优于基于 2D 最大投影和切片的变体。我们进一步将视觉表示与预训练的蛋白质语言模型（ESM2）进行对齐，并表明跨模态监督为三维模型带来了更大的提升。通道交叉注意力和频域正则化对于利用 3D 空间上下文至关重要。在蛋白质-蛋白质相互作用任务中，MAE-3D 实现了 0.865 的 ROC-AUC，比先前的方法提高了多达 +0.025。在蛋白质定位方面，我们最好的 3D 模型达到了最先进的 AUC$_{\text{micro}}$ (0.952) 和 F1$_{\text{micro}}$ (0.742)，分别比先前的方法绝对提高了 +0.003 和 +0.010。总体而言，这些结果展示了原生 3D 建模和多模态对齐在单细胞显微镜表示学习中的优势。
- **PDF**: https://arxiv.org/pdf/2606.23964v1

--- 
## 📚 学科: `cs.*`

本期 `cs.*`（计算机科学）学科汇集了人工智能、强化学习和机器人技术领域的突破性进展。ACL 2026 论文通过自主经验探索和后验经验利用显著提升了小型多模态大模型在 GUI 界面任务规划上的泛化能力；KDD 2026 工作室论文探讨了工业级语义求职搜索中的 RLAIF 框架，揭示了奖励塑造（Reward Shaping）对算法防作弊的重要性；ICML 2026 Spotlight 论文提出的自回归玻尔兹曼生成器（ArBG）打破了传统的流模型限制，在复杂分子系统平衡态采样上取得了重大突破；EMNLP 2026 投稿论文深入社交媒体隐秘语言检测，提出了一套面向编码机制的新型分类法；IROS 2026 论文（BOWConnect）则巧妙地将窗口贝叶斯优化引入双向并行运动规划中，完美解决了狭窄空间中的机器人控制难题。

### Empowering GUI Agents via Autonomous Experience Exploration and Hindsight Experience Utilization for Task Planning
- **分数**: 6
- **链接**  https://arxiv.org/abs/2606.27330v1
- **作者**: Tianyi Men, Zhuoran Jin, Pengfei Cao, Yubo Chen, Kang Liu, Jun Zhao
- **备注**: Accepted to ACL 2026 Main
- **摘要**: 多模态网页智能体可以辅助人类操作重复的 GUI 任务，其中有效的任务规划对于将复杂任务分解为可执行的动作至关重要。虽然与商业大模型相比，小型开源 MLLM 具有成本效益和保护隐私的优势，但它们面临着规划能力弱以及跨网站泛化能力有限的问题。为了解决这些局限性，我们引入了规划经验探索与利用（PEEU）方法，该方法自主探索环境以发现经验，并利用后验经验（hindsight experience）来合成严格对齐的高级训练数据。为了定量分析推动这种性能的泛化行为，我们提出了任务分解层次分析框架（TDHAF），以系统研究三种任务粒度（低、中、高水平）下的组合泛化。我们的分析表明，掌握低级的原子技能并不能保证高级的规划能力，而高级任务训练能带来更强的 OOD（分布外）泛化。在真实世界基准上的实验证明了 PEEU 的卓越有效性：我们的 7B 模型实现了 30.6% 的准确率，表现优于大得多的 Qwen2.5-VL-32B 模型。这表明构建后验高级任务并利用经验对于提升小型 MLLM 的 OOD 规划能力至关重要。
- **PDF**: https://arxiv.org/pdf/2606.27330v1

### Designing Reward Signals for Portable Query Generation: A Case Study in Industrial Semantic Job Search
- **分数**: 6
- **链接**  https://arxiv.org/abs/2606.27291v1
- **作者**: Ping Liu, Qianqi Shen, Jianqiang Shen, Wenqiong Liu, Rajat Arora, Yunxiang Ren, Chunnan Yao, Dan Xu, Baofen Zheng, Wanjun Jiang, Andrii Soviak, Kevin Kao, Jingwei Wu, Wenjing Zhang
- **备注**: Accepted to KDD 2026 Workshop on AI Agent for Information Retrieval (Agent4IR)
- **摘要**: 求职平台依赖于低带宽的查询接口，这些接口往往无法捕捉求职者画像的高维复杂性。我们提出了一个端到端的 RLAIF（基于 AI 反馈的强化学习）框架来生成“可移植的”求职查询（即在保留可推广的资质的同时，抽离出求职者特有标识符的术语）。这项任务引入了一个高度对抗性的奖励表面，在此表面上，策略优化经常会利用“LLM 作为裁判”细则中的缺陷，从而导致退化的逐字复制行为。我们进行了全面的实证实验，以分离优化机制对结构化奖励工程的影响。我们的结果表明，对于无判别器（critic-free）的优化器，性能绝大部分取决于强健的奖励塑造（reward shaping），而具体算法的选择在很大程度上无关紧要。虽然无判别器的单次 rollout 基线方法（RLOO 和 REINFORCE++）天然能够抵抗奖励黑客攻击（reward-hacking），但 GRPO 中的组相对优势归一化（group-relative advantage normalization）似乎对伪奖励信号特别敏感，使其格外容易受到欺骗。我们表明，引入确定性的、基于规则的奖励下限来纠正分配给逐字复制的奖励，可以缓解这一失效模式，从而使交叉家族评估裁判的质量大幅提升了 $+0.147$。最终，我们表明训练时的奖励模型使性能提升虚高了 $2.4\times$，这证实了训练的成功从根本上依赖于强制执行奖励塑造规程，而不是选择其他的优化器。
- **PDF**: https://arxiv.org/pdf/2606.27291v1

### Autoregressive Boltzmann Generators
- **分数**: 5
- **链接**  https://arxiv.org/abs/2606.27361v1
- **作者**: Danyal Rehman, Charlie B. Tan, Yoshua Bengio, Avishek Joey Bose, Alexander Tong
- **备注**: ICML 2026 (Spotlight)
- **摘要**: 在热力学平衡下对分子系统进行高效采样是统计物理学中的一个重大挑战。这一挑战推动了玻尔兹曼生成器（BGs）的发展，它通过结合生成模型、精确似然和重要性采样修正，能够快速生成无关联的平衡样本。然而，现代 BG 主要依赖于归一化流（NFs），这要么由于严格的可逆性约束（离散时间）而导致表达能力受限，要么面临着计算昂贵的似然度（连续时间）。在本文中，我们提出了自回归玻尔兹曼生成器（ArBG）——一种新型的自回归建模框架——它通过脱离基于流的 BG 范式克服了这些局限性。ArBG 避开了流的拓扑约束，并允许在推理时进行顺序干预，同时通过利用在大语言模型中行之有效的架构提供了更强的可扩展性。我们凭经验证明，在所有基准测试中，ArBG 相比于基于流的模型均有显著改善，特别是在更大的肽系统（如10残基的 Chignolin）中。此外，我们引入了 Robin，这是一个拥有 1.32 亿参数、基于 ArBG 框架训练的可迁移模型，它比先前的最先进技术有所改进，在 8 残基系统上将零样本能量误差 E-W$_2$ 降低了 60$\%$ 以上。代码可在 https://github.com/danyalrehman/autobg 获得。
- **PDF**: https://arxiv.org/pdf/2606.27361v1

### Beyond Surface Forms: A Comprehensive, Mechanism-Oriented Taxonomy of Indirect Linguistic Encoding for LLM-Based Coded Language Detection
- **分数**: 4
- **链接**  https://arxiv.org/abs/2606.27314v1
- **作者**: Hamid Reza Firoozfar, Mohammadsadegh Abolhasani, Reza Mousavi, Paul Jen-Hwa Hu
- **备注**: Submitted for review in ARR for EMNLP 2026
- **摘要**: 为了避免社交媒体上的审核和监控，一些用户经常发明间接语言表达（ILE）来掩盖敏感含义。这些表达根据意图和语境呈现为“平台黑话”（algospeak）、委婉语和对抗性模糊处理，并涉及循环出现的编码机制。我们提出了一种全面的、面向机制的 ILE 分类法，该分类法抽象掉了交流目标，转而对编码和恢复含义的底层操作进行分类。我们通过将该分类法融入大语言模型（LLM）的提示中，并使用 2,000 条人工标注的 TikTok 和 Bluesky 帖子，将其与四种现有的分类法以及无分类法的基线进行比较，以此来评估该分类法。所提出的分类法在三种 LLM 中均获得了最强的文档级和跨度（span）级性能，相比于表现最好的基准模型，其准确率提高了 4.7%，F1 分数提高了 5.4%。实证结果表明，一个全面的、面向机制的分类法对于作为检测新兴隐秘语言的稳定框架以及作为内容审核的有用输入至关重要。免责声明：本文包含可能属于亵渎、粗俗或冒犯性的内容。
- **PDF**: https://arxiv.org/pdf/2606.27314v1

### BOWConnect: Parallel Bayesian Optimization over Windows with Learned Local Cost Maps for Sample-Efficient Kinodynamic Motion Planning
- **分数**: 4
- **链接**  https://arxiv.org/abs/2606.27292v1
- **作者**: Sourav Raxit, Abdullah Al Redwan Newaz, Jose Fuentes, Leonardo Bobadilla
- **备注**: Accepted to the 2026 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS 2026)
- **摘要**: 本文提出了 BOWConnect，这是一种双向并行运动学动力学（kinodynamic）路径规划器，旨在解决现有基于采样的方法的三个根本局限性：高维状态空间中的样本低效性、动力学约束下不可靠的代价启发式算法，以及在狭窄通道环境中的低劣表现。与依赖随机控制采样和几何距离启发式算法的经典规划器不同，BOWConnect 将窗口贝叶斯优化（BOW）作为一种基于学习的转向函数集成到基于并行树的探索框架中，使每个工作器能够学习局部代价地图和约束，从而引导采样走向动力学可行且无碰撞的控制。双向架构在并行线程中同时从起点和目标区域构建前向和后向树，空间哈希机制可实现快速连接查询，而边值问题求解器则可生成运动动力学一致的桥接轨迹。在十个基准环境中的广泛评估表明，BOWConnect 实现了 100% 的成功率，同时在复杂场景（包括最先进规划器失败或性能显著退化的狭窄通道和非凸空间）中提供了最快或接近最快的规划时间。在地面车辆和四轴飞行器上的实际部署证实了其无碰撞的实时规划能力。视频和开源代码见 https://bow-connect.github.io/。
- **PDF**: https://arxiv.org/pdf/2606.27292v1

--- 
## 📚 学科: `math.*`

本期 `math.*`（数学）学科推荐了一篇被 COLT 2026 录用的杰出论文。该研究攻克了高维截断高斯分布学习这一统计学与机器学习领域的经典难题。作者针对未知半空间截断下的高斯分布，提出了一种极速且样本复杂度最优的算法。其核心突破在于将低阶矩用“相对截断参数”重新解释，从而巧妙绕过了传统方法中极其耗时的投影随机梯度下降步骤。该成果在理论上实现了在半空间截断下“免费”学习高斯分布的卓越性能。

### Fast algorithms for learning a Gaussian under halfspace truncation with optimal sample complexity
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.27298v1
- **作者**: Haitong Liu, Deepak Narayanan Sridharan, David Steurer, Manuel Wiedmer
- **备注**: 88 pages; accepted at the 39th Annual Conference on Learning Theory (COLT 2026)
- **摘要**: 我们研究了在未知半空间截断下学习高维高斯分布的根本问题。Lee、Mehrotra 和 Zampetakis (FOCS'24) 最近首次获得了该问题的多项式时间算法，但其样本和时间复杂度界限并不是最优的。在非平凡截断下，对于任何目标精度 $\varepsilon > 0$ 和维度 $d$，我们给出了一种高效的算法，该算法使用 $n = \tilde{O}(d^2/\varepsilon^2)$ 个样本，并在全变差距离内以误差 $\varepsilon$ 学习潜在的高斯分布。我们的算法速度也很快：其运行时间主要由计算经验协方差矩阵的成本决定。即便在没有截断的情况下，我们的样本和时间复杂度在 $d$ 和 $\varepsilon$ 方面也是最优的：在这方面，我们可以在半空间截断下“免费”学习高斯分布。我们结果背后的关键要素是：针对截断高斯分布的低阶矩，根据相对截断参数提出了一种新颖的重新解释。该相对截断参数唯一地确定了未截断高斯分布的参数，并使得能够进行直接参数恢复。这种重新解释使我们能够绕过在截断学习中广泛使用的、耗时的投影随机梯度下降过程。
- **PDF**: https://arxiv.org/pdf/2606.27298v1

--- 
## 📚 学科: `astro-ph.*`

本期 `astro-ph.*`（天体物理学）学科精选了5篇极具分量的学术论文，主要聚焦于下一代巨型射电望远镜——平方千米阵（SKA）所引领的前沿科学研究以及星际介质的化学和物理性质。研究涵盖了利用 SKA AA4 重构三维空间中的 3D 磁场矢量、通过 SKA 探索行星形成盘中复杂的厘米波分子前体、结合机器学习（iSEEDs 项目）高效挖掘年轻原恒星盘物理和化学丰度、以及利用 SKA-Low 协同粒子探测器测量银河系至银河外过渡能区的高能宇宙线质量成分。此外，还有一篇利用 MUSE 仪器对富勒烯行星状星云 Tc 1 的消光和电子分布性质进行的细致光谱观测研究。

### 3D Magnetic Field Vectors in Space: Bubbles, Clouds, and Filaments
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.27346v1
- **作者**: Mehrnoosh Tahani, Anna Ordog, Jennifer West, Georgia V. Panopoulou, Hiroko Shinnaga, Marijke Haverkorn
- **备注**: Published in Advancing Astrophysics with the SKA II (AASKAII), 2026 (arXiv:2606.20366). Report-no:AASKAII/Tahani01. Advancing Astrophysics with the SKA II (AASKAII) outlines the transformative scientific advances that will be enabled by the SKA telescopes. 30 pages, 5 figures
- **摘要**: 磁场在不同空间尺度的恒星形成过程中起着重要作用。磁场强度（星际介质能量预算的关键组成部分）与磁场方向相对于密度结构之间的相互作用，影响着星际物质如何向恒星形成演化。为了理解星系向恒星、行星以及最终生命的演化，我们需要在三维（3D）空间中绘制三维磁场矢量图。然而，由于投影效应以及可观测追踪物与磁场几何形状之间的复杂关系，确定完整的矢量信息仍然具有挑战性。我们概述了可用于探测弥散星际介质（ISM）中的超新星遗迹（SNR）、超级气泡、HII 区和 HI 纤维状结构，以及致密 ISM 中的分子云、纤维状结构和核等物体的 3D 磁场结构的观测技术。主要的平方千米阵（SKA）特有观测技术包括同步辐射发射以及致密源和弥散发射的法拉第旋转。我们讨论了 SKA AA4 如何利用与现有数据集相比大幅提高的灵敏度、分辨率和 uv 覆盖度，来实现我们所描述的技术。这将增强我们重构 3D 磁场矢量的能力，从而推进我们对星系演化和恒星形成中磁场的理解。
- **PDF**: https://arxiv.org/pdf/2606.27346v1

### Unveiling Complex Chemistry in Planet-forming Disks with the SKAO
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.27289v1
- **作者**: Linda Podio, Lisa Giani, Catherine Walsh, Audrey Coutens, Izaskun Jiménez-Serra, Claudio Codella, María José Maureira, Marta De Simone, John D. Ilee, Manuela Lippi, Chin-Fei Lee, Romane Le Gal, Mayank Narang, Giovanni Sabatini, Eleonora Bianchi, Elenia Pacetti, Danai Polychroni, Bihan Banerjee, Paola Caselli, Cecilia Ceccarelli, Amin Farhang, Antonio Garufi, Greta Guidi, Adriano Ingallinera, Stavro L. Ivanovski, Pamela Klaassen, Ana López-Sepulcre, Liton Majumdar, Giulia Perotti, Jaime E. Pineda, Daniel J. Price, Manoj Puravankara, Pablo Rivière-Marichalar, Alvaro Sánchez-Monge, Eugenio Schisano, Paolo M. Simonetti, Leonardo Testi, Claudia Toci, Diego Turrini, Alessio Traficante, Yinhao Wu
- **备注**: Published in Advancing Astrophysics with the SKA II (AASKAII), 2026 (arXiv:2606.20366). Report-no:AASKAII/Podio01. Advancing Astrophysics with the SKA II (AASKAII) outlines the transformative scientific advances that will be enabled by the SKA telescopes
- **摘要**: 行星的化学成分继承自行星形成时其母体原行星盘的化学成分。近年来，我们在表征原行星盘化学方面取得了巨大进展。（亚）毫米波干涉仪（如 ALMA）使我们能够探测从简单到复杂有机分子的发射线，并探测它们在原行星盘中的径向和垂直分布。另一方面，JWST 已开始揭示原行星盘冰的成分，以及来自原行星盘最内侧区域的谱线发射。SKA 的到来将通过在厘米范围内观察具有峰值发射的更重分子（包括重碳链和环以及前生命期分子）的发射线，从而在该领域开启新的篇章。此外，SKA 还将探测来自那些在毫米波长下被尘埃不透明度遮挡的区域（即原行星盘中平面，通常是内部 30 au 区域）的分子发射。这些观测将限制原行星盘演化和行星形成的初始条件，使我们能够预测正在形成的行星及其大气的化学成分。将这些结果与未来关于系外行星大气以及太阳系中原始天体化学成分的研究结果进行对比，将为包括我们自身在内的行星系统的起源和演化提供新的启示。
- **PDF**: https://arxiv.org/pdf/2606.27289v1

### Astrochemical Study of Early Embedded Disks
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.27278v1
- **作者**: Eleonora Bianchi
- **备注**: Accepted for publication in Frontiers in Astronomy and Space Sciences
- **摘要**: 我们的行星是如何形成的，以及更广泛地，行星系统是如何形成的问题是极其基础的，并且已在广泛的研究领域中得到了探讨。然而，我们仍然缺乏对恒星和行星形成过程基本方面的全面理解。特别是，测量年轻原恒星盘的质量和化学成分的挑战迄今为止阻碍了与观测到的系外行星群进行有意义的比较。在不久的将来，这对于解读欧洲空间任务（如 Ariel）的结果将变得至关重要，该任务将提供系外行星质量和化学成分的全面清单。基于天体化学和数据科学的最新发展，本前沿观点探讨了研究年轻行星形成盘的未来研究方向，并介绍了“早期嵌入盘的天体化学研究”（iSEEDs）项目。通过将机器学习和数据挖掘与天体化学相结合，iSEEDs 提供了一个强大的框架，可以系统地提取隐藏在原恒星环境高分辨率数据集中的物理条件和分子丰度。
- **PDF**: https://arxiv.org/pdf/2606.27278v1

### Origins of Cosmic Rays in the Galactic-extragalactic Transition Energy Range
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.27270v1
- **作者**: A. Corstanje, S. Saha, S. Bouma, J. Bray, S. Buitink, V. de Henau, E. Dickinson, B. Hare, A. Haungs, H. He, J. Hörandel, T. Huege, C. James, P. Laub, X. Li, H-J. Mathes, K. Mulrey, A. Nelles, F. Schlüter, O. Scholten, R. Spencer, C. Sterpka, K. Terveer, S. Thoudam, G. Trinh, P. Turekova, D. Veberic, K. Watanabe, C. Zhang, P. Zhang, Y. Zhang
- **备注**: Published in Advancing Astrophysics with the SKA II (AASKAII), 2026 (arXiv:2606.20366). Report-no:AASKAII/Corstanje01
- **摘要**: 抵达地球的宇宙线的能量范围从 $10^9$ 到超过 $10^{20}$ eV。高能宇宙线科学中尚未解决的问题之一涉及能够被银河系源加速的最高能量宇宙线的起源，以及超出此能量后只能由银河外源提供的过渡能量。测量质量成分为将测量结果与源和传播模型进行对比提供了关键信息，这既源自源处的丰度，也源自与粒子电荷（因而与其质量）成正比的最大可达能量。来自银河系的最高能量宇宙线存在于 $10^{16}$ 到 $10^{18}$ eV 的范围内，这一范围非常适合进行无线电探测。基于在 LOFAR 测量宇宙线十年的经验，我们表明，通过配备小型粒子探测器阵列，SKA-Low 非常适合通过在此能量范围内测量宇宙线的质量成分来推动该领域的发展。
- **PDF**: https://arxiv.org/pdf/2606.27270v1

### MUSE Imaging Spectroscopy of the Fullerene Planetary Nebula Tc 1
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.27245v1
- **作者**: J. R. Walsh, M. J. Barlow, A. Monreal-Ibero, J. Cami, E. Peeters, R. Wesson, J. Bernard-Salas, N. L. J. Cox, G. F. J. Watt
- **备注**: 24 pages, 5 Appendices, 11 tables and 17 figures (PDF). Accepted by A&A
- **摘要**: 对行星状星云 Tc 1（PN G345.2 -08.8，银河系中罕见的在红外波段显示富勒烯发射的行星状星云之一）使用 MUSE 宽场模式并结合自适应光学进行了观测，波长范围为 4750-9300Å。展示了由碰撞激发和重组线比率得到的消光、电子温度 ($T_e$) 和密度 ($N_e$) 图像。该星云拥有一个 12 角秒的高表面亮度核心，一个围绕中心恒星的主轴为 2.8 角秒的椭圆环以及一些低电离结，还有一个尺寸为 55 角秒的扩展晕；在核心和晕之间是一个具有过渡性质的环带，包括比核心更高的 $T_e$ 和更低的 $N_e$。由氢巴耳末线比率得到的可见光消光图像结构非常复杂，并在紧邻核心处显示出一个低消光环带，其消光度低于视线方向上的星际消光。本文研究了产生这种异常低消光区域的仪器效应以及来自星云尘埃散射特性的固有效应；两者都无法完全解释该低消光区域，最可能的原因是局部的非标准尘埃红化定律。该低消光区域还显示出异常高的 He I 7281/6678Å 线比率，这可能是由污染线引起的，但目前尚未能确定具体的谱线。提取了中心恒星的光谱，并由 31000K 的模型大气进行拟合，其类型为 O7.5I(f)。在扩展区域上，发现检测到的连续谱相比于星云连续谱有所增强，这在 MUSE 观测到的其他一些行星状星云中也能看到。低消光环带出现在最强富勒烯发射区域之外，处于 $N_e$ 下降而 $T_e$ 上升的区域。由此推断出与高密度核心星云和低密度晕之间的这一过渡区域环境相关的尘埃性质变化。
- **PDF**: https://arxiv.org/pdf/2606.27245v1

--- 
## 📚 学科: `stat.*`

本期 `stat.*`（统计学）学科精选了3篇涵盖计算统计与机器学习理论的高水平论文。ICML 2026 论文针对共享词汇表的 LLM 家族提出了“FisherSketch”，通过估计联合激活-误差空间中的 Fisher 对齐，在词汇表尺度上优雅地解决了无训练源选择与迁移诊断难题；另一篇 COLT 2026 录用论文针对高维半空间截断下的高斯分布学习，提出了一种突破性的高效参数恢复算法，在保持最优样本复杂度的同时实现了计算上的“免费”截断学习；最后，PCIC 2024 论文将高斯图模型与预算约束相结合，研究了部分测量下的因果效应估计与实验设计优化，在制药与工业分析中展现了极高的实用价值。

### The Geometry of Updates: Fisher Alignment at Vocabulary Scale
- **分数**: 6
- **链接**  https://arxiv.org/abs/2606.27242v1
- **作者**: John Sweeney
- **备注**: Accepted at the 43rd International Conference on Machine Learning (ICML 2026), PMLR 306. 64 pages total (main paper plus appendix), 4 figures, 29 tables
- **摘要**: 在 SMILES、蛋白质和基因组序列等科学字符串领域中，出现了针对共享词汇表的大语言模型（LLM）家族进行无训练源选择的需求，这些候选语料库共享同一个分词器，但在预测目标上存在差异。这创造了一种“激活黑暗”的境界：在没有关于标签条件误差几何的假设下，表示相似性度量可能毫无用处，而经典的更新几何度量在词汇表规模上由于计算成本高昂而令人望而却步。我们展示了在共享输出头设置下，表示度量（例如 CKA）对于迁移是不可识别的；模型可以共享完全相同的表示，但具有正交的头部更新。关键等式在于，头部 Fisher 对齐正是联合激活-误差空间中核均值嵌入之间的余弦值，从而暴露出激活、误差和耦合因子，而不需要实例化 Fisher 矩阵。FisherSketch 在单个流式传递中直接估计该余弦值，使得使用 16 KB 的任务签名（$m=4096$）和 192 KB 的单任务流状态就能实现实际的 $K=128,256$ 头部 Fisher 对齐。除了源选择之外，相同的签名和边缘分布还提供了一种诊断工具，用于研究 LLM 任务相似性是由激活、误差还是其耦合驱动的。
- **PDF**: https://arxiv.org/pdf/2606.27242v1

### Fast algorithms for learning a Gaussian under halfspace truncation with optimal sample complexity
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.27298v1
- **作者**: Haitong Liu, Deepak Narayanan Sridharan, David Steurer, Manuel Wiedmer
- **备注**: 88 pages; accepted at the 39th Annual Conference on Learning Theory (COLT 2026)
- **摘要**: 我们研究了在未知半空间截断下学习高维高斯分布的根本问题。Lee、Mehrotra 和 Zampetakis (FOCS'24) 最近首次获得了该问题的多项式时间算法，但其样本和时间复杂度界限并不是最优的。在非平凡截断下，对于任何目标精度 $\varepsilon > 0$ 和维度 $d$，我们给出了一种高效的算法，该算法使用 $n = \tilde{O}(d^2/\varepsilon^2)$ 个样本，并在全变差距离内以误差 $\varepsilon$ 学习潜在的高斯分布。我们的算法速度也很快：其运行时间主要由计算经验协方差矩阵的成本决定。即便在没有截断的情况下，我们的样本和时间复杂度在 $d$ 和 $\varepsilon$ 方面也是最优的：在这方面，我们可以在半空间截断下“免费”学习高斯分布。我们结果背后的关键要素是：针对截断高斯分布的低阶矩，根据相对截断参数提出了一种新颖的重新解释。该相对截断参数唯一地确定了未截断高斯分布的参数，并使得能够进行直接参数恢复。这种重新解释使我们能够绕过在截断学习中广泛使用的、耗时的投影随机梯度下降过程。
- **PDF**: https://arxiv.org/pdf/2606.27298v1

### Optimizing Experimental Design for Causal Effect Estimation with Partial Measurements
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.26818v1
- **作者**: Leopold Mareis
- **备注**: Published at the 6th Pacific Causal Inference Conference (PCIC 2024)
- **摘要**: 工具变量回归通过利用工具变量 $ X_1 $ 来量化可能存在混杂的干预变量 $ X_2 $ 与响应变量 $ X_3 $ 之间的因果效应。我们的工作考虑了这样一种设定：已给出了 $ X_{123} $ 联合分布的一些先验信息（可能通过初始数据集获取）。然而，必须收集更多样本以提高估计的准确性。我们表明，在高斯图形模型中的特定参数配置下，采集部分样本（例如仅来自 $ X_{12} $）可以减少一致估计量的渐近方差。通过在每个（部分）样本的成本上添加预算约束，这一想法得到了进一步拓展。该优化问题在实数范围内是解析可解的，并能给出所需的部分样本和完整样本的最优数量。我们提供了在最优预算分配下检测非零因果效应的显著性水平、检验效能和样本量计算方法。我们的方法可以显著减少所需预算和完整样本的数量。最后，我们展示了自适应因果效应估计在汽车分析和制药研究中的优势和适用性。
- **PDF**: https://arxiv.org/pdf/2606.26818v1

--- 
## 📚 学科: `econ.*`

本期 `econ.*`（经济学）学科精选了2篇将现代技术（如大模型）与传统经济学理论相结合的优秀论文。第一篇论文针对基座模型在离散选择预测中常常违背经济学常识（如价格上涨需求反而上升）的痛点，创新性地提出了一种两阶段适配器，将表格基座模型的预测嵌入多项式 Logit 模型中，在显著提高预测准确率的同时，从数学上保证了时间价值和成本单调性等经济学逻辑。第二篇论文则在传统国际贸易框架下构建了两国两期模型，深入探讨了发展中国家如何通过在前期加大创新资本投入以提高全要素生产率（TFP），从而在贸易自由化（全球化）中实现获益。

### Embedding Foundation Model Predictions in Discrete-Choice Models with Structural Guarantees
- **分数**: 4
- **链接**  https://arxiv.org/abs/2606.26432v1
- **作者**: Yingshuo Wang, Xian Sun, Yanhang Li, Zhichao Fan, Zexin Zhuang
- **备注**: Extends arXiv:2605.26559 (ICML 2026 FMSD Workshop)
- **摘要**: 表格基座模型在选择预测任务上取得了极高的准确率，但其预测往往违反了这些任务所要求的经济学逻辑：提高价格可能会增加预测需求，隐含的支付意愿估计经常为负或不切实际，且不可用的备选项也会获得非零概率。我们提出了一种两阶段适配器，该适配器将基座模型预测的选择概率作为预计算的特征，并将其嵌入到多项式 Logit（multinomial logit）的效用函数中。在第一阶段，我们通过具有符号约束的最大似然法拟合多项式 Logit 的结构系数；在第二阶段，我们冻结这些系数，并拟合一个作用于基座模型预测的微小神经修正。我们证明，这种组合精确地保留了多项式 Logit 的边际替代率，因此分析可计算的时间价值（value-of-time）成为一种数学保证，而非经验上的偶然。在三个数据集和两个基座模型上的实验表明，该适配器在测试准确率上比多项式 Logit 平均提升了 6.4 个百分点（最高达 12.8 个百分点），同时保持了 100% 的成本单调性，并在交通数据集上产生了符合已发表交通经济学范围的时间价值。在基座模型上下文受限的情况下，性能退化十分温和。
- **PDF**: https://arxiv.org/pdf/2606.26432v1

### Globalization, economic growth, and innovation: A two-country two-period model
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.23861v1
- **作者**: Cuong Le Van, Duc V. Le, Thanh Tam Nguyen-Huu
- **备注**: 23 pages, 3 figures. Authors' final peer-reviewed manuscript of the article published in: International Economics, Vol. 187 (2026), 100725
- **摘要**: 本文探讨了发展中国家如何从贸易自由化中受益。我们构建了一个两阶段模型（包含自给自足阶段和全球化阶段）以及一个两国框架（包含一个发展中国家和一个代表世界其他地区的发达国家）。我们的研究结果表明，当发展中国家的全要素生产率（TFP）显著低于发达国家时，全球化可能会使发展中国家处于不利地位。然而，我们证明，发展中国家仍可以通过在自给自足时期将部分资本分配给创新，从而提高其全要素生产率，进而从贸易开放中获得收益。
- **PDF**: https://arxiv.org/pdf/2606.23861v1

---