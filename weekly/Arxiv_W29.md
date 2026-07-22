# 🗓️ 周报 (2026-W29)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-07-19

--- 
## 📚 学科: `eess.*`

**本周 `eess.*`（电气工程与系统科学）学科总结**：
本周该领域的论文涵盖了人机物理交互、无线通信、多模态智能体、人工智能安全以及医学图像分割。在机器人与人机交互方面，学者们探索了高难度的人机多球杂耍实时规划和新型混合智能体博物馆导游系统，展示了精细控制与多模态交互对用户体验的提升。在医疗应用上，结合SAM模型的视觉提示分割框架ViPSAM有效解决了低对比度非增强CT的分割难题。此外，针对电磁感应通信中的天线部署优化，以及从历史社会技术灾难中反思AI系统级安全风险的论述，都展现了该学科从底层硬件优化到高层系统治理与临床应用的多元发展趋势。

### Catch, Throw, Repeat: Planning for Human-Robot Partner Juggling
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.15129v1
- **作者**: Jonathan Rainer Lippert, Kai Ploeger, Abir Chowdhury, Hermann Müller, Jan Peters, Alap Kshirsagar
- **备注**: Accepted at the 2026 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS 2026)
- **摘要**: 由于感知、时序和富接触交互中的不确定性，人类与机器人之间的动态物体交换仍然是一个具有挑战性的问题。人类-机器人杂耍是该问题中一个特别苛刻的实例，需要精确的实时协调、带反馈控制的预测运动规划，以及对人类运动变异性的鲁棒性。实现这些技能对于推动物理人机交互和共享自主性具有重要意义。我们提出了一种用于人机伙伴杂耍的实时规划和控制架构，使机器人能够与人类伙伴在同步的多球模式中可靠地接球和抛球。该系统整合了预测性球体追踪、使用多重打靶法（multiple-shooting formulation）的自适应在线轨迹优化，以及基于状态机的协调逻辑，以实现同步的多球人机伙伴杂耍。在对8名具有从初学者到专家不同杂耍水平的参与者进行的用户研究中，我们证明了我们的系统可以实现机器人和人类之间共享的三球级联杂耍。所有参与者在10分钟的测试环节内都超过了此前报道的最佳结果，其中一名参与者将此前共享三球级联杂耍的记录延长了五倍，达到了连续20次机器人接球，另一名参与者在单球接投设置中实现了100%的成功率，连续接球40次。视频文档可在以下网址找到：https://kai-ploeger.com/partner-juggling
- **PDF**: https://arxiv.org/pdf/2607.15129v1

### Effect of Antenna Deployment on Achievable Rate in Cooperative Magnetic Induction Communication
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.14701v1
- **作者**: Honglei Ma, Erwu Liu, Rui Wang, Xinyu Qu
- **备注**: This work was published in IEEE Communications Letters, with the DOI: 10.1109/LCOMM.2019.2929790
- **摘要**: 磁感应（MI）通信可应用于矿井、地下河等一些穿地场景。为了提高MI通信的传输速率，我们提出了一种具有放大转发（AF）中继的协作MI（CMI）方案。与现有研究不同，我们主要关注具有任意天线位置和方向（天线部署，AD）的中继。我们推导了中继的CMI可达数据速率增益（CMG）的闭式表达式以及CMI信道带宽的闭式表达式。仿真表明，部署合适天线（AD）的中继可以显著提高MI系统的可达速率。
- **PDF**: https://arxiv.org/pdf/2607.14701v1

### Mixed-Agent Museum Tour Guide Design Improves Gendered Learning Outcomes and Visitor Preferences
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.14468v1
- **作者**: Annette M. Masterson, Wonse Jo, Helena C. Sieh, Lionel P. Robert,, Dawn Tilbury
- **备注**: Accepted on IROS 2026, 8 pages
- **摘要**: 机器人正越来越多地融入日常场景，包括博物馆，在这些场景中它们既可以娱乐也可以教育游客。为了增强游客的体验和参与度，我们提出了一种新型的混合智能体导游系统，该系统将实体机器人与投影的虚拟智能体相结合，虚拟智能体通过对话和互动积极参与导览，从而在单一平台上实现了两个移动智能体的丰富交互性。我们通过对30名参与者进行内组（within-subjects）研究来验证该系统，以评估其参与度、体验质量和学习效果。参与者体验了不同的对话风格和智能体配置，并通过问卷调查、行为传感器和访谈收集了数据。结果显示，在不同条件下，参与度和体验质量保持一致。学习效果呈现出显著的性别调节差异：混合智能体条件提高了女性参与者的学习表现。这表明本文提出的双人对话风格对不同性别的学习效果产生了不同的影响。尽管如此，在访谈中，无论性别如何，参与者都表示更倾向于混合智能体团队，并将互动视为其体验的关键因素。
- **PDF**: https://arxiv.org/pdf/2607.14468v1

### Unsafe at any AUC: Unlearned Lessons from Sociotechnical Disasters for Responsible AI
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.14353v1
- **作者**: Joshua A. Kroll, Andrew Smart, R. Stuart Geiger, Abigail Z. Jacobs
- **备注**: Accepted to the Harvard Data Science Review, Volume 8(3), Summer 2026
- **摘要**: 随着自动决策和数据驱动技术渗透到社会中并用于管理具有重大影响的结果，在具体情境中理解技术的能力、局限性和随之而来的风险需要对完整的社会技术系统进行分析。对高度复杂系统中的风险进行社会技术分析，为人工智能系统的设计和评估提供了清晰的教训，超越了对可靠或“负责任设计”组件的技术关注，从而在系统层面理解风险。人类制造的灾难因其严重性已被研究了数十年：例如切尔诺贝利、三里岛、福岛第一核电站、博帕尔、挑战者号航天飞机灾难。一个常见的误解是，这类事件是由于复杂系统中固有的不可预测的相互作用而导致的离奇事故。仔细的研究表明，风险和危害在事前早已广为人知，但由于社会结构、政治和经济因素而未被采取行动。我们概述了人工智能的开发和使用可以从这些未吸取的教训中受益的几个领域：组织层面上改进风险感知、沟通和分析；需求和责任的可追溯性；以及将社会和组织动态作为首要工程关注点的责任和安全整体方法。对于每个领域，我们提供了具体的未吸取教训，并举例说明了它们如何导致先前的事故，以及这些教训在现代计算系统（特别是人工智能）中仍未被吸取的例子。
- **PDF**: https://arxiv.org/pdf/2607.14353v1

### ViPSAM: Visual Prompting Medical Image Segmentation Using Segment Anything Model
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.14328v1
- **作者**: San Lee, Nalee Kim, Jeong Il Yu, Hee Chul Park, Boah Kim
- **备注**: Accepted at MICCAI 2026
- **摘要**: 在质子治疗规划中，呼吸门控非增强CT（NCCT）常用于病变分割；然而，由于病变与背景的对比度低，准确勾画仍具挑战性。尽管基于学习的方法表现出强大的性能，但它们通常在非增强图像分割方面面临困难。受到临床实践（即参考增强MRI在NCCT上勾画病变）的启发，我们提出了ViPSAM，这是一个利用互补跨模态信息的视觉提示框架。ViPSAM基于Segment Anything Model (SAM)构建，引入了视觉提示编码器以从增强图像中提取引导特征，并引入了视觉引导的交叉注意力模块以整合非增强和增强特征，从而增强低对比度区域中与病变相关的表征。此外，掩膜解码器以参数高效的方式进行了调整，以有效利用视觉提示。我们在用于质子治疗的NCCT上进行的肝脏病变分割评估了所提方法。实验结果表明，ViPSAM优于代表性的基于U-Net和SAM的方法，表明跨模态视觉提示能够在非增强图像中实现更鲁棒和精确的分割。
- **PDF**: https://arxiv.org/pdf/2607.14328v1

--- 
## 📚 学科: `q-bio.*`

**本周 `q-bio.*`（定量生物学）学科总结**：
本周定量生物学领域选入了一篇将控制理论与生物医学应用相结合的突破性论文。该研究聚焦于安全控制理论中的经典框架——Hamilton-Jacobi可达性（HJR），攻克了在存在外部“对手”（不确定性或干扰）的情况下，双目标值函数精确分解的理论难题。作者不仅在数学上证明了该分解的有效性，更将其成功应用于临床医学中的“优化药物给药方案设计”。这一工作展示了控制论、博弈论与定量生物学的深度交叉，为个性化医疗和安全临床决策提供了坚实的控制理论支持。

### Exact Decomposition of Adversarial Dual-Objective Value Functions, with Applications to Optimal Drug Dosing
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.14023v1
- **作者**: Dylan Hirsch, William Sharpless, Sylvia Herbert
- **备注**: D.H. and W.S. contributed equally to this work. 8 pages, 2 figures. Accepted to 2026 Conference on Decision and Control (CDC)
- **摘要**: Hamilton-Jacobi可达性（HJR）是安全控制理论中的核心框架。虽然HJR传统上专注于一些基础任务，但人们对将其扩展到更复杂的战略目标越来越感兴趣。最近的研究探讨了在无对手设定下，两个基础双目标任务的值函数的精确分解。然而，在存在对手的情况下，并非HJR中的所有值函数分解都保持有效。在这项工作中，我们开发了理论方法来证明，对于这两个复合值函数，所提出的分解在存在对手的情况下仍然成立。最后，我们展示了这些结果如何解决将HJR应用于优化药物给药方案设计时出现的问题。
- **PDF**: https://arxiv.org/pdf/2607.14023v1

--- 
## 📚 学科: `cs.*`

**本周 `cs.*`（计算机科学）学科总结**：
本周计算机科学领域的论文展示了人工智能、算法理论和边缘计算的前沿突破。在因果推理与多模态AI方面，学者利用大语言模型辅助城市驾驶数据的因果分析，并提出Symbal系统有效检测多模态大模型在图像描述中产生的“系统性错配”；在医疗图像领域，CRISP框架在冻结权重的前提下，利用概率排名稳定性攻克了跨域图像分割中的分布偏移难题。此外，算法理论研究对仅通过得分序列解决竞赛图经典问题给出了统一的理论刻画，而物联网传感研究则通过“哨兵辅助”卡尔曼滤波框架实现了无线传感器网络中极低能耗下的高精度异常监测。整体而言，本周CS论文在实用性工具开发与底层算法理论上均取得了实质性进展。

### teLLMe Why (Ain't Nothing but a Jam): Exploratory Causal Analysis of Urban Driving Data
- **分数**: 6
- **链接**  https://arxiv.org/abs/2607.15254v1
- **作者**: Qiwei Li, Jorge Ortiz
- **备注**: Accepted at the NeurIPS 2025 Workshop on UrbanAI. 6 pages
- **摘要**: 交通管理机构现在可以获取大量基于视频的数据来研究安全和拥堵。这些数据中的大多数是观测性的，且是在没有干预的情况下收集的，这使得诸如“降雨如何改变交通密度？”之类的因果问题难以回答。我们介绍了 teLLMe，一个用于城市驾驶数据集探索性因果分析的系统。该系统从基于行车记录仪标注构建的结构化事件表开始，并将因果结构学习与 PC 算法、基于自助法（bootstrap）的稳定性检查，以及使用线性回归和 DoWhy 的特定查询效应估计相结合。自然语言问题通过感知模式（schema-aware）的大语言模型（LLM）映射到结构化的因果查询，从而允许用户指定干预、结果和子群体。teLLMe 返回一张“因果卡”（Causal Card），其中总结了效应估计、调整集、有向无环图（DAG）支持和假设，并辅以简短的自然语言解释。在源自 BDD 的交通事件案例研究中，系统能够发现涉及天气、高峰时段和交通密度的合理关系，同时明确展示了不确定性和模型选择。该系统被设计为假设生成和专家推理的工具，而非确定性因果结论的来源。
- **PDF**: https://arxiv.org/pdf/2607.15254v1

### CRISP: Constrained Refinement via Iterative Squeezing Process for Robust Medical Image Segmentation under Domain Shift
- **分数**: 4
- **链接**  https://arxiv.org/abs/2607.15231v1
- **作者**: Yizhou Fang, Pujin Cheng, Yixiang Liu, Xiaoying Tang, Longxi Zhou
- **备注**: X pages, 3 figures, 3 tables; submitted to AAAI 2027
- **摘要**: 医学成像中的分布偏移（distribution shift）仍然是临床转化医疗AI的核心瓶颈。未能解决这一问题可能会导致在未见环境中的严重性能退化，并加剧健康不平等。现有的领域自适应方法受限于通过模拟偏移或伪监督穷尽预定义的可能性。此类策略在开放且不可预测的真实世界中显得力不心，因为那里的分布偏移实际上是无限的。为了应对这一挑战，我们采用“阳性区域的等级稳定性”作为分布偏移下的工作假设，并利用它来推导源域单模分割的鲁棒空间提示。在该假设的指导下，我们提出了 CRISP，一个与模型无关的框架，与部署时自适应不同，它不需要测试时参数更新，也不需要目标域数据——这是一个目标无关的、即插即用的精细化框架，在冻结权重的情况下进行分割。CRISP 不是利用排名来直接输出掩膜，而是利用分布偏移下概率排名的稳定性来推导鲁棒的空间先验。通过潜在特征扰动，扰动不变的高等级区域定义了高精度（HP）核心，而在至少一次扰动下仍保持潜在前景的体素则定义了高召回率（HR）支撑；然后，这两个先验在扰动下进行递归细化。接着，我们设计了一个迭代训练框架，逐步将 HP 和 HR 压缩到最终的分割结果中。在多中心心脏 MRI 和基于 CT 的肺部血管分割上的广泛评估表明，CRISP 具有卓越的鲁棒性，显著优于最先进的方法，在多中心、人口统计学和模态偏移方面，HD95 显著降低，分别提高了 0.14 像素（提升 7.0%）、1.90 像素（提升 13.1%）和 8.39 像素（提升 38.9%）。
- **PDF**: https://arxiv.org/pdf/2607.15231v1

### Symbal: Detecting Systematic Misalignments in Model-Generated Captions
- **分数**: 4
- **链接**  https://arxiv.org/abs/2607.15216v1
- **作者**: Maya Varma, Jean-Benoit Delbrouck, Sophie Ostmeier, Akshay Chaudhari, Curtis Langlotz
- **备注**: ICML 2026
- **摘要**: 多模态大语言模型（MLLMs）在生成图像描述（captions）时经常会引入错误，导致图像-文本对出现错配。我们的工作重点关注一类我们称为“系统性错配”（systematic misalignments）的描述错误，即 MLLM 生成的描述中反复出现的错误与配对图像中特定视觉特征的存在密切相关。给定一个带有 MLLM 生成描述的视觉-语言数据集，我们在这项工作中的目标是检测此类错误，我们称之为“系统性错配检测”任务。作为我们的第一个关键贡献，我们提出了 Symbal，它利用具有现成基础模型的结构化、双阶段设置来识别系统性错配并用自然语言总结结果。作为我们的第二个关键贡献，我们引入了 SymbalBench，这是一个旨在评估我们提出的任务上的自动化方法的基准。SymbalBench 包含来自两个领域（自然图像和医学图像）的 170 万个图像-文本对，组织在 420 个标有系统性错配的视觉-语言数据集中。Symbal 在该基准上表现出强劲的性能，正确识别了 63.8% 数据集中的系统性错配，比最接近的基线提高了近 4 倍。我们通过真实世界的评估来补充我们在 SymbalBench 上的评估，结果表明：（1）Symbal 能够准确发现四个 MLLM 生成的描述中的系统性错配，并且（2）Symbal 是审计现成图像-描述数据集的强大工具。最终，我们新颖的任务、方法和基准可以帮助用户审计 MLLM 生成的描述并识别关键错误，而无需访问底层的 MLLM。代码开源于 https://github.com/Stanford-AIMI/Symbal。
- **PDF**: https://arxiv.org/pdf/2607.15216v1

### The Power of the Score Sequence of a Tournament
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.15260v1
- **作者**: Prantar Ghosh, Sahil Kuchlous, Shravan Mehra, Sagnik Mukhopadhyay
- **备注**: To appear in ESA 2026
- **摘要**: 如果仅知道一个竞赛图（tournament）的得分序列，我们可以解决它的哪些问题？竞赛图是有向完全图，无论从组合还是算法的角度来看，它们都是被广泛研究的一类有向图（digraphs）。多年来，研究人员已经确定了多个经典的图问题，这些问题在竞赛图中可以仅通过其得分序列（入度序列）来解决。这些问题包括无环性测试和拓扑排序、s,t-可达性、强连通性以及强连通分量（SCC）分解，还有顶点排序问题如割宽和最佳线性排列。这些先前的研究通过为各个具体问题设计不同的算法，证明了得分序列的充分性。在这项工作中，我们提供了一个简单的统一框架，仅使用入度即可解决所有这些问题，并且实际上完全刻画了由入度信息决定的问题类别：即其答案在循环反转（cycle reversals）下保持不变的问题。这一刻画是我们建立的一个更通用结果的特例：对于任意有向图，其骨架（底层无向图）和顶点入度知识完全决定了其在循环反转下保持不变的性质。作为我们结果的副产品，我们在流模型、双人通信模型和割查询计算模型中，获得了竞赛图和“准竞赛图”上各种基于连通性、基于割以及顶点排序问题的算法。其中一些算法达到了现有的最优界限，另一些则提供了优于现有技术水平的界限。
- **PDF**: https://arxiv.org/pdf/2607.15260v1

### Adaptive Sampling for Spatiotemporal Anomaly Monitoring in Wireless Sensor Networks
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.15235v1
- **作者**: Guoqing Lu, Yixuan Sun, Yiwen Jiang, Bernard Butler
- **备注**: Accepted paper for IEEE ISSC 2026 conference, Limerick, Ireland
- **摘要**: 无线传感器网络（WSN）中的长期环境监测通常使用稀疏采样来延长网络寿命，但稀疏传感可能会遗漏短暂的、局部的且具有潜在扩散性的异常情况。本文提出了一种哨兵辅助的自适应采样框架，作为用于 WSN 异常监测的协作传感-控制管线。在正常期间，节点执行由卡尔曼滤波器（KF）预测不确定性驱动的稀疏传感。在异常期间，持续采样的哨兵节点执行基于混合广义似然比（GLR）且具有节点相对阈值的检测，并且局部检测触发一跳邻域唤醒与恢复感知的警报控制。在具有突发随机时空异常的英特尔伯克利研究实验室温度数据集上进行的实验表明，所提方法在主实验中将异常窗口采样率（AWSR）从 0.439 提高到 0.933。它还在减少总成本分别达 15.4% 和 2.1% 的同时，比自适应数据采集与能效及关键传感保证（AAS）以及自适应 e-采样提高了 AWSR。这些结果表明，将基于 KF 的稀疏采样、哨兵 GLR 检测和局部警报传播相结合，可以在保持较低采样成本折衷的同时，提高异常窗口的可见性。
- **PDF**: https://arxiv.org/pdf/2607.15235v1

--- 
## 📚 学科: `math.*`
_本周缺少高价值论文_

---
## 📚 学科: `astro-ph.*`

**本周 `astro-ph.*`（天体物理学）学科总结**：
本周天体物理学领域的研究展示了从系外行星演化到恒星动力学以及观测设备的最新进展。系外行星方向，学者利用模拟证明了大多数热木星可能形成于水冰线之外，并研究了年轻岩石行星表面岩浆洋时期释气与逃逸对大气成分的共同塑造。在恒星与星团研究上，针对即将爆发的北冕座T再发新星，研究者结合历史演化给出了最新的爆发约束窗口；同时，对古老星团 Berkeley 32 的化学-动力学分析研究了银河系盘内的径向迁移机制。此外，结合 SKA-LOW 的亚太低频 VLBI 网络提案展示了未来低频射电天文观测灵敏度大幅提升的宏伟蓝图。

### When will T Coronae Borealis next erupt as a nova? Constraints from recurrence, orbital phase, and accretion-state evolution
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.15245v1
- **作者**: Songpeng Pei, Xiaowan Zhang, Renzhi Su, Ziwei Ou, Yongzhi Cai, Qiang Li, Yu Liu, Xiaoqin Ren, Taozhi Yang
- **备注**: 7 pages, 1 figure, Accepted for publication in Monthly Notices of the Royal Astronomical Society Letter (MNRAS Letter)
- **摘要**: 北冕座T（T CrB）是最近的共生再发新星，目前正受到对其下一次爆发的密切监测。我们结合了三个关于爆发时间的限制条件：历史再发性、轨道相位以及最近的吸积态演化。在2026年7月11日之前未发生爆发的前提下，三个有效的历史间隔给出了具有说明性的、受生存条件约束的概率：2026年剩余时间内为30.2%，随后一年内为56.9%；这些是经验性指标，而非物理预测概率。采用的四个历史爆发相位并未选出唯一的点火相位，而是在 $φ\simeq0.44$ 和 $φ\simeq0.62$ 附近形成了两个松散的配对，在此仅用作监测窗口。1946年前的非典型变暗很难仅通过单纯的吸积率下降或标准尘埃消光来解释，可能涉及吸积重构和依赖于源的遮蔽。如果2026年重新开始的变暗是1946年前的真实对应物，那么2026年12月左右的爆发仍然是合理的。相反，如果2024年后的亮度保持在2014-2023年的高态之下，吸积赤字估计给出的最早下限接近2029年5月。因此，数据支持有条件的监测窗口，而非单一的确定日期。这些是条件性诊断情景，而非相互竞争的点预测；最终的爆发时期将检验它们的潜在假设。
- **PDF**: https://arxiv.org/pdf/2607.15245v1

### The majority of hot Jupiters formed beyond the water ice line
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.15144v1
- **作者**: Yaxing He, Bertram Bitsch, Adrien Houge, Joe Williams, Masahiro Ogihara
- **备注**: 8 pages, 5 figures, 2 tables. Accepted for publication in A&A Letters
- **摘要**: 巨型系外行星的大气成分可以保留其形成环境的信息，因为挥发性物种在原行星盘的不同温度下会发生冷凝。我们研究了热木星的大气成分是否可以约束它们的形成位置。我们使用 ChemComp 代码进行了行星形成模拟，包括卵石漂移、卵石与气体吸积、行星迁移、恒星丰度，以及两个额外的化学过程：耐熔有机物的热分解和水冰中 CO/CO2 的捕获。我们将该框架应用于九个已观测到的热木星系统，并将产生的气体大气金属丰度（C/H 和 O/H）与观测约束进行了对比。我们发现，这九个热木星系统的观测大气丰度可以通过在相对于 H2O 和 CO2 雪线的不同位置形成的行星来重现。我们的结果表明，九个系统中至少有六个与在 H2O 雪线以外形成相一致。结合观测到的轨道间距、偏心率和自转轨道倾角，这些推断出的形成位置表明，许多系统可能经历了动力学散射以及随后的潮汐演化。大气丰度与详细的轨道参数相结合，可以为热木星系统的形成和迁移历史提供强大的诊断工具，从而为理解巨行星的起源开辟了新的途径。
- **PDF**: https://arxiv.org/pdf/2607.15144v1

### Berkeley 32: A Metal-poor and Dynamically Evolved Open Cluster with Evidence of Radial Migration
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.15131v1
- **作者**: Deniz Cennet Çınar, D. Bisht, Ing-Guey Jiang, W. H. Elsanhoury, K. Belwal, Selçuk Bilir
- **备注**: 27 pages, including 15 figures and 4 tables, accepted for publication in the The Astronomical Journal (AJ)
- **摘要**: 我们present了一项基于 Gaia DR3 天体测量学和 Gaia-ESO Survey DR5.1 光谱学，对古老且贫金属的疏散星团 Berkeley 32 进行了全面的化学-动力学分析。利用高斯混合模型对自行分量和三角视差进行分析，确定了星团的成员身份。等时线拟合得出其年龄为 4.9 +/- 0.5 Gyr，日心距离为 3325 pc，消光为 A_V = 0.38 +/- 0.12 mag。光谱成员星表现出 [Fe/H] = -0.39 +/- 0.02 dex 的平均金属丰度、接近太阳的 alpha 元素丰度，以及 V_rad = 106.26 +/- 0.03 km s^-1 的加权平均视向速度。[Y/Mg] 化学钟得出的年龄为 4.73 +/- 2.39 Gyr，与等时线估计一致。轨道积分表明其具有中等偏心率的轨道（e = 0.268 +/- 0.004），引导半径为 R_g = 8.82 kpc。推断出的化学诞生半径 R_b = 9.82 kpc 以及 DeltaR ~ -1 kpc 表明存在中等的向内径向迁移，而 R_b、R_g 和 R_GC 之间的偏差与混合（churning）和模糊（blurring）过程一致。光度分析确定，对于质量比 q >= 0.5 的系统，双星比例为 f_b = 0.449 +/- 0.017，这意味着存在大量未解析的双星群。径向累积分布函数进一步揭示了显着的质量分层，演化星比主序星更向中心聚集。这些结果表明，Berkeley 32 是一个动态演化的古老盘星团，其如今的结构和轨道保留了银河系盘内内部动力学演化和径向迁移的特征。
- **PDF**: https://arxiv.org/pdf/2607.15131v1

### Low-Frequency VLBI Network Using SKA-LOW
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.15039v1
- **作者**: Hideyuki Kobayashi, Tomoaki Oyama, Kazuma Fujita, Syunsaku Suzuki, Shintaro Yoshiura, Hiroaki Misawa, Fuminori Tsuchiya, Kazuhiro Takefuji, Kenta Fujisawa, Kohtaro Niinuma, Keitaro Takahashi, Yashwant Gupta, Bhal Chandra Joshi, Vishwesh Marthi, M. A. Krishnakumar, Zhiqiang Shen, Wu Jiang, Yihua Yan, Wei Wang, Linjie Chen
- **备注**: Published in Advancing Astrophysics with the SKA II (AASKAII), 2026 (arXiv:2606.20366). Report-no:AASKAII/Kobayashi01
- **摘要**: 我们建议开发一个工作在 100-350 MHz 频段、并纳入平方公里阵列低频段（SKA-LOW）的低频甚长基线干涉测量（VLBI）网络。SKA-LOW 预计将在该频段内实现极高的灵敏度。通过将 SKA-LOW 与分布在亚太地区的其他高灵敏度射电望远镜相整合，所提出的网络预计将比现有的 VLBA 提供高达两个数量级的灵敏度提升。尽管已经提出了利用低频 VLBI 的若干科学主题，我们特别倡导利用现有的 VLBI 测站进行天体测量研究，以展示该频率范围的可行性和科学潜力。此外，将 SKA-LOW 与其他射电望远镜相结合将能够实现高保真度的成像观测，从而显着增强低频 VLBI 科学的质量和范围。
- **PDF**: https://arxiv.org/pdf/2607.15039v1

### Atmospheric evolution through outgassing and escape on young molten rocky exoplanets
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.15011v1
- **作者**: Emma Postolec, Tim Lichtenberg, Harrison Nicholls, Laurent Soucasse, Floris van der Tak
- **备注**: Accepted for publication in A&A; 10 figures, 19 pages; abstract shortened to conform with arXiv requirements
- **摘要**: 早期岩石行星的大气是由初始挥发物储量与大气逃逸之间的竞争决定的。在年轻的岩浆洋行星上，释气与大气逃逸相互竞争，控制着挥发物的保留和大气演化。我们研究了岩浆洋结晶过程中的大气逃逸和通过释气进行的补给如何塑造岩石行星的大气。我们扩展了一个内部-大气耦合模型，通过引入能量限制的大气逃逸模块，来模拟岩浆洋时期的岩石行星演化。通过对比辐射-对流大气和规定-对流大气，我们定量分析了大气能量传输如何影响逃逸。我们探索了广泛的轨道间距、逃逸效率、氧化状态和初始挥发物储量，以确定持续岩浆洋释气或逃逸主导的区间。我们估算了类太阳恒星和M型矮星周围年轻岩石行星在地球物理时间尺度上的大气流失和成分。大气逃逸通过减弱温室保温作用缩短了岩浆洋的寿命。与纯对流情况相比，辐射-对流大气减少了凝固时间尺度。挥发物在岩浆洋中的溶解与逃逸相互作用，通过保留更多可溶性物种，随时间对行星的挥发物预算进行化学分馏。对于地球质量的行星，如果流失率保持温和，大气就能存活。地幔氧化还原状态仍是保留大气成分的关键控制因素：高氧逸度（fO2）产生较重的、富含 H2O 和 CO2 的大气，而低 fO2 产生轻的、以 H2 或 CO 为主的大气，这与先前的研究一致。轨道间距、初始挥发物储量和恒星类型产生了多样的演化路径，从裸露的岩石行星到具有厚大气的岩浆洋（范围从以 H2 为主到以 SO2 为主）。
- **PDF**: https://arxiv.org/pdf/2607.15011v1

--- 
## 📚 学科: `stat.*`

**本周 `stat.*`（统计学）学科总结**：
本周统计学领域的两篇论文聚焦于隐私保护机制与时间序列分析。在数据隐私方面，研究者针对举报人面临的报复威胁，首次将保护机制形式化为每条报告的 $(0, δ)$-差分隐私，并提出了一种将隐私审计简化为“隐私持续计数”的创新算法框架，显著提升了强对手模型下的安全防范能力。在应用统计领域，针对可穿戴设备产生的高维时间序列，学者提出了贝叶斯脉冲-平板谱分析框架，实现了多维生理信号中共享与特异性节律的高分辨率、稀疏提取。这两项工作在隐私计算理论和健康医疗数据分析上均提供了兼具严谨数学论证与强实用性的统计学方案。

### Plausible Deniability Guarantees for Whistleblowers
- **分数**: 6
- **链接**  https://arxiv.org/abs/2607.13928v1
- **作者**: Leo Richter, Matt J. Kusner
- **备注**: Accepted at three ICML 2026 workshops, including the ICML Workshop on Technical AI Governance Research
- **摘要**: 举报人是防范组织不当行为的关键保障，但报复的威胁阻碍了举报。现有的举报人保护方案缺乏正式的隐私保证，且现有的差分隐私机制没有直接针对自然的威胁模型——即被审计组织自身观察审计员的选择决定并以此来识别举报人。我们将针对强对手威胁模型的保护形式化为审计选择转录本上针对每条报告的 $(0, δ)$-差分隐私。在此框架内，我们证明了一种自然的方法——在选择步骤应用随机回答（randomized response）——在任何视界（horizon）内都无法比均匀随机审计好过 $δ$。然后，我们提出了一种通用机制，将隐私审计转化为隐私持续计数：任何 $(0, δ)$-DP 持续计数器都可以通过后处理接入，并且审计转录本继承相同的每条报告保证。将该还原方案与最近在持续计数方面的工作结合，在 $T$ 次审计决定的视界中，可以实现噪声按 $O(\sqrt{\log T})$ 缩放的每条报告 $(0, δ)$-DP。效用定理表明，只要最常被举报的组织与第二名之间的噪点报告差距增长快于 $\sqrt{\log T}$，选择误差就会消失。模拟实验显示，相比随机回答，该方法有显著的改进。
- **PDF**: https://arxiv.org/pdf/2607.13928v1

### Frequency Selection in Bayesian Spectral Modeling of Time Series Data with Applications to Wearable Device Measurements
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.15157v1
- **作者**: Beniamino Hadj-Amar, Vaishnav Krishnan, Marina Vannucci
- **备注**: Accepted for publication in the Annals of Applied Statistics
- **摘要**: 本文介绍了一种用于时间序列数据谱分析的贝叶斯脉冲-平板（spike-and-slab）框架。所提方法将频率选择和降维与候选频率的细化网格相结合，能够高分辨率地恢复振荡分量，同时通过结构化的脉冲-平板先验促进稀疏性。随机搜索算法高效地探索后验空间，产生量化每个频率相关性的后验包含概率。我们通过频率包含模式上的分层先验将该框架扩展到多元信号，使模型能够捕获多个时间序列中共享的和特定于分量的节奏。广泛的模拟研究表明，与现有方法相比，该方法在频率估计和谱功率重构中具有鲁棒性和优异的性能。应用于具有部分发作性癫痫个体的活动记录仪（actigraphy）数据时，单变量模型识别出了临床相关的昼夜和超昼夜（ultradian）节律。在第二个应用中，对健康个体的身体活动和皮肤温度进行联合分析，多变量模型揭示了与已知生理耦合一致的、部分重叠的节律分量。这项工作建立了一种强大且可解释的谱分析方法，对可穿戴数据、时间生物学和个性化健康监测具有广泛的适用性。
- **PDF**: https://arxiv.org/pdf/2607.15157v1

--- 
## 📚 学科: `econ.*`

**本周 `econ.*`（经济学）学科总结**：
本周经济学领域探讨了物理学与政治经济学的跨学科交叉。研究者将统计力学中的热力学概念引入选举投票分析，创新性地在非线性振动系统的能量守恒、概率范数与政党得票率之间建立映射，利用瑞利-金斯热化与凝聚原理解释了欧盟选举和法国总统大选中选票的分布规律。这一热力学投票理论不仅能精准拟合代表不平等的洛伦兹曲线与帕累托曲线，也为用统计物理手段剖析社会群体决策行为和政治极化现象开辟了全新的跨学科视角。

### Thermodynamic theory of voting and EU elections
- **分数**: 3
- **链接**  https://arxiv.org/abs/2607.15119v1
- **作者**: Klaus M. Frahm, Dima L. Shepelyansky
- **备注**: 7 pages, 6 figures + 3 pages SupMat with 12 figures, may include certain unpublished parts of arXiv:2512.06420, arXiv:2506.17720, arXiv:2606.17965, arXiv:2607.07315
- **摘要**: 我们引入了一种投票的热力学理论，并表明它能很好地描述欧盟选举中政党选票的分布。该理论在耦合非线性振子系统能量与政党得票率之间建立了平行关系。这种经典系统演化的特征是总能量和概率范数守恒，从而导致低能量状态下的瑞利-金斯（Rayleigh-Jeans, RJ）热化和凝聚。类似的热化也描述了社会中的财富不平等。这一特征属于统计力学中为人熟知的约束驱动凝聚现象。我们展示了 RJ 理论很好地描绘了从欧盟投票结果中获得的洛伦兹曲线和帕累托曲线。该理论还复现了法国第一轮总统选举中候选人之间选票的分散情况。
- **PDF**: https://arxiv.org/pdf/2607.15119v1

---