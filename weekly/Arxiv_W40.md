```markdown

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
# 🗓️ 周报 (2026-W40)
> 更新时间: 2026-10-04

--- 
## 📚 学科: `eess.*`
### Port-Hamiltonian Neural Networks for Systems with Multiple Asymptotically Stable Equilibria
- **分数**: 6
- **链接**  https://arxiv.org/abs/2610.01356v1
- **作者**: Simon Heilig, Jens Püttschneider, Mohammad Itani, Asja Fischer, Timm Faulwasser
- **备注**: Accepted at NeurIPS 2026 Workshop: AXIOM - Foundations of Efficient Deep Learning
- **摘要**: 稳定的端口-哈密顿神经网络在构建上保证了渐近稳定性。然而，它们的哈密顿量是一个具有单一全局最小值的全局李雅普诺夫函数，因此它们只能表示具有一个吸引子的动力学系统。我们证明了这排除了即使是具有形成双阱能量景观的简单系统，并且我们通过将哈密顿量参数化为由一个输入凸网络生成的 Bregman 散度的乘积来克服这一限制。我们证明了所得模型具有局部李雅普诺夫稳定性，稳定平衡态的共存迫使其他非渐近稳定平衡态存在，所有平衡态都位于一个有界区域内，并且在双曲性假设下，几乎处处稳定性成立。在三个系统上，我们的方法能够恢复能量表面特征并将收敛速度提高 1.8 至 8.5 倍。
- **PDF**: https://arxiv.org/pdf/2610.01356v1

### MDIRNET: Multi-Degradation Image Restoration Network via Deep Unfolding
- **分数**: 4
- **链接**  https://arxiv.org/abs/2610.01655v1
- **作者**: Talha Nadeem, Arslan Majal, Muhammad Tahir, Khurram Ali
- **备注**: Accepted for publication in IEEE Transactions on Instrumentation and Measurement (IEEE TIM), 2026
- **摘要**: 真实图像通常表现出未知的混合退化，由于在同一观测中多种失真类型相互作用，使得恢复比单任务图像恢复更具挑战性。因此，现有方法通常依赖于退化类型的先验知识或单独的特定任务模型，这可能会过度平滑精细结构或留下残留伪影，从而激发了一种紧凑的模型驱动替代方案。我们提出了多退化图像恢复网络（MDIRNET），这是一个将模型驱动的低秩先验与端到端学习相结合的统一框架。在这里，“统一”是指对三种退化类型（噪声、雨水和模糊）进行联合训练。单个 MDIRNET 模型可以恢复所有这三种退化，在推理时不需要特定任务的模型、模块或分支。低秩先验利用了自然图像块的冗余和紧凑结构。为了确定这种底层的低维表示，我们通过正交变分 PCA (OVPCA) 将恢复公式化，并将其迭代推理转化为深度展开网络。为了处理空间非均匀损坏和局部内容变化，我们还引入了一种可学习的块划分策略和一个轻量级的动态秩分配模块，该模块预测每个区域的适当子空间维度。使用监督注意力模块进行空间自适应重建细化。在标准去噪、去模糊和去雨基准测试上的广泛实验表明，MDIRNET 在大多数指标上均达到了与强基准相当或更优的性能，而受控的混合退化实验表明，在评估的合成退化组合中性能一致。代码可在 https://github.com/ScholarForge/mdirnet.git 获得。
- **PDF**: https://arxiv.org/pdf/2610.01655v1

### Interactive Power Flow in the Browser
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.01922v1
- **作者**: Samuel Talkington, Frederik Geth, Qian Zhang, Le Xie, Skyler Liu
- **备注**: 9 pages, 3 figures, 6 tables. To appear in the Inaugural ACM Conference on Digital Transformation (ACM DXConf 2026), Ann Arbor, MI, USA
- **摘要**: 本文介绍了 tellegen，这是一个开源框架，用于在浏览器中运行交互式潮流 (PF) 和最优潮流 (OPF) 研究。这为编译为 WebAssembly 的电力系统分析工具提供了直观且民主化的访问途径。用户可以拖放案例文件，通过点击并拖动来更改节点需求或线路额定值，通过敏感性分析预览影响，并在释放时获得精确的重新求解。用户案例文件和结果完全保留在设备上：tellegen 传输的零关键阻碍能源/电力基础设施信息 (CEII)。该框架包括一个用于 PF 和 OPF 的核心数值引擎、可重复使用的浏览器组件、保存的研究以及用于智能体交互的结构化 WebMCP 工具。我们通过与 PGLib 基准比较目标函数来评估输电 OPF 求解器；通过与 OpenDSS 比较电压和电流来评估配电 PF 求解器；并通过与 PowerModels.jl 比较来评估 WebAssembly 执行时间。在现实的合成电网上，WebAssembly OPF 求解时间仅比原生二进制求解长 25-43%。该实现展示了工程师如何将可执行的数值研究作为 URL 进行分发，从而在保持案例数据本地化的同时减少安装和托管要求。
- **PDF**: https://arxiv.org/pdf/2610.01922v1

### Token Economy Design for Fair and Efficient Highway Congestion Management with Express Lanes
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.01680v1
- **作者**: Leonardo Pedroso, Juan Pablo Bertucci, W. P. M. H. Heemels, Mauro Salazar
- **备注**: Accepted to the 2026 IFAC Workshop on Cyber-Physical Human Systems
- **摘要**: 我们研究了用于高速公路车道分配的代币经济设计，旨在提高公平性而不牺牲交通效率。受圣马特奥 101 快速车道项目的启发，我们考虑了一种环境，其中高占用车辆可以无限制地进入快速车道，而其余用户可以通过赚取和使用非货币代币在常规车道和快速车道之间交替。我们将由此产生的交互建模为具有异构时间偏好和有限信息演化策略修订的有限人口动态拥堵博弈。基于平均场逼近，我们导出了代币价格，这些价格强制执行系统最优的车道划分，同时通过轮流机制随时间引入公平性。该方案在具有真实世界需求数据的微观交通模拟中进行了评估。结果表明，所提出的价格产生的平均旅行时间与没有保留车道作为快速车道的基准场景几乎相同，同时大幅减少了紧急权重感知的旅行时间。这些发现强调了代币经济是货币拥堵定价的一种有前途的替代方案，可以更公平地管理稀缺的道路容量。
- **PDF**: https://arxiv.org/pdf/2610.01680v1

### Open-Source Multi-Wire SPI Readout for Wearable Ultrasound Probes
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.01623v1
- **作者**: Federico Villani, Soumyo Bhattacharjee, Lisa Odermatt, Cédric Hirschi, Luca Benini, Andrea Cossettini
- **备注**: 4 pages, 3 figures. This work has been accepted for publication in the 2026 IEEE International Ultrasonics Symposium (IUS) proceedings. The final published version will be available via IEEE Xplore
- **摘要**: 可穿戴超声探头必须传输越来越大的采集负载，同时保持紧凑、低功耗的电子设备。在 TinyProbe 中，当前数据传输的瓶颈发生在采集 FPGA 和无线系统控制器之间。本工作提出了一种开源的多线 SPI 读取接口，该接口使用串行命令和地址阶段，随后是构建时可选的双通道或四通道有效载荷阶段，旨在通过在保持与以微控制器为中心的可穿戴超声架构兼容的同时增加超过 Wi-Fi 限制的潜在传输带宽来解决这一瓶颈。该接口模拟串行闪存，实现与广泛的微控制器系列及其现有外设接口的兼容。在 FPGA 上，数据路径通过时钟域交叉、样本重构和打包成 32 位字将现有的采集 FIFO 连接到 SPI 接口。双线 SPI 读取已集成到现有的 IGLOO2/SiWG917 TinyProbe 架构中，并在 5 MHz 的 SCLK 频率下进行了验证。使用一个独立的 Kria K26 测试平台在不依赖采集和无线子系统的情况下对 FPGA SPI 接口进行表征，证明了在高达 66 MHz 的 SCLK 频率下无误差传输。这些测量将 SiWG917 多通道 SPI 实现确定为下一个带宽限制组件，并激发了未来对系统控制器的升级。HDL 和 MCU 实现已在宽松的开源许可下发布。
- **PDF**: https://arxiv.org/pdf/2610.01623v1

#### 学科总结
本期电子与系统工程（`eess.*`）方向精选了 5 篇高质量论文，涵盖了系统控制、图像处理、电力系统、智能交通及硬件设计等多个前沿领域。其中包括：提出新型哈密顿神经网络以解决多稳定平衡态系统控制难题；通过深度展开设计统一的图像多退化恢复网络（MDIRNET）；开发在浏览器中利用 WebAssembly 高效运行的最优潮流计算框架；设计基于代币经济的公平高效高速公路拥堵管理机制；以及为可穿戴超声探头开发开源的多线 SPI 读取硬件接口。这些成果展示了软硬件协同及模型驱动方法在解决实际工程问题中的强大潜力。

--- 
## 📚 学科: `q-bio.*`
### CellMSA: Context Modeling for Single-Cell Representation Learning
- **分数**: 7
- **链接**  https://arxiv.org/abs/2609.38908v1
- **作者**: Suyuan Zhao, Minghao Liu, Yizhen Luo, Zaiqing Nie
- **备注**: Accepted by NeurIPS 2026, code released
- **摘要**: 单细胞转录组学能够以空前的分辨率剖析细胞状态，但其高维性、稀疏性和技术批次效应给表示学习带来了重大挑战。现有的单细胞基础模型通常独立编码每个细胞，或者仅对来自同一批次的细胞进行建模以进行去噪，从而未能充分利用跨批次和细胞类型的丰富关系信息来建模基因表达模式。我们认为，单细胞模型可以从更具信息量的细胞上下文建模中受益。通过比较细胞之间的一致性和变异，模型可以捕获与细胞状态相关的细粒度基因-基因依赖性，这对于学习高质量表示至关重要。受蛋白质建模中多序列比对（MSA）上下文使用的启发，我们提出了 CellMSA，这是一个单细胞表示学习框架，它将受 MSA 启发的归纳偏置引入到转录组建模中。对于每个目标细胞，CellMSA 检索来自不同批次和生物学相关细胞类型的相关细胞作为上下文，并将跨细胞模式总结为依赖于上下文的基因对表示。然后将该表示注入到感知对的目标细胞编码器中，以进行细粒度的表示学习。我们在包含约 1.09 亿个细胞观测值（包括 6560 个万原生观测值）的大规模人类单细胞语料库上对 CellMSA 进行了预训练。实验表明，我们的框架在多个基准测试中始终优于现有方法。代码可在以下仓库中获得：https://github.com/PharMolix/CellMSA。
- **PDF**: https://arxiv.org/pdf/2609.38908v1

### pCoMole: Pareto-Constrained Molecule Editing with Discrete Flows
- **分数**: 6
- **链接**  https://arxiv.org/abs/2610.01663v1
- **作者**: Tong Chen, Maximilian Holsman, Lin Zhao, Pranam Chatterjee
- **备注**: Published at NeurIPS 2026. (Proceedings of the 40th Conference on Neural Information Processing Systems, Sydney, Australia)
- **摘要**: 生物分子治疗通常从已知序列开始，需要针对性地编辑以改善多种属性，同时满足苛刻的生化和可制造性约束。然而，现有的生成方法并不共同支持多目标优化、硬可行性以及在离散、变长生物空间中的序列编辑。在这项工作中，我们引入了帕累托约束分子编辑（pCoMole），这是一个构建在离散流匹配上的框架，它引导预训练的编辑流（Edit Flow）走向用户指定的偏好，同时强制执行终端可行性。pCoMole 使用增强的 Tchebycheff 效用定义了可行性门控的终端分布，并通过底层编辑过程的 Doob-h 变换实现所得的偏好倾斜。为了使这种构建实用，我们通过在候选编辑上进行简短的蒙特卡洛演练来近似所需的调和函数，从而产生具有可证明偏好一致性的高效引导编辑器。我们通过缩短 GFP 同时保留荧光相关属性、缩短多种 Cas9 直系同源物同时保留 PAM 特异性，以及将肽结合剂压缩为在硬约束下优化七种药物相关属性的短拟肽，验证了 pCoMole。在湿实验测试中，两种由 pCoMole 设计的 229 残基 eGFP 变体在发生 10 次缺失（并伴有 1 次或 2 次替换）后，在 BL21 细胞中保留了明显的绿色荧光。总之，pCoMole 实现了离散、变长空间中生物分子序列的约束感知、帕累托对齐的编辑。
- **PDF**: https://arxiv.org/pdf/2610.01663v1

### Evolutionary foraging in grids: Intermittent search dynamics emerge in finite, depletable landscapes
- **分数**: 6
- **链接**  https://arxiv.org/abs/2609.39239v1
- **作者**: Shailendra Bhandari, Alex Szorkovszky, Anis Yazidi, Pedro G. Lind
- **备注**: Accepted at NeurIPS 2026. Project webpage: https://evo-foraging.github.io/
- **摘要**: 搜索策略在有限、可消耗的景观中如何演化仍然是觅食理论中的一个问题。我们通过演化模拟来研究这个问题，在模拟中，个体在包含均匀分布或呈莱维粉尘（Lévy dust）分布的非再生资源的二维环面晶格上觅食。每个个体携带一个编码步长、速度和转弯角度的遗传基因组，选择作用于结合了能量获取、运动成本和覆盖效率的适应度函数。通过允许运动特征在不施加预设幂律步长分布的情况下发生演化，我们测试了演化出的轨迹是否能被间歇性搜索（intermittent-search）或莱维飞行（Lévy-walk）动力学更好地描述。我们的结果表明，在本文考虑的有限消耗驱动景观中，演化出的搜索与间歇性动力学比与严格的无标度莱维运动更一致。我们通过将二阶和四阶位移矩拟合到间歇性搜索和莱维飞行模型来表征动力学。虽然类莱维随机游走很好地拟合了演化轨迹（在大多数测试条件下平均调整后 $R^2$ > 0.9），但对于所有测试的资源分布，间歇性搜索实现了更紧密的拟合（平均调整后 $R^2$ > 0.99）。在测试的网格尺寸和资源密度中，这种偏好保持一致。在名义资源密度 $\rho$ = 0.15 的 503 x 503 网格上，每个环境进行五个独立的演化运行，重现了对均匀环境和五个莱维粉尘环境的这种偏好。演化迅速将运动基因组重塑为短位移，同时保留了较长搬迁的稀疏尾部，这与偶尔转移点缀的局部开发一致。该框架为研究资源受限下搜索规则如何涌现提供了一个受控环境，并可能为自主系统中的资源受限探索提供信息。
- **PDF**: https://arxiv.org/pdf/2609.39239v1

### From DNA Design to DNA Slimming: Auditable Agentic Discovery of a Deletion-Only Designer
- **分数**: 4
- **链接**  https://arxiv.org/abs/2609.40143v1
- **作者**: Joel Shor
- **备注**: 40th Conference on Neural Information Processing Systems (NeurIPS 2026). Workshop: Agentic AI for Biological Discovery
- **摘要**: 紧凑的调控 DNA 可以释放载体有效载荷中的空间，减少合成和化验负担，并揭示哪些序列特征驱动了预测的活性。然而，大多数基于模型的核酸设计器通过替换来优化固定长度的序列；它们不会询问现有功能元件的哪些碱基可以在保留预测活性的同时被移除。我们将序列瘦身（sequence slimming）的任务定义为在保留活性的同时选择精确长度、保持顺序的子序列。模拟设计基准 NucleoBench，我们提出了一个平衡序列减少与维持功能的瘦身定量评估。每个瘦身器必须返回子序列及其源索引，这可用于验证瘦身器是否遵守任务要求。据我们所知，这是针对该仅删除（deletion-only）问题的首个专用基准。编码智能体经验研究助手（ERA）随后搜索了可执行的设计器程序。ERA 接收任务提示和成功的仅替换设计器 GrAdaBeam 作为起始程序，并对其进行修改以产生 GRADASLIM。我们报告了五个转录因子结合目标的留出评估，比较了 400 和 100 bp 处的随机、贪婪和 ERA 引导的瘦身。ERA 在 9/10 的设置中具有最高均值。ERA 减去贪婪的配对自助区间在所有五个 400-bp 设置中均大于零，在一个 100-bp 设置中小于零，在其余四个中与零重叠。
- **PDF**: https://arxiv.org/pdf/2609.40143v1

### Not all solutions are created equal: An analytical dissociation of functional and representational similarity in deep linear neural networks
- **分数**: 4
- **链接**  https://arxiv.org/abs/2609.38998v1
- **作者**: Lukas Braun, Erin Grant, Andrew M. Saxe
- **备注**: 28 pages, 5 figures. ICML 2025 camera-ready version. Presented at ICML 2025 and CCN 2025
- **摘要**: 联结主义的一个基本原则是，感知、行动和认知产生于简单、相互连接的单元之间的并行计算，这些单元生成并依赖于神经表示。因此，研究人员采用多元模式分析来解码和比较人工和生物网络的神经编码，旨在揭示它们的功能。然而，对于网络的表示和功能如何关联，目前的分析理解还很有限，尽管这对于任何关于底层功能或功能相似性的定量概念都是至关重要的。我们利用可分析的两层线性网络和非线性网络中的数值模拟来解决这个问题。我们发现功能和表示是分离的，允许在没有功能相似性的情况下存在表示相似性，反之亦然。此外，我们表明输入噪声的鲁棒性和泛化误差水平都不约束表示去贴合任务。相反，对参数噪声具有鲁棒性的网络其表示灵活性有限，必须采用特定于任务的表示。我们的研究结果表明，表示对齐反映了超越单纯功能对齐的计算优势，这对解释和比较联结主义系统的表示具有重要意义。
- **PDF**: https://arxiv.org/pdf/2609.38998v1

#### 学科总结
本期定量生物学（`q-bio.*`）领域精选了 5 篇极具启发性的论文，深入探讨了生物数据表征、分子设计及演化动力学。重点包括：提出受多序列比对启发的单细胞表示学习框架 CellMSA，在大规模数据集上性能显著；开发基于离散流匹配的帕累托约束分子编辑框架 pCoMole，并在湿实验中成功验证了 eGFP 变体的荧光活性；利用演化模拟揭示了在有限可消耗资源下，间歇性搜索动力学比单纯莱维飞行更具适应性；提出首个专用于 DNA 序列瘦身（仅删除）的评估基准 GRADASLIM；以及通过双层线性网络解析证明了神经网络中功能与表示的解耦现象。这些研究为 AI 赋能生命科学提供了创新的理论与工具。

--- 
## 📚 学科: `cs.*`
### Trust the Direction, Search the Step: Zero-and-First-Order Methods for LLM Fine-Tuning
- **分数**: 7
- **链接**  https://arxiv.org/abs/2610.02190v1
- **作者**: Cristian McGee, El Houcine Bergou, Aritra Dutta
- **备注**: Accepted to 40th Conference on Neural Information Processing Systems (NeurIPS 2026). Code: https://github.com/nizswan/Zeroth-First-Order-Framework
- **摘要**: 步长选择仍然是大规模神经网络优化中的核心挑战；保守的步长会减慢收敛，而激进的步长则会使其不稳定。我们结合了零阶和一阶优化（ZFO），并提出了一个将方向选择与步长解耦的轻量级框架。ZFO 使用一个值得信赖的一阶优化器来确定方向，并仅沿着这个一维子空间进行零阶评估以选择移动多远。利用当前的梯度信息和两次额外的目标函数评估，ZFO 实例沿着建议的方向构建目标函数的局部模型，并在有界搜索区间内选择一个感知曲率的步长。这产生了一种自适应步长选择机制，其成本低于完全线搜索。我们提供理论保证来表明，共享样本评估可产生可靠的有限差分曲率估计，诱导的局部模型在搜索区间内选择接近最优的步长，并且 ZFO 收敛到平稳点的邻域。在评估的设置、语言模型和数据集中，相对于固定步长的一阶基线，ZFO 经常提高优化和最终性能，其幅度和首选局部模型取决于目标。我们的代码公开在：https://github.com/nizswan/Zeroth-First-Order-Framework。
- **PDF**: https://arxiv.org/pdf/2610.02190v1

### KaliBench: A Fine-Grained Benchmark for Cybersecurity Tool Use on Kali Linux with Runtime-Free Verifiable Rewards
- **分数**: 6
- **链接**  https://arxiv.org/abs/2610.02206v1
- **作者**: Pengfei Li, Naufal Suryanto, Sicheng Zhang, Muzammal Naseer
- **备注**: Accepted at NeurIPS 2026 Evaluations and Datasets Track. Project page: https://risys-lab.github.io/KaliBench/ | Github: https://github.com/RISys-Lab/KaliBench
- **摘要**: 大语言模型（LLM）正越来越多地应用于网络安全工作流，期望它们能将分析人员的意图转化为工具调用。然而，现有的评估侧重于基于知识的评估或端到端智能体任务，没有直接衡量 LLM 为现实世界网络安全工具生成可执行命令的能力。这一差距至关重要，因为网络安全操作依赖于严格的命令行界面（CLI），其中微小的语法错误、不正确的参数-值绑定或参数顺序错误都可能使执行失效。我们引入了 KaliBench，这是一个用于在 Kali Linux 上进行自然语言到 CLI 翻译的细粒度基准和数据集，包含 8,504 个查询-命令对，涵盖 23 个能力维度和 5 个安全阶段的 1,642 个工具。KaliBench 是通过基于手册的管道构建的，具有确定性的规范化和感知别名的评估，从而能够对工具选择和参数构造进行精确且可复现的评估。为了确保语义正确性和实际可执行性，我们开发了一个多阶段验证管道，该管道结合了基于 LLM 的验证、沙盒终端执行和人机协同微调。利用这些细粒度的确定性信号，KaliBench 进一步支持用于训练的免运行期可验证奖励。在 24 种开源通用和安全微调模型的配置及 3 种评估模式下，在无限制设置中没有开源模型的精确命令准确率超过 42%，这突显了在没有显式工具提示的情况下精确进行基于 CLI 的网络安全工具调用的困难。我们进一步表明，利用从 KaliBench 导出的可验证奖励进行监督微调和强化学习，可以显著提升一个 8B 模型的性能，并达到与 685B MoE 模型相当的水平。
- **PDF**: https://arxiv.org/pdf/2610.02206v1

### SILSA: Sliding-Window Slice Latents for Topology-Preserving High-Resolution 3D Generation
- **分数**: 6
- **链接**  https://arxiv.org/abs/2610.02201v1
- **作者**: Tianjiao Yu, Xinzhuo Li, Yifan Shen, Ying Shen, Kiet A. Nguyen, Adheesh Sunil Juvekar, Ismini Lourentzou
- **备注**: Accepted at NeurIPS 2026. Project link: https://plan-lab.github.io/silsa
- **摘要**: 高分辨率 3D 生成越来越多地依赖于体素潜变量和多阶段管道，这些管道首先预测活动结构，然后合成局部几何。虽然有效，但这种设计将连续表面碎片化为许多局部 token，增加了生成成本，并且往往会削弱薄或高度连接形状的拓扑一致性。我们引入了 SILSA，这是一个拓扑感知 3D 生成框架，它使用紧凑的滑动窗口切片潜变量来表示形状。SILSA 不是生成昂贵的体素 token，而是沿着三个规范轴使用一组固定的重叠切片，其中每个 token 总结一个局部深度窗口，以保持横截面连续性并支持单阶段整流流（rectified-flow）生成。Slice VAE 将定向表面样本编码为多轴切片潜变量，并使用稀疏体积解码器对其进行重建，而体积锚格网通过共享 3D 工作空间协调定向切片流。为了保持结构正确性，我们引入了切片级拓扑监督，以匹配持续同调图（persistence diagrams）并对齐相邻切片之间的贝蒂数（Betti）过渡。实验表明，SILSA 提高了结构保真度，同时大幅降低了生成成本。与最强基准相比，SILSA 将 PSNR 提高了 $8.7\%$，覆盖率提高了 $5.96$ 个百分点，贝蒂误差降低了 $9.2\%$，同时使用的 token 比次紧凑基准少 $70.0\%$，比稀疏或分层分词器少 $98\%$ 以上，有效降低了 $40.4\%$ 的训练内存并缩短了 $58.5\%$ 的推理时间。定性结果进一步表明，对薄结构、重复部件和长程连接性的保留有所改善。
- **PDF**: https://arxiv.org/pdf/2610.02201v1

### Omni-Embed-Mini: Binding Modalities Without Forgetting via Dense Distillation
- **分数**: 5
- **链接**  https://arxiv.org/abs/2610.02148v1
- **作者**: Mohammed Irfan Kurpath, Jaseel Muhammad Kaithakkodan, Sahal Shaji Mullappilly, Ivan Laptev, Hisham Cholakkal
- **备注**: Findings of EMNLP 2026. 26 pages, 8 figures, 14 tables. Project page: https://omniembed.cvmbzuai.com
- **摘要**: 将文本嵌入模型扩展到新的模态通常会降低文本检索质量，而现有的全模态嵌入器则通过数十亿参数进行补偿。我们提出了 Omni-Embed-Mini，这是一个 0.9B 参数的模型，可将文本、语音、音频、图像、视频和视觉丰富的文档映射到单个共享的余弦空间中，而无需更新任何文本侧参数。我们的核心见解是，教师信号不需要单独的嵌入模型：每个媒体样本都与一个密集的级联文本描述配对，而教师目标仅仅是冻结的骨干网络自身对该描述的嵌入。因为教师和学生共享相同的骨干权重，所以它们存在于字节完全相同的几何空间中，而轻量级投影仪加上模态编码器上的分阶段 LoRA 适配器就足以进行对齐。训练将 Matryoshka SigLIP 对比损失与在线混合硬负样本挖掘器相结合，其负样本随着编码器的改进而变得更加尖锐。通过换入原生视觉-语言骨干网络，该配方可以延续到 2.3B 变体。Omni-Embed-Mini-0.9B 保持其文本权重与骨干网络完全一致，因此训练不会导致文本检索衰退（在 MTEB-v2 BEIR-8 上为 49.57 nDCG@10），同时将其扩展到五个额外的模态，并且比我们对比的每个开源全模态嵌入器小约 2.7 倍至 9.5 倍。2.3B 变体与闭源的 gemini-embedding-2 相比极具竞争力，在整体模态平均值上略占优势。模型、代码、数据和评估套件可在我们的项目页面找到：https://omniembed.cvmbzuai.com。
- **PDF**: https://arxiv.org/pdf/2610.02148v1

### VISTA: A Visual Harness for Reasoning in an Interactive World
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.02200v1
- **作者**: Qiushi Han, Keya Hu, Linlu Qiu, Cathy Wu, Kaiming He
- **备注**: Tech report. An early version of this manuscript was in a blogpost published in Aug 5, 2026: https://vista-research.github.io/
- **摘要**: 我们展示了多模态模型具有强大的推理能力，而适当的控制套件（harness）可以释放它们在不同交互环境中解决任务的潜力。我们引入了 VISTA，这是一个视觉控制套件，赋予通用多模态模型长程视觉能力。VISTA 允许模型通过视觉观测直接感知环境，并维护一个无损的视觉记忆，以原始形式保留过去的观测。模型在推理时可以主动检索这些观测并重新组织其视觉输入。在 ARC-AGI-3 上，VISTA 将 Claude Opus 5.0 的相对人类行动效率得分从 40.68 提升到了完美的 100.00，模型在完成所有 25 个公开游戏时使用的行动比首次参与的人类减少了 57.4%。VISTA 简单的设计也使其能够以最少的适应自然地扩展到各种视觉环境。在涵盖各种视觉游戏和解谜的另外三个基准测试中，它在使用相同底层模型且仅配备极简控制套件的情况下，显著优于基准方法。我们的结果强调了 VISTA 作为一种通用视觉控制套件，在复杂视觉环境中推进多模态智能体发展的巨大潜力。
- **PDF**: https://arxiv.org/pdf/2610.02200v1

#### 学科总结
本期计算机科学（`cs.*`）领域精选了 5 篇极具应用和理论价值的论文。在模型优化方面，提出 ZFO 框架，结合零阶与一阶算法来解决大模型微调中的自适应步长难题；在安全应用上，推出 KaliBench，首个针对网络安全工具自动生成的细粒度 CLI 基准，可显著提升小模型的能力；在 3D 生成与多模态嵌入方向，SILSA 框架利用切片潜变量和拓扑约束，实现了更低成本的高保真、拓扑保持 3D 生成；Omni-Embed-Mini 则利用密集蒸馏实现了 0.9B 参数下的无损多模态嵌入；最后，视觉控制套件 VISTA 显著提升了多模态智能体在复杂交互环境中的长程视觉推理能力。

--- 
## 📚 学科: `math.*`
### Trust the Direction, Search the Step: Zero-and-First-Order Methods for LLM Fine-Tuning
- **分数**: 7
- **链接**  https://arxiv.org/abs/2610.02190v1
- **作者**: Cristian McGee, El Houcine Bergou, Aritra Dutta
- **备注**: Accepted to 40th Conference on Neural Information Processing Systems (NeurIPS 2026). Code: https://github.com/nizswan/Zeroth-First-Order-Framework
- **摘要**: 步长选择是大规模神经网络优化中的核心挑战。我们结合零阶和一阶优化（ZFO），提出了一个将方向选择与步长解耦的轻量级框架。ZFO 使用信赖的一阶优化器确定方向，并仅沿该一维子空间进行零阶评估来选择移动距离。利用梯度信息和两次额外的目标函数评估，ZFO 沿着该方向构建目标函数的局部模型，并在有界搜索区间内选择感知曲率的步长。这产生了一种自适应步长选择机制，成本低于完全线搜索。我们提供了收敛性及在语言模型微调上改进表现的理论和实验保证。
- **PDF**: https://arxiv.org/pdf/2610.02190v1

### Wasserstein Gradient Flows and Forward-Only Diffusion Are Not Enough for Multimodal Sampling
- **分数**: 6
- **链接**  https://arxiv.org/abs/2610.02081v1
- **作者**: Daniel McBride, Pratik Khandagale, Cristina Garcia-Cardona, Yen Ting Lin
- **备注**: 20 pages, 5 figures, accepted by NeurIPS 2026 Position Track
- **摘要**: 基于 Wasserstein 梯度流 (WGF) 和仅前向扩散过程 (FODP) 的采样算法近期蓬勃发展，通常伴随着指数级快速收敛到目标分布的理论保证。这些保证经常被解释为这些方法可以高效采样复杂多峰分布的证据。在这项工作中，我们证明了这种解释具有根本性的误导。通过调用 Jordan-Kinderlehrer-Otto (JKO) 方案和 Otto 微积分，我们确定了经典的 WGF 采样动力学和过阻尼前向扩散共享相同的密度演化，因此继承了非平衡态统计物理中长期研究的亚稳态和慢混合现象。我们使用谱分析和平均首次通过时间 (MFPT) 分析这两个互补工具对该采样器族进行了分析，结果表明良好分离的多峰性会导致与小谱隙和罕见的模式间跃迁相关的指数级长混合时间。对于普遍采用的对数线性退火方案，我们发现引入中间分布并不能消除总输运时间的指数级缩放。这种局限性是结构性的而非具体实现所致：纯局部的、梯度驱动的输运机制可能需要指数级长的时间来跨越良好分离的模式输运概率质量。我们认为，这代表了标准形式下基于 WGF 和 FODP 采样的根本局限性，并激发了未来开发用于高效多峰采样的根本性非局部机制的研究。
- **PDF**: https://arxiv.org/pdf/2610.02081v1

#### 学科总结
本期数学（`math.*`）领域精选了 2 篇聚焦于机器学习优化与采样理论的深度论文。第一篇论文提出了结合零阶与一阶优化的 ZFO 框架，利用几何分析和局部曲率估计来解决大规模非凸优化中自适应步长选择的瓶颈。第二篇论文是一篇关于多峰采样的立场性论文（Position Track），运用 Jordan-Kinderlehrer-Otto (JKO) 方案和 Otto 微积分等现代几何测度论工具，严谨证明了基于 Wasserstein 梯度流和前向扩散的经典采样算法在面对多峰分布时存在结构性的“慢混合”和指数级传输时间屏障，这一发现对当前扩散模型和流匹配算法的理论局限性给出了极具穿透力的数学剖析。

--- 
## 📚 学科: `astro-ph.*`
### A New Framework for Modeling Solar Flares from MHD to Kinetic Processes
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.02149v1
- **作者**: Joel C. Allred, Graham S. Kerr, Silvina E. Guidoni, Joel T. Dahlin, Marc Swisdak, Judith T. Karpen, Valeriy Tenishev
- **备注**: 21 pages, 12 figures, accepted for publication by Astrophysical Journal
- **摘要**: 太阳耀斑中的物理过程跨越了许多空间和时间尺度数量级，因此，一个考虑所有相关过程的单一统一模型在计算上仍然是无法实现的。相反，研究人员已经开发了专门的代码，针对特定领域来解决太阳耀斑问题的特定方面。在这里，我们提出了一个综合框架，将三个模型联系起来，以捕获耀斑的触发和能量释放、随后的粒子加速、这些粒子的传播和热化，以及最终对低层太阳大气的加热。我们使用 2.5D ARMS 磁流体力学 (MHD) 代码来模拟模拟活动区中磁场的应力、电流片的形成、磁重联以及新形成的耀斑环的演化。我们使用 ARMS 电流片中的条件来初始化 kglobal 模型，该模型预测随时间变化的非热电子和质子分布。最后，我们使用 RADYN+FP 将这些分布注入新重联的 ARMS 环中，并计算随后的粒子输运、大气加热和辐射发射。这是首次详细展示在同一环中跟踪非热电子和质子的 RADYN+FP 模拟。在讨论发生的有趣物理过程的同时，我们注意到这导致了与观测一致的白光耀斑发射高度。这项工作是构建完全 3D 耀斑建模框架的第一步。
- **PDF**: https://arxiv.org/pdf/2610.02149v1

### Spurious sources in high-resolution VLA surveys
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.02028v1
- **作者**: Eric F. Jiménez-Andrade, Emmanuel Momjian, Eric J. Murphy, James J. Condon, Miguel Vega
- **备注**: Accepted for publication in the Revista Mexicana de Astronomía y Astrofísica (RMxAA)
- **摘要**: 盲河外射电连续谱巡天正越来越多地在亚角秒角分辨率下进行。然而，这些巡天中包含的伪源比纯高斯噪声统计所预期的要多得多。我们利用卡尔·G·扬斯基超大天线阵 (VLA) 获得的 10GHz GOODS-N 马赛克图像调查了这些错误探测的起源，该图像达到了 0.22 角秒的原生角分辨率，并表现出几乎高斯分布的像素噪声。我们表明，在高角分辨率下伪源比例增加的部分原因自然来自更多数量的独立分辨率元，而与主束响应相关的残留宽场成像效应仅做出了很小的贡献。然而，即使考虑到这些效应，观测到的错误探测比例仍然比高斯噪声预测的高出几倍。对噪声自相关函数的分析表明，具有相对稀疏 uv 覆盖的图像保留了显著的脏束（dirty-beam）旁瓣，这些旁瓣引入了相关的噪声波动，从而大大增加了错误探测的概率。我们得出结论，伪源的过量是 uv 采样不完整的一个内在结果，而不是成像方法本身的问题，这强调了未来的深度射电连续谱巡天不仅需要高角分辨率，还需要足够密集的 uv 覆盖以尽量减少伪探测。
- **PDF**: https://arxiv.org/pdf/2610.02028v1

### The Impact of a Clumpy Ambient Medium on the Dynamics and Synchrotron Emission of AGN Jets
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.01983v1
- **作者**: Ivan Almeida, Christian Fendt, Bhargav Vaidya
- **备注**: 19 pages, 13 figures, accepted for publication in MNRAS
- **摘要**: 来自活动星系核 (AGN) 的相对论性喷流预计会穿过非均匀的星际介质 (ISM)，但小尺度气体非均匀性在其早期演化中的作用仍不确定。我们使用 PLUTO 进行 3D 特殊相对论磁流体力学模拟来研究这个问题，追踪一个洛伦兹因子为 10 的喷流穿过秒差距尺度的介质。我们将均匀环境介质与两个块状环境介质模型进行了比较（其灵感来自核区 ISM 中的致密气体），其中云团占用的体积填充因子分别为 0.1% 和 1%。我们通过扩散激波加速的拉格朗日宏观粒子计算了合成同步辐射图和光谱。喷流与云团的相互作用会使流向发生偏转，增强激波形成，并产生比均匀 ISM 情况下更不对称的茧状结构。总的来说，这导致了明显更强的质量负载：卷吸质量从均匀模拟中的 0.43 $M_{\odot}$ 增加到块状模拟中的 5.3 和 8.8 $M_{\odot}$。块状 ISM 还改变了喷流茧内的湍流和物质混合。我们发现的动力学差异转化为了更亮、更不规则的同步辐射。对于相同的注入喷流，具有块状介质的模型比均匀模型产生更强的频率积分同步辐射，SED 的最大差异发生在亚毫米到红外/光学波段。我们的结果表明，加入小尺度 ISM 结构可以对年轻 AGN 喷流的早期动力学演化及其辐射性质提供更完整的描述。
- **PDF**: https://arxiv.org/pdf/2610.01983v1

### Wolf-Rayet formation through L/M-dependent superwinds
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.01953v1
- **作者**: Aisling McKeown, Ciarán Furey, Gautham N. Sabhahit, Jorick S. Vink
- **备注**: Accepted in A&A(24th September), 7 pages, 7 figures, 1 table
- **摘要**: 红超巨星（RSG）中的质量损失尚未被完全理解，恒星演化模型依赖于经验配方。近年来，提出了包括 $L/M$ 依赖性的新型超级风质量损失思想，这与传统的仅基于 $L$ 依赖性公式化的 RSG 风配方不同。我们研究了不同的 RSG 质量损失配方如何影响大质量恒星从其 RSG 阶段开始的晚期演化。我们使用 MESA 创建了一系列初始质量在 $10\,{\rm M}_\odot - 40\,{\rm M}_\odot$ 之间的恒星演化模型，采用了 RSG [VS23] $L/M$ 配方和传统质量损失配方。独立于恒星包层的处理，我们发现对于 25$\,{\rm M}_\odot$ 的恒星，由于其反质量依赖性，$L/M$ 配方达到的质量损失率比传统配方高出一个数量级。由于 RSG 的光度由核质量决定，并且在很大程度上对当前的恒星质量不敏感，这创造了一个驱动失控包层剥离的正反馈回路。因此，初始质量 $M_{\rm init} \sim \,20\,{\rm M}_\odot$ 的恒星能够剥离其氢包层并形成经典的沃尔夫-拉叶（WR）星。我们得出这一结论不仅是基于它们在 HRD 上的位置，还基于我们用 PoWR 恒星大气代码计算的预测发射谱线。初始质量 $M_{\rm init}<20\,{\rm M}_\odot$ 的恒星没有完全剥离，这意味着它们在核氦燃烧后膨胀。在附录 A 中，我们提出了一个通用的解析模型，表明失控剥离的倾向随着质量损失对质量的反比例标度强度的增加而迅速增加。我们的模型证明了一条可行的单星演化途径进入黄超巨星和 WR 阶段。完全和部分剥离的量对超新星（SN）的前身星有直接影响，包括部分剥离的 IIb 型超新星。
- **PDF**: https://arxiv.org/pdf/2610.01953v1

### LACHESIS: Robust stellar parameters through Bayesian model averaging of isochrone grids
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.01931v1
- **作者**: Jose I. Vines, Austin T. Ware
- **备注**: Accepted in A&A. 12 pages, 7 figures, 1 page of appendix, abstract changed from accepted version due to character constraints
- **摘要**: 准确的恒星参数是大部分天体物理学的基础，从系外行星系统到银河系考古学。对于孤立的野外恒星，质量、尤其是年龄通常是从恒星演化模型中推断出来的，但这些推断取决于所选的模型网格，并且网格之间的系统差异可能与任何单一流程的统计不确定性相抗衡。我们介绍了 LACHESIS，这是一个 Python 包，它从光度学和光谱学中确定恒星质量、半径和年龄，同时明确解释了选择模型网格带来的系统不确定性。我们基于数据在 [Fe/H]、对数年龄和等效演化阶段上插值了五个独立的等时线网格，用嵌套采样对每个网格进行采样，并通过贝叶斯模型平均法组合每个网格的后验，每个网格的权重由其贝叶斯证据决定。我们针对 Kepler 星震矮星和次巨星的基准验证了 LACHESIS。质量的恢复具有约 4% 的鲁棒散射，半径约为 2%，半径偏差极小（<1%），质量系统误差较小（~3%）。年龄的恢复具有约 30% 的鲁棒散射，这强烈取决于演化阶段；网格间的系统误差贡献了约 9% 的底限，这是一个次要但真实的项，单一网格拟合会忽略它。模型平均比选择单一网格校准得更好：一旦包含参考不确定性，其置信区间就接近名义覆盖率，并且即使生成模型位于系综之外，在注入测试中也能接近名义覆盖率。通过对恒星模型网格系综进行边缘化，LACHESIS 将网格选择的系统误差直接折叠到后验中，因此报告的不确定性不再仅反映网格内的数据噪声。这为系外行星宿主和恒星群体研究提供了均匀且表征良好的质量、半径和年龄。
- **PDF**: https://arxiv.org/pdf/2610.01931v1

#### 学科总结
本期天体物理（`astro-ph.*`）领域精选了 5 篇涵盖恒星演化、星际介质、高能天体物理及数据处理等方向的高质量论文。研究成果包括：开发出从磁流体力学（MHD）到动力学过程的新型太阳耀斑综合模拟框架；深入探讨高分辨率 VLA 巡天中因 uv 采样不完整产生的伪源机制；通过 3D 特殊相对论 MHD 模拟揭示块状星际介质对活动星系核（AGN）喷流早期演化及同步辐射的巨大影响；利用 MESA 和 PoWR 探索基于新型质量损失配方的单星演化至沃尔夫-拉叶（WR）星的路径；以及开发基于贝叶斯模型平均的 Python 包 LACHESIS，用以稳健估算恒星参数。这些工作极大推进了多物理场观测与理论模型的结合。

--- 
## 📚 学科: `stat.*`
### Wasserstein Gradient Flows and Forward-Only Diffusion Are Not Enough for Multimodal Sampling
- **分数**: 6
- **链接**  https://arxiv.org/abs/2610.02081v1
- **作者**: Daniel McBride, Pratik Khandagale, Cristina Garcia-Cardona, Yen Ting Lin
- **备注**: 20 pages, 5 figures, accepted by NeurIPS 2026 Position Track
- **摘要**: 基于 Wasserstein 梯度流 (WGF) 和仅前向扩散过程 (FODP) 的采样算法近期蓬勃发展，通常伴随着指数级快速收敛到目标分布的理论保证。这些保证经常被解释为这些方法可以高效采样复杂多峰分布的证据。在这项工作中，我们证明了这种解释具有根本性的误导。通过调用 Jordan-Kinderlehrer-Otto (JKO) 方案和 Otto 微积分，我们确定了经典的 WGF 采样动力学和过阻尼前向扩散共享相同的密度演化，因此继承了非平衡态统计物理中长期研究的亚稳态和慢混合现象。我们使用谱分析和平均首次通过时间 (MFPT) 分析这两个互补工具对该采样器族进行了分析，结果表明良好分离的多峰性会导致与小谱隙和罕见的模式间跃迁相关的指数级长混合时间。对于普遍采用的对数线性退火方案，我们发现引入中间分布并不能消除总输运时间的指数级缩放。这种局限性是结构性的而非具体实现所致：纯局部的、梯度驱动的输运机制可能需要指数级长的时间来跨越良好分离的模式输运概率质量。我们认为，这代表了标准形式下基于 WGF 和 FODP 采样的根本局限性，并激发了未来开发用于高效多峰采样的根本性非局部机制的研究。
- **PDF**: https://arxiv.org/pdf/2610.02081v1

### The Curvature of Regret in Contextual Linear Optimization
- **分数**: 6
- **链接**  https://arxiv.org/abs/2610.01980v1
- **作者**: Konstantinos Ziliaskopoulos, Alexander Vinel, Alice E. Smith
- **备注**: 4 pages main body plus appendix, 3 figures. Accepted to the NeurIPS 2026 Workshop on MLxOR
- **摘要**: 由于优化器的不连续性，线性优化的决策聚焦学习变得复杂，其中微小的成本误差可能会使决策保持不变，或将其移动到不同的顶点。我们证明，在对数据分布进行平均后，这种非平滑的点对点行为在局部变为二次方，并且我们推导出了闭合形式的曲率，具体而言，是支撑在法锥扇（normal fan）墙壁上的矩阵值测度。该测度仅取决于可行集，数据分布仅作为权重进入。然后，我们为该曲率提供了一种易于处理的近似，只需对可行集进行一次投影即可计算。我们证明了该近似弱收敛于真实的总体曲率。我们提供了我们发现的一个应用，即针对期望成本线性优化的决策感知场景生成方法。我们的实验测试了二次和弱收敛定律，并显示在电池套利上比亚马逊均匀分配提高了 30.8% 的遗憾值（regret）。
- **PDF**: https://arxiv.org/pdf/2610.01980v1

### No Model Required: Text Entropy Rate Filtering Mitigates Iterative Fine-Tuning Collapse
- **分数**: 4
- **链接**  https://arxiv.org/abs/2610.01493v1
- **作者**: Lewis Mitchell
- **备注**: 17 pages, 8 figures, NeurIPS 2026
- **摘要**: 在合成数据上进行迭代微调会导致模型崩溃：随着罕见模式的逐渐丢失，输出多样性变窄，这种特征最明显地表现为短语级别的重复。现有的缓解方法要么需要模型对数概率、外部预言机，要么需要持续获取真实的真实人类数据。在这里，我们开发了一种基于数学信息论的新方法：非参数 Kontoyiannis 熵率估计器 $h_k$，它完全通过匹配长度统计从原始文本计算得出，不需要任何模型。我们证明，在完全合成的单谱系微调设置中，这在文本多样性指标上实际上是一个更优的训练数据过滤器。在 Llama-3.1-8B 的六代 QLoRA 崩溃实验中，基于对数概率的过滤（最完善的需要模型访问的基线）在任何指标上都没有提供显著的文本多样性益处（$p > 0.23$），而 $h_k$ 过滤产生了 $+42\%$ 的唯一三元组、$+30\%$ 的词汇量和 $-19\%$ 的重复（均满足 $p < 0.001$）。我们在 4 个领域、2 个温度、2 个生成器-打分器模型对以及 1,520 个生成的文档中，验证了 $h_k$ 作为一个跨领域熵代理（$\beta = 0.924$, $R^2 = 0.746$）和崩溃检测器（$\rho = +0.454$, $p < 0.0001$）。我们的结果表明，缓解崩溃的信息论方法是高效的，并为保持多智能体多样性提供了新途径。
- **PDF**: https://arxiv.org/pdf/2610.01493v1

### MCIR: A Feature Dependence-Aware Explainability Method with Reliability Guarantees
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.01641v1
- **作者**: Poushali Sengupta, Sabita Maharjan, Frank Eliassen, Shashi Raj Pandey, Yan Zhang
- **备注**: Accepted for publication in Transactions on Machine Learning Research (TMLR)
- **摘要**: 现代机器学习模型通常包含强依赖或冗余特征，由于共享的预测信息可以分布在相关的预测因子中，这使得特征归因变得困难。因此，现有方法（如 SHAP、LIME、HSIC、MI/CMI 和 SAGE）在多重共线性或近乎重复的预测因子下可能会产生不稳定的排名。我们提出了互相关影响比率法（MCIR-M），这是一种依赖感知的全局特征重要性方法，它量化了每个特征在选定的依赖邻域之外贡献的独特预测信息。MCIR-M 引入了互相关影响比率（MCIR），它将每个特征置于强依赖的邻域上，并计算条件信息与块级信息的归一化比率。在精确的条件冗余下，总体得分位于 [0,1] 并且等于零。我们还引入了一种轻量级的估计程序，该程序使用一小部分可用数据计算 MCIR，并评估与全数据解释的一致性。在受控合成冗余实验和 UCI HAR 基准测试中，MCIR 表现出依赖感知的排名行为，其在注入的近乎重复预测因子下具有最明显的优势。与独立和条件 SHAP、SAGE、HSIC、基于 MI 的得分以及 CIR 系列基线的比较在真实数据标准上各有千秋。减少解释样本降低了评估配置中的计算负担，而与全数据解释的一致性是通过排名、头部集和忠实度诊断进行单独评估的。总的来说，MCIR-M 为强特征依赖下的全局解释提供了一种实用的依赖感知诊断。
- **PDF**: https://arxiv.org/pdf/2610.01641v1

### Platonic Task Arithmetic
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.00929v1
- **作者**: Junghwan Park, Woojin Cho
- **备注**: NeurIPS2026
- **摘要**: 为同一任务而专门化的模型会收敛到相似的行为，但产生这种行为的参数更新不共享共同的坐标系，因此权重空间任务算术局限于单个模型，并且在没有结构对应关系的情况下无法跨越架构。借鉴柏拉图的洞穴寓言，我们假设这些特定于模型的更新是一个共享的、与模型无关的对象的影子，我们称之为“柏拉图任务向量”（platonic task vector）。为了使其在图像或音频编码器与文本编码器配对的模型中发挥作用，我们引入了通用任务描述符：这些矩阵的形状独立于架构和嵌入维度，记录了任务的功能效果，并支持矩阵加法和取反操作。将描述符转移到目标中意味着编辑目标，直到它在任务的无标签探测图像和类名提示上重现该描述符，这不需要每张图像的标签。我们以两种方式实现这种编辑。首先，描述符分解为图像嵌入上的偏移场，因此单个最小二乘求解就产生了一个线性算子，该算子作为权重编辑折叠到目标的最后一层；由于线性性质，一组这样的算子允许以有符号和的形式进行任意强度的任意组合。其次，在相同目标上训练的低秩适配器可以到达每一层并联合拟合组合，代价是每次编辑需要进行一次优化。异构模型仅部分共享此对象，其特定于模型的残差在范数上与共享部分相当，但跨模型转移仍能保留目标自身描述符 74-80% 的收益。在六个模型家族、八个分类任务和一个音频-文本设置中的实验表明，任务知识在两种实现下都可以跨异构模型进行转移和组合。
- **PDF**: https://arxiv.org/pdf/2610.00929v1

#### 学科总结
本期统计学（`stat.*`）领域精选了 5 篇具有极高理论广度与应用深度的论文。研究方向包括：对 Wasserstein 梯度流与前向扩散采样在多峰分布下局限性的理论反思；推导数据分布下线性优化中遗憾值（Regret）的局部二次曲率解析式，并用于决策感知场景生成；首次提出无需模型的非参数熵率估计器 $h_k$，通过信息论方法有效过滤合成训练数据以缓解 LLM 迭代微调中的模型崩溃；提出互相关影响比率法（MCIR-M）解决强特征依赖下的全局可解释性与特征归因难题；以及提出“柏拉图任务向量”概念，在异构多模态模型之间实现了免标注的任务知识高效转移与代数算术组合。

--- 
## 📚 学科: `econ.*`
### When One Leak Pays Forever: Context Binding and the Price of Deterring Collusion
- **分数**: 6
- **链接**  https://arxiv.org/abs/2609.36667v1
- **作者**: Tingyi Lin, Shawn Yu, Ruoran Lai, Huanxi Zhang
- **备注**: Accepted at NeurIPS 2026
- **摘要**: 当联盟出售的东西能够持续发挥作用时，偏差一次的联盟可以获利多次。在阈值加密内存池（防止最大可提取价值 MEV 的主导防御措施）中，向抢跑者出售解密能力的解密委员会法定人数会暴露该能力仍可解密的后续每一个区块。我们询问多大的惩罚（例如可罚没的质押金）能震慑这种合谋。在我们的重复博弈中，单调授权联盟家族（例如 $n$ 个委员会成员中的任意 $k$ 个）中的任何联盟发生一次泄露，就会解锁一系列未来轮次，付出一次性惩罚，并结束该联盟的参与。我们表明，每一次动态偏差都归结为选择泄露时间，因此当且仅当每个联盟'的惩罚覆盖了单次泄露所达到的最大折现价值时，威慑才能成立。在不进行折现的情况下，在 $T$ 轮单位价值完全复用的博弈中需要 $T$ 的惩罚，而将每次泄露限制在它自己的轮次中需要 $1$，因此没有在时间跨度上呈常数的惩罚能够威慑无限制的复用；宽度为 $w$ 轮的复用窗口最多产出每轮最大价值 $w$ 倍的损失。震慑每个联盟的最低成员质押金配置解决了覆盖线性规划问题。对于区块链设计，每个时期的密钥将所需质押金从密钥生命期的价值降低到一个时期的价值；我们在以太坊抢跑数据上校准了该差距，并将 Ferveo 和 Shutter 置于该模型中。该分析扩展到密封递价拍卖、多权威投票以及共享密钥下的联邦学习。
- **PDF**: https://arxiv.org/pdf/2609.36667v1

### Robustness in Mechanism Design
- **分数**: 3
- **链接**  https://arxiv.org/abs/2610.01805v1
- **作者**: Jason Hartline
- **备注**: This is a preprint of a review article that is accepted to appear in the Annual Review of Economics in August of 2027. It contains an additional section on the revelation gap that, for space reasons, was mostly removed from the published version
- **摘要**: 本文回顾了拍卖的稳健设计 and 分析，侧重于计算机科学文献中的主导范式，该范式通过稳健拍卖的性能与环境最优拍卖性能之间的最坏情况（在不同环境下）比率来量化稳健性。应用包括福利目标的经典拍卖（如第一价格拍卖）的稳健分析、收入目标的先验稳健拍卖设计，以及贸易所得目标的交易机制的先验稳健设计。最后，启示原理（revelation principle）在稳健机制设计中并不是无损的。潜在的损失可以通过启示间隙（revelation gap）来量化，即当从所有机制限制为启示机制时，最优稳健保证所损失的比例。
- **PDF**: https://arxiv.org/pdf/2610.01805v1

### Does AI Help or Harm? Endogenous Information Acquisition with AI Advice
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.35137v1
- **作者**: Kexin Chen, Tao Lin, Jianwei Huang
- **备注**: Accepted by WINE 2026
- **摘要**: AI 建议在代价高昂的信息获取和最终行动之前，正越来越多地进入人类的决策工作流。本文研究了这种建议如何影响决策质量（通过最终行动的总效用来衡量）。在决策者选择具有均匀后验可分（UPS）成本的获取实验之前，建议会转移信念。该分析通过净最优获取所产生的延续总价值来表征总效应。该价值函数的凸性是每个 AI 信号在每个先验下均能微弱改善总效用的充要条件，而非凸性则允许二元信号造成总损害。该标准给出了紧凑的状态空间结果。在具有任意行动、收益和 UPS 成本的二元状态问题中，每个 AI 信号在总效用上都是微弱改善的。由于集中的停工（有价值的获取停止），一个最小的三状态问题可能会产生总损害。对于具有香农获取成本的分类问题，该标准变成了激活集斜率测试。它保证了同构分类和所有三状态加权分类问题的微弱总改善，而最小的四状态失败产生于注意力稀释（获取从高风险的区别转移开）。沿着布莱克威尔递增的混合路径，总效用可以先减小后增加。在内生解释下，更便宜的解释可以降低总效用。
- **PDF**: https://arxiv.org/pdf/2609.35137v1

#### 学科总结
本期经济学（`econ.*`）与博弈论领域精选了 3 篇兼具理论深度和机制设计创新的高质量论文。第一篇论文针对区块链内存池防 MEV 合谋问题，建立了可重复博弈模型，推导出了抵御解密密钥单次泄露及无限复用风险的最低质押惩罚机制。第二篇是由领域专家撰写的综述预印本，系统梳理了计算机科学视角下拍卖和交易机制的“先验稳健设计”，并深入剖析了启示间隙及其理论损失。第三篇论文探讨了 AI 建议对人类内生信息获取和决策质量的双刃剑效应，通过后验可分成本和凸性分析，给出了 AI 信号如何促进或损害决策福利的数学判断边界。这些工作极大地拓宽了算法机制设计在数字经济与人工智能治理中的应用前景。

---
```