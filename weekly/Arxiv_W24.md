# 🗓️ 周报 (2026-W24)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-06-14

--- 
## 📚 学科: `eess.*`
本周精选论文主要集中在语音交互系统、自动控制及博弈论领域。研究重点包括：多方语音通话中的实时轮替管理机制；通过预测端点来降低语音对话系统的延迟；应用于欠驱动航天器姿态控制的物理启发神经网络与模型预测控制（MPC）结合方案；以及针对多说话人语音识别中 ASR 与话者重叠识别的平衡策略。此外，还有关于 N 玩家线性二次博弈中反馈纳什均衡的理论计算研究。这些成果均已被 Interspeech、IEEE LCSS 等顶级会议或期刊接收。

### Adaptive Turn-Taking for Real-time Multi-Party Voice Agents
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13544v1
- **作者**: Soumyajit Mitra, Prabhat Pandey, Abhinav Jain, Shanmukha Sahith, K V Vijay Girish
- **备注**: Accepted for publication at Interspeech 2026
- **摘要**: 多方语音对话中的轮替（Turn-taking）仍是语音代理面临的核心挑战，尤其是在动态的发言竞争和多变的用户预期下。我们提出了 ModeratorLM，这是一种角色扮演语音代理，它根据多方场景中明确分配的角色来调节轮替行为。该系统构建在一个以分块流式方式运行的语音大语言模型之上。我们进一步引入了一种推理增强变体，它在对话上下文和分配的角色上结合了思维链（CoT）推理。我们构建了 RolePlayConv，这是一个包含多种助手角色的大规模合成多方口语对话数据集。在真实会议数据和 RolePlayConv 上的实验表明，与非角色条件的基准模型相比，该方法将轮替精确度提高了 40% 以上，召回率提高了 70% 以上，同时大幅减少了误报中断。
- **PDF**: https://arxiv.org/pdf/2606.13544v1

### Endpoint Anticipation for Low-Latency Spoken Dialogue
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13450v1
- **作者**: Sathvik Udupa, Shinji Watanabe, Petr Schwarz, Jan Cernocky
- **备注**: Accepted at Interspeech 2026
- **摘要**: 虽然低延迟交互对语音对话至关重要，但级联架构往往受限于反应性的轮替完成检测。我们提出了“端点预测”（Endpoint Anticipation），将反应性检测转变为对轮替结束信号的主动预测。我们的语音模型可以提前多达 2.56 秒预测端点，从而允许 LLM 和 TTS 流水线在部分上下文上进行推测执行。我们引入了量化指标来平衡实现的延迟降低与计算冗余。在对话式和任务导向型数据集上的评估显示，我们的模型始终优于具有竞争力的基于 VAP 的基准。与 Unmute 框架的集成表明，平均延迟减少了 505 毫秒，推测计算增加了 28.4%，有效地掩盖了序列瓶颈，从而在实时语音到语音交互中实现复杂的推理。
- **PDF**: https://arxiv.org/pdf/2606.13450v1

### MPC for underactuated spacecraft control with a Lyapunov supervised physics-informed neural network correction layer
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13113v1
- **作者**: Amirhossein Ayanmanesh Motlaghmofrad, Carlo Cena, Mauro Martini, Marcello Chiaberge
- **备注**: Accepted at SPAICE (AI in and for Space) 2026
- **摘要**: 欠驱动航天器面临可控性限制以及对环境扰动的高度敏感性，这使得姿态机动和稳定变得复杂。由于欠驱动轴缺乏控制权限，传统控制器无法直接稳定所有姿态组件，因此需要参考规划策略。此外，MPC 方法对转动惯量不确定性和未建模的动力学耦合保持敏感，导致失配下跟踪性能下降。为解决这些问题，我们考虑一种集成三层的分层架构：(i) 非线性模型预测控制器 (NMPC)，用于约束和欠驱动感知的机动规划及执行器限制下的标称闭环稳定性；(ii) 物理启发神经网络 (PINN)，在模拟数据上进行离线训练以估计残余扰动力矩，其损失项加强了与刚体旋转动力学的一致性；(iii) 基于 Lyapunov 的监督安全机制，在线评估学习到的修正量，并限制或抑制其影响以保持基准控制器的稳定性。该架构在模拟反作用轮动力学、执行器饱和和环境扰动的高保真仿真环境中进行了评估。蒙特卡洛研究表明，与独立 NMPC 相比，该方法显著降低了稳态姿态误差，同时在不确定性下保持了稳健行为。
- **PDF**: https://arxiv.org/pdf/2606.13113v1

### Balancing ASR and diarization in end-to-end LLMs for multi-talker speech recognition
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13095v1
- **作者**: Naijun Zheng, Yuke Lin, Sanli Tian, Mengtian Li, Zhiwei Lin, Longshuai Xiao, Dandan Tu
- **备注**: Accepted in Interspeech 2026
- **摘要**: 多人语音识别通常通过在流水线系统中结合自动语音识别 (ASR) 和说话人日志 (diarization) 来解决。近期，基于 LLM 的方法通过联合建模语义和说话人信息展示了潜力，但它们通常需要大规模且标注昂贵的多人语音语料库。本文研究如何利用有限的真实录音数据高效训练基于 LLM 的系统，同时保持高精度的说话人归属。我们提出了几种策略：(1) 双编码器架构以提取语义和说话人特征；(2) 特征交错格式将这些特征作为 LLM 输入；(3) 长度感知的说话人 ID 损失以增强日志能力；(4) 针对 ASR 损失计算的自适应阈值策略，以减轻语音重叠导致的幻觉。这些策略平衡了 ASR 和日志任务之间的训练。我们的系统优于开源基准方法，在 AliMeeting 语料库上实现了 18% 的相对提升，在 Aishell4 语料库上提升了 24%。
- **PDF**: https://arxiv.org/pdf/2606.13095v1

### Characterization and Computation of Feedback Nash Equilibria in Scalar Discounted N-Player Linear Quadratic Games
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13087v1
- **作者**: Chiara Cavalagli, Alberto Bemporad, Mario Zanon
- **备注**: Accepted for publication in IEEE Control Systems Letters (LCSS), 2026
- **摘要**: 本文研究了具有 $N$ 个玩家的标量折扣线性二次 (LQ) 博弈中的反馈纳什均衡 (FNE)。通过显式引入折扣因子，我们展示了有限成本均衡可能无法稳定原始系统，从而引出了 FNE 与稳定 FNE 之间的区别以及充分稳定性条件。基于策略的参数化特征，我们提出了计算所有均衡的数值方法。特别关注了对称博弈，推导了对称 FNE 的闭式表达式以及存在多达 $M\leq2^N-2$ 个均衡的条件。数值实验阐明了均衡多重性如何取决于博弈配置，并突出了有限成本非稳定均衡的出现。
- **PDF**: https://arxiv.org/pdf/2606.13087v1

--- 
## 📚 学科: `q-bio.*`
本周定量生物学领域的研究展现了 AI 与生物学的深度融合。重点论文探讨了使用小型语言模型（LLM）进行低成本生物医学断言验证，以及蛋白质语言模型（pLM）在处理稀有病毒蛋白质序列时的几何表征特性。此外，还介绍了针对具有分层结构的成分数据（如微生物组）的新型正交分解方法，以及利用进化替换矩阵增强蛋白质属性预测的柔性核方法。最后，一项研究通过策略压缩框架探讨了人类决策中不可规避的不确定性成本，为理解认知偏差提供了新视角。相关论文多发表于 ICML 2026 等顶级人工智能会议。

### Small LLMs for Biomedical Claim Verification: Cost-Effective Fine-Tuning, Structural Dataset Shortcuts, and Cross-Domain Generalization
- **分数**: 6
- **链接**  https://arxiv.org/abs/2606.12854v1
- **作者**: Gaurav Kumar
- **备注**: 8 pages, 2 figures, 12 tables. To appear at BioNLP Workshop, ACL 2026
- **摘要**: 诸如 GPT-4o 等大语言模型在生物医学断言验证上表现出强劲的零样本性能，但成本和不透明性限制了其大规模应用。我们通过 QLoRA 在 SciFact 和 HealthVer 数据集上微调了三个小型 LLM：Phi-3-mini (3.8B)、Qwen2.5-3B 和 Mistral-7B。这是首个对比 QLoRA 模型与 GPT-4o 以及微调后的 BioLinkBERT 编码器的研究。仅使用 1,008 个训练样本，Mistral-7B QLoRA 的性能就超过了 GPT-4o（F1 分数提升高达 12%），且成本极低。我们进行了深入的领域内和跨领域评估，并识别出 SciFact 中一个此前未被报告的结构性人工痕迹（artifact），该痕迹会虚高领域内得分。研究表明，在结构合理的数据上训练可实现稳健的跨领域迁移。
- **PDF**: https://arxiv.org/pdf/2606.12854v1

### Viral Proteins Reveal Geometry of Protein Language Models
- **分数**: 6
- **链接**  https://arxiv.org/abs/2606.12609v1
- **作者**: Arthur Bigot, Harmon Bhasin, Core Francisco Park, Eugene Shakhnovich, Dianzhuo Wang
- **备注**: Accepted at ICML 2026 GenBio Workshop and FM4LS Workshop
- **摘要**: 蛋白质语言模型（pLM）是在高度不平衡的数据集上训练的，这引发了一个问题：它们如何表征代表性不足的生物序列。我们以病毒蛋白为案例，通过 ESM 模型系列研究发现，在嵌入空间中存在一个主导的“原生性”（nativeness）轴，它与掩码重建困惑度对齐，将序列从建模良好的细胞蛋白、病毒蛋白排序到打乱及随机序列。模型缩放会不均匀地收缩各病毒家族的这一轴线。尽管如此，pLM 嵌入仍保留了病毒特异性信号：病毒蛋白在零样本困惑度和浅层序列特征之外仍保持线性可分性。这些结果表明，pLM 表征由通用的原生性概念构建，同时保留了特定生物类群的信息。
- **PDF**: https://arxiv.org/pdf/2606.12609v1

### Tree-Structured Orthonormal Decomposition of the Aitchison Simplex
- **分数**: 6
- **链接**  https://arxiv.org/abs/2606.11646v1
- **作者**: Daisuke Yamada, Qijun Zhang, Travis Pence, Barbara B. Bendlin, Federico Rey, Vikas Singh
- **备注**: Accepted at ICML 2026. To appear in PMLR vol. 306
- **摘要**: 成分数据（编码相对比例的向量）广泛存在于生态学、地球化学和基因组学等科学领域。这些数据通常具有已知的分层结构（如分类学、系统发育），但现有方法要么忽略此结构，要么丢弃内在的 Aitchison 几何特性。我们提出了 PolyILR，这是一种与任何树拓扑结构对齐的 Aitchison 切空间规范正交分解方法。我们的构建在每个内部节点定义了捕捉完整分支结构的加权局部几何，然后将其提升到全局正交基，其中每个坐标对应一个特定的树位置。在微生物组和单细胞基准测试中，PolyILR 产生了稳定且可解释的特征，并支持多尺度树分辨率的推理。
- **PDF**: https://arxiv.org/pdf/2606.11646v1

### Flexible Kernels for Protein Property Prediction
- **分数**: 6
- **链接**  https://arxiv.org/abs/2606.11057v1
- **作者**: Martin Jankowiak, Yerdos Ordabayev, Rudraksh Tuwani, Henry N. Ward, Hunter Nisonoff, James M. McFarland, Gevorg Grigoryan
- **备注**: 50 pages; to appear at ICML 2026
- **摘要**: 尽管从稀疏实验数据预测蛋白质属性（如结合亲和力和热稳定性）对蛋白质设计至关重要，但这仍是一项挑战。为此，我们引入了一类序列核，它们利用进化替换矩阵和局部线性。结果表明，由此产生的离散高斯过程提供了数据高效的蛋白质属性景观模型，性能经常优于依赖基础模型嵌入的替代方案。此外，通过学习实质上的结构感知替换矩阵，我们的核可以轻松整合来自基础模型的结构信息。实验证明，这些结构条件核非常适合跨多个蛋白质属性景观的多任务学习，并且能显著超越局部监督学习方法。
- **PDF**: https://arxiv.org/pdf/2606.11057v1

### Including the Cost of Irreducible Uncertainty in the Policy Compression Framework
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13132v1
- **作者**: Álvaro Garrido-Pérez, Pieter Simoens, Amrapali Pednekar, Yara Khaluf
- **备注**: Accepted at the 5th International Conference on Hybrid Human-Artificial Intelligence, 2026
- **摘要**: AI 决策支持系统可以从预见人类决策偏好中获益。许多此类偏好可能源于人类的认知局限。策略压缩框架将决策建模为奖励最大化与编码状态相关行动策略的认知成本（互信息）之间的权衡。我们认为这一描述并不完整，因为它将条件熵（给定状态下选择哪种行动的不可规避不确定性）视为无成本的，尽管经验证据表明它会调节反应时间。因此，我们将认知成本定义为策略复杂性与加权条件熵项之和。由此产生的最优策略保留了标准指数形式，但变得更加敏锐，使得策略精度能够更独立于奖励敏感性而变化。这一修正意味着标准框架可能低估了行动选择的认知成本。
- **PDF**: https://arxiv.org/pdf/2606.13132v1

--- 
## 📚 学科: `cs.*`
计算机科学领域的选文涵盖了强化学习的应用、图神经网络（GNN）的理论分析、低资源语言处理及多模态合成。主要研究包括：DoorDash 开发的利用延迟市场反馈进行目标权重自适应的强化学习系统；对 GNN 中截断位置编码表达能力的理论研究；首个针对斯洛伐克语的大规模文本嵌入基准 SkMTEB 及其模型优化；结合生成式 AI 的印度斯坦音乐交互式虚拟伴奏系统；以及评估不同离散语音表征在 3D 面部动画合成中的效果。

### Multi-Agent Reinforcement Learning from Delayed Marketplace Feedback for Objective-Weight Adaptation in Three-Sided Dispatch
- **分数**: 6
- **链接**  https://arxiv.org/abs/2606.13604v1
- **作者**: Haochen Wu, Yi Hou, Shiguang Xie
- **备注**: Accepted at ICML 2026 Workshop on Reinforcement Learning from World Feedback (RLxF)
- **摘要**: 三方市场中的调度是强化学习在现实世界反馈中学习的典型场景：决策由延迟的运营结果（如送货速度、骑手利用率和商户拥堵）进行评估。我们介绍了 DoorDash 部署的一套强化学习系统，该系统利用延迟信号在大规模食品配送市场中自适应调整调度目标权重。该系统并未取代组合优化器，而是通过从历史数据中学习的门店级策略选择离散乘数，从而改变优化器在配送质量和拼单效率之间的平衡。在生产环境的切换实验（switchback experiment）中，该离散策略在不降低客户配送体验的前提下，增加了拼单量并降低了骑手的时间成本。
- **PDF**: https://arxiv.org/pdf/2606.13604v1

### Understanding Truncated Positional Encodings for Graph Neural Networks
- **分数**: 4
- **链接**  https://arxiv.org/abs/2606.13671v1
- **作者**: James Flora, Mitchell Black, Weng-Keen Wong, Amir Nayyeri
- **备注**: 28 pages, 4 figures, ICML 2026
- **摘要**: 位置编码（PE）在理论和实证上都增强了图神经网络（GNN）的能力。光谱族和基于步行（walk-based）族是两类最流行的 PE，理论上在“完整”版本下表达能力等价，介于 1-WL 和 3-WL 测试之间。然而，完整版本需要 $O(n^3)$ 的复杂度，实践中常使用截断变体（如前 $k$ 个特征空间）。本工作开启了对截断 PE 的研究。理论上，我们证明在截断情况下，几种 PE 家族的表达能力存在根本差异。作为推论，我们证明截断的光谱 PE 不再强于 1-WL 测试。实验表明，在现实世界数据集中，混合使用截断 PE 优于任何单一家族。
- **PDF**: https://arxiv.org/pdf/2606.13671v1

### SkMTEB: Slovak Massive Text Embedding Benchmark and Model Adaptation
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13647v1
- **作者**: Marek Šuppa, Andrej Ridzik, Daniel Hládek, Natália Kňažeková, Viktória Ondrejová
- **备注**: ACL 2026
- **摘要**: 我们推出了 SkMTEB，这是首个针对斯洛伐克语（一种低资源西斯拉夫语）的综合性 MTEB 风格文本嵌入基准，包含 7 类任务中的 31 个数据集。我们对 31 个嵌入模型进行的评估显示，经过指令微调的大型多语言模型表现最强。为了满足高效、本地部署的需求，我们通过词表裁剪和微调开发了 \texttt{e5-sk-small} (45M 参数) 和 \texttt{e5-sk-large} (365M)。尽管模型尺寸减小了高达 62%，我们的开源模型在语义搜索和检索增强生成（RAG）任务中仍能与闭源 API 竞争。
- **PDF**: https://arxiv.org/pdf/2606.13647v1

### The Moving Drone: Negotiating Agency Between the Voice and the Virtual
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13640v1
- **作者**: Nithya Shikarpur, Victor Arul, Anna Huang
- **备注**: Published in NIME music track 2026
- **摘要**: 印度斯坦音乐中的旋律素材通常与主音相关联，由名为 tanpura 的四弦持续音（drone）乐器维持。本作将传统上静态的持续音转化为动态，通过 Max/MSP 中的四个独立循环器充当“虚拟”持续音。随着歌手即兴发挥，系统实时循环填充，在人声与虚拟音之间创建有机演化的反馈。该作品还集成了 GaMaDHaNi（一种由歌手驱动的音高到语音生成 AI 模型）来重新合成音频。与追求高保真的 AI 趋势不同，本作有意利用低保真输出，强调人类的解释和情境感。
- **PDF**: https://arxiv.org/pdf/2606.13640v1

### From Tokens to Faces: Investigating Discrete Speech Representations for 3D Facial Animation
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13630v1
- **作者**: Pedro Correa, Olivier Perrotin, Samir Sadok, Paula Costa, Thomas Hueber
- **备注**: This work has been accepted in Interspeech 2026
- **摘要**: 语音表征的选择在语音驱动的 3D 面部动画中至关重要。我们评估了四类语音表征（SSL 特征、神经编解码器潜变量、ASR 风格标签等）在 3D 面部合成中的效果。通过客观指标和感知评估，我们发现编码音素类别对于准确预测面部动画大有裨益。基于此，我们引入了一个音视频文本转语音（AVTTS）流水线，利用离散表征作为共享空间来同时解码语音和 3D 面部运动。
- **PDF**: https://arxiv.org/pdf/2606.13630v1

--- 
## 📚 学科: `math.*`
_本周缺少高价值论文_

## 📚 学科: `astro-ph.*`
本周天体物理领域的研究涵盖了从恒星形成反馈到高红移星系探测等多个前沿方向。重要研究包括：通过模拟分析原恒星喷流反馈如何调节年轻星团的形成效率及结构；评估地面近红外光谱仪在变天背景下采用上坡采样（UTR）的可行性；探讨近核混合对大质量吸积恒星震荡特性的影响；在红移 $z=7.31$ 的星系中首次直接探测到冷分子气体；以及利用 JWST 数据研究 NGC 628 星系中恒星团的物理性质演化。这些成果发表于 MNRAS、ApJ 等权威天文期刊。

### Centrally concentrated star formation in young clusters II: Jet feedback
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13666v1
- **作者**: Adilkhan Assilkhan, Sabrina M. Appel, Bekdaulet Shukirgaliyev, Ernazar Abdikamalov, Simon Portegies Zwart, Eric P. Andersson, Mukhagali Kalambay, Mordecai-Mark Mac Low
- **备注**: Data products will be publicly available via AMNH Digital Library after publication
- **摘要**: 原恒星喷流是恒星反馈的最早形式之一。我们研究了在中心集中的分子云中，原恒星喷流如何影响恒星形成效率、时间变率、星团结构及早期动力学状态。使用 Torch 框架，我们对比了有无喷流反馈的六组模拟。结果显示，具有喷流反馈的模型实现的恒星形成效率（12-16%）明显低于无喷流模型（19-33%）。喷流导致恒星形成以离散爆发而非连续方式发生，产生更延展且具有子结构的恒星系统。带有喷流的运行能更好地重现年轻星团中观测到的投影结构参数 $Q_{2D}$ 范围。
- **PDF**: https://arxiv.org/pdf/2606.13666v1

### Feasibility of up-the-ramp sampling under variable sky for ground-based spectrographs
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13600v1
- **作者**: Gaia Gaspar, Marcin Sawicki, Nelson Nunes, Rubén J. Díaz, James E. H. Turner
- **备注**: To appear in SPIE Proceedings 2026
- **摘要**: 许多现代近红外仪器采用 H2RG 探测器，其积分时间可达 300-600s。上坡采样 (UTR) 在宇宙射线剔除和动态范围方面具有优势，但地面 K 波段天空亮度在分钟尺度上存在 3-10% 的波动。我们通过 GIRMOS 数据模拟器进行了可行性研究，利用 Gemini-NIRI 估算的天空变化进行评估。结果表明，UTR 的优势在读取噪声受限的谱线间区域依然成立，可节省 4-10% 的观测时间。但在天空发射线上，性能会受到 SNR 下降和错误的宇宙射线标记的影响。该研究为地面近红外光谱仪实现 UTR 提供了依据。
- **PDF**: https://arxiv.org/pdf/2606.13600v1

### The effect of near-core mixing on rejuvenation and the asteroseismic properties of massive accretors
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13567v1
- **作者**: Jan Henneco, Dominic M. Bowman
- **备注**: Accepted for publication in MNRAS
- **摘要**: 双星相互作用在高、中质量恒星系统中非常普遍。我们探讨了质量吸积后，近核区域（对流核外围）的混合假设（特别是半对流）如何影响星震学特征。研究显示，对流边界混合对恒星“返老还童”现象及吸积后的星震属性有主导影响。吸积后的热弛豫过程是决定最终近核结构和星震印记的关键。通过对周期间隔模式进行傅里叶变换，可以有效量化不同混合假设和吸积率对信号的影响。
- **PDF**: https://arxiv.org/pdf/2606.13567v1

### Direct detection of cool molecular gas in a star-forming galaxy at $z=7.31$
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13393v1
- **作者**: Karin Cescon et al.
- **备注**: Accepted for publication in MNRAS
- **摘要**: 我们调查了红移 $z=7.31$ 的高质量恒星形成星系 REBELS-25 的分子气体含量。通过 VLA 和 ALMA 观测，探测到了 CO(3-2) 和 CO(7-6) 发射，这是迄今为止在最高红移处探测到的低 $J$ CO 跃迁。推导出的分子气体质量约为 $10^{11} M_{\odot}$，直接证实了在大爆炸后仅 7 亿年就存在极大规模的气体库。这意味着该星系具有极高的气体占比（$f_{gas} \simeq 0.95$）和约 1.2 Gyr 的消耗时标。这一结果展示了在 $z > 7$ 探测低 $J$ CO 谱线的可行性，为研究早期星系质量增长提供了关键见解。
- **PDF**: https://arxiv.org/pdf/2606.13393v1

### Feedback in Extragalactic Star Clusters (FEAST): Spectral Energy Distributions and the Physical Properties of Star Clusters in NGC 628 with CIGALE
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13391v1
- **作者**: Sean T. Linden et al.
- **备注**: Accepted in ApJ
- **摘要**: 利用 HST 和 JWST 对 NGC 628 的观测，我们对超过 12,000 个星团进行了光谱能量分布（SED）拟合。我们发现新兴年轻星团（eYSC）的年龄峰值在 3-5 Myr 之间，其中约 12% 的星团具有高消光（$E(B-V)>2$），表明存在尘埃埋藏群体。数据揭示了从被埋藏状态到清除周围尘埃和气体的演化序列，PDR 清除时标约为 4 Myr。旋臂中的星团通常比臂间区域的星团质量更大、红化更严重。
- **PDF**: https://arxiv.org/pdf/2606.13391v1

--- 
## 📚 学科: `stat.*`
本周统计学与机器学习理论的选文重点关注复杂过程的建模与泛化。研究课题包括：PULSE 框架——一个针对直翅目昆虫生物声学的半监督多任务分类器，展示了主动学习在生态监测中的潜力；关于“可模拟过程”学习理论的研究，证明了在具有模拟器访问权限时，复杂相关数据同样能获得经典的 VC 维度泛化保证；以及对两层线性自回归模型在处理观测不完全的线性动力系统时，如何自然学习到近似卡尔曼滤波潜状态的理论证明。

### Decoding Insect Song: A Multitask Semisupervised Orthoptera Bioacoustic Classifier
- **分数**: 4
- **链接**  https://arxiv.org/abs/2606.13236v1
- **作者**: Olga Isupova, Danil Kuzin, Ella Browning, Tom Mills, Steven Reece
- **备注**: ICML 2026 Workshop on Machine Learning for Audio
- **摘要**: 被动声学监测对生态推断极具潜力，但现有自动工具通常训练受限且难以迁移。我们提出了 PULSE，这是一个用于直翅目昆虫（如蝗虫、蟋蟀）生物声学的半监督多任务框架，结合了弱监督物种分类、无标签现场音频的自监督学习以及通用模型的知识蒸馏。我们的领域自适应专家模型在所有指标上均优于最先进的通用模型，结合主动学习后 F1 分数进一步提升至 0.34，AUC 达 0.84。
- **PDF**: https://arxiv.org/pdf/2606.13236v1

### Learning with Simulators: No Regret in a Computationally Bounded World
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.13576v1
- **作者**: Sasha Voitovych, Abhishek Shetty, Noah Golowich, Alexander Rakhlin
- **备注**: To appear at COLT 2026
- **摘要**: 大多数学习理论结果严重依赖于数据生成过程的独立性。为填补这一空白，我们引入了“可模拟过程”（simulatable processes）框架，其中学习者可以访问一个逼近数据分布的模拟器。令人惊讶的是，给定此类模拟器，我们证明可以恢复与独立数据古典设置相同的学习保证。我们还展示了单一种算法能同时学习受限于计算时间的任何 VC 类，其后悔值（regret）受过程的时间有界 Kolmogorov 复杂度控制，显著拓宽了经典的 PAC 模型。
- **PDF**: https://arxiv.org/pdf/2606.13576v1

### Two-Layer Linear Auto-Regressive Models Estimate Latent States
- **分数**: 3
- **链接**  https://arxiv.org/abs/2606.12691v1
- **作者**: Yahya Sattar, Sunmook Choi, Leo Maynard-Zhang, Yassir Jedra, Maryam Fazel, Sarah Dean
- **备注**: ICML 2026
- **摘要**: 自回归模型在序列数据处理中表现强劲，但其如何学习潜在表征仍是开放性问题。本工作证明了当在部分观测的线性动力系统数据上进行经验风险最小化训练时，两层线性自回归模型会自然地学会近似卡尔曼滤波。具体而言，学习到的隐藏表征在相似变换下与最优滤波器产生的状态估计一致，尽管模型并不显式知晓潜在动力学。我们提供了关于预测误差、参数估计误差和潜状态恢复的有限样本保证。
- **PDF**: https://arxiv.org/pdf/2606.12691v1

--- 
## 📚 学科: `econ.*`
_本周缺少高价值论文_