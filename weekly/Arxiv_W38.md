# 🗓️ 周报 (2026-W38)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-09-20

--- 
## 📚 学科: `eess.*`
本期 `eess.*` 学科挑选了5篇高质量论文，涵盖了儿童生物特征识别、低资源语言口语问答、医学视频技能评估、脑部疾病医学影像分类以及控制系统线性算子学习等前沿方向。这些研究展现了电子与系统科学在结合深度学习、多模态处理和控制理论时的广泛应用。研究者们通过引入合成数据生成协议、超图注意力网络以及基座视频模型等手段，显著提升了系统在小样本、复杂结构及泛化场景下的表现。整体来看，本周论文强调了在医疗、语音及控制等垂直领域，利用结构化先验与先进表征模型提升鲁棒性与可解释性的技术趋势。

### Synthetic Fingerprints for Children Under Four: Generation and Biometric Evaluation
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.20621v1
- **作者**: Faheem Ahmad, Ajan Ahmed, Mst Rumana Sumi, Stephanie Schuckers, Masudul Imtiaz
- **备注**: Accepted at Ubiquitous Computing, Electronics, and Mobile Communication (UEMCON) 2026
- **摘要**: 4岁以下儿童的指纹识别对于长期身份应用具有重要意义，但该年龄段的研究受限于真实指纹数据的有限可用性和敏感性。如果对生成的样本在生物特征质量、与真实训练数据的相似性以及身份多样性方面进行仔细评估，合成数据可能提供有益的补充资源。本文提出了一种评估和筛选从小儿科数据集中生成的合成指纹的协议。该协议应用于由年龄条件生成器产生的32,000个候选样本，该生成器使用来自9名儿童的205个指纹进行微调。利用NFIQ 2、NBIS细节点提取与匹配、指纹模式分类、与完整真实参考集的相似性以及保留的合成样本之间的成对相似性对候选样本进行评估。在候选样本过滤和最终的对称成对验证后，保留了1,985个合成指纹。最年轻的年龄组在采样预算内继续产生保留样本，而最年长的原始年龄组产生了24个保留指纹。数据衍生双组年龄表征改善了年轻组的模式分布一致性。固定合成身份的重复渲染产生了与真实匹配分数相当的基于细节的匹配分数，尽管DINOv2纹理表征显示出明显更大的生成器内部相似性。结果表明，合成儿童指纹可以支持受控研究使用，但其评估应包括真实与合成的相似性以及合成与合成的多样性，且结论应保持针对所使用的匹配器和测量方法。
- **PDF**: https://arxiv.org/pdf/2609.20621v1

### VākQA: A Benchmark and Evaluation Study for Telugu Spoken Factoid Question Answering
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.19879v1
- **作者**: Bhavana Akkiraju, Ravi Sastry Kolluru, Sri Charan D, Srihari Bandarupalli, Santosh Kesiraju, Anil Vuppala
- **备注**: Paper is accepted in IEEE SLT 2026
- **摘要**: 随着大型语言模型的发展，问答技术取得了快速进步，但主要集中在高资源语言的文本和口语设置中。泰卢固语的口语问答（SQA）基准仍未得到探索，且在这种设置下自动评估的可靠性尚未被量化。我们推出了 VākQA，这是一个包含 2,001 个事实性问答对的泰卢固语 SQA 基准，涵盖六个领域，包含 2.53 小时的语音音频、双语转写和人工验证的参考答案。我们首先针对人类判断验证了评估方法：Gemini-as-a-judge 最接近人类评分，但其严格程度不均匀，而开源权重裁判则系统性地惩罚了表面形式与参考答案不同的正确泰卢固语回答。使用这一验证过的设置，我们对不同输入模态、语言和领域的开源和商业模型进行了基准测试。我们观察到，泰卢固语的措辞保留了在翻译中丢失的文化特异性，语音输入引入了改变问题含义的语音混淆，且级联的 ASR-MT 错误会进行渐进式累积。VākQA 已开源发布。
- **PDF**: https://arxiv.org/pdf/2609.19879v1

### Video Based Assessment of Surgical Skills Using Frozen Pretrained Video Foundation Models
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.19772v1
- **作者**: Sangrock Lee, FNU Rahul, Suvranu De
- **备注**: Accepted for publication in npj Digital Medicine
- **摘要**: 自动基于视频的手术技能评估已取得快速进展，但在未见过的受试者层面泛化到新学员的情况下，对连续标准化评分预测的严格评估仍然有限。我们引入了 VBA-Net+，这是一个仅使用视频的框架，它利用预训练的视频基座模型作为冻结的特征提取器，来进行腹腔镜手术基础（FLS）评分回归和通过/失败分类。我们在缝合和图案裁剪这两个 FLS 数据集上评估了 VideoPrism、V-JEPA2 和 VideoMAE v2，并以帧级 SimCLR 作为基线。我们在离线嵌入上训练了一个轻量级的全卷积头部，并在标准评估协议中使用留一受试者（LOUO）交叉验证进行了受试者级别的评估。对于连续评分预测，最佳表征在缝合上达到了 $R^2$=0.6367，在图案裁剪上达到了 0.9261。对于官方 FLS 阈值下的通过/失败分类，受试者工作特征曲线下面积（AUC）分别达到了 0.9073 和 0.9906。冻结视频编码器流水线的表现普遍优于帧级 SimCLR 流水线，尤其是在缝合方面，为仅基于视频的 FLS 评估提供了基准。
- **PDF**: https://arxiv.org/pdf/2609.19772v1

### HyperAMS-Net: Adaptive Multi-Scale Spatial Hypergraph Network for Brain Disorder Classification
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.19755v1
- **作者**: Proloy Kumar Mondal, Md Kamran Hussin Chowdhury, Hoi Leong Lee
- **备注**: Accepted at the 17th International Workshop on Machine Learning in Medical Imaging (MLMI 2026), held in conjunction with MICCAI 2026
- **摘要**: 针对神经影像数据对脑部疾病进行精确分类仍然具有挑战性，这是由于受试者之间存在显著的异质性，且功能连接和形态表征中存在复杂的长多尺度模式。为了应对这些挑战，我们提出了 HyperAMS-Net，这是一个深度学习框架，用于使用源自静息态功能核磁共振成像（rs-fMRI）或结构核磁共振成像（sMRI）的神经影像表征来进行脑部疾病分类。HyperAMS-Net 融合了自适应多尺度卷积、超图注意力、空间-通道注意力以及自适应特征融合。具体而言，自适应多尺度卷积可在多个感受野上学习数据驱动的权重，以捕获不同尺度上的互补模式。超图注意力通过节点-超边-节点消息传递来对学习到的特征表征之间的高阶依赖关系进行建模，而空间-通道注意力则增强了判别性特征的学习。自适应特征融合进一步聚合了跨并行网络分支的互补信息。HyperAMS-Net 在跨越不同脑部疾病的三个基准数据集上进行了评估：自闭症谱系障碍的 ABIDE、重度抑郁症的 REST-meta-MDD 和阿尔茨海默病的 ADNI，采用了 5 折分层交叉验证。HyperAMS-Net 在所有评估的数据集上均达到了最先进的性能，在对比方法中获得了最高的准确率和 AUC。消融实验进一步证明了每个提出组件的贡献，其中移除超图注意力时性能下降最为显著。
- **PDF**: https://arxiv.org/pdf/2609.19755v1

### Demystifying Linear Operator Learning for Control Systems
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.19428v1
- **作者**: Max Beier, Nicolas Hoischen, Sandra Hirche, Petar Bevanda
- **备注**: accepted to the 65th IEEE Conference on Decision and Control; authors' version
- **摘要**: 本文提出了一种从数据中学习控制系统线性算子的结构化方法。我们同时解决了该问题的结构和学习理论方面。为了推导结构性假设，我们建议使用成熟的发展方程（半）群框架，因为控制系统中的算子属于同种类型。此外，我们建议通过逆问题框架的视角来分析学习算法。这揭示了学习到的模型如何通过误差分解、收敛性保证和最佳正则化来依赖于数据，从而使我们能够比较现有方法并推导出具有证明优势的算法。为了获得这些结果，我们将范围限制在希尔伯特空间上的有界算子上。尽管这看起来可能具有局限性，但现有的方法通常隐含地做出这一假设以获得类似于矩阵的表示。我们通过推导时变系统的收敛估计器，展示了使用这些框架的强大功能。
- **PDF**: https://arxiv.org/pdf/2609.19428v1

--- 
## 📚 学科: `q-bio.*`
本期 `q-bio.*` 选取了3篇高质量论文，主要聚焦于将前沿算法与生物医学机制相结合。这些研究涵盖了：利用敏锐度感知最小化（SAM）提升拉曼光谱在细菌耐药性便携诊断中的泛化性；将经典物理别构模型（MWC）显式融入深度多模态网络，以实现受体构象解耦与高精度药物结合活性预测；以及结合多源医学先验知识增强电子健康病历（EHR）的可解释性，从而实现低算力的医院再入院率预测。这批论文充分展示了物理和临床知识引导的机器学习在提升生物信息学算法的泛化性、可解释性以及实际临床应用落地方面的巨大潜力。

### Sharpness-Aware Minimization (SAM) Improves Classification Accuracy of Bacterial Raman Spectral Data Enabling Portable Diagnostics
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.19453v1
- **作者**: Kaitlin Zareno, Jarett Dewbury, Siamak K. Sorooshyari, Hossein Mobahi, Loza F. Tadesse
- **备注**: Accepted for oral presentation at the ICLR 2024 Workshop on Practical ML for Low Resource Settings (PML4LRS)
- **摘要**: 到2050年，抗生素耐药性预计每年将夺走1000万人的生命，且资源有限的地区受到的影响最为严重。拉曼光谱是一种新型的病原体诊断方法，有望在几小时内完成快速且便携的抗生素耐药性测试，而使用金标准方法则需要几天时间。然而，目前的拉曼光谱分析算法存在以下局限：1）在不同患者群体的有限数据集上难以很好地泛化；2）由于需要非平凡的预处理步骤（如特征提取，这对于减轻拉曼光谱数据的低质量特性至关重要），从而导致复杂度增加。在这项工作中，我们通过使用敏锐度感知最小化（SAM）来解决这些局限性，以增强模型在临床细菌分离物分类任务中对各种超参数的泛化能力。我们证明，在光谱分类任务中，相比传统的优化器 Adam，SAM 在单次划分中实现了高达 10.5% 的准确率提升，并在所有划分的平均准确率上提升了 2.7%。这些结果展示了 SAM 推进人工智能辅助拉曼光谱工具在临床应用中的潜力。
- **PDF**: https://arxiv.org/pdf/2609.19453v1

### GPCR Ligand Bioactivity Prediction with Physics-Informed Dual-State Query Learning
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.16468v1
- **作者**: Shuo Zhang, Huifeng Zhang, Rongqi Hong, Jian K. Liu
- **备注**: Accepted by APBC2026
- **摘要**: 预测小分子针对G蛋白偶联受体（GPCRs）的生物活性特征是药物研发中的一个挑战。尽管深度学习加速了结合亲和力的预测，但由于忽略了动态构象平衡，现有方法往往难以区分功能效能。此外，基于结构的方法经常受到高分辨率激活态晶体结构稀缺以及静态表征中构象状态无法区分的限制。为了弥合黑箱预测与生物物理现实之间的差距，我们提出了双态查询（DSQ），这是一种物理启发的神经网络多模态架构，将 Monod-Wyman-Changeux (MWC) 别构效应模型显式嵌入其中。与依赖显式 3D 结构的传统模型不同，DSQ 利用可学习的正交查询来提取处于激活和未激活受体状态的解耦表征。这些潜在表征由一种新型的神经 MWC 门控模块控制，该模块从配体-状态亲和力与受体固有构象能量势垒之间的热力学竞争中，数学地推导出受体激活的概率。还引入了对比排序目标来施加差分亲和力约束，以确保物理一致性。广泛的实验表明，DSQ 优于其他基线模型，特别是在激动剂子集上。额外的同源性分层、温度敏感性、扰动、聚类和效率分析表明，DSQ 提供了有用的热力学归纳偏置，同时也暴露了其在低同源性受体上的明显局限。代码可在 https://github.com/jiankliu/DSQ 获取。
- **PDF**: https://arxiv.org/pdf/2609.16468v1

### Knowledge-Enriched Structured EHR Features for 30-Day Hospital Readmission Prediction on MIMIC-IV
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.15713v1
- **作者**: Mohamad Najafi, Hongyun Fu, Mathias Brochhausen, Jian Wu, Yaohang Li
- **备注**: 15 pages, 3 figures. Accepted at SDSC 2026 Mid-Atlantic
- **摘要**: 最近用于预测30天内医院再入院的方法主要依赖于应用于出院小结的预训练语言模型。尽管这些方法取得了强大的性能，但它们依赖于临床病历的可获得性，产生了巨大的计算成本，并且产生的表征缺乏可解释性。我们提出了一种富含知识的特征表征方法，该方法无需使用临床病历，即可通过四种医学知识源来增强结构化电子健康档案（EHR）数据，这四种来源包括：疾病本体映射、手术分类、药物成分词汇表和器官系统实验室指标聚合。每个特征维度对应一个命名的临床概念，从而产生稀疏且具有可解释性的患者表征。该方法在 MIMIC-IV v2.2 队列上使用六种分类器进行了评估。在 20 折交叉验证下，最佳配置达到了 0.743 的 AUROC。这一性能与之前在该数据集上报道的方法（包括仅使用结构化数据和引入临床病历的方法）相当，同时所需的计算成本要低得多。可解释性分析表明，人口学特征、器官系统实验室指标、药物成分特征和一级本体疾病类别主导了预测，而更深层次的层次结构贡献微乎其微。这些发现表明，在预测30天再入院时，富含知识的结构化特征为临床病历嵌入提供了一种具有竞争力和高效的替代方案。
- **PDF**: https://arxiv.org/pdf/2609.15713v1

--- 
## 📚 学科: `cs.*`
本期 `cs.*` 精选了3篇在 EMNLP 和 IEEE VIS 录用的高水平论文。研究内容涉及当前大模型和智能体系统的核心痛点。具体包括：提出了有状态检索增强生成框架 RAFT，解决了复杂故障排除智能体在多阶段任务中忽略上下文历史的问题；深刻揭示了 GPT 系列模型在安全对齐过程中存在的“伤害洗白”现象，指出传统毒性分类器无法有效识别被转换形式的隐性性别歧视；以及设计了解析动作图（Semantic Action Graph），搭建起生成式视频智能体与人类用户之间可解释、可引导的桥梁。这些成果不仅提升了具体任务的性能，更为评估 LLM 的安全性以及人机协同系统的交互设计提供了关键的方法论参考。

### RAFT: A Stateful Retrieval-Augmented Framework for Troubleshooting Agents
- **分数**: 6
- **链接**  https://arxiv.org/abs/2609.20754v1
- **作者**: Mingxuan Zhang, Xiaowen Wang, Anupma Sharan, Zhengyi Chen, Chenyu Diana Zhang, Shanshan Yang, Chittibabu Pacharu
- **备注**: Accepted to the EMNLP 2026 Industry Track
- **摘要**: 企业客户支持中高效的故障排除助手依赖于从相似的历史案例中检索可执行的指导，然而现有的检索增强生成（RAG）系统将支持案例视为静态文档，忽略了它们多阶段、有状态的本质。我们引入了 RAFT（有状态的故障排除助手检索增强框架），这是一种有状态的 RAG 框架，它将每个已关闭的历史案例抽象为时间线条目的有向链，并在条目级别进行检索，从而找出中间状态与当前活跃案例相匹配的历史案例，并返回锚定在匹配状态的父案例轨迹；一个可选的案例级图通过可配置的相似性表征将案例联系起来。我们直接对该检索层进行评估，这与评估整个智能体系统不同，无需生产部署。由于公开的多阶段故障排除数据极少，我们结合了基于微软 Learn Windows Server 文档构建的合成基准以及带有分析师创建的重复标记的真实 Apache Jira 问题。在案例进展的每个阶段，RAFT 在 Case Hit 指标上均优于传统 RAG 和 GraphRAG 基线，并且相比最强的基线具有统计学上的显著提升；Jira 的实验结果提供了方向性的证据，表明该优势可以转化到真实的案例历史中。我们发布了我们的基准、实现和 Apache Jira 评估集。
- **PDF**: https://arxiv.org/pdf/2609.20754v1

### Harm Laundering in GPT Models: Evidence That Gender Discrimination Is Transformed Rather Than Reduced Across Safety-Trained Generations
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.20779v1
- **作者**: Sarah Wyer, Sue Black, Noura Al Moubayed
- **备注**: Accepted at EMNLP 26 Main Conference
- **摘要**: 大语言模型的安全评估主要依赖于表面形式分类器，这些分类器报告随着模型世代更新，伤害评分有所下降。我们提供了这种评估方法在系统性上不完整的证据：显式的歧视性内容被转化而非消除。我们称之为“伤害洗白”（harm laundering）。通过分析从 GPT-2 到 GPT-5（OpenAI GPT 谱系，包含三种人口学条件）共 15 个模型中产生的 450,000 条针对性别的补全文本，我们展示了在 GPT-2 针对女性的输出中普遍存在的性暴力集群在 GPT-4 中消失了，而针对男性的补全则获得了女性补全所没有的正向表征领域（如照料、情感范围、盟友身份）。这一模式在 GPT-5 中最为明显：主题5（1,997篇文档）将乳腺癌框定为男性权利辩论，而在针对女性的输出中没有出现同等集群。三个独立的分类器将此类内容评分为无毒。情感评分在 GPT-4 处发生反转：早期的模型贬低女性，而后的模型过度修正。在 GPT-4 对齐边界处，针对女性补全的主题多样性相对于男性下降了 36%（女/男比例由 GPT-2 的 0.91 降至 0.58）。REGARD 表征伤害差异与发布日期呈正相关（$ρ= +0.55$, $p = .034$），而 Detoxify 评分则不相关（$ρ= -0.23$, $p = .42$）：随着表征伤害的增加，毒性得分反而在下降。我们将伤害洗白形式化为三准则测试，并提供了一个适用于任何生成模型的三阶段检测协议。在 OpenAI GPT 谱系中，毒性评分的降低并不是减少伤害的充分代表。
- **PDF**: https://arxiv.org/pdf/2609.20779v1

### Semantic Action Graph: A Shared Representation for Agent Grounding and Human Interpretation of Sports Highlights
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.20768v1
- **作者**: Tica Lin, Deepak Chandran, Gauri Jagatap, Chen Chen, Andrea Fanelli, David Gunawan, Josh Kimball
- **备注**: 5 pages, 3 figures, Accepted for publication at IEEE VIS 2026 Workshop on GenAI, Agents, and the Future of VIS
- **摘要**: 生成式智能体越来越多地被用于选择和讲述视频集锦，但它们通常运行在无结构或帧级别的表征上。因此，观众很难验证其输出，并针对个人偏好进行引导。我们提出了解析动作图（semantic action graph），这是一种轻量级的领域模式（schema），它将一场体育比赛表示为执行者、动作、接收者、时刻和状态节点，并通过角色、时间和结果边进行连接。该模式展示了三个关键属性：1）连接的事件序列，2）共享的闭环词汇表，以及3）帧寻址时刻。这使其适合同时服务于两个消费者：一个用于撰写叙述性集锦的智能体流水线，以及一个可供观众查询和检查相同结构的视觉界面。我们在 SportSAGE 中实例化了它，这是一个将四模块集锦流水线与图界面配对的设计探针，并报告了来自12名足球迷的反馈。参与者对生成的集锦和叙述质量表示满意，并使用图界面来搜索、导航和解读比赛集锦。这些结果提供了早期证据，表明一个精简的、人类可读的模式可以同时作为智能体生成的底层基础，并支持人类的理解。
- **PDF**: https://arxiv.org/pdf/2609.20768v1

--- 
## 📚 学科: `math.*`
_本周缺少高价值论文_

--- 
## 📚 学科: `astro-ph.*`
本期 `astro-ph.*` 精选了5篇高水平论文，涵盖了恒星演化、系外行星、中子星物理、空间等离子体及星际化学等天体物理学前沿方向。研究成果包括：利用 UKIRT 近红外成像构建了 M31 矮椭球星系中 TP-AGB 恒星的大样本目录，从而更精确地示踪中等年龄恒星形成历史；探讨了假定大气的气体成分对中子星 PSR J0740+6620 半径推断产生的系统误差，强调了贝叶斯证据在拟合优度中的重要作用；分析了帕克太阳探测器观测到的两个极近磁转弯（switchbacks）的微观等离子体差异；宣布利用 JWST 直系成像发现了一颗围绕年轻红矮星运行的低质量巨行星 RX J0534.0-0221 b 及其碎屑盘；以及利用 ALMA Band 6 数据对恒星形成区 G35.2N 中的醇-硫醇类似物进行了局部约束。

### A near-IR survey of luminous asymptotic giant branch stars in the satellites and stellar halo of M31
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.20810v1
- **作者**: Jess M. Howell, Annette M. N. Ferguson, Olivia C. Jones, Mike. J. Irwin, Maria-Rosa L. Cioni, Geraint F. Lewis, Nicolas. F. Martin, Alan. W. McConnachie
- **备注**: Accepted for publication in MNRAS; 19 pages, 11 figures
- **摘要**: 我们利用英国红外望远镜（UKIRT）3.8米望远镜上的宽野相机进行的近红外成像，对仙女座星系（M31）的矮椭球（dSph）卫星星系和恒星晕进行了研究。我们的同质化分析覆盖了12个矮椭球星系中的恒星范围，以及它们周围的晕场星族。我们利用色等图和双色图识别了富碳（C）和富氧（M）的热脉冲渐近巨星支恒星（TP-AGBs），这也能有效剔除污染源。在12个矮椭球星系中的8个星系中检测到了 TP-AGB 恒星，这表明在相当比例的样本中存在少量中等年龄的星族；在 M31 的大部分恒星晕中也发现了大量的这类恒星。通过将 316 个新探测到的源与文献中先前报道的源的修正分类相结合，我们将矮椭球星系中的 TP-AGB 候选星族从 82 个增加到了 359 个。我们利用得到的矮椭球和星晕 AGB 样本计算了 C/M 比例，并推断了矮椭球以及具有非零 AGB 计数且相邻的星晕场的金属丰度。在 M31 的恒星晕中，向外延伸至约 150 kpc 处观察到明显的金属丰度梯度，这与其他示踪剂得出的结果一致。利用主序折点光度法测得的文献恒星形成历史，我们发现矮椭球星系中碳星的数量与过去 0.5-3 Gyr 内形成的恒星质量之间存在紧密的关联。这项研究强调了 AGB 恒星作为中等年龄恒星形成的定量示踪剂的前景，特别是在本征暗弱的系统中，并提供了一个供后续跟进观测的候选 TP-AGB 恒星目录。
- **PDF**: https://arxiv.org/pdf/2609.20810v1

### Systematic Effects of Hydrogen and Helium Atmosphere Mismatch on Radius Inference in PSR~J0740+6620-like Synthetic NICER Data
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.20795v1
- **作者**: Isiah M. Holt, M. Coleman Miller, Alexander J. Dittmann, Frederick K. Lamb
- **备注**: 23 pages, 10 figures, 6 tables. Accepted to ApJ
- **摘要**: 中子星半径的约束为深入了解其内部冷而致密物质的性质提供了线索。先前使用合成中子星内部成分探测器（NICER）脉冲波形数据的研究表明，从中推导出的半径推断对于几类建模系统误差具有鲁棒性。在这里，我们利用基于类似 $\sim 2.1~M_\odot$ 的脉冲星 PSR~J0740$+$6620 的合成数据，探索了假定错误的空气成分所带来的后果。我们发现，当合成数据假定为氦大气而实际假定为氢大气（反之亦然）时，在实际 PSR~J0740$+$6620 数据的斑点与背景比例下，对推断半径产生的偏差很小。然而，当我们将斑点与背景的比例提高约20倍，同时保持总计数固定在观测到的 $\sim 5.5\times 10^5$ 时，我们发现大气成分失配会产生显著偏差的半径估计，同时这种偏差依然会隐藏在统计学上可接受的拟合残差中。即使在这些情况下，贝叶斯证据也能一致地识别出正确的大气模型。我们的发现强调了使用贝叶斯证据进行模型比较和拟合优度检验的重要性。
- **PDF**: https://arxiv.org/pdf/2609.20795v1

### Microphysical Diversity in Two Very Closely Spaced Magnetic Switchbacks Observed by Parker Solar Probe
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.20760v1
- **作者**: Dipali Vadher, Ankush Bhaskar, Smitha Thampi, Kamlesh Pathak
- **备注**: 26 pages, 9 figures, 1 table. Accepted for publication in Physical Review D
- **摘要**: 帕克太阳探测器（PSP）在太阳附近的观测揭示了被称为“磁转弯”（switchbacks, SBs）的频繁且突然的磁场反转。尽管它们无处不在，但在 SBs 内部的等离子体结构和相关加热现象仍未得到充分理解。我们展示了一个针对 2020 年 1 月 24 日观测到的两个距离极近的磁转弯（文中简称为 SB_1 和 SB_2）的案例研究，研究中采用了高频磁场和等离子体测量。磁场涨落被分解为平行和垂直于平均场的两个分量，并通过分析它们的功率谱来表征湍流级联。应用增量偏方差（PVI）方法来识别间歇性的类电流片结构。两个 SB 间隔均表现出明显的阿尔芬特性和增强的径向流；然而，它们的微观物理过程存在差异：与 SB_2 相比，SB_1 表现出更高的质子温度、更大的涨落幅度以及更密集的电流片分布。这两个事件在谱指数方面也有所不同，SB_1 比 SB_2 表现出更陡峭的垂直斜率。SB_1 中升高的间歇性、质子温度以及瞬态的 $β> 1$ 偏移表明，小尺度结构上的局域耗散是观测到的加热现象的合理驱动因素。这些发现表明，磁转弯不仅是统一的运动学偏转，更是动态演化的等离子体结构，其内部湍流可能会调节局域能量转换，并对近太阳太阳风的空间间歇性加热做出贡献。
- **PDF**: https://arxiv.org/pdf/2609.20760v1

### The JWST Sub-Jupiters Survey: Direct Imaging Discovery of a Giant Planet and a Debris Disk Around the Young M-dwarf RX J0534.0-0221
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.20748v1
- **作者**: Rodrigo Ferrer-Chavez, Jason J. Wang, Kevin Wagner, Kellen Lawson, Aarynn L. Carter, Beth Biller, Raphael Bendahan-West, Patrick McCreery, Patricia Luppe, Steve Ertel, Andrew D. James, Ellis Bogat, Rohan Kane, Ben J. Sutlieff, Giovanni M. Strampelli, William O. Balmer, Rachel Bowens-Rubin, Evelyn L. Bruinsma, Andy Skemer, Julien H. Girard, Mark Booth, Klaus Subbotina Stephenson, Katie A. Crotts, Sebastian Marino, Aniket Sanghi, Michael Liu, Nour Skaf, Emily Rickman, Marshall D. Perrin, Laurent Pueyo, Brendan P. Bowler, James Mang, Isabel Rebollido, Michael Meyer, Tim Pearce, Markus Bonse, Clémence Fontanive, Jared Carlson, Jon Rees, Justin Rupert, Gabriel Weible, Jacob Isbell, Juan Carlos Guerra, Xueqing Chen, Mia Belle Parkinson, Vito Squicciarini, Gael Chauvin, Elisabeth Matthews, Kyle Franson, Maxwell A. Millar-Blanchaer
- **备注**: 32 pages, 12 figures. Accepted for publication at ApJL
- **摘要**: 我们宣布发现了 RX J0534.0-0221 b，这是一颗绕着绘架座 $β$ 移动星群中的红矮星（M-dwarf）运行的巨行星。RX J0534 最初是由詹姆斯·韦布空间望远镜（JWST/NIRCam）通过 F444W 和 F200W 滤光片进行观测的。在 F444W 下的观测显示，在距离主星约 0.41 角秒（约 14 au）处存在一个信噪比为 $\sim17.5$ 的点源，而在 F200W 下则未检测到该源。利用大双筒望远镜干涉仪（LBTI/LMIRCam）在 $L'$ 波段进行的后续观测，在 JWST 观测纪元 16 个月后重新检测到了该源，从而为共行自行动作（而非与背景干扰源的偶发对齐）提供了 6-7$\sigma$ 级别的证据。对现有光度学数据的大气网格模型拟合得出了玻色度光度 log$_{10}(L/L_\odot) = -5.48^{+0.10}_{-0.19}$ dex。在 18-26 Myr 的年龄下，热启动演化模型预测其质量为 $M=2.8^{+0.5}_{-0.5}$ M$_{\text{Jup}}$，有效温度 $T_{\text{eff}}=674^{+57}_{-49}$ K。从 $L'-F444W$ 的颜色和星等中，我们发现了该行星大气中存在非平衡化学或金属丰度增强的证据。此外，在 JWST F200W 观测中还检测到了一个延伸结构，这与一个峰值密度半径为 $79^{+3}_{-3}$ au、倾角为 $56.5^{+1.5}_{-1.5}$ 度的被解析碎屑盘相吻合。RX J0534 b 是迄今为止成像的质量最低的行星之一。继 TWA 7 b 之后，它是第二颗成像的、在太阳系尺度（首颗在 50 au 以内）轨道上绕红矮星运行的行星，并且是首颗通过共行运动确认的行星。未来的轨道监测和大气表征将揭示其形成历史，鉴于在红矮星周围形成巨行星极具挑战性，这成为了一个特别有趣的科学问题。
- **PDF**: https://arxiv.org/pdf/2609.20748v1

### Local constraints on alcohol--thioalcohol analogs in G35.2N
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.20671v1
- **作者**: Xuefang Xu, Shanghuo Li, Qian Gou, Chunguo Duan, Laurent Pagani, Di Li, Jun Kang, Jiaxin Du, Jiaxiang Jiao
- **备注**: 8 pages, 9 figures, 6 tables, published in A&A
- **摘要**: 在致密的恒星形成环境中，含硫复杂有机分子的化学机制仍不确定，部分原因在于致密气体和冰中主要的硫储藏库仍未被明确识别。醇-硫醇对可以对结构相关的含氧和含硫分子进行直接对比。我们展示了在 G35.2N 的 MM3-MM5 区域内的三个光谱提取位置（MM3-pos、MM4-pos 和 MM5-pos），利用 ALMA Band 6 观测到的 CH$_3$OH/CH$_3$SH 和 C$_2$H$_5$OH/C$_2$H$_5$SH。局部热力学平衡模型给出了柱密度和丰度比。为了减轻光深度效应，CH$_3$OH 的柱密度是从 $^{13}$CH$_3$OH 推导出来的（假设 $^{12}$C/$^{13}$C = 50）。在所有三个位置，CH$_3$OH、CH$_3$SH 和 C$_2$H$_5$OH 均得到了可靠的约束；C$_2$H$_5$SH 在 MM3-pos 和 MM5-pos 处得到了可靠约束，但在 MM4-pos 处仍为暂定。采用的相应柱密度范围为 $(1.8-2.7)\times10^{18}$、$(1.7-2.6)\times10^{16}$、$(5.7-8.5)\times10^{16}$ 和 $(2.4-4.6)\times10^{15}$ cm$^{-2}$。在误差范围内，不同位置的 CH$_3$OH/C$_2$H$_5$OH 和 CH$_3$OH/CH$_3$SH 比例是一致的，标称值分别为 31-32 和 100-110。与化学物质丰富的源以及升温化学模型的对比表明，CH$_3$OH/C$_2$H$_5$OH 落在在其他地方测得的范围内，而 CH$_3$OH/CH$_3$SH 则表现出更大的源间差异。由于文献中许多 C$_2$H$_5$SH 的测量仅提供了下限，乙基水平的 O/S 对比仍然不太确定。因此，在这些数据中，CH$_3$OH/CH$_3$SH 是受约束最好的 O/S 醇-硫醇比率，并为研究源相关的含硫有机化学提供了实证探测手段。需要更灵敏的 C$_2$H$_5$SH 观测来检验 C$_2$H$_5$OH/C$_2$H$_5$SH。
- **PDF**: https://arxiv.org/pdf/2609.20671v1

--- 
## 📚 学科: `stat.*`
本期 `stat.*` 收录了2篇统计学前沿论文，分别关注因果图结构的学习理论和应用于光谱生物数据的优化算法。第一篇论文解决了混合数据集（如含有序变量、计数和连续变量）中因果发现的识别难题，将有序-泊松结果推广到了通用的单参数指数族分布，并给出了实用的优化算法。第二篇论文探讨了在样本量小且信噪比低的复杂医学光谱分类任务中，如何利用敏锐度感知最小化（SAM）算法优化超参数，进而显著提升对临床细菌药敏测试的分类准确性。两篇研究结合了扎实的理论推导和应用实践，为解决现实高维混合数据分析以及生物统计诊断提供了强大的数学工具。

### Epidemiological Causal Graph Identification: Challenges, Identifiability and Algorithms
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.20676v1
- **作者**: Sambit Mishra, Yingying Wang, Christine K. Johnson, Urbashi Mitra
- **备注**: 5 pages, 2 figures, accepted at the 60th Asilomar Conference on Signals, Systems, and Computers 2026
- **摘要**: 从观测数据中进行因果发现是统计学和机器学习的基础，但在没有干预的情况下确定因果方向需要结构性假设。现有的可识别性研究主要集中在加性噪声模型下的连续变量，往往忽略了包含有序尺度、计数和连续测量的混合数据集。本文研究了在有向无环图（DAGs）中的因果发现，其中节点遵循有序分布（通过有序 logit 模型）或常规的单参数指数族分布。我们证明了有序节点与指数族节点之间的边缘方向对于通用参数值是分布可识别的。我们的发现将先前的“有序-泊松”结果推广到了更广泛的指数族。在计算上，我们引入了一种基于评分的穷举搜索，以及一个针对较大图使用 DAGMA 的掩码连续优化框架。数值实验验证了该理论，恢复了在经典结构方程模型下无法识别的马尔可夫等价类中的边缘方向。
- **PDF**: https://arxiv.org/pdf/2609.20676v1

### Sharpness-Aware Minimization (SAM) Improves Classification Accuracy of Bacterial Raman Spectral Data Enabling Portable Diagnostics
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.19453v1
- **作者**: Kaitlin Zareno, Jarett Dewbury, Siamak K. Sorooshyari, Hossein Mobahi, Loza F. Tadesse
- **备注**: Accepted for oral presentation at the ICLR 2024 Workshop on Practical ML for Low Resource Settings (PML4LRS)
- **摘要**: 到2050年，抗生素耐药性预计每年将夺走1000万人的生命，且资源有限的地区受到的影响最为严重。拉曼光谱是一种新型的病原体诊断方法，有望在几小时内完成快速且便携的抗生素耐药性测试，而使用金标准方法则需要几天时间。然而，目前的拉曼光谱分析算法存在以下局限：1）在不同患者群体的有限数据集上难以很好地泛化；2）由于需要非平凡的预处理步骤（如特征提取，这对于减轻拉曼光谱数据的低质量特性至关重要），从而导致复杂度增加。在这项工作中，我们通过使用敏锐度感知最小化（SAM）来解决这些局限性，以增强模型在临床细菌分离物分类任务中对各种超参数的泛化能力。我们证明，在光谱分类任务中，相比传统的优化器 Adam，SAM 在单次划分中实现了高达 10.5% 的准确率提升，并在所有划分的平均准确率上提升了 2.7%。这些结果展示了 SAM 推进人工智能辅助拉曼光谱工具在临床应用中的潜力。
- **PDF**: https://arxiv.org/pdf/2609.19453v1

--- 
## 📚 学科: `econ.*`
本期 `econ.*` 选入了一篇发表于运筹学顶刊《Operations Research数学基础》（MOR）的开创性论文。该研究首次将属性测试（property testing）引入博弈论机制设计领域，系统地探讨了如何高效地检测单参数分配机制是否具备“激励相容性”（IC）。通过把经济学中的机制设计与理论计算机科学中的布尔函数单调性测试结合，作者设计出了近乎最优的单调性测试算法（查询复杂度为 $\tilde{O}(n/ε)$），并证明了匹配的下界。该成果不仅解决了多博弈者机制设计在实际复杂应用中难以检测合规性的技术痛点，也为微观经济学与博弈论机制的算法化设计、定价规则评估和合规性验证开辟了全新的跨学科方向。

### On testing the incentive compatibility of single-parameter allocation mechanisms
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.17406v1
- **作者**: Jason Milionis, William Pires
- **备注**: 42 pages, accepted at journal of Mathematics of Operations Research
- **摘要**: 本文是博弈论与属性测试交叉领域的首项工作，给出了用于高效测试分配机制是否满足激励相容性（IC）的算法 and 下界。我们提出去区分一个机制是否“远离”IC（即当观察到许多单调性“违规”时）。在概念上，受到布尔函数单调性测试文献的启发，我们为离散单参数分配规则构建了一个测试器。在技术上，我们的工作是首次考虑超网格上向量值函数的单调性测试。我们给出了一个查询复杂度为 $\tilde{O}(n/ε)$ 的算法，用于测试一个函数（代表含有n个博弈者的分配机制）是坐标单调的，还是远离单调的。我们还展示了一个匹配的下界：在布尔超立方体或超网格上，坐标单调的向量值函数类需要 $\tildeΩ(n/ε)$ 次查询才能测试其是否远离单调性，即使测试器是双侧的且允许进行自适应查询，该结论依然成立。最后，我们将我们的上界推广到了分配机制的定价函数，并给出了具有相同查询复杂度的测试器。这需要克服一个技术挑战，即函数空间中通往最近 IC 机制的路径可能涉及到对价格和分配规则两者的相互依赖性改变。
- **PDF**: https://arxiv.org/pdf/2609.17406v1

---