# 🗓️ 周报 (2026-W42)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-10-18

--- 
## 📚 学科: `eess.*`
本周 EESS 学科论文涵盖电池健康预测、传感器故障诊断、多智能体协同控制与无线通信波束跟踪。亮点论文包括发表于 NeurIPS 2026 的 NOCE-Net，提出了用于电池运行上下文的嵌套序列学习架构；以及利用 Reachability-CBF 实现高可靠通信与碰撞预防的多智能体追逐控制算法。此外，针对柴油机排放诊断与毫米波自适应波束选择的研究也展示了数据驱动与控制理论在工程应用中的深度融合。

### NOCE-Net: Representation Learning for Battery Operational Context via Nested Sequence Modelling
- **分数**: 7
- **链接**  https://arxiv.org/abs/2610.21391v1
- **作者**: Arnab Bhattacharjee, Wayes Tushar, Tapan Kumar Saha
- **备注**: 38 pages, Accepted in NeurIPS 2026
- **摘要**: 从电池运行历史中学习有效的特征表示对于预测性健康管理和面向控制的应用至关重要。现有方法依赖于基于响应的手工工程特征或早期短生命周期窗口，这限制了泛化能力，并排除了无法获取未来响应的前瞻性场景。我们提出了 NOCE-Net，一种深层嵌套序列模型，可直接从原始循环运行或遥测数据中学习支持控制的特征表示。我们的数据流水线 re-BatteryData 将异构老化数据集标准化为由绝对充电吞吐量定义的语义等效的全等效循环（FEC），从而实现在多样化运行模式下的端到端学习。NOCE-Net 结合了用于循环内动态的多 Patch Transformer 编码器和用于循环间状态演化的 GRU 骨干网络，在跨越 300 多个运行模式的 10 个公开数据集中的约 700 个电池上运行。在针对未见过的电池化学性质和使用模式的零样本评估中，NOCE-Net 在电压响应预测中实现了 13.7% 的 MAPE，在减少 40 倍参数的同时，性能超越强长序列基线 43% 以上。对所学隐藏状态的形状和组件诊断表明，GRU 的主要演化方向与所有具有单调衰减特性的数据集（包括零样本测试电池）的容量衰减轨迹达到了平均 Spearman $|ρ| \ge 0.95$，证明了该特征表示编码了可迁移至电池响应建模之外的下游任务的衰减动态。代码开源于 https://github.com/BeArnab96/NOCE-Net 。
- **PDF**: https://arxiv.org/pdf/2610.21391v1

### Sensor Diagnosis for Fuel and Emissions Monitoring in Heavy-Duty Diesel Vehicles
- **分数**: 6
- **链接**  https://arxiv.org/abs/2610.21188v1
- **作者**: Tejas Dahiya, Saurabh Kumar Gupta
- **备注**: Accepted at the Tackling Climate Change with Machine Learning workshop at NeurIPS 2026
- **摘要**: 故障传感器读数会扭曲柴油发动机的燃料消耗和二氧化碳排放估计。我们评估了两种利用从健康测量中学习到的关系来诊断故障并指导燃料修正的方法。诊断过程测试用估计的健康值替换可疑的故障读数是否有助于模型更准确地预测另一个传感器记录的读数，然后预测故障类型并决定是否报告诊断结果。我们在来自重型柴油发动机的 217 个稳态运行点上评估了五种合成故障类型，在训练中排除了选定发动机转速下的所有测量。在 31500 个注入故障的组中，它为 77.3% 的组发布了诊断，其中发布的诊断准确率达到 92.1%。燃料修正过程在单个运行点使用不同的传感器选择规则，测试每次替换如何改变所有六个传感器上的最大预测误差。燃料修正需要故障报警以及接近训练条件的发动机转速和扭矩。仅当替换某个燃料读数能够比替换其他传感器更充分地降低最大预测误差时，才会替换该读数。在假定 1% 的一小时场景存在故障、传感器和故障类型概率均等以及每个测量条件时间相等的情况下，选定的燃料修正使计算出的燃烧 CO2 平均绝对误差降低了 83.8%。在这个发动机图谱上，学到的关系支持完整的传感器诊断和燃料修正，改善了排放核算，同时保留了不受影响的读数。
- **PDF**: https://arxiv.org/pdf/2610.21188v1

### Robust Multi-Agent Pursuit with Preemptive Communication via Reachability-Based Control Barrier Functions
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.22198v1
- **作者**: Madison Book, Justin Bradley
- **备注**: 6 pages, 4 figures. Accepted to the 2026 IEEE Conference on Decision and Control (CDC)
- **摘要**: 安全的多智能体协调通常假设受资源约束的真实机器人所无法提供的条件：持续且完美的受限状态共享。稳健的控制策略必须与稳健的通信策略相结合，以实现具备韧性的部署。在本文中，我们提出了一种统一的控制/通信策略，该策略提供安全控制以保证间歇通信下智能体间的安全性，并在追逐-逃逸场景中验证了其有效性。每个智能体根据最后接收到的状态信息计算相邻智能体的可达集，然后基于控制障碍函数（CBF）求解安全控制输入以确保智能体避免碰撞。我们证明了只要通信陈旧度保持有界，智能体间的碰撞避免就能得到保证。随着状态传输之间可达集的膨胀，每个智能体根据表征不确定性风险和运动学风险的新颖指标，推理何时预先向相邻智能体传输其状态信息。我们实现并仿真了多种追逐-逃逸场景，结果表明，与周期性和事件触发基线相比，预先通信在保持零碰撞的同时将消息数量减少了 77.5%。
- **PDF**: https://arxiv.org/pdf/2610.22198v1

### Confidence-Guided Adaptive Beam Selection for Vision-Aided Beam Tracking in mmWave Systems
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.21880v1
- **作者**: Sohani Munteha Hiam, Mohammad Soleymani, Rafael F. Schaefer
- **备注**: Accepted at IEEE Communications Letter
- **摘要**: 毫米波系统中的视觉辅助波束跟踪通过从摄像头观测中预测波束索引来降低波束训练开销。然而，固定 Top-$K$ 选择为所有预测分配相同的候选波束预算，忽视了不同样本和预测时界之间的不确定性变化。本文提出了基于置信度引导的自适应候选波束选择方法：对预测器的 Logits 进行温度校准，在最大预算约束下保留累积概率达到目标阈值的最小顶级波束集合。在 DeepSense 6G 场景 8 上，在 5 个随机种子和相同开销条件下，该策略在无需重新训练预测器的情况下，将候选集准确率提升了最多 3.80 个百分点，归一化接收功率提升了 0.32 个百分点，并将中断概率降低了 2.06 个百分点。
- **PDF**: https://arxiv.org/pdf/2610.21880v1

--- 
## 📚 学科: `q-bio.*`
本周 q-bio 学科关注生成式 AI 在科学预测中的局限性与具身认知建模。研究通过流匹配（Flow-matching）模型探讨了在生理与生物分子数据中未见非加性科学效应的恢复与“幻觉”现象，揭示了条件生成模型外推的边界；另一项研究则基于主动推断（Active Inference）框架，解耦了具身智能体应对身体紧急需求时的信息精准度提高与偏好重置机制，为理解认知与生物体生存策略提供了新视角。

### Predicting Unseen Scientific Interactions: Conditional Flow Models Hallucinate Non-Additive Effects
- **分数**: 6
- **链接**  https://arxiv.org/abs/2610.20288v1
- **作者**: Sam Gijsen, Moritz Seiler, Kerstin Ritter
- **备注**: Accepted as an oral at NeurIPS 2026 Workshop: AI Data Readiness for Scientific Discovery (AIDaR). Code: https://github.com/SamGijsen/interaction-flows
- **摘要**: 条件生成模型越来越多地被用于超出直接训练支持范围的科学预测。然而，科学问题往往关注一种干预是否会改变另一种干预的效果。这种相互作用（交互作用）可能是主要研究兴趣所在，但可能仅能解释总变化中的极少部分，从而使模型在未还原相关科学效应的情况下看似整体准确。目前尚不清楚这些模型如何学习相互作用以及它们何时能成功推断至未见条件。因此，我们利用生理时间序列模拟器、药物剂量-响应数据、组合细胞扰动和分子构象生成，研究了流匹配（Flow-Matching）模型中的相互作用恢复问题，并将真实的恢复与幻觉出的相互作用结构区分开来。在受控设置下，模型对个体效应的学习远早于相互作用，并且模型会在不存在相互作用的地方产生幻觉。在不同设置下，我们发现了质地不同的泛化问题，成功预测取决于条件结构是否从已观测目标延续至留出目标。当结构延续时，相互作用是可恢复的；反之，模型可能会生成合理的响应但遗漏相互作用。此外，我们发现随着目标可识别性降低，幻觉会增加，且在非线性读取下输出空间中的成功相互作用恢复可能会失效。最后，我们表明聚合保真度指标可能会掩盖模型是否真正学习并推断了相互作用。
- **PDF**: https://arxiv.org/pdf/2610.20288v1

### Two Routes to Interoceptive Prioritisation: Dissociating Likelihood Precision and Preference Reweighting in Active Inference
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.18617v1
- **作者**: St John Grimbly, Nicolas Kuske, Evert A. Boonstra, Charel van Hoof, Rowan Hodson, Benjamin Rosman, Ryan Smith, Mark Solms, Jonathan P. Shock
- **备注**: Accepted at IWAI 2026, forthcoming in the Springer proceedings. 17 pages: the 13-page camera-ready paper, reproduced without alteration apart from one typographical fix, followed by 4 pages of supplementary material. Code: https://github.com/sgrimbly/interoceptive-prioritisation-iwai2026-snapshot
- **摘要**: 具身智能体必须在相互竞争的身体需求之间确定优先级。在主动推断（Active Inference）框架中，智能体可以通过提高关于紧急需求的信息精准度，或者通过增加对缓解该需求结果的偏好来响应紧急需求。我们在一个具有三种致命需求的搜粮网格世界中，分别及联合比较了这两种干预措施，并探讨了它们如何改变智能体的生存率、感知以及所学习的身体模型。精确度提高了内感受后验分布的锐度并提升了生存率。偏好重置使得身体状态远离致命边界，并改变了智能体从中进行学习的状态，因此其学到的模型覆盖的需求层级更少，在所有层级上的质量较低，但在其访问的层级上质量略高。在另外 72 种布局上的实验未能建立对困难布局预期的偏好收益，但两种干预措施都提高了平均生存率，且它们的交互作用为正。因此，仅凭生存率无法完整说明模型如何优先处理需求并学习其身体状态。
- **PDF**: https://arxiv.org/pdf/2610.18617v1

--- 
## 📚 学科: `cs.*`
本周 CS 学科聚焦生成式 AI 效率优化、具身智能基准、世界模型验证及数据管理。重点论文包括 NeurIPS 2026 接收的 DaTMe（基于扩散动态的高效图像生成 Token 合并框架）、LIBERO-PeRM（具身机器人个性化操作偏好学习基准）和 OmniVerifier-C1（用于规则驱动世界建模的二元与连续分级验证器）。此外，论文还涉及视觉故事讲述中的跨上下文一致性控制，以及数据库中轨迹数据的高效基数估计。

### Which Tokens to Merge? Diffusion Dynamics for Efficient Image Generation
- **分数**: 7
- **链接**  https://arxiv.org/abs/2610.22370v1
- **作者**: SeungJu Cha, Ye-Chan Kim, HyunGee Kim, Sungho Koh, Dong-Jin Kim
- **备注**: Accepted at NeurIPS 2026. Code: https://github.com/SeungJuCha/DaTMe
- **摘要**: Token 合并已成为一种有效的免训练策略，通过减少冗余 Token 计算同时最大程度减少生成质量下降来加速扩散模型。一个核心挑战是确定哪些 Token 可以安全合并，哪些应该被保留用于后续计算。现有方法通过保留与提示词对齐的前景区域来解决这个问题，从而保护语义相关的结构。然而，这种文本相关性标准忽略了背景物体以及提示中未明确提及的局部细节，从而导致结构一致性下降。在这项工作中，我们提出了动态感知 Token 合并（DaTMe），一种将 Token 合并建立在底层扩散动态基础上的免训练框架。我们的核心洞察是，Token 的重要性应该反映该 Token 在去噪过程中是否仍未解决以及它是否包含结构信息。为此，DaTMe 从 Tweedie 去噪估计中构建了一个动态感知的重要性图。该图将测量预测清晰图像跨步骤变化的实时时间信号与捕获局部高频内容（如边界和精细细节）的结构信号结合起来。利用该图，DaTMe 在给定的压缩率下自适应地将 Token 分配到合并角色中：重要 Token 作为锚点被保留，而时间和结构上均稳定的 Token 被选为安全合并候选者。在 PixArt-a 和 FLUX 上的实验表明，DaTMe 在整个图像中维持了视觉保真度，突显了扩散动态作为高效生成中有效的 Token 级别合并决策依据。代码开源于 https://github.com/SeungJuCha/DaTMe 。
- **PDF**: https://arxiv.org/pdf/2610.22370v1

### LIBERO-PeRM: Benchmarking Personalized Robotic Manipulation
- **分数**: 5
- **链接**  https://arxiv.org/abs/2610.22372v1
- **作者**: Zhixu Li, Keqian Tang, Litian Gong, Jingyu Yao, Wenqian Zhang, Tianze Xu, Zehao Wang, Yuping Wang, Junge Zhang, Jiachen Li
- **备注**: Conference on Neural Information Processing Systems (NeurIPS 2026); Project Website: https://libero-perm.github.io/
- **摘要**: 个性化是通用机器人进入家庭环境并实现真正实用性的关键。尽管通用机器人操控已被广泛研究，但个性化机器人操控（PeRM）缺乏一个用于解耦任务完成与偏好满足的受控基准。我们引入了 LIBERO-PeRM，这是一个用于具身智能体偏好学习的基准测试。LIBERO-PeRM 研究了五个问题：1) 策略在零样本设定下如何遵循偏好；2) 它们如何从演示中学习单一偏好；3) 随着演示的增加，它们获取偏好的效率如何；4) 学到的偏好如何在不同布局和任务之间泛化；5) 策略如何组合偏好以及在冲突下的行为。我们在仿真中提出了可观测偏好的受控形式化和分类法，涵盖运动、技能和用户属性选择。该形式化仅限于可在 LIBERO 中实例化而不改变任务目标、可自动评估且跨任务复用的语言可表达偏好。基于 LIBERO，我们的程序化流水线生成了包含和不包含偏好的成对演示。我们创建了五个任务套件（312 个任务），附带高质量演示、丰富元数据和偏好满足度指标。实验表明，当前的 VLA 策略在零样本个性化方面面临挑战，而 SFT 使偏好具备可学习性。混合训练比顺序适配具有更好的无偏好保持效果，并比仅偏好训练提升了上下文提示性能；但偏好泛化、分解与冲突处理仍具挑战。代码和数据集见项目主页：https://libero-perm.github.io/ 。
- **PDF**: https://arxiv.org/pdf/2610.22372v1

### OmniVerifier-C1: Decomposed Graded Verifier for Rule-Governed Generative World Modeling
- **分数**: 4
- **链接**  https://arxiv.org/abs/2610.22355v1
- **作者**: Bowei Liu, Xinchen Zhang, Xuhuan Li, Tianlin Zhang, Kaian Jiang, Jingwei Liu, Congyang Zhao, Yifei Qian, Junhong Liu, Zhiheng Li, Yujiu Yang, Yang Cai, Ling Yang
- **备注**: NeurIPS 2026. Project: https://github.com/Cominclip/OmniVerifier
- **摘要**: 生成式视觉验证器在推进多模态智能方面发挥着关键作用。为了增强视觉验证器在涉及组合要求的复杂多模态场景中的鲁棒性，我们超越了仅产生 True/False 离散判断的传统二元验证器，引入了一种自动将复杂提示或环境规则分解为细粒度组件并赋予逐点打分以提供连续且包含更多信息批判信号的验证器。我们的实验进一步证明，这些结构化且可解释的输出提高了验证器对域外多模态批判任务的泛化能力。为了训练该验证器，我们引入了解耦 RL 训练策略，利用精确的局部反馈共同优化子问题级二元判断和全局对齐打分，以开发细粒度的验证能力，为全局层面的可靠连续打分奠定基础。在通用强化学习框架下，我们首先从实证上证明了所提出的逐点分级验证器在传统文本到图像场景中显著优于二元验证器。随后我们将研究扩展到规则驱动的生成式世界建模。从理论角度看，当存在真实参考图像时，成对验证范式能比逐点形式化产生更准确的评价，在 Maze 和 Sudoku 等多样化结构化世界建模任务上的实证结果进一步验证了该方法的有效性。总体而言，我们的发现表明了一个关键洞察：从生成模型向结构化世界建模智能体的演进，关键取决于准确的成对分级视觉验证器的可用性。
- **PDF**: https://arxiv.org/pdf/2610.22355v1

### Not Just a Subject: Capturing Adaptive Scene-Specific Variance for Visual Storytelling
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.22320v1
- **作者**: SeungJu Cha, Ye-Chan Kim, Kwanyoung Lee, Dong-Jin Kim
- **备注**: Accepted at ACCV 2026. Code: https://github.com/SeungJuCha/EOS-Story
- **摘要**: 扩散模型的最新进展显著改善了文本到图像的生成，使其能够应用于视觉故事讲述（Visual Storytelling），即从叙事提示中生成连贯的图像序列。然而，现有方法主要关注身份保持（Identity Preservation），通常无法适应多样的场景变化，导致语义错位和结构缺乏灵活性。我们提出了 EOS-Story，这是一个免训练框架，在文本和视觉空间中协调了身份一致性与特定场景的自适应。在文本空间中，我们将叙事解耦为身份和场景子提示以防止信息稀释，但这使得场景无法获得外观线索。为了填补这一空白，我们引入了跨上下文桥接（Cross-Contextual Bridging），它将短语级别的外观残差软注入到场景的 `<EOS>` 嵌入中。在视觉空间中，我们发现身份主体和场景主体之间的尺度不匹配会导致少数身份 Token 被重复传输，从而产生结构伪影。我们通过自适应身份保持（Adaptive Identity Preservation）来解决这个问题，该技术将身份特征固定在特定场景的尺度上（身份锚定），并通过身份感知自注意力机制整合它们。为了评估不同空间组合下的性能，我们扩展了 Consistory+ 基准。广泛的实验表明，EOS-Story 在两个基准上都取得了具有竞争例或更优的性能。
- **PDF**: https://arxiv.org/pdf/2610.22320v1

### TraHist: Fast and Accurate Cardinality Estimation for Trajectory Data (Extended Version)
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.22310v1
- **作者**: Yujeong Jo, Incheol Baek, Changbeom Shim, Yon Dohn Chung
- **备注**: Extended version of the paper to appear in PACMMOD Vol. 4, No. 6 (SIGMOD 2027)
- **摘要**: 基数估计是数据库系统查询优化的基础。基于直方图的估计器因其简单高效而被广泛使用，但依赖于假设记录独立的以点为中心的分区。这一假设在轨迹数据中失效，在轨迹数据中，来自同一移动对象的记录显示出强烈的时空依赖性。因此，传统的轴对齐直方图跨分区边界割裂了轨迹，通过重复计数导致高估。为了解决这个问题，我们提出了 TraHist，这是一种基于直方图的估计器，通过高效的基于网格的传播来近似密度对齐的分区。TraHist 构建密度自适应的矩形桶，以保持轨迹连续性和局部密度连贯性，同时保持直方图的效率。在大规模真实世界数据集上的实验表明，在轨迹割裂是估计误差主要来源的查询体制中，TraHist 相对于最强的竞争估计器将估计误差降低了 20 倍以上，同时保持了亚毫秒级的查询延迟和极具竞争力的构建成本。
- **PDF**: https://arxiv.org/pdf/2610.22310v1

--- 
## 📚 学科: `math.*`
本周数学学科聚焦于图论与算法图论的前沿突破。重点论文通过紧凑的 SAT 序编码求解图的 Boxicity 和 Cubicity 问题，显著提升了求解效率，并成功否定了关于 Kneser 图 Boxicity 的长期猜想（证明了 $\operatorname{boxicity}(K(7,3))=3$）；另一项研究针对量子信息中的 GHZ 态实验模型，给出了基于图顶点连通度的 GHZ 图维数的通用上界证明，连接了组合图论与量子光学实验设计。

### Geometric Graph Representations via Compact SAT Encodings
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.22241v1
- **作者**: L. Sunil Chandran, Rishikesh Gajjala, Suraj Kumar Sahoo, Aatman Supkar
- **备注**: To appear in ALENEX 2027
- **摘要**: 我们提出了用于图的 Boxicity 和 Cubicity 的紧凑 SAT 编码与验证确切求解器。图的 Boxicity 是将其表示为轴对齐超箱的交集图所需的最小维度；Cubicity 使用单位立方体类似地定义。基于网格的形式化面临几何离散化瓶颈，随着目标维度的增加增长迅速。我们通过编码每个坐标中区间端点的全序来避免这一瓶颈。对于 $n$ 个顶点的图和目标维度 $d$，我们的 Boxicity 编码使用 $O(n^2d)$ 个变量和 $O(n^3d)$ 个子句，均随 $d$ 线性增长。要求左端点和右端点的顺序一致可以得到相同渐进大小的 Cubicity 编码。满足模型被解码为可独立检查的几何表示，而用作下界证据的不可满足实例带有机械验证的 DRAT 证书。在包含标准和结构化图族的 186 次测试的对照评估中，全序编码解决了 96.8% 的测试，而已知网格形式化仅为 71.0%，并将平均 PAR-2 时间从 178.21 秒减少到 21.70 秒。该流水线还证明了几种有名图的确切值。我们通过证明每个 $k\ge3$ 且 $n\ge2k+1$ 的 Kneser 图 $K(n,k)$ 都包含一个诱导 Desargues 图，将其中一个确切值转化为可复用的阻碍结构。得到的下界与 $K(7,3)$ 的显式三维表示结合，确立了 $\operatorname{boxicity}(K(7,3))=3$。这否定了 Caoduro 和 Sebo 关于对所有 $k\ge3$ 且 $n\ge2k+1$ 都有 $\operatorname{boxicity}(K(n,k))=n-k$ 的猜想。
- **PDF**: https://arxiv.org/pdf/2610.22241v1

### Connectivity Bounds for GHZ Graphs
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.22190v1
- **作者**: L. Sunil Chandran, Rishikesh Gajjala
- **备注**: To appear in FSTTCS 2026
- **摘要**: Greenberger-Horne-Zeilinger (GHZ) 态是多体纠缠量子态，在量子信息论中发挥着核心作用，应用于量子通信、密码学和分布式量子计算。主要的实验目标是使用多个纠缠粒子创建高维 GHZ 态。Krenn、Gu 和 Zeilinger 发现了这些量子光学实验与图论之间令人惊讶的桥梁：某些光子实验可以用边着色、边加权的图来表示，所产生的 GHZ 态的维度等于可行的单色继承顶点着色的数量。这促使 Krenn 和 Gu 猜想每个顶点数大于 4 的 GHZ 图的维度最多为 2。反例将给出一种新的高维多体 GHZ 构造，而证明则能明确量子光学中的基本资源限制。已知该猜想对顶点连通度最多为 2 的图成立。然而，先前尚不知道仅取决于顶点连通度的通用上界。我们证明了每个具有至少四个顶点的简单连通 GHZ 图 $G$，其维度最多为 $2^{\kappa(G)-1}+\binom{\kappa(G)}{2}$，其中 $\kappa(G)$ 为 $G$ 的顶点连通度。我们还证明了关于边连通度和最大度的最新界限。
- **PDF**: https://arxiv.org/pdf/2610.22190v1

--- 
## 📚 学科: `astro-ph.*`
本周天文学学科涵盖系外行星、太阳物理与恒星/星际介质观测研究。亮点工作包括提出利用时间偏移光谱法解耦系外行星 3D 大气晨昏肢不对称性（应用于 WASP-94A b）；基于 Gaia 等多源巡天构建的厚盘热木星寄主星样本分析；针对 X9.0 级太阳耀斑及准周期脉动（QPP）的日冕磁场三维重建；以及利用 MCMC 算法在双星光谱中无模板分离星际弥散带（DIB）与初生行星状星云 Vy 2-2 的演化机制研究。

### A New Method for Constraining 3D Exoplanet Atmospheres: Application to WASP-94A b's Panchromatic Spectrum
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.22271v1
- **作者**: Sagnick Mukherjee, Luis Welbanks, Guangwei Fu, David K. Sing, Michael R. Line
- **备注**: Accepted for publication in The Astrophysical Journal Letters
- **摘要**: 越来越多的掩星系外行星表现出光谱证据，表明其晨昏肢存在差异。解释这些观测结果目前是主要瓶颈。对肢分辨掩星深度进行拟合的标准方法会导致掩星深度高度负相关，将它们视为独立测量可能会导致检索到的分子丰度产生严重偏差（$3\sigma$）。我们提供了一个利用肢不对称性的时间特征来避免这些相关性的推断框架。这种随波长变化的凌星中点时间偏移（“时间偏移光谱”）携带肢不对称性信息，可以从现有光变曲线中用球对称掩星模型测得，且与球平均掩星深度无关。通过用每个肢的独立大气柱同时拟合生成的传输光谱和时间偏移光谱，能够从两个独立测量中检索出肢分辨特性。我们证明，与目前该领域采用的第二好方法相比，这种方法将检索到的分子丰度的均方误差降低了约 30-50 倍，并将检索到的丰度精度提高了约 3-6 倍。我们将该框架应用于 WASP-94A b，并展示了其跨越 0.8-5 $\mu$m 的全色肢分辨光谱。该行星的晨肢在整个范围内保持被气溶胶遮挡，而其昏肢限定了 H$_2$O、CO$_2$、CO 和 H$_2$S 的丰度。我们测得在 1 mbar 处的肢间温差为 $415\pm58$ K。
- **PDF**: https://arxiv.org/pdf/2610.22271v1

### A Sample of Thick-Disk Stars Hosting Hot Jupiters
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.22254v1
- **作者**: Victoria DiTomasso, Samuel W. Yee, Romy Rodriguez Martinez, Emily K. Pass, Phillip A. Cargile, David Charbonneau, Andrew Vanderburg, David W. Latham, Vedant Chandra
- **备注**: Accepted for publication in AJ
- **摘要**: 我们对 268 颗已确认和候选的掩星热木星寄主星（4800K < Teff < 6200K）进行了均匀分析。我们结合高分辨率 TRES 光谱、Gaia、2MASS 和 WISE 光度学以及 Gaia 天体测量学，确定了这些恒星的 Teff、log g、Rstar、[alpha/Fe] 和 [Fe/H]。基于其 [alpha/Fe] 和 [Fe/H]，我们将这些恒星分类为银河薄盘、厚盘或中间过渡族群的成员。我们识别出 2 颗已确认的热木星（WASP-81 b 和 TOI-5322 b）和 3 颗候选热木星，它们围绕先前未被识别的高 alpha 厚盘成员运行。我们比较了三个族群中确认行星的属性，并指出族群之间存在潜在差异的两个迹象：高 [alpha/Fe] 确认行星和 11 颗模糊盘确认行星中的 8 颗质量均小于低 [alpha/Fe] 行星的中位数；且高 [alpha/Fe] 或模糊盘确认行星中没有一颗的轨道周期短于 2.7 天，而在低 [alpha/Fe] 族群中这一比例为 22%。我们的编目是目前最大的经化学识别的高 [alpha/Fe] 厚盘热木星寄主星样本。
- **PDF**: https://arxiv.org/pdf/2610.22254v1

### Investigation of an X-class Flare and Quasi-Periodic Pulsations in NOAA AR 13842 using SDO, Aditya-L1 and Solar Orbiter
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.22165v1
- **作者**: Pawan Kumara, Sanjay Kumara, Sushree S. Nayak, Sadashiv, Sachin Rajkapoor Kanaujiyac, Ramesh Chandrad
- **备注**: 23 Pages, 14 Figures, Accepted in Advances in Space Research (ASR)
- **摘要**: 我们利用太阳动力学天文台（SDO）、Aditya-L1 和太阳探测器（Solar Orbiter）的观测数据，研究了 NOAA 活动区 13842 中的 X9.0 级耀斑（SOL2024-10-03T12:08）及相关的准周期脉动（QPP）。为了探讨磁场结构在耀斑中的作用，我们采用了非无力场外推技术重建了整个耀斑过程中日冕磁场的序列。外推记录了通量绳、剪切拱和包围通量绳与拱的双曲通量管（HFT）的存在。通量绳在向磁环不稳定区域上升时扭转度增加，使其成为喷发的可能候选者。在剪切拱内以及 HFT 处发生的重复磁重联被推测为引起 QPP 的原因。
- **PDF**: https://arxiv.org/pdf/2610.22165v1

### Disentangling Multi-epoch Single-lined Binary Star Spectra to Reveal Interstellar Medium Features via MCMC
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.21997v1
- **作者**: Shao-Song Huang, Jian-Jun Chen, Xiao-Xiao Ma, Ji-Wei Shi
- **备注**: 21 pages, 12 figures, 3 tables, accepted for publication in Reasearh in Astronomy and Astrophsics
- **摘要**: 弥散星际带（DIB）是光学和近红外光谱中载体未明的星际吸收特征。在冷星光谱中观测时，它们受到恒星谱线的严重污染。我们提出了一种不依赖模板的算法，通过利用轨道运动来分离双星光谱中的恒星和星际特征：恒星谱线随着视向速度（RV）的变化而移动，而 DIB 在静止系中保持不动。实现为基于 RV 的贝叶斯马尔可夫链蒙特卡洛框架的 MCMC-RVSD 算法同时拟合两个分量。我们在模拟 LAMOST 中分辨率观测的伪光谱上验证了该方法，精确复原了 DIB $\lambda$6614 的参数。对 LAMOST 中分辨率巡天的 434 个真实双星源的应用表明，RV 跨度 $>20$ km/s 是成功实现谱线分离的主要驱动力。
- **PDF**: https://arxiv.org/pdf/2610.21997v1

### Intermediate- and high-resolution optical spectroscopy on the nascent planetary nebula Vy 2-2: Evidence of binary-star evolution
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.21988v1
- **作者**: Roldán A. Cala, Luis F. Miranda, José F. Gómez, Lucero Uscanga, J. Ricardo Rizzo
- **备注**: Accepted for publication in A&A. 14 pages, 5 figures, 8 tables
- **摘要**: 行星状星云（PNe）往往展现出壮观的非球形形状，其起源尚未得到完全理解。我们对初生行星状星云 Vy 2-2 进行并分析了新的中分辨率和阶梯高分辨率光谱，以获取其化学丰度及其争议极大的丰度差异因子（ADF）的新值，探究其内部运动学和电离情况，并推断其可能的形成过程。分析表明 Vy 2-2 包含一个相对高激发态的中心区域和两个低激发态的双极喷流/极瓣，新的 ADF(O$^{2+}$)=13.6$\pm$2.6 表明 Vy 2-2 属于具有异常高 ADF 的 PNe 群体，指向 Vy 2-2 宿主着一个共有包层后双星系统（post-common-envelope binary system）。
- **PDF**: https://arxiv.org/pdf/2610.21988v1

--- 
## 📚 学科: `stat.*`
本周统计学与定量方法领域重点探讨了非高斯随机过程建模与 AI 安全博弈论。重点论文提出了 STOCHLOB 框架，将重尾 Lévy 噪声与 alpha-稳定过程引入扩散 Score 匹配，显著提升了限价单簿（LOB）高频金融数据的极端风险预测能力；另一项研究通过博弈论模型分析了 AI 供应链中上下游企业对安全投资的激励机制，探讨了市场竞争与监管干预对模型安全性的影响。

### StochLOB: Heavy-Tailed Score Matching for Robust Limit Order Book Trend Prediction
- **分数**: 5
- **链接**  https://arxiv.org/abs/2610.21081v1
- **作者**: Arshia Abolghasemi, Seyed Reza Tavakoli, Parsa Naderi, Nazanin Mirzaei, Behrad Jahani, Saba Yousefzadeh, Tahereh Javaheri, Mohammad Hosein Rohban, Gholamali Aminian, Ali Habibnia
- **备注**: 32 pages, 5 figures. NeurIPS 2026 Workshop: AI for Stochastic Dynamics
- **摘要**: 基于 Score 的扩散方法通常使用布朗高斯噪声扰动数据。对于市场时间序列，这种 SDE 可能是一种较差的抽象：限价单簿（LOB）订单流具有重尾、突发性和偶尔跳跃的特性。我们研究了 STOCHLOB，一种仅训练的 Score 匹配框架，它改变了前向扩散损坏律，同时保持部署的预测器为确定性。损坏过程没有采用仅有布朗运动的高斯损坏，而是使用了两种受非高斯 SDE 启发的替代方案：通过复合泊松方差混合的跳跃-Lévy 噪声，以及通过正稳定高斯尺度混合的截断 $\alpha$-稳定噪声。这些损坏在训练中注入了有限跳跃和重尾残差，而在推理时不需要逆向时间扩散采样。在 Coinbase LOB 数据上的实验表明，所提出的变体在未损坏的 BTC 和山寨币测试时界上保持了竞争力，并改善了几个实现的尾部窗口压力诊断。代码开源于 https://github.com/ArshiAbolghasemi/Penny 。
- **PDF**: https://arxiv.org/pdf/2610.21081v1

### Market Incentives for AI Safety Investment
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.21607v1
- **作者**: Nikita Tsoy
- **备注**: NeurIPS 2026
- **摘要**: 尽管具有重大的实用意义，现代 AI 系统仍带来显著的社会风险。缓解这些风险不仅取决于技术可行性，还取决于开发和部署这些系统的企业的激励机制。我们展示了在包含上游 LLM 提供商和多家竞争性下游企业的 AI 供应链中，利润最大化如何塑造安全投资。在博弈论模型中，我们导出了市场驱动的安全投资水平，并将其与使市场福利和行业利润最大化的水平进行比较。我们发现，下游竞争通常会促使下游企业在安全上的投资高于行业利润最佳水平。相比之下，上游提供商相对于这些基准可能投资不足，因为它未能完全获得安全投资带来的溢出盈余。最后，我们分析了不同的监管干预如何影响参与者的激励和利润，以及由此产生的模型安全水平。
- **PDF**: https://arxiv.org/pdf/2610.21607v1

--- 
## 📚 学科: `econ.*`
_本周缺少高价值论文_