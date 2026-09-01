# 🗓️ 周报 (2026-W35)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-08-30

--- 
## 📚 学科: `eess.*`
本期 `eess.*`（电气工程与系统科学）学科精选了5篇高质量论文，涵盖了三维目标检测、控制系统信息率优化、传感器标定以及智能电网/工业过程调度等前沿方向。研究成果包括：提出一种任务感知的可变形预测方法（TADP）以提升单阶段三维目标检测性能；探讨了带有辅助信息的局部可观测线性系统的最小信息率优化问题；利用无人机不精确且异步的离散GPS轨迹进行高精度摄像机标定；此外，还有两篇针对工业能源管理的研究，分别提出了用于离散工业过程高效调度的连续RTN建模方法（cRTN），以及用于虚拟电厂（VPP）异构资源最优功率分配的实时运行策略，显著降低了计算开销并提升了经济效益。

### TADP: Task-Aware Deformable Prediction for Single-Stage 3D Object Detection
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27282v1
- **作者**: Su Wang, Yaochen Li, Min Yang, Jiaohao Nie, Chang Liu, Yuehu Liu
- **备注**: Accepted to the 2023 IEEE Intelligent Vehicles Symposium (IV 2023)
- **摘要**: 大多数单阶段三维目标检测器使用相同的提取特征完成不同的任务。然而，将特征投影到一个自适应于所有任务的公共空间中是不可能的。为了解决这个问题，我们提出了一种用于单阶段三维目标检测的新型任务感知可变形预测（TADP）方法。首先，设计了一个三重特征精细化聚合模块来动态提取三级特征。此外，我们设计了多尺度特征聚合模块，以尺度感知的方式融合多尺度特征。最后，利用设计的即插即用任务感知变形头部对每个任务的预测进行变形，它能够感知每个任务的重点和交互作用。我们还设计了三种不同的变形模块。实验结果表明，所提出的变形头部在其他检测方法上表现出了良好的效果。在KITTI数据集上的实验结果表明，汽车平均精度（mAP）达到80.91%，超越了KITTI基准上的许多先进方法。
- **PDF**: https://arxiv.org/pdf/2608.27282v1

### Minimum Rate For Partially Observable Linear System with Side Information: LQG Plant and Gaussian-Markov Source
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.26917v1
- **作者**: Sijie Li, Hyeji Kim
- **备注**: accepted for CDC 2026, full version
- **摘要**: 本文研究了带有辅助信息的局部可观测线性系统所需的最小信息率。我们考虑了线性二次高斯（LQG）对象和高斯-马尔可夫源。我们证明了一类线性策略足以优化条件定向信息下界。我们还表明，对于时变和时不变系统中的标量情况，所得的优化问题是凸的。我们的研究结果推广了以往仅考虑完全或部分观测情况，以及完全观测和辅助信息情况的工作。本文还给出了数值模拟，以说明辅助信息对局部可观测系统的影响。
- **PDF**: https://arxiv.org/pdf/2608.26917v1

### Camera Calibration Using Inaccurate and Asynchronous Discrete GPS Trajectory from Drones
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.26548v1
- **作者**: R. Yang, Y. Bar-Shalom, H. A. J. Huang
- **备注**: 11 pages, 12 figs, published on JAIF
- **摘要**: 本文研究了静止摄像机标定问题，该问题利用无人机记录的GPS轨迹来估计摄像机的偏航角（yaw）、俯仰角（pitch）和翻滚角（roll）。使用GPS轨迹作为摄像机标定的真值面临三个挑战：其一，GPS数据的高度不精确且存在未知的偏差；其二，GPS接收器和摄像机时间不同步，系统之间存在未知的时间偏移；其三，GPS轨迹在时间上是离散的，需要进行精确插值，因为这实际上是一个还需要速度信息的估计问题。针对前两个挑战，我们将该问题表述为一个参数估计问题，以估计包含GPS高度偏差、时间偏移以及摄像机偏航、俯仰和翻滚偏差在内的向量。针对第三个挑战，我们随后开发了一种使用迭代最小二乘算法的特殊极大似然估计器，该估计器可处理非同步的时间离散GPS轨迹。由于摄像机测量误差通常很小，这需要很高的标定精度，因此标定后的残余偏差误差与测量误差标准差相比不应过于显著。标定精度高度依赖于无人机的轨迹。本文还推荐了一种能够产生良好标定精度的合适无人机轨迹（即测量误差标准差的14%）。我们进行了仿真测试以证明该算法的性能，估计结果满足克拉美-罗下界（CRLB），因为相对于CRLB的归一化估计误差平方在统计上是可接受的。
- **PDF**: https://arxiv.org/pdf/2608.26548v1

### Efficient Scheduling of Discrete Industrial Processes Through Continuous Modeling
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.26487v1
- **作者**: Ruike Lyu, Xiangbo Su, Ershun Du, Hongye Guo, Qixin Chen, Chongqing Kang
- **备注**: Published in: IEEE Transactions on Smart Grid ( Volume: 16, Issue: 6, November 2025)
- **摘要**: 资源-任务网络（RTN） model 已广泛应用于表示钢铁制造等复杂工业过程（IP）的技术约束，为工业需求响应奠定了基础。然而，传统的RTN模型包含大量的二进制变量，并且对非灵活和灵活过程应用不同的公式，限制了其计算效率和适用性。为了系统地提高工业过程模型的计算性能，我们提出了一种连续RTN模型（cRTN）。这是一种新颖的建模方法，使用连续变量来表示生产任务和进度，然后将其整合到统一且计算有利的公式中，以应对离散工业过程中的技术约束（包括资源平衡、任务执行、等待时间限制和生产目标）。与传统模型相比，cRTN具有更少的二进制变量、更短的求解时间和更好的可扩展性，同时保持了相同的精度。基于某钢铁厂的数值测试表明，在典型情况下，cRTN的计算速度比传统模型快10倍，并且在批次规模增加时仍能保持可解性（在传统模型中，这会导致问题规模扩大和无法接受的求解时间）。cRTN还通过解决传统模型中报告的舍入误差问题，实现了能源成本的降低。
- **PDF**: https://arxiv.org/pdf/2608.26487v1

### Real-Time Operation Strategy of Virtual Power Plants With Optimal Power Disaggregation Among Heterogeneous Resources
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.26486v1
- **作者**: Qixin Chen, Ruike Lyu, Hongye Guo, Xiangbo Su
- **备注**: Accepted by Applied Energy
- **摘要**: 虚拟电厂（VPP）可以聚合需求侧的柔性资源，为电网提供调频服务，从而帮助应对供需平衡带来的挑战。在部署调频时，VPP会实时地在其内部异构资源之间分解所请求的功率调整。由于资源的随时间耦合特性、调频信号的不确定性以及快速响应的要求，在这一过程中实现最优功率分解具有挑战性。因此，现有的研究主要依赖于启发式方法（如比例分解），未能充分利用多种资源的异构性。在此，我们提出了一种VPP提供调频服务的最优运行策略，通过优先使用低成本资源并考虑时间耦合，来开发异构资源的互补特性。为了减少在线部署的计算开销，我们进一步提出了一种快速分解算法，从而消除了对优化求解器的依赖。我们对由温控负荷和工业生产过程等资源组成的VPP运行进行了案例研究。结果验证了在所提策略下，VPP的运行成本降低、利润增加，且在线计算时间仅需毫秒级。我们相信，我们的工作有助于更好地开发需求侧的灵活性。
- **PDF**: https://arxiv.org/pdf/2608.26486v1

--- 
## 📚 学科: `q-bio.*`
本期 `q-bio.*`（定量生物学）学科精选了2篇具有重要学术价值的研究论文。第一篇论文关注天体生物学，利用高分辨率光照模型和月球表面遥感数据，探讨了月球南极极低温度和紫外线通量区域中微生物生存的可能性，揭示了该区域可能存在利于微生物以隐生状态存活的潜在生态位。第二篇论文结合合成生物学与深度学习，提出了一种集成深度神经网络与大规模并行筛选的框架，用于预测并优化启动子邻近DNA序列，从而显著提升体外转录（IVT）反应中的mRNA产量，为疫苗设计和治疗性蛋白质递送提供了高效的数据驱动方法。

### Potential survivable niches for microbial life on the lunar south pole
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.24751v1
- **作者**: Prabal Saxena, Stefano Bertone, Heather V. Graham, Natalie M. Curran, Aaron B. Regberg, Andrew Needham, D. E., Pugel, Noah E. Petro
- **备注**: 43 pages, 3 figures, 3 tables, Preprint of Science Advances published on Aug. 19, 2026
- **摘要**: 大多数月球表面环境对于微生物的生存来说都极其严酷。高强度的紫外线辐射、极端温度以及高能粒子辐射限制了微生物在大多数无保护的月球表面上的存活，尤其是在此前所有载人探测任务发生赤道地区。然而，考虑到地形效应，这些严酷的条件是否在月球两极广泛存在尚未得到深入研究。在这里，我们通过结合最新的微生物生存数据和月球表面遥感，揭示了月球极地地区可能存在适宜生存的生态位。利用遥感数据和高分辨率光照模型对地形和纬度驱动的表面条件进行分析表明，月球南极拥有大片具有持续低温和低紫外线通量的区域。通过将这些条件与特定微生物的生存数据进行对比，我们发现显著的月球极地区域可能具有适合微生物生存的表面条件。我们的发现表明，月球极地地区对微生物生存的敌意可能比以前认为的要低。这不包括生长的可能性，而是指在隐生状态（cryptobiotic state）下的生存，如果存在宜居条件，在这种状态下生长将成为可能。鉴于在计划进行的众多近期任务中，许多被检测的微生物可能会在载人月球南极探测期间被带到月球上，因此月球极地的潜在微生物生存能力显得尤为重要。深思熟虑地规划探测并追踪其影响是限制和了解可能发生的意外生命向月球转移的关键。
- **PDF**: https://arxiv.org/pdf/2608.24751v1

### Optimizing RNA yield using deep neural networks coupled to massively parallel screening
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.23722v1
- **作者**: Dinghai Zheng, Justin Hong, Jun Wang, Adrien Villain, Mickaël Costallat, Fernando Ulloa Montoya, Vikram Agarwal
- **备注**: Accepted at the CIBB 2026 conference (https://cibb2026.teralab.ai/)
- **摘要**: 基于信使RNA（mRNA）的疗法已成为疫苗、蛋白质替代疗法和癌症免疫疗法的强大平台。mRNA开发中的一个关键瓶颈是以经济的方式制造大量的RNA（以体外转录（IVT）反应产生的RNA产量衡量）。然而，启动子邻近的DNA序列如何影响RNA产量仍不清楚。在此，我们提出了一个集成的深度学习框架，该框架利用大规模并行下一代测序（NGS）技术在庞大的序列空间中测量RNA产量。我们设计了一个包含10^5个随机寡核苷酸序列的文库，以系统地探索在特定结构背景下的序列多样性。利用Illumina测序技术并行量化了DNA和RNA的丰度，从而实现了序列与产量关系的大规模高分辨率测量。研究人员对这些序列进行了独热编码，并用于训练基于卷积神经网络架构的深度学习模型。该模型在预留的测试集上，预测的RNA产量与实验测量的RNA产量之间的皮尔逊相关系数达到了0.94，展现出在不同序列背景下的强大泛化能力。重要的是，训练好的模型可以部署在生产环境中，对新型RNA序列设计的预测IVT产量进行评分和排序，从而实现高性价比、实验前的最易制造候选物优先级排序。该框架建立了一种可扩展的、数据驱动的DNA和RNA序列优化方法，广泛适用于疫苗抗原设计、治疗性蛋白质递送和合成生物学。通过将高通量实验与先进的深度学习建模相结合，该方法显著降低了筛选成本，并缩短了RNA工程周期。
- **PDF**: https://arxiv.org/pdf/2608.23722v1

--- 
## 📚 学科: `cs.*`
本期 `cs.*`（计算机科学）学科精选了5篇已被顶级会议或期刊（如EMNLP, ECCV, RA-L, ISSTA）接收的高水平论文。研究内容非常多元且前沿：在自然语言处理方面，提出了D2C-Routing方法，用于识别混合来源的AI生成文本；在三维计算机视觉领域，MILO框架利用大型重建模型（LRM）实现了单张图像的高精度人机交互三维重建；在具身智能领域，引入了全新的具身场景重排规划（ESRP）任务和基准测试；在软件工程方面，推出了首个多轮代码审查基准测试MCR-Bench，以评估大语言模型在动态缺陷状态感知下的表现；最后，在算法理论方面，探索了利用马尔可夫决策过程解决经典罗宾斯问题（秘书问题变体）的高效近似方法。

### D2C-Routing: Dimension-to-Composition Evidence Routing for Mixed-Origin AI-Generated Text Detection
- **分数**: 7
- **链接**  https://arxiv.org/abs/2608.27380v1
- **作者**: Xin Chen, Fuwei Zhang, Yiqi Tong, Wei Guo, Yutian Xiao, Fuzhen Zhuang
- **备注**: 17 pages, 4 figures. To appear in EMNLP 2026
- **摘要**: AI生成文本检测通常被构建为关于文本是人类撰写还是机器生成的二分类文档级判断。这种构建方式在面对混合来源写作（即内容来源和表达来源可能不同的情况）时会失效。我们将混合来源检测视为“维度到组合”的来源归属问题，即在将内容来源和表达来源组合成四种协作类型之前，先对它们进行推断。我们提出了“维度到组合路由”（D2C-Routing）方法，它将内容侧和表达侧的证据路由到受监督的维度头部，然后通过学习到的门控组合层预测最终标签。在源自HART混合来源基准的重建划分数据集MixD2C上，我们公开的基于D2C-Routing的检测器系统达到了0.8603的四分类平均真阳性率（在1%假阳性率下，Avg TPR@1%FPR），比相同划分的RACE-local重运行结果高出6.5个百分点。核心消融实验支持了路由设计，而误差分析表明，区分“AI内容/人类表达”与“完全AI生成的文本”仍然是最困难的边界。代码可在 https://github.com/bystander563/d2c-routing-artifact 获取。
- **PDF**: https://arxiv.org/pdf/2608.27380v1

### Reconstructing Humans and Objects in Interaction using Large Reconstruction Models
- **分数**: 4
- **链接**  https://arxiv.org/abs/2608.27407v1
- **作者**: Agniv Chatterjee, Georgios Pavlakos
- **备注**: Accepted at ECCV 2026. Project Page: https://ac5113.github.io/MILO
- **摘要**: 三维人机交互（3D HOI）估计是三维计算机视觉中的一个基本问题，在AR/VR、机器人技术和具身智能中都有应用。然而，由于深度歧义、遮挡和物体形状的多样性，在三维空间中重建这些交互仍然具有挑战性。现有的方法主要关注重投影和接触约束，将参数化人体模型和物体模板拟合到二维图像。在本文中，我们探索了一条不同的途径。我们提出了MILO框架，该框架利用大型重建模型（LRM）的视觉能力，从单张图像中恢复详细的三维人机交互。我们的核心观察是，LRMs提供了一个强大的几何支架，保留了人与物体的相对排列和邻近线索。这显著简化了重建过程，将问题重新表述为对LRM网格的解释：我们将其分割为人类和物体部分，将参数化身体模型拟合到人类部分，并（在有模板的情况下）可选地将物体模板对齐到物体部分。MILO在多个基准测试和交互场景中取得了极高的重建精度，并超越了现有的基线方法。我们的代码可在 https://ac5113.github.io/MILO 获取。
- **PDF**: https://arxiv.org/pdf/2608.27407v1

### Embodied Scene Rearrangement Planning
- **分数**: 4
- **链接**  https://arxiv.org/abs/2608.27371v1
- **作者**: Canzhi Chen, Zan Wang, Siqi Zhu, Qi Wu, Yixuan Li, Wei Liang
- **备注**: Accepted for publication in IEEE Robotics and Automation Letters (RA-L), 2026. Project page: https://bit-pie.github.io/ESRP/ Code: https://github.com/BIT-PIE/ESRP Dataset: https://huggingface.co/datasets/serendipity800/ESRP-PD
- **摘要**: 本文引入了具身场景重排规划（ESRP），这是一项全新的任务，要求具身智能体仅使用自我中心观测和自顶向下的目标布局，重新排列三维场景中的家具以匹配目标配置。与先前的重排任务不同，ESRP排除了全局状态访问并引入了物体间的相互遮挡，这反映了现实世界机器人部署的实际约束。这些因素使得将局部的自我中心观测与全局目标布局对齐，在长程规划中变得尤为困难。为了促进研究，我们展示了基于OmniGibson构建的综合基准ESRP-Bench，其中包含5400多个场景对和8200个物体。我们定义了三个多层级指标来评估重排质量，并提供了四种基线方法：分层任务与运动规划方法、基于视觉语言模型的方法以及两种基于学习的方法（模仿学习IL和强化学习RL）。实验结果表明，当前的方法难以高效地完成该任务，这凸显了ESRP是具身智能体在场景理解和长程任务规划领域中极具挑战性的前沿课题。这项工作为在现实场景中部署智能代理奠定了基石。项目主页：https://pie-lab.cn/ESRP/。
- **PDF**: https://arxiv.org/pdf/2608.27371v1

### From Static to Dynamic: Benchmarking Real-World Code Review with MCR-Bench
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27442v1
- **作者**: Dewu Zheng, Yanlin Wang, Xiwen Wang, Kefeng Duan, Hongyu Zhang, Xilin Liu, Yuchi Ma, Zibin Zheng
- **备注**: Accepted at ISSTA 2026
- **摘要**: 在现实世界的软件开发中，代码审查通常涉及开发人员和审查人员之间的迭代交互，以提高软件质量，这使得该过程成本高昂且耗时。尽管近期的工作探索了使用大语言模型（LLM）进行自动代码审查，但大多数方法将代码审查过度简化为单轮静态决策任务，这无法捕获现实审查场景中固有的多轮交互性质和复杂的解题过程。为了弥补这一差距，我们引入了MCR-Bench，这是首个专为现实多轮代码审查设计的缺陷状态感知基准。MCR-Bench涵盖了五种常用的编程语言，包含2269个真实的多轮代码审查任务，每个任务都标注了细粒度的缺陷信息和跨轮状态标签。MCR-Bench中的每个任务都配备了细粒度的缺陷元数据（例如描述、类型、严重程度）以及动态状态标注，捕获了缺陷在整个多轮过程中的完整演变轨迹。我们通过在MCR-Bench上使用主流LLM进行广泛的实验，获得了以下几点发现：（1）整体能力有限：实验表明，主流LLM在缺陷检测和缺陷生命周期状态跟踪方面的整体表现有限，且随着交互轮数的增加，性能显著下降；（2）缺陷敏感性：LLM的性能在不同缺陷类型和严重程度水平上差异巨大，语义复杂或显著性低的缺陷明显更容易被遗漏；（3）潜在失效机制：我们的深度错误分析剖析了导致误报和漏报的不同驱动因素，揭示了跨轮时间不匹配和长程记忆不足等关键缺陷。
- **PDF**: https://arxiv.org/pdf/2608.27442v1

### Algorithms for Robbins' Problem using Markov Decision Processes
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27419v1
- **作者**: Léonard Brice, F. Thomas Bruss, Anirban Majumdar, Jean-François Raskin
- **备注**: Extended version of article published in Principles of Verification
- **摘要**: 在本文中，我们研究了罗宾斯问题（Robbins' problem），它是著名的秘书选择问题的一个完全信息变体。在这个版本的问题中，目标是最小化在按顺序面试的 $n$ 个候选人中被选中者的期望排名，并且必须在面试结束后立即做出是否选择第 $m$ 个候选人的决定（因此无法看到后面的 $n-m$ 个候选人，且不能反悔）。我们首先展示了如何将罗宾斯问题的实例建模为无限马尔可夫决策过程（MDP）。然后，我们提出了这些MDP的几种有限状态抽象方法，使我们能够近似固定 $n$ 下该问题的价值。虽然已知以往候选人价值的完整记忆对于实现最优期望排名最小化是必需的（这使得该问题的分析极具挑战性），但我们指出，简单的记忆结构足以获得接近最优的选择策略。此外，我们提供了候选人人数 $n$ 高达100的罗宾斯问题的近似值，此前对于这些情况尚无良好的近似值（确切价值仅在 $n \leq 4$ 的实例中已知，且数值近似仅适用于不超过个位数的极小 $n$ 值）。对于所有 $n : 5 \leq n \leq 100$，我们给出了比以往已知的更好的近似值。
- **PDF**: https://arxiv.org/pdf/2608.27419v1

--- 
## 📚 学科: `math.*`
本期 `math.*`（数学）学科精选了1篇关于应用概率与决策理论的代表性论文。该研究聚焦于经典的罗宾斯问题（Robbins' Problem）——一种全信息的秘书选择问题变体，旨在最小化顺序面试中选择候选人的期望排名。作者通过将罗宾斯问题的实例建模为无限状态马尔可夫决策过程（MDP），并提出了一系列有限状态抽象方法，成功实现了对固定候选人数下问题价值的逼近。该工作设计了简单的记忆结构，在保证策略接近最优的同时，首次为多达100个候选人的罗宾斯问题提供了极佳的数值近似，突破了以往研究仅能处理个位数候选人的局限。

### Algorithms for Robbins' Problem using Markov Decision Processes
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27419v1
- **作者**: Léonard Brice, F. Thomas Bruss, Anirban Majumdar, Jean-François Raskin
- **备注**: Extended version of article published in Principles of Verification
- **摘要**: 在本文中，我们研究了罗宾斯问题（Robbins' problem），它是著名的秘书选择问题的一个完全信息变体。在这个版本的问题中，目标是最小化在按顺序面试的 $n$ 个候选人中被选中者的期望排名，并且必须在面试结束后立即做出是否选择第 $m$ 个候选人的决定（因此无法看到后面的 $n-m$ 个候选人，且不能反悔）。我们首先展示了如何将罗宾斯问题的实例建模为无限马尔可夫决策过程（MDP）。然后，我们提出了这些MDP的几种有限状态抽象方法，使我们能够近似固定 $n$ 下该问题的价值。虽然已知以往候选人价值的完整记忆对于实现最优期望排名最小化是必需的（这使得该问题的分析极具挑战性），但我们指出，简单的记忆结构足以获得接近最优的选择策略。此外，我们提供了候选人人数 $n$ 高达100的罗宾斯问题的近似值，此前对于这些情况尚无良好的近似值（确切价值仅在 $n \leq 4$ 的实例中已知，且数值近似仅适用于不超过个位数的极小 $n$ 值）。对于所有 $n : 5 \leq n \leq 100$，我们给出了比以往已知的更好的近似值。
- **PDF**: https://arxiv.org/pdf/2608.27419v1

--- 
## 📚 学科: `astro-ph.*`
本期 `astro-ph.*`（天体物理学）学科精选了5篇已被ApJ、A&A和MNRAS等顶尖天文学期刊接收的论文，主要聚焦于恒星演化、原行星盘动力学以及系外行星宜居性。研究成果包括：利用詹姆斯·韦布空间望远镜（JWST）对五个碎片盘系统进行多色日冕仪成像，揭示了水冰的存在及其径向分布；通过流体动力学模拟研究了真实尘埃粒径分布对低质量行星迁移的尘埃力矩影响；构建了12颗邻近低质量和类日恒星的全波段光谱能量分布（SED），为评估其宜居带内行星的大气保持能力提供依据；对四重原恒星系统VLA1623的生存能力进行了N体模拟；以及利用NGTS测量了七个年轻疏散星团中恒星的自转周期分布，加深了对恒星自转演化的理解。

### The JWST/NIRCam Scattered Light Disks GTO 2780 program: panchromatic coronagraphic imaging of the HD 10647, HD 32297, HD 61005, HD 107146, and HD 181327 debris disk systems
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27437v1
- **作者**: András Gáspár, Jarron M. Leisenring, Schuyler Grace Wolff, Kellen Lawson, George H. Rieke, Dingshan Deng, Marcia J. Rieke, Antranik A. Sefilian, Charles Beichman, Joshua B. Lovell, John Krist, Marie Ygouf, Jorge Llop-Sayson, Geoffrey Bryden, Christopher C. Stark, Christine H. Chen
- **备注**: 52 pages, 42 figures, accepted for publication in ApJ
- **摘要**: 碎片盘由岩石、巨石、微行星以及它们碰撞产生的尘埃组成，是成熟行星系统中最容易观测到的组成部分。它们也是极有价值的诊断工具，能够用于研究行星的动力学相互作用和矿物组成。在从光学到无线电波段的观测中，每个波段都能揭示关于尘埃群的独特信息。光学和近红外观测对从微米级颗粒表面散射的光尤为敏感。在此，我们展示了来自JWST/NIRCam GTO计划2780的研究结果，该计划旨在利用NIRCam冠状仪的六个滤光片，观测五个先前在光学波段被发现异常明亮的碎片盘系统（HD 10647, HD 32297, HD 61005, HD 107146 和 HD 181327）。NIRCam的数据对这些系统先前较短波段的图像进行了补充。这些数据以高分辨率和高信噪比展示了来自盘体以及在辐射力影响下由微小颗粒构成的延伸晕圈的散射光。所有系统都显示出存在水冰的证据，尽管水冰可能具有不同的径向分布，并且在晕圈中往往表现出更强的特征。在我们可以分析的两个案例中，盘中的散射相位函数与太阳系中尘埃的行为相似，并有证据表明晕圈中的前向散射有所增强，这与晕圈由微小颗粒组成的假设相一致。两个系统的MIRI图像比短波段图像更加向中心集中，表明被拖入的较大颗粒发挥了作用。
- **PDF**: https://arxiv.org/pdf/2608.27437v1

### Dust torques for realistic dust size distributions
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27353v1
- **作者**: V. Roatti, G. Picogna, F. Marzari
- **备注**: Accepted for publication in Astronomy & Astrophysics
- **摘要**: 先前的研究表明，具有固定斯托克斯数（Stokes number）的尘埃颗粒群可以对嵌入在原行星盘中的低质量行星产生实质性的力矩，从而改变其迁移率。我们的目标是表征在真实的尘埃颗粒尺寸分布下，低质量行星所受到的尘埃力矩。我们使用PLUTO代码，并加入代表尘埃动力学的拉格朗日超级粒子，对行星与原行星盘的相互作用进行了二维流体动力学模拟。我们应用了基于能量的准则来排除引力绑定在行星上的粒子，以防止环行星流干扰力矩的测量。我们发现，尘埃力矩主要由尺寸分布中最大的颗粒主导，并且对最大颗粒尺寸高度敏感。对于典型的原行星盘条件，对于弱耦合的颗粒（$\mathrm{St} \gtrsim 10^{-2}$），力矩变为正值，并且在存在厘米级卵石（pebbles）的情况下可以超过气体力矩，从而导致低质量行星向外迁移。与先前的研究不同，在探索的 $α= 10^{-4}$ 到 $3\times 10^{-3}$ 范围内，湍流尘埃扩散对力矩的影响可以忽略不计。最主要的贡献来自行星希尔球内部，这突出了高空间分辨率和粒子轨迹精确积分的必要性。我们推导出了尘埃力矩作为最大颗粒尺寸和行星质量函数的标度律，适用于群体合成模型。
- **PDF**: https://arxiv.org/pdf/2608.27353v1

### Panchromatic Spectra of Nearby Low-mass and Sun-like Stars with Directly Imageable Habitable Zones
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27344v1
- **作者**: Sarah Peacock, Breanna A. Binder, Edward W. Schwieterman, Margaret C. Turnbull, Stephen R. Kane, Katherine Garcia-Sage, Alison Farrish
- **备注**: 29 pages, 8 Figures, 7 Tables, accepted to ApJ
- **摘要**: 表征恒星的高能辐射环境在确定哪些系统的行星能够保留大气层并维持宜居条件方面起着至关重要作用。从X射线到紫外线（UV）的辐射驱动着行星大气的化学反应、加热和逃逸，这使得精确表征恒星高能辐射对于解释未来的系外行星观测和确定最有前景的生命探测目标至关重要。我们为12颗邻近的、具有可直接成像宜居带的低质量和类日恒星构建了跨越X射线到无线电波段的全波段光谱能量分布（SEDs），这些恒星是宜居世界天文台（HWO）和极大望远镜（ELTs）的优先观测目标。这些SED是利用现有的归档X射线和紫外线观测数据作为指导和约束，通过前向恒星大气模型生成的。我们发现，与现代太阳相比，该样本中的许多恒星表现出更强的高能辐射环境，其宜居带的X射线和极紫外（XUV）通量频繁超出太阳数值1到2个数量级。这种偏高的辐射可能反映了样本选择效应、恒星年龄和自转的差异，以及内在磁场活动变化的综合影响，而多周期观测表明，仅活动性变化本身就能显著改变推导出的辐射环境。这些结果强调了高能辐射是识别最有望孕育宜居行星的宿主恒星的重要判据，并表明需要扩大X射线和紫外线观测，以完成对HWO目标进行优先级排序所需的恒星特征表征。
- **PDF**: https://arxiv.org/pdf/2608.27344v1

### Exploring the survivability of higher-order multiple protostellar systems -- The case of VLA1623
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27294v1
- **作者**: N. M. Murillo, A. Pérez-Villegas
- **备注**: 11 pages, 3 figures. Accepted for publication in MNRAS (Accepted 2026 August 27. Received 2026 August 27; in original form 2025 December 17)
- **摘要**: 在低质量恒星形成的早期阶段，通常能观测到高阶原恒星系统（$\geq$3个成员）。在恒星形成和演化中一个持久的问题是，这些高阶原恒星系统是作为引力绑定的系统存活下来，还是随着时间的推移瓦解为双星。我们以嵌入式四重原恒星系统VLA1623及其观测约束为例研究了这个问题，假设其成员A1、A2、B和W是引力绑定的。利用N体模拟，我们运行了一组考虑引力、原恒星上的质量吸积、原恒星云核的存在及其驱散的网格模型。模拟在一个8百万年（Myr）的时间段内进行积分，以考虑从原恒星阶段（0类和I类，1 Myr），经过主序前阶段（II类和III类，2-3 Myr），并进入主序星阶段（4 Myr）的演化。我们的结果表明，从当前状态算起，VLA1623有30%的概率在长达8 Myr的时间内保持为引力绑定的四重系统。VLA1623也有25-30%的概率瓦解为一个三重系统。这表明，四重原恒星系统的瓦解促进了稳定的三重（原）恒星系统的形成。成员A1和A2最有可能被抛射，而W被抛射出系统的概率较低。VLA1623的稳定性取决于成员相对于主星的质量比、间距以及偏心率的综合作用。
- **PDF**: https://arxiv.org/pdf/2608.27294v1

### NGTS clusters survey - VI: Stellar rotation in seven young open clusters within the PLATO LOPS2 field
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27170v1
- **作者**: Alexander Hughes, Edward Gillen, Matthew Battley, Deepak Chahal, Beatrice Caccherano, David Anderson, Ioannis Apergis, Daniel Bayliss, Matthew Burleigh, Jorge Fernández Fernández, Michael Goad, George Harvey, James S. Jenkins, Alicia Kendall, James McCormac, Jose Moyano, Gavin Ramsay, Suman Saha, Jose Vines, Richard G. West, Peter J. Wheatley
- **备注**: 21 pages, 10 figures, Accepted by MNRAS
- **摘要**: 我们展示了NGTS对PLATO首个长期凝视LOPS2场内、年龄跨度约为40至700 Myr的七个年轻疏散星团中FGKM型恒星自转周期分布的测量结果。我们测定了1063个自转周期，其中479个作为星团特定自转研究的一部分进行了新分析，而有63个周期是最近的TESS全天自转巡天中未曾报道的独特周期。在1063个自转周期中，有285个利用色振图和Gaia天体测量学被识别为可能的联星或更高阶的多星系统。这些是Trumpler 10、NGC 2451B和Alessi 3的首个全面自转周期分布，同时扩展了NGC 2451A、NGC 2516、Collinder 135和IC 2391的现有分布，从而对PLATO LOPS2场中年轻恒星的自转状态描绘出更完整的图像。我们发现，在年龄约为40 Myr的年轻星团NGC 2451B中，主序太阳质量恒星形成了一条可以与其在约70-80 Myr的对应恒星相区分的慢自转序列，从而显著降低了可以通过自转序列对年轻恒星群进行相对测年的年龄下限。我们还观察到，从NGC 2451A的年龄到至少NGC 2516的年龄（~70-150 Myr），在质量 $\gtrsim1$ $M_{\odot}$ 的恒星中存在停滞的自转减速现象，这支持了先前的预测，即角动量重新分配和移除应该会导致一波随着质量和年龄而传播的停滞自转减速。最后，我们利用微分陀螺年代学测年法，提供了Alessi 3的新年龄估计值，为687$\pm$106 Myr。
- **PDF**: https://arxiv.org/pdf/2608.27170v1

--- 
## 📚 学科: `stat.*`
本期 `stat.*`（统计学）学科精选了5篇优质论文，重点展示了统计方法与机器学习、推荐系统以及不确定性量化的结合。内容包括：基于预测驱动推理（PPI）提出一种结合人工判断与自动评分的评估框架，并引入新指标度量节省人工标注的比例；构建基于声学分布的音乐艺术家邻接关系 recover 机制，验证了专家乐评数据的建构效度；针对多步信道状态信息（CSI）预测，提出了一种轨迹自适应共形风险控制方法（TRACE-CRC），实现了可靠的轨迹级不确定性量化；针对不完全先验下的逆问题，开发了主动扩散推断求解器；最后，利用因果模型优化增量推荐，在减少推荐曝光的同时保持了用户消费体验。

### Which Metrics Save the Most Human Annotation? Prediction-Powered Evaluation and Meta-Evaluation
- **分数**: 6
- **链接**  https://arxiv.org/abs/2608.26638v1
- **作者**: Mingqi Gao, Anthony Sicilia, Weiyan Shi
- **备注**: Accepted at EMNLP 2026 (Main). Code available: https://github.com/CHATS-lab/ppi-eval
- **摘要**: 在各种无法验证的任务中，人工评估可靠但昂贵，而自动评估指标更具扩展性但往往存在偏差。基于预测驱动推理（PPI），我们提出了“预测驱动评估”（prediction-powered evaluation），这是一个将有限的人工判断与大规模自动评分相结合的框架，以获得可证明无偏的数据高效系统比较。我们开发了参数和非参数流程，分析了配对和非配对设计之间的效率折衷，并在六个WMT数据集上验证了该框架。我们还引入了“预测驱动节省率”（PPSR）这一元指标，用于衡量在预测驱动评估中使用自动指标时可以节省多少人工标注。PPSR直接针对自动指标在预测驱动评估中的实用性，并能产生比现有系统级元指标更具区分度和稳定性的指标排名。总体而言，我们的新范式将自动评估指标重新定位为减少人工标注成本的工具，而非取代人类判断，并广泛适用于无法验证的任务。
- **PDF**: https://arxiv.org/pdf/2608.26638v1

### Recovering Expert Critic-Sourced Network Adjacency between Musical Artists from Acoustic Distributions: A Construct-Validity Approach
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27291v1
- **作者**: Elena Badillo-Goicoechea, Fengfeng He
- **备注**: Accepted workshop paper at USR Workshop, RecSys, 2026, Minneapolis, MN, USA
- **摘要**: 音乐推荐主要依赖于两种信号：用户-物品交互（在冷启动情况下会失效）以及固有的音乐内容（任何音视频记录都具有该信号）。我们认为，第三种很大程度上尚未被开发的信号不仅更丰富，也更有原则：即评论家邻接关系（critical adjacency）——指专家评论家在长篇散文中明确将两位艺术家联系起来时所建立的配对关系。它编码了关于哪些艺术家属于同一类别的深思熟虑的判断。先前的工作确立了其内部效度，表明它能够恢复出连贯、可解释的社群，并且在无用户数据的情况下，在用户满意度模拟中能够达到协同过滤的效果。目前所缺失的是外部验证：即这种源自评论家的关系是否根植于音乐本身，而非仅仅基于社会学背景。我们对照声学内容测试了这一关系，将其重新表述为建构效度（construct validity）问题。我们将艺术家表示为在80个低级Essentia声学描述符上的经验分布，并通过边缘最优传输（Wasserstein）距离对成对相似度进行建模，进而评估在冷启动、艺术家不交叉划分下，评论家邻接关系在多大程度上可通过声学内容进行恢复。我们的集成模型在外推AUC上恢复了这些边，达到0.767（95%置信区间为0.761-0.775）。可恢复性随着评论家共识的增加而单调上升，在多源证实的边上达到了0.865。分层评估与流派的社会学模型相吻合：界限紧密的、基于特定场景的流派显示出比宽泛的行业概括性词汇更高的可恢复性。因此，评论家的话语是推荐系统信息的丰富来源，可分解为可重现的“声学核心”和由叙事定位、亚文化背景及经典定位驱动的“社会学剩余”。该工作为音乐信息检索（MIR）和音乐推荐系统（MRS）研究提供了一种可扩展的冷启动发现机制和一种植根于社会学的方法。
- **PDF**: https://arxiv.org/pdf/2608.27291v1

### TRACE-CRC: Trajectory-Adaptive Conformal Risk Control for Multi-Step Channel State Information Prediction
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27124v1
- **作者**: Kiarash Rezaei, Mehdi Sattari, Javad Aliakbari, Tommy Svensson, Paolo Monti, Carlos Natalino
- **备注**: Published in Proceedings of Machine Learning Research (PMLR), volume 329, Conformal and Probabilistic Prediction with Applications (COPA 2026)
- **摘要**: 时变信道状态信息（CSI）的可靠预测对于高效的无线通信至关重要。每个CSI帧是无线信道响应的矩阵值表示，而一串CSI帧构成了时间信道轨迹。然而，现代基于深度学习的CSI预测器通常仅提供点预测，缺乏校准后的不确定性估计。这种局限性在多步CSI预测中尤为棘手，因为其目标是未来CSI矩阵的序列，如果预测轨迹的任何部分不可靠，下游决策（如波束成形或调度）都可能会失败。我们提出了“轨迹自适应校准与误差剖析共形风险控制”（TRACE-CRC），这是一种在多步CSI预测中进行轨迹感知不确定性量化的方法。TRACE-CRC在预测的CSI矩阵周围构建Frobenius范数不确定性球，并控制至少一个未来帧未被覆盖的风险。TRACE-CRC没有独立校准每个未来步骤，而是结合了依赖于未来步骤的误差剖析、轨迹难度分层以及“先学习后测试”（LTT）风险控制。实证表明，TRACE-CRC以比保守的多步修正小得多的不确定性球实现了可靠的轨迹级覆盖，同时避免了紧凑逐步和自适应共形基线方法的轨迹欠覆盖问题。
- **PDF**: https://arxiv.org/pdf/2608.27124v1

### Active Diffusion-Based Inference for Ill-Posed Inverse Problems under Incomplete Priors
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.27080v1
- **作者**: Jitao Xu, Nobuo Sato, Yaohang Li
- **备注**: Accepted for publication in the Proceedings of IJCAI-ECAI 2026
- **摘要**: 许多科学和工程应用需要从实验可观测数据中估计未知参数——由于非线性、噪声和病态性，这是一个本就极具挑战性的逆问题。在本文中，我们提出了一种基于主动扩散的逆问题求解器。研究人员训练了一个扩散模型（DM）来学习参数空间与可观测空间之间的映射关系。通过利用后验不确定性迭代检测和纠正模型失配，该方法发现并学习了参数空间的正确区域，即使初始训练边界排除了真实参数。这为不完全先验知识下的逆问题提供了原则性的、贝叶斯合理的自适应定义域扩展，并确保了鲁棒的推断。我们展示了该逆问题求解器在一个具有无限解的玩具逆问题中的有效性，以及在核子结构量子色动力学分析中，将量子相关函数参数化为事件可观测量的有效性。
- **PDF**: https://arxiv.org/pdf/2608.27080v1

### Incremental Recommendation via Causal Models
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.26804v1
- **作者**: Athanasios Vlontzos, David Gustafsson, Michael O'Riordan, Ciarán M. Gilligan-Lee
- **备注**: Accepted at the CONSEQUENCES Workshop @ RecSys'26
- **摘要**: 推荐曝光是一项有限的资源，因此将推荐内容推送给原本会自然（有机地）发现该内容的用户，并不会产生增量价值，反而会挤占其他原本能产生价值的推荐空间。为了解决这个问题，我们利用已经作为常规实验基础设施收集的对照组（holdback）数据，将现有的生产环境推荐模型扩展为因果架构，从而无需收集新数据。一个核心挑战是，处理组和对照组观测之间的归因窗口不同：处理组用户在很短的直接响应窗口内被归因推荐流，而对照组用户则在多天的窗口内被归因自然流。这种不匹配使得单纯的处理效应相减失效。我们通过双阈值定向策略解决了这一问题，该策略仅在处理流概率高且自然流概率低时才进行推荐推送。在针对数百万Spotify用户的大规模生产环境A/B测试中，该策略在不显著减少推荐内容总消费量的情况下，将推荐曝光减少了7%。我们进一步表明，结合对照组数据进行联合训练提高了处理头相对于生产基线的校准度，并认为这可以作为因果模型比仅在观测数据上训练的模型能够学习到更具泛化性表征的证据。
- **PDF**: https://arxiv.org/pdf/2608.26804v1

--- 
## 📚 学科: `econ.*`
本期 `econ.*`（经济学）学科精选了1篇已被顶级期刊《欧洲经济评论》（European Economic Review）有条件接收的高质量跨学科研究论文。该研究探讨了国家文化对宪法合规性（constitutional compliance）的影响，填补了 formal constraints 在不同社会中有效性差异的理论空白。通过对115个国家的跨国数据分析及工具变量估计，研究发现，个人主义程度较高的社会展现出更高的宪法合规水平。这一发现揭示了一条从文化特质到长期经济增长的新型传导机制：个人主义文化增强了宪法自我承诺的公信力，同时也证明了正式制度的成效高度依赖于其所嵌入的非正式制度环境。

### Culture and constitutional compliance
- **分数**: 3
- **链接**  https://arxiv.org/abs/2608.23369v1
- **作者**: Jerg Gutmann, Anna Lewczuk-Czerwińska, Jacek Lewkowicz, Stefan Voigt
- **备注**: Conditionally accepted in European Economic Review
- **摘要**: 宪法作为一个国家法律和政治系统的正式基础，具有重要的经济和政治影响。然而，关于为什么宪法在某些社会中能够对政治家设置有效的约束，而在其他社会中却基本上被忽视，我们仍然知之甚少。在本文中，我们探讨了国家文化是否对宪法合规性（constitutional compliance）有所影响。我们利用全新的宪法合规性指标，对115个国家的跨国数据进行了研究。我们发现，个人主义程度较高的社会展现出更高的合规水平。这些结果是鲁棒的，并且可以推广到工具变量估计中。它们意味着一条从文化特质到长期经济增长的新型传导路径：个人主义的国家文化增强了宪法自我承诺的公信力。我们的分析还支持了一个更具普遍性的观点，即正式制度的作用取决于其所嵌入的非正式制度环境。在宗教方面，我们的结果与以往的研究一致，这些研究将现代伊斯兰世界发展不足归因于制度质量的缺陷。
- **PDF**: https://arxiv.org/pdf/2608.23369v1

---