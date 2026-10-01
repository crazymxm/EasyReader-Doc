# 🗓️ 周报 (2026-W39)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-09-27

--- 
## 📚 学科: `eess.*`
本周 `eess.*`（电气工程与系统科学）学科精选了三篇高质量论文。第一篇针对静电致动器，提出了一种利用光电耦合器作为有源元件的高压反馈放大器，显著降低了谐波失真并提升了带宽；第二篇聚焦于航空航天控制，提出了一种向飞行控制系统注入“全谐波”正交多弦信号的新方法，并在微型八轴飞行器悬停状态下成功进行了系统辨识；第三篇针对未来大孔径天线阵列的辐射近场通信，开发了一种基于部分松弛（PR）的低复杂度近场非视线（NLoS）上行信道估计框架，大幅提升了多路径和多用户干扰环境下的估计性能。

### High-Voltage Optocoupler Amplifier for Electrostatic Actuators
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.29914v1
- **作者**: George C. Jurgiel, Alex S. Miller, Jeffrey H. Lang
- **备注**: To be published in the proceedings of the 2026 IEEE Energy Conversion Congress & Expo (ECCE)
- **摘要**: 许多静电致动器在亚毫安电流下需要数千伏的驱动电压，这一任务不适合传统的开关器件。作为替代方案，我们展示了一种使用光电耦合器作为有源元件的高压放大器。该放大器产生 20-kV 的峰峰值输出，带宽高达 500 Hz，同时保持极少的元件数量。通过在反馈中将光电耦合器用作线性器件，实现了比等效 PWM 放大器更低的谐波失真和更高的带宽。该设计通过提供一种更简单的方法来获得有用的驱动波形，提高了静电致动器的可行性。
- **PDF**: https://arxiv.org/pdf/2609.29914v1

### System Identification of an Octocopter in Hover using Full-Harmonic Orthogonal Multisine Inputs
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.29832v1
- **作者**: Justin J. Matt, George V. Altamirano
- **备注**: 31 pages, 18 figures. Presented at the AIAA AVIATION Forum 2025. Accepted for publication in the AIAA Journal of Aircraft
- **摘要**: 本文提出了一种用于系统辨识的多输入飞行机动设计新方法。该方法包括向飞行控制系统注入“全谐波”正交多弦信号。通过重复改变多弦极性的机动来实现正交性。多弦信号可以包含相同的频率成分，这可以简化频率响应估计，并允许将较长的飞行机动拆分为几个较短的机动，同时保持相同的频率分辨率和最低频率。本文提出了一种输入分配方案，该方案增强了多弦信号，以围绕特定自由度调整飞行器的响应幅度。通过在接近悬停条件下的微型八轴飞行器的飞行测试，证明了所开发方法的有效性。成功利用输入分配方案来增加绕偏航轴的激发。辨识了电功率、电机转速和刚体动力学模型，并表明它们能够准确预测飞行器和电机的响应。模型主要由旋翼拉力和扭矩系数参数化，使其适用于飞机飞行动力学和单个旋翼空气动力学的分析。结果表明，在忽略旋翼桨毂力矩、旋翼系数变化、滚转和俯仰中的陀螺力矩以及气动相互作用效应的情况下，可以准确地建模接近悬停的飞行动力学。
- **PDF**: https://arxiv.org/pdf/2609.29832v1

### Low-Complexity Multi-User Non-Line-of-Sight Channel Estimation
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.29342v1
- **作者**: Mohammad Abu Aqoulah, Doğa Gürgünoğlu, Gábor Fodor, Gonzalo Seco-Granados
- **备注**: 6 pages, 5 figures. Accepted to IEEE CSCN 2026
- **摘要**: 未来的无线接入网络预计将依赖大孔径天线阵列，其覆盖区域的越来越大一部分可能落在辐射近场内。在这种情况下，传统的远场模型变得不准确，且接收的空间特征共同取决于传播距离和方位角，这使得可靠的上行信道获取成为关键的物理层挑战。许多现有的近场估计工作依赖于简化的视线主导或单路径信道模型，这些模型无法捕捉实际的非视线（NLoS）多径环境。相比于先前的单路径近场部分松弛（PR）公式，本文开发了一种基于 PR 的近场 NLoS 上行信道估计框架，通过将每个用户信道建模为以其距离和方位角为特征的多个球面波分量的叠加。对于已知导频的情况，我们开发了一种基于贪婪 PR 的最大似然估计器，可在减轻多用户干扰的同时迭代提取主导传播路径。对于未知符号的情况，我们提出了一种基于 PR 的秩自适应协方差拟合方法来捕捉多径结构。我们进一步推导了这两种情况下相应的 Cramér-Rao 界。数值结果表明，所提出的基于多径 PR 的方法具有很强的估计性能，接近相应的界，并且在所考虑的场景中优于近场二维多信号分类（MUSIC），支持了它们与未来大孔径上行链路系统的相关性。
- **PDF**: https://arxiv.org/pdf/2609.29342v1

--- 
## 📚 学科: `q-bio.*`
本周 `q-bio.*`（定量生物学）学科精选了一篇关注植物物候高通量分析的论文。该工作提出了 RootQuantV2 框架，将自监督视觉基座模型（DINOv3 ViT-L/16）与混合参数高效微调方案相结合，从微根管（Minirhizotron）的原位图像中直接进行作物根系性状（如长度和表面积）的回归预测。该方法仅训练极少量的参数，便取得了极高的拟合优度并显著降低了误差，成功实现了对历史遗留数字存档的重新利用。

### RootQuantV2: Adapting a Vision Foundation Model for Root-Trait Regression from Minirhizotron Imagery
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.25567v1
- **作者**: Kinjalk Parth, Sebastian Varela, Andrew D. B. Leakey
- **备注**: 20 pages (15 main + 5 references), 4 figures, 5 tables. Accepted to the Computer Vision in Plant Phenotyping and Agriculture (CVPPA) Workshop at ECCV 2026. Code and weights: https://github.com/leakey-lab/RootQuantV2
- **摘要**: 由于缺乏针对田间种植作物根系性状的高通量表型分析解决方案，严重制约了对地下性状和过程的理解与改良。微根管（Minirhizotrons）是田间环境下标准的无损根系表型分析方法。需要计算机视觉解决方案来实现大规模的自动性状估计，但训练数据稀缺，且人类标注往往由于存在于仅导出每幅图像根长和表面积标量总和的专用软件中而无法获取。然而，这些根系性状的大量数字历史存档已经存在。RootQuant 表明可以直接通过回归从整幅图像中预测这些性状，从而从流水线中移除了手动追踪的掩膜；RootQuantV2 通过用自监督 ViT 替换 RootQuant 的 CNN 骨干网络，进一步推进了这一想法。我们使用混合参数高效方案调整了冻结的 DINOv3 ViT-L/16。仅训练 11.9M 个参数（模型的 3.78%），RootQuantV2 实现了分别达 0.950 和 0.930 的长度和面积 $R^2$，同时相比 RootQuant 将长度/面积的 RMSE 降低了 24.3%/20.7%。因此，RootQuantV2 重新利用了遗留的数值存档，用于高通量、自动化的根系性状估计。
- **PDF**: https://arxiv.org/pdf/2609.25567v1

--- 
## 📚 学科: `cs.*`
本周 `cs.*`（计算机科学）学科精选了五篇发表于 NeurIPS 2026 和 EMNLP 2026 的前沿论文。研究内容涵盖：1）利用代数稀疏化和双曲几何缓解大模型长程推理中的探索与复合偏差（SAGE）；2）在具身强化学习中，利用连续梯度的时间相关性构建梯度逆向攻击，重现私有轨迹（TRACE）；3）通过 LLM 潜在语义细化与谱对齐提升不完整数据下的多模态情感分析性能（SemMSA）；4）揭示多模态大模型逐层对齐分数背后的“对齐幻觉”，提出几何诊断指标（PA gap）；5）提出解耦上下文的策略感知多阶段 Agent 规划框架（GRASP），大幅提升了复杂推理任务的可靠性。

### SAGE: Mitigating Long-Horizon Reasoning Biases via Topological Guidance
- **分数**: 7
- **链接**  https://arxiv.org/abs/2609.30192v1
- **作者**: Xinyue Zeng, Jiawei Zhang, Yujun Yan, Dawei Zhou
- **备注**: Accepted by NeurIPS 2026
- **摘要**: 长程推理（Long-horizon reasoning）在稀疏奖励机制下仍是大语言模型（LLM）面临的核心挑战。我们认为，这种脆弱性源于复杂推理空间引发的两种偏差：一种是探索偏差，即模型容易被局部合理但结构不稳定的分支所吸引；另一种是复合偏差，即微小的局部偏差会在深度上累积并抑制稀疏奖励。我们引入符号闭包分析（Symbolic Closure Analysis, SCA）作为理论视角，表征分支结构和稀疏奖励如何在具有局部容许性的长程推理中诱发这些偏差，并作为在非正式推理任务中设计结构先验的原则。受此分析启发，我们提出了 SAGE（结构容许性引导探索），这是一个统一的框架，通过注入结构引导来缓解长程推理中的探索偏差和复合偏差。SAGE 结合了两种互补的结构引导：代数稀疏化（将局部容许的候选投影到以算子为索引的代数子空间上，以抑制伪分支并减轻探索偏差）以及双曲结构引导（将推理状态嵌入到负常曲率空间中，以提供深度的深度信号并减轻复合偏差）。在 12 个基准测试和 7 个模型家族中，SAGE 的表现优于具有竞争力的基线。特别是，在 Andrews-Curtis 问题（一个开放的现实世界长程任务）上，SAGE 实现了高达 8 倍的提升。
- **PDF**: https://arxiv.org/pdf/2609.30192v1

### Temporal Gradient Inversion for Private Trajectory Reconstruction in Embodied Reinforcement Learning
- **分数**: 6
- **链接**  https://arxiv.org/abs/2609.30258v1
- **作者**: Sudip Bhujel, Shanghao Shi, Ruiquan Huang, Ning Zhang, Yang Xiao
- **备注**: Accepted at NeurIPS 2026
- **摘要**: 具身强化学习智能体中的分布式学习通过在设备上保留原始传感器数据并仅向服务器传输策略梯度，提供了一定程度的隐私保护。然而，时间结构会放大这种泄露，使其超出单帧攻击的范围。我们引入了 TRACE（基于连续编码的时间重构攻击），这是一种摊销时间梯度逆向攻击，它从每步策略学习梯度中自回归地重构私有观测-动作轨迹序列。该攻击利用了先前单帧方法忽略的两个结构信号：（i）连续具身梯度之间的跨时间相关性（我们通过条件互信息界对其进行了形式化），以及（ii）从策略头梯度结构中进行闭式动作恢复（我们证明了当标准熵正则化足够小时，该恢复是精确。在留出的具身场景中，TRACE 达到了 18.8 dB 的 PSNR，且在每重构帧 3-4.5 毫秒的情况下实现了近乎完美的动作恢复，在所有重构指标上均优于基于学习的基线，且在运行速度提高几个数量级的同时超越了优化攻击。进一步的评估表明，TRACE 具有更广泛的适用性，可跨越循环、残差和紧凑 Transformer 受害者架构、多模态输入以及更大的离散动作空间。防御实验表明，保护时间梯度流可能需要具备序列感知能力的隐私机制。
- **PDF**: https://arxiv.org/pdf/2609.30258v1

### SemMSA: Latent Semantic-Aided Robust Multimodal Sentiment Analysis with Incomplete Data
- **分数**: 6
- **链接**  https://arxiv.org/abs/2609.30238v1
- **作者**: Wenhao Li, Zhibin Wu, Chong Xiao, Qiangchang Wang
- **备注**: Accepted by NeurIPS 2026
- **摘要**: 近年来，多模态情感分析（MSA）的研究主要集中在利用不完整数据从语言、视觉和听觉模态中学习以推断人类情感。大多数研究通常通过重构模态特征或设计复杂的融合机制来弥补缺失的信息。然而，由于在部分观测的多模态证据中缺乏高水平的语义落地，这些方法仍然存在伪生成和噪声引导的问题。为了解决这些问题，我们提出了 SemMSA，一个潜在语义辅助的框架，该框架利用大语言模型（LLM）构建丰富的与情感相关的语义，并通过无锚点的谱对齐与所有模态完全整合。它主要由跨模态语义细化（CSR）和跨模态谱对齐（CSA）组成。具体而言，CSR 首先通过相应的适配器自适应地提取视觉和听觉表示，以便在冻结的 LLM 嵌入空间中与语言形成统一的多模态前缀。然后，它通过不解码显式文本的高效 Token 潜在细化过程，迭代地产生连续的判别性语义状态。接着，CSA 通过增强其核 Gram 矩阵的主导谱分量，同时将细化后的语义与所有模态对齐。这捕捉了所有表示之间的全局非线性依赖关系，而无需依赖预定义的锚定模态。此外，实例级的谱分离约束保留了跨样本的判别性并缓解了表示崩溃。在 SIMS、MOSI 和 MOSEI 基准测试上的广泛实验表明，SemMSA 达到了最先进的性能。
- **PDF**: https://arxiv.org/pdf/2609.30238v1

### The Alignment Illusion in Multimodal Large Language Models
- **分数**: 6
- **链接**  https://arxiv.org/abs/2609.30210v1
- **作者**: Hong-Han Wang, Yuntao Wang, Hu Ding
- **备注**: Accepted to NeurIPS 2026
- **摘要**: 多模态大语言模型（MLLM）中的逐层视觉-文本相似性被广泛解释为语言模型逐步将视觉内容整合到共享表示空间中的证据。这种解读基于一个假设，即标量对齐分数反映了内容层面的跨模态交互。为了检验这一假设，我们对视觉流应用了控制干预。在涵盖 5 个家族、参数量从 0.5B 到 72B 的 13 个 MLLM 中，用高斯噪声替代投影器输出的视觉 Token 会急剧降低任务准确率，然而四种标准的标量度量指标（CKA, SVCCA, MIR 以及领先的主角余弦值）却无法一致地将损坏的视觉流与原始流区分开来。我们将这种失效称为“对齐幻觉”，并将其归因于共享的语言模型路径：各向异性的 MLP 下投影将视觉和文本 Token 拉向共同的输出方向，从而产生了权重引起的对齐。由于该成分本质上是一维的，我们引入了主角间隙（PA gap），定义为前两个主角余弦值之间的差异，它将权重引起的相似性与多方向的视觉结构区分开来。在渐进的视觉损坏下，PA 间隙比我们考虑的标量分数能更一致地追踪任务准确率；在结构化但无关的图像下，它进一步揭示了内部几何与任务准确率脱节的情况。因此，MLLM 中的内部视觉-文本对齐最好被解读为语言模型内部视觉流的几何诊断，而不是内容级跨模态交互的直接代理，并且在通过受控任务证据进行校准时最具信息量。
- **PDF**: https://arxiv.org/pdf/2609.30210v1

### GRASP: Generating, Revising, and Assessing for Strategic Planning with Agentic AI
- **分数**: 6
- **链接**  https://arxiv.org/abs/2609.30147v1
- **作者**: Arunabh Srivastava, Mohammad A., Khojastepour, Srimat Chakradhar, Sennur Ulukus
- **备注**: Accepted at the Second Workshop for Research on Agent Language Models (REALM) at EMNLP 2026
- **摘要**: 大语言模型（LLM）通常表现出一种性能特征，即随着任务复杂度的增加，其可靠性会降低。我们通过引入 GRASP（一种策略感知的多阶段规划框架），解决了为复杂任务生成高质量自然语言可执行规划的挑战。GRASP 将规划流水线解耦到专门的、上下文隔离的模块中：它预编译全局宏观指南（GenPlan），在隔离的上下文窗口中探索替代的局部策略（RevPlan），并使用多标准判别器独立评估轨迹（VerPlan）。实证评估表明，GRASP 在各种数据集上一致地建立了新的最先进水平，相比于直接的 LLM 规划器，在 Natural Plan 日历调度（提高约 12.4%）、ZebraLogic（提高约 30.8%）和 SciBench 数学上取得了显著的准确率提升。至关重要的是，在多任务扩展下（标准规划器会立即发生性能崩溃），GRASP 完全平摊了多任务退化惩罚。在交错的双任务环境中，GRASP 相比于直接的 LLM 规划器实现了高达 16.7% 的绝对准确率提升。此外，通过隔离上下文并强制执行严格的宏观正则化，GRASP 领先前沿推理模型（如 GPT-5-mini）达 14.5% 的优势。
- **PDF**: https://arxiv.org/pdf/2609.30147v1

--- 
## 📚 学科: `math.*`
_本周缺少高价值论文_

---
## 📚 学科: `astro-ph.*`
本周 `astro-ph.*`（天体物理学）学科精选了五篇发表于 A&A、MNRAS、ApJ 和 ApJL 的重要成果。研究涵盖：1）从几何学和相空间测度角度，重新解释了开普勒双星热偏心率分布规律的物理起源；2）在 PLUTO 代码中引入了一种全新的多组分尘埃-气体-辐射三相耦合热力学数值流体模拟方案；3）提出了一种盘介导的角动量输运模型，解决了双星演化中吸积星质量增长受阻的历史难题；4）利用太阳探测器 Aditya-L1 的最新空间光谱数据，揭示了日珥爆发中绿线发射与极紫外晚期的物理联系；5）通过哈勃望远镜与韦伯望远镜的联合成像，首次在散射光波段探测到绘架座 $\beta$ 碎片盘中特殊的“猫尾巴”结构。

### The geometric origin of the thermal eccentricity law
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.30259v1
- **作者**: Václav Pavlík
- **备注**: Accepted for publication in Astronomy & Astrophysics; a century-old problem finally gets a geometrical excuse; 4 pages, no figures or tables, but plenty of equations
- **摘要**: 分布 $f(e)=2e$ 通常被称为开普勒双星的“热偏心率分布”。然而，该结果并不需要热平衡，并且其通常的推导掩盖了为什么该分布在偏心率上是线性的。我们寻求对该结果及其与更一般偏心率分布的关系进行简单的几何解释。我们考虑在维度 $D\geq2$ 的欧几里得空间中的束缚开普勒轨道，其相空间分布仅取决于能量，并从刘维尔测度推导出偏心率分布。我们得到 $f_D(e)=(D-1) e (1-e^2)^{(D-3)/2}$，因此，在此家族中，$D=3$ 是分布函数关于 $e$ 呈线性的唯一情况。这是由 $D-1$ 个横向动量维度和开普勒周期简并性决定的。我们进一步表明，两种已知的推广形式——即归一化角动量的幂律加权和恒定的速度各向异性——实际上是同一个单参数偏心率分布家族的两种表现形式。
- **PDF**: https://arxiv.org/pdf/2609.30259v1

### Simulating the thermodynamics of gas, radiation, and multispecies dust: Method and applications to protoplanetary disks
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.30252v1
- **作者**: Dhruv Muley, David Melon Fuksman, Prakruti Sudarshan, Alexandros Ziampras, Mario Flock
- **备注**: 18 pages (+7 pages appendix), 13 figures. Accepted to Astronomy and Astrophysics; further comments and questions welcome
- **摘要**: 原行星盘的热力学由气体、尘埃和辐射之间复杂的相互作用所主导，对其在大尺度和小尺度上的形态和动力学都有着强烈的影响。历史上，流体动力学模拟使用近似配方处理热力学，例如局部等温性、参数化的 $\beta$-冷却以及处于气尘热平衡状态的辐射流体动力学。然而，更全面且自洽的方法能够更准确地再现观测中发现的丰富特征，这些特征在现代已达到了前所未有的光谱、角分辨率和垂直分辨率。出于这一动机，我们为 PLUTO 代码设计了一种辐射流体动力学方案，具有气体、辐射和多种尘埃之间的能量交换（通过吸收、发射和碰撞）。通过将每种尘埃视为无压力、扩散的流体来处理尘埃-气体动力学，确保我们的方案能够表示由颗粒沉降和俘获引起的盘面照明变化。我们在几个测试问题中展示了该方案的有效性，并最后讨论了其与原行星盘研究中悬而未决问题的相关性。
- **PDF**: https://arxiv.org/pdf/2609.30252v1

### Disc-mediated angular momentum transport resolves the mass-gain problem in rotating binaries
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.30230v1
- **作者**: Sebastian Ljung, Avishai Gilkis, Sandro Tacchella
- **备注**: Accepted for publication in MNRAS
- **摘要**: 很大一部分恒星在其寿命期间会与近邻伴星发生相互作用，其中质量和角动量的转移塑造了它们的演化和最终归宿。标准的受自转限制吸积模型预测，吸戏星在仅获得其质量的一小部分后就会达到临界自转，从而严重抑制进一步吸积。这与对相互作用后系统的观测存在冲突，后者需要大量的质量增长。我们引入了一种盘介导的角动量输运方案，用于向恒星伴星进行质量转移。这基于一种新型的微扰、解析星-盘边界模型，该模型允许吸积星在接近临界自转时继续有质量流入。此外，该模型重现了先前的数值结果，即对超临界自转的微扰会导致盘施加负转矩，提取过剩角动量，同时允许持续的质量流入。我们在使用 MESA 进行的具有较差自转的详细双星演化计算中实现了该机制，并计算了跨越主星质量、轨道周期和质量比的网格。虽然受自转限制的模型预测 $\beta_{\rm eff}\lesssim 0.1$，但该盘模型在临界自转附近产生了持续的质量流入，在大部分参数空间中有效质量转移效率为 $\beta_{\rm eff}\sim 0.4$-$1$。所得吸积星的属性与观测到的相互作用后的 sdOB+Be 双星大致一致。因此，盘介导的角动量输运可能代表了标准双星演化模型中缺失的关键要素，对快速自转恒星和致密天体前身星具有重要意义。
- **PDF**: https://arxiv.org/pdf/2609.30230v1

### Coronal Green-Line Emission During a Solar Prominence Eruption: Spectroscopic Evidence of Its Correspondence with the EUV Late Phase
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.30164v1
- **作者**: P. Vemareddy, R. Ramesh, V. Muttu Priyal
- **备注**: Accepted to publish in ApJ, 12 pages, 7 figures
- **摘要**: 我们报告了 2025 年 10 月 9 日太阳西边缘一次日珥爆发期间的光谱观测，该爆发与 12:11 UT 开始的 M2.0 级耀斑相关。该事件由搭载于 Aditya-L1 的可见发射线日冕仪（VELC）以凝视（sit-and-stare）模式捕获，提供了对 Fe XIV 5303 Å 日冕绿线的连续观测。空间平均的绿线发射表现出与在多个 SDO/AIA 通道中观测到的极紫外晚期（EUV late-phase, ELP）发射的清晰对应关系。特别是在 15:24 UT 增强的 5303 Å 发射峰与 AIA 211、171、193 和 335 Å 通道中的次级峰相吻合，发生在 X 射线峰值后约 173 分钟。5303 Å 线宽信息为负责 ELP 的机制提供了重要约束。在接近 ELP 峰值时，线宽逐渐减少约 28%，这与耀斑后日冕环的冷却大致一致。这一行为表明 ELP 主要与等离子体冷却有关，而来自磁重联的额外能量输入相对较弱，这并未产生显著的线宽增强。估算的非热速度从冲击相期间的约 36 km s$^{-1}$ 减少到渐变相期间的约 21 km s$^{-1}$，表明等离子体湍流运动减弱。多普勒速度从爆发上升相期间的主导正值演变为后期渐变相期间的负值，意味着等离子体先上升后下降。据我们所知，本研究提供了第一个将日冕绿线发射与太阳耀斑期间的 ELP 及其起源联系起来的空间光谱证据。
- **PDF**: https://arxiv.org/pdf/2609.30164v1

### Deep HST/STIS Coronagraphic Imaging of the $β$ Pictoris Debris Disk: On the Scattered Light Component of the Cat's Tail
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.30111v1
- **作者**: Arin M. Avsar, Kevin Wagner, Daniel Apai, Isabel Rebollido, Antranik A. Sefilian, Marshall D. Perrin, Christopher C. Stark, Gabriel Weible, Andras Gaspar
- **备注**: 24 pages, 16 figures, 3 Tables. Accepted for publication in ApJL
- **摘要**: 绘架座 $\beta$（$\beta$ Pictoris）碎片盘是一个独特的系统，利用 JWST/MIRI 进行的中红外日冕仪成像揭示了一个被称为“猫尾巴”（Cat's Tail）的新空间分辨子结构。我们展示了在散射光中对 $\beta$ Pic 进行的深哈勃太空望远镜（HST/STIS）日冕仪成像，结合了 2012 年至 2025 年之间的六个观测历元，以寻找“猫尾巴”的散射光成分。我们首次利用 HST/STIS 在 500 au 的投影距离处探测到了该盘，在 50 至 200 au 之间的中平面大部分区域实现了大于 100 的信噪比（SNR）。我们报告了对“猫尾巴”子结构在可见光/近红外散射光成分的探测。通过注入-恢复分析，我们发现“猫尾巴”的散射光成分总通量为 MIRI F1550C 通量的 $0.1-0.4\%$。利用测得的 STIS-to-MIRI 通量比，我们模拟了“猫尾巴”的尘埃颗粒属性，发现这些颗粒具有高度多孔性，且几乎完全由有机耐熔物质组成，这与 JWST/MIRI 的发现相一致。我们使用太阳系矮行星和本地星际介质（ISM）中的尘埃有机物含量作为代理，来估计能够产生“猫尾巴”中看到的足够有机耐熔物质的碰撞前身星的大小。我们发现，每个碰撞前身星的质量必须至少达到 $1-3\times 10^{21}$ kg，与我们柯伊伯带中的卡戎（Charon）和鸟神星（Makemake）相当。此外，我们在 $\beta$ Pic 的外层尘埃晕中发现了显著的扭曲形态和表面亮度不对称性。我们将观测到的晕形态和不对称性与预测的垂直结构进行了比较，这些结构可能源于行星-盘的相互作用。
- **PDF**: https://arxiv.org/pdf/2609.30111v1

--- 
## 📚 学科: `stat.*`
本周 `stat.*`（统计学）学科精选了一篇关于因子图近似推断的理论突破。该工作提出了“直接消息近似”（DMA）框架，通过直接近似因子到变量的传递消息而非传统的边缘分布，有效克服了传统期望传播（EP）和变分消息传递（VMP）容易出现负精度消息和点估计塌缩的弊端。论文提供了严格的 KL 散度一致性证明与收敛界限，并成功将其应用于贝叶斯神经网络（BNN）的单次快速前向/后向推断。

### Direct Message Approximation (DMA): A Consistency-Based Framework for Tractable Approximate Inference on Factor Graphs
- **分数**: 4
- **链接**  https://arxiv.org/abs/2609.29466v1
- **作者**: Ralf Herbrich, Rainer Schlosser, Jan Lemcke, Johann Ukrow, Anna Kazachkova, Nicolas Alder, Leonhard Hennicke, Theo Bardey, Nico Grimm, Luca Kleinschmidt, Philipp Kolbe, Cezary Kujath, Johanna Schlimme, Karl Matti Schütz
- **备注**: Submitted to ICLR 2027
- **摘要**: 因子图上的近似消息传递构成了两种主要概率推断算法家族的基础：期望传播（EP）和变分消息传递（VMP）。这两种方法都近似每个因子边上的边缘分布，从而迫使采用迭代轮询调度，面临负精度消息的风险，并且对于 VMP 而言，会塌缩为狄拉克-德尔塔（Dirac-delta）因子处的点估计。我们引入了直接消息近似（DMA），它直接近似“因子到变量”的消息，而不是边缘分布。对于可归一化的因子，我们定义了一个一致性条件（要求当所有其他输入消息均为狄拉克-德尔塔时精确）来指导消息构建。我们证明了一个主定理（适用于任何图、合适的因子消息），该定理从消息 KL 散度界定了边缘 KL 散度，并带有三个结构推论：狄拉克输入一致性、无 EP 式的内环迭代以及无负精度消息。此外，我们证明了乘积因子本质上不合适的后向消息具有 $O(1/r^2)$ 的互补保证，而该消息的闭式处理在先前的工作中一直难以解决。作为一个具体的实例化，我们推导了乘积和 leaky-ReLU 因子的显式 DMA 消息，并组装了一个贝叶斯神经网络（BNN）推断算法，每个训练样本只需进行一次前向/后向扫描，且没有梯度学习率超参数，验证了结构保证转化为在数据稀疏区域（包括模型失配下）变宽的预测不确定性。
- **PDF**: https://arxiv.org/pdf/2609.29466v1

--- 
## 📚 学科: `econ.*`
本周 `econ.*`（经济学）学科精选了三篇探讨前沿博弈论和 AI 时代商业决策的论文。第一篇研究在生成式 AI 降低造假成本背景下的“信任套利”现象，揭示了高质量市场因核实延迟而暂时成为欺诈温床的自限性机制；第二篇针对委托-代理合同，探讨了代理人策略性披露行动空间以重塑委托人认知的博弈，并给出了福利与收益的理论保证；第三篇则设计了一种基于里程碑和实物期权叠加的层次分析法框架，为被 AI 深度重塑商业模式的企业（特别是 AI 服务商）提供了更具审计性的估值方法。

### When Trust Attracts Fraud: AI and Trust Arbitrage
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.27404v1
- **作者**: Xieyu Yin, Fenghua Wen
- **备注**: 11 pages, 1 figure. Author accepted manuscript. Published in Economics Letters
- **摘要**: 当信任延迟了核实时，它可能会吸引欺诈。我们开发了一个双市场信号模型，其中生成式人工智能降低了伪造、核实和靶向定位的成本。当伪造在核实之前变得有利可图时，声称的可信度首先下降，随后恢复。跨市场来看，较高的先前质量可能会延迟核实，从而创造一个只有较低质量市场进行检查的区间。如果靶向定位在此区间内变得有利可图，欺诈性卖家就会进入质量较高但警惕性较低的市场，而他们的进入最初会逆转该市场的可靠性优势。这种流入也会触发核实并阻止进一步进入。我们将这种自我限制的机制称为信任套利。因此，在生成式人工智能时代，信任会产生一种内生但暂时的保护真空，从而在不同市场之间重新引导欺诈行为。
- **PDF**: https://arxiv.org/pdf/2609.27404v1

### Strategic Disclosure of Action Space in Principal-Agent Contracts
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.25410v1
- **作者**: Xiaotie Deng, Ningyuan Li
- **备注**: Full version of the manuscript accepted at WINE 2026. A one-page extended abstract will appear in the conference proceedings. A substantially revised version with more general results is planned
- **摘要**: 我们研究了委托-代理合同中行动空间的策略性披露，其中代理人选择一个披露的行动集，以便在合同设计前塑造委托人对其能力的认知。委托人在未意识到策略性披露的情况下，假定披露的行动集是完整且准确的，从而设计出收益最优的合同。我们考虑了以成本可验证性区分的两种变体。当成本不可验证时，代理人可以提取全部的第一最优剩余，使委托人获得零收益。当成本可验证时，我们表征了代理人在二值结果设定下的最优披露策略，并且更一般地，在委托人受限于线性合同时，将代理人的问题简化为双变量凸优化问题。我们证明了代理人可以获得至少占第一最优剩余 $1/e$ 分额的效用，这在最优披露下也产生了一个 $1/e$ 的社会福利保证。尽管与第一最优剩余相比，委托人的收益可能任意小，但当非空基本行动中最大期望回报与最小期望回报的比率至多为 $L$ 时，我们确立了相对于第一最优剩余 $\Theta(1/\log L)$ 的收益保证。我们还比较了策略性披露下的效用和福利与经典模型中的对应物。最后，在不限制委托人使用线性合同的情况下，我们将代理人的 $1/e$ 效用保证推广到了一般的结果空间。我们的结果表明，策略性行动空间披露如何改变剩余的分配，同时在代理人的最优披露下保留了常数因子的福利保证。
- **PDF**: https://arxiv.org/pdf/2609.25410v1

### Firm Valuation When AI Shapes the Business Model: A Milestone-Based Real-Options Framework for the AI Valuation Uncertainty Problem
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.24181v1
- **作者**: Walter Kurz, Wojtek Stricker, Stefan Marx, Frank Reinhardt, Florian Kollberg
- **备注**: 19 pages, 0 figures. Published in Swissi AI Journal under CC BY 4.0
- **摘要**: 标准的估值方法，包括现金流折现法、收益法（德国公共审计师协会的标准 IDW S 1）和市场乘数法，将里程碑概率、后续选择权（续期期权）和风险转移压缩到不透明的综合参数中；没有一种方法能够为将 AI 整合分解为可审计的期权级假设提供结构化的协议。我们提出了一种不限行业的分类法，将 AI 集成商与 AI 提供商区分开来。AI 集成商根据其集成深度级别进一步分类，范围从无集成到以 AI 为产品或流程的核心。基于里程碑关口的实物期权叠加层将里程碑状态价值分解为五个部分，而基于层次分析法的“成功就绪指数”则通过结构化的两两比较得出每个期权的概率，以便进行情景分析。应用于一家 AI 原生的能源软件即服务（SaaS）公司时，该框架产生了一个可追踪到明确期权级假设的相干估值区间。风险集中在后期阶段的后续选择权中，这符合对 AI 提供商的结构性预测。该协议适用于整个公司生命周期，包括并购尽职调查。本案例是对协议连贯性的单公司论证，而非实证检验；针对已实现的退出后估值进行的多案例测试留给未来的研究。
- **PDF**: https://arxiv.org/pdf/2609.24181v1

---