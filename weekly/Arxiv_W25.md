# 🗓️ 周报 (2026-W25)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-06-21

--- 
## 📚 学科: `eess.*`
**学科总结**：本周 `eess` 领域的研究集中在生成式模型与语音信号处理。重点包括：PRDiT 框架通过像素级残差扩散 Transformer 实现了高质量 3D CT 影像生成；语音方面涵盖了针对日语重音质量评估的 PASQA 模型、利用预训练分类器引导的语音生成技术、以及针对口吃检测和零样本 TTS 的改进方案。这些研究显著提升了医疗影像合成的精度及语音交互的自然度。

### Pixel-Level Residual Diffusion Transformer: Scalable 3D CT Volume Generation
- **分数**: 6
- **链接**: https://arxiv.org/abs/2606.20112v1
- **作者**: Zhenkai Zhang, Markus Hiller, Krista A. Ehinger, Tom Drummond
- **备注**: Accepted at ICLR 2026. Code available at https://github.com/Fredy-Zhang/PRDiT
- **摘要**: 生成具有精细细节的高分辨率 3D CT 体数据仍然面临巨大挑战，这源于现有生成模型固有的计算需求和优化困难。在本文中，我们提出了像素级残差扩散 Transformer (PRDiT)，这是一个可扩展的生成框架，可以直接在体素级别合成高质量的 3D 医学影像。PRDiT 引入了一种两阶段训练架构，包括：1) 一个基于 MLP 的盲估计器形式的局部去噪器，在重叠的 3D 补丁上运行以高效分离低频结构；2) 一个全局残差扩散 Transformer，采用内存高效的注意力机制来建模和精炼整个体数据的高频残差。这种由粗到精的建模策略简化了优化，增强了训练稳定性，并有效地保留了微细结构，且不受自动编码器瓶颈的限制。在 LIDC-IDRI 和 RAD-ChestCT 数据集上的大量实验表明，PRDiT 持续优于 HA-GAN、3D LDM 和 WDM-3D 等前沿模型，在 3D FID、MMD 和 Wasserstein 距离得分上显著降低。
- **PDF**: https://arxiv.org/pdf/2606.20112v1

### PASQA: Pitch-Accent-Focused Speech Quality Assessment Model Trained on Synthetic Speech with Accent Errors
- **分数**: 4
- **链接**: https://arxiv.org/abs/2606.20137v1
- **作者**: Masaya Kawamura, Yuma Shirahata, Kentaro Mitsui, Reo Shimizu
- **备注**: Accepted to INTERSPEECH 2026
- **摘要**: 现有的平均意见得分 (MOS) 预测模型通常预测语句级别的自然度 MOS，且对局部音高重音错误不敏感。我们提出了 PASQA（关注音高重音的语音质量评估），专门针对音高重音的正确性。为了训练我们的模型，我们通过使用重音可控的文本转语音系统改变重音模式，构建了一个受控的日语重音错误数据集，并从重音错误率计算伪重音质量分数。PASQA 基于自监督表示，并采用音拍调节融合、排名损失、辅助重音错误定位任务和说话人无关训练。实验表明，传统模型无法保持重音错误严重程度的排序，而 PASQA 在已知和未见过的说话人上均实现了高排序准确度。此外，PASQA 与人类重音正确性判断的一致性更强。
- **PDF**: https://arxiv.org/pdf/2606.20137v1

### Repurposing a Speech Classifier for Guided Diffusion-Based Speech Generation
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.20457v1
- **作者**: Rostislav Makarov, Timo Gerkmann
- **备注**: Accepted for publication in the Proceedings of Interspeech 2026
- **摘要**: 分类器引导是通过使用受噪声调节的分类器来引导采样过程朝向目标类别，从而控制扩散生成的一种方法。分类器引导的一个缺点是它需要两个分别训练的模型：一个分类器和一个扩散模型。因此，我们研究了一种更紧凑的替代方案，即将传统训练的语音分类器重新用作扩散生成的骨干。从 log-Mel 空间中冻结的受噪调节分类器出发，我们附加了一个轻量级子网络，该网络重用分类器的中间表示，并仅在去噪分数匹配目标下训练该子网络。我们的工作表明，预训练分类器可以重新用于条件生成，在判别模型和条件语音合成之间提供了一个极具吸引力的桥梁，从而在单一骨干模型内实现了高语音质量，同时减少了内存占用和计算成本。
- **PDF**: https://arxiv.org/pdf/2606.20457v1

### Stuttering Classification and Segmentation with Attention-Based Multiple Instance Learning
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.20338v1
- **作者**: Petar Sušac, Sebastian P. Bayerl, Hrvoje Džapo
- **备注**: Accepted at Interspeech 2026
- **摘要**: 利用深度学习方法进行口吃检测和分类具有改善口吃严重程度评估过程的潜力。大多数口吃分类数据集仅提供片段级标签，使其不适用于确定单个口吃失语时长所需的细粒度帧级分类。为了克服这一挑战，我们提出了一种基于微调的 wav2vec 2.0、WavLM 和 Whisper 编码器的多示例神经网络架构。我们应用基于示例和基于嵌入的多示例学习方法，在片段级数据集上训练模型，以同时执行片段级和帧级口吃分类任务。结果显示，帧级 F1 分数提高了 23%，片段级 F1 分数提高了 2% 至 9%，证明了我们的模型利用片段级数据进行帧级分割的能力。
- **PDF**: https://arxiv.org/pdf/2606.20338v1

### Transcript-Free Flow-Matching Text-to-Speech via Speech Feature Conditioning
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.20266v1
- **作者**: SooHwan Eom, Hee Suk Yoon, Eunseop Yoon, Mark Hasegawa-Johnson, Chang D. Yoo
- **备注**: Accepted to Interspeech 2026
- **摘要**: 最近的流匹配文本转语音 (TTS) 模型（如 F5-TTS）在推理时依赖于从外部 ASR 系统获得的参考文本。这种依赖性使得零样本 TTS 在面对带有口音或构音障碍的说话人时变得脆弱，而这恰恰是最需要此类场景的时候。此外，我们发现基于文本的参考调节可能会将不寻常语音中的非典型声学模式传播到合成结果中，即使有标注文本也是如此。为此，我们提出了 RTFree-F5，它通过一个轻量级适配器，将连续的自监督语音表示映射到 F5-TTS 的文本调节空间中，从而取代了参考文本，同时重用了预训练检查点。在构音障碍语音上，RTFree-F5 将词错误率 (WER) 从 24.6% 降低到 10.4%，甚至超过了基于标注文本的基准线，同时提高了自然度，并且在不需要任何参考文本的情况下在标准基准测试中保持竞争力。
- **PDF**: https://arxiv.org/pdf/2606.20266v1

--- 
## 📚 学科: `q-bio.*`
**学科总结**：本周 `q-bio` 领域展现了 AI 与生物学的深度融合。研究包括：AMPGAN v3 及其 Agent 框架 PepCraft 用于发现非天然抗菌肽；scGTN 通过深度孪生图变换器改进了单细胞 RNA 测序的聚类效果；受婴儿自发运动激发的强化学习探索机制提升了学习效率；此外还有针对非洲热带森林生态监测的分类模型更新，以及针对孟加拉本土鱼类的蛋白质序列识别研究。

### Agentic Discovery of Non-Canonical Antimicrobial Peptides with AMPGAN v3
- **分数**: 5
- **链接**: https://arxiv.org/abs/2606.17127v1
- **作者**: Jay Jung, Xiaohan Zhang, Shenghan Song, Mahmoud Sayedahmed, Chijian Xiang, Yunong Xu, Ahmed AbdelKhalek, Severin T. Schneebeli, Matthew J. Wargo, Jianing Li, Safwan Wshah
- **备注**: Presented at the GenBio Workshop, ICML 2026
- **摘要**: 抗菌素耐药性每年导致超过一百万人死亡。抗菌肽 (AMPs) 是一种很有前景的解决方案，但现有的生成式 AMP 模型尚无法设计包含非天然氨基酸和/或化学修饰的肽，而这对于实际的肽类药物至关重要。我们提出了 AMPGAN v3，这是一种多目标条件 GAN，它将生成词汇扩展到了 D-型氨基酸和 N/C 端修饰（如酰胺化）。通过在两个专门的判别器中分离对抗性监督和活性感知监督，AMPGAN v3 显著提高了训练稳定性，并在外部分类器上的表现超过了之前的生成式 AMP 模型。我们通过体外实验验证了涵盖三个结构类别的五个候选物；其中两个对革兰氏阳性菌株表现出活性，表现最好的候选物对枯草芽孢杆菌的最小抑菌浓度 (MIC) 达到 8 μg/mL。为了支持下游筛选，我们进一步提出了 PepCraft，这是一个用于端到端 AMP 发现的多智能体框架，其中规划智能体协调专门的执行器进行生成、过滤和验证。其优先级建议与我们的体外实验结果一致。
- **PDF**: https://arxiv.org/pdf/2606.17127v1

### scGTN: Deep Siamese Graph Transformer Network for Single-cell RNA Sequencing Clustering
- **分数**: 4
- **链接**: https://arxiv.org/abs/2606.18672v1
- **作者**: Jinke Wu, Yifan Wang, Siyu Yi, Caiyang Yu, Ziyue Qiao, Nan Yin, Jiancheng Lv, Wei Ju
- **备注**: Accepted by IJCAI 2026
- **摘要**: 单细胞 RNA 测序 (scRNA-seq) 在表征细胞水平的基因表达方面起着关键作用，能够识别细胞类型并推进对细胞异质性的理解。尽管 scRNA-seq 数据聚类取得了显著进展，但我们认为当前方法往往忽略了稀疏性和噪声，以及 scRNA-seq 数据中固有的复杂细胞间结构信息。为此，本文提出了一种通过深度孪生图变换器网络进行单细胞 RNA-seq 聚类的新框架 (scGTN)，该框架明确集成了基因表达谱和细胞间结构依赖性进行细胞聚类。特别地，我们将 scRNA-seq 数据表述为一个图，并构建了两个增强图视图作为双视图，以捕获互补的细胞间信息。然后，采用孪生图变换器网络显式地结合最短路径信息和节点距离，以捕捉细胞间更丰富的结构关系。最后，我们采用最优传输策略以自监督的方式指导细胞聚类。
- **PDF**: https://arxiv.org/pdf/2606.18672v1

### Infant Spontaneous Movement Noise Improves Exploration in Deep RL
- **分数**: 4
- **链接**: https://arxiv.org/abs/2606.16590v2
- **作者**: Francisco M. López, Markus R. Ernst, Francisco Cruz, Matej Hoffmann, and Jochen Triesch
- **备注**: Accepted at IEEE ICDL 2026
- **摘要**: 深度强化学习 (RL) 中的探索通常实现为时间上不相关的白噪声。然而，最近的研究表明，时间相关的有色噪声可以通过产生具有更好状态空间覆盖度的平滑轨迹来提高探索效率。我们探究受婴儿自发运动启发的动作噪声是否也能改善深度 RL 中的探索。我们发现婴儿末端执行器速度的功率谱密度遵循一个有色噪声过程，其光谱指数随年龄增长而增加。受此发育模式启发，我们引入了一种机制，在 RL 训练期间逐渐增加探索噪声的时间自相关性，使其与婴儿统计数据匹配。在多个 RL 环境中的实验表明，受婴儿启发的噪声产生了结构化的探索行为，并且与传统的探索策略相比，可以提高学习效率。
- **PDF**: https://arxiv.org/pdf/2606.16590v2

### DeepForestVisionV2: Ecology-Driven Taxonomy Expansion for Camera-Trap Monitoring in African Tropical Forests
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.20223v1
- **作者**: Hugo Magaldi, et al.
- **备注**: Accepted at ICPR 2026 Workshop
- **摘要**: 非洲热带森林的红外相机监测正越来越多地从密闭林冠扩展到河岸、林间空地和公园边缘。我们提出了 DeepForestVisionV2，这是一个生态驱动的扩展版本，将预测类别从 35 类增加到 64 类（61 个动物类，加上人、车辆和空白），旨在解决三个反复出现的部署梯度：垂直分层、场景开放程度和人为界面。DeepForestVisionV2 在来自多个非洲热带森林项目的 1,535,010 张照片和 243,354 段视频上进行了训练。在部署基准测试中，尽管分类任务更加困难，它依然保持或提高了基准准确度，同时将林内视频识别出的分类群数量从 22 种增加到 29 种，河岸处从 4 种增加到 9 种。在公园边缘用例中，它将准确度从 0.62 提高到 0.86，并将虚警次数从 11 次减少到 0 次。
- **PDF**: https://arxiv.org/pdf/2606.20223v1

### Protein-Based Fish Species Identification: Dataset, Models, and Insights from Native Bangladeshi Fish
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.18302v1
- **作者**: Md Nasiat Hasan Fahim, Md. Abid Ullah Muhib, Mohammad Shahidur Rahman
- **备注**: Published in 2026 IEEE QPAIN
- **摘要**: 正确识别鱼类物种对于孟加拉国的粮食安全、经济发展和气候适应具有重要意义。本研究引入了第一个包含 9 种孟加拉国本土鱼类、2845 条高质量蛋白质序列的策划数据集。我们提出了一种可实际部署的新型混合架构 MotifCNN-Transformer+TA-PE。我们的新架构实现了 79.80% 的准确率，且比微调后的蛋白质语言模型 ProtBERT 快约 5 倍，体积小 42 倍。我们的研究展示了系统发育关系对序列相似性的影响，并为南亚蛋白质依赖型经济中的渔业管理、食品鉴定和生物多样性保护开辟了路径。
- **PDF**: https://arxiv.org/pdf/2606.18302v1

--- 
## 📚 学科: `cs.*`
**学科总结**：本周 `cs` 领域涵盖了模型偏见评估、贝叶斯学习和代码能力基准等前沿课题。核心论文包括：StylisticBias 揭示了多模态大模型对社会偏见的视觉诱因；Multi-Task 贝叶斯语境学习框架提升了不确定性量化效率；Multi-LCB 将代码生成基准扩展至 12 种语言以检测 Python 过拟合；此外还有针对无人驾驶导航中快速预测人类注意力的轻量化模型 GazeLNN。

### StylisticBias: A Few Human Visual Cues Drive Most Social Biases in MLLMs
- **分数**: 7
- **链接**: https://arxiv.org/abs/2606.20527v1
- **作者**: Shaghayegh Kolli, Timo Cavelius, Nafiseh Nikeghbal, Samantha Dalal, Jana Diesner
- **备注**: Accepted to ICML 2026 Workshop
- **摘要**: 多模态大语言模型 (MLLMs) 越来越多地部署在涉及个人和社会重要后果的场景中，然而塑造模型如何判断人的视觉线索仍未被充分理解。我们引入了 StylisticBias，这是一个用于评估 MLLMs 属性级社会偏见的受控基准。我们生成了 500 个写实的基础面孔，并为每个面孔创建了约 50 个单属性变体，共产生约 2.5 万张图像。该设计保持身份固定，一次仅更改一个视觉属性。我们评估了 6 个 MLLMs 在 25 个二元社会判断场景下的表现。研究发现，年龄和体型主导了身份层面的影响，而时尚风格和其他视觉线索驱动了最大的属性层面偏移。此外，大约 15 个属性解释了近 80% 的总变异，表明偏见集中在少数视觉线索中。
- **PDF**: https://arxiv.org/pdf/2606.20527v1

### Multi-Task Bayesian In-Context Learning
- **分数**: 4
- **链接**: https://arxiv.org/abs/2606.20538v1
- **作者**: Qingyang Zhu, Eric Karl Oermann, Kyunghyun Cho
- **备注**: ICML 2026
- **摘要**: 贝叶斯预测推理为不确定性量化、数据效率和稳健泛化提供了原则性框架。然而，精确推理往往难以处理，而可扩展的近似方法可能计算昂贵。我们引入了一个多任务语境学习框架，用于摊销层次贝叶斯预测推理，该框架显式地将先验信息表示为语境数据集的前缀。在序列先验和目标任务上训练的 Transformer 学习跨先验家族自适应其预测。在包括分布外先验和具有高维潜在结构的先验在内的一系列评估中，我们的方法匹配了 Oracle 贝叶斯预测器，同时速度快了几个数量级。我们进一步在真实世界的时空温度预测基准上证明了其应用价值。
- **PDF**: https://arxiv.org/pdf/2606.20538v1

### Multi-LCB: Extending LiveCodeBench to Multiple Programming Languages
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.20517v1
- **作者**: Maria Ivanova, et al.
- **备注**: ICLR 2026
- **摘要**: LiveCodeBench (LCB) 已成为评估大语言模型 (LLMs) 代码生成任务的广泛基准，但此前仅限于 Python。我们引入了 Multi-LCB，这是一个用于评估 LLMs 在包括 Python 在内的 12 种编程语言中表现的基准。Multi-LCB 将 LCB 数据集中的 Python 任务转换为其他语言的等效任务，同时保留了 LCB 的污染控制和评估协议。我们对 24 个 LLMs 进行了评估，发现了 Python 过拟合、特定语言污染以及多语言性能显著差异的证据。
- **PDF**: https://arxiv.org/pdf/2606.20517v1

### Fast Human Attention Prediction for Fixation-guided Active Perception in Autonomous Navigation
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.20491v1
- **作者**: Fatma Youssef Mohammed, Grzegorz Malczyk, Kostas Alexis
- **备注**: Accepted to IROS 2026
- **摘要**: 我们引入了 GazeLNN，这是一种计算量极轻的扫描路径预测模型，它利用液体神经网络 (Liquid Neural Networks) 作为回归引擎，并采用 MobileNetV3 进行特征提取。尽管仅需 0.61 GFLOPs，GazeLNN 在 MIT 低分辨率数据集上实现了 SOTA 性能，计算成本降低了 99.40%，推理速度加快了 6 倍。我们将 GazeLNN 集成到通过强化学习训练的主动摄像机-机器人控制策略中，实现了自主导航过程中的人类注视引导感知，并通过空中机器人的实际部署验证了其有效性。
- **PDF**: https://arxiv.org/pdf/2606.20491v1

--- 
## 📚 学科: `math.*`
**学科总结**：本周 `math` 领域的代表性研究提出了针对物理信息神经网络 (PINNs) 的进化两阶段超参数优化策略，通过结合进化算法的全局探索能力与梯度下降的局部精炼能力，解决了 PINNs 在求解偏微分方程时面临的非凸损失函数优化难题。

### Evolutionary Two-Stage Hyperparameter Optimization Strategies for Physics-Informed Neural Networks
- **分数**: 6
- **链接**: https://arxiv.org/abs/2606.20442v1
- **作者**: Fedor Buzaev, et al.
- **备注**: Accepted to the ICLR 2026 Workshop on AI and PDEs
- **摘要**: 物理信息神经网络 (PINNs) 通过将物理规律嵌入神经网络训练来求解偏微分方程 (PDEs)。然而，由于物理信息损失函数具有高度非凸和多项结构，其性能常受到收敛不稳定、训练平台期以及对架构和优化超参数高度敏感的影响。我们提出并研究了一种基于进化算法的两阶段方法。在第一阶段，我们使用截断周期的低保真训练运行来快速筛选候选配置；在第二阶段，仅对最有希望的候选者进行标准梯度优化器的完整训练。在平流方程、Klein-Gordon 和 Helmholtz 方程上的评估表明，该方法在固定计算预算内显著降低了平均误差。
- **PDF**: https://arxiv.org/pdf/2606.20442v1

--- 
## 📚 学科: `astro-ph.*`
**学科总结**：本周 `astro-ph` 领域涵盖了软件工具开发、恒星演化及行星大气研究。包括：用于自动估计星系棒长度的 Python 包 `elma`；用于创建光度数据立方体的工具 `lightstack`；对食联星 V505 Mon 的演化阶段分析；对木星 X 射线和紫外线对太阳活动响应的长期观测研究；以及对未来十年 X 射线极化测量仪器的前瞻设计。

### ELMA: ELlipse-based bar MAjor axis estimator
- **分数**: 4
- **备注**: Published in RNAAS. 自动化星系棒长度估计工具。
- **摘要**: 星系棒是圆盘星系中关键的非轴对称结构。我们推出了 `elma`，这是一个独立的 Python 包，用于对已识别为棒旋系统的星系进行自动棒长估计。该方法通过迭代椭圆等光度线拟合来追踪径向椭率剖面。
- **PDF**: https://arxiv.org/pdf/2606.20370v1

### A long-term spectro-temporal study of Jovian X-ray and Ultraviolet response to solar activity
- **分数**: 3
- **备注**: Accepted for publication in MNRAS. 木星与太阳活动关系研究。
- **摘要**: 我们利用 IUE 和 Chandra 空间望远镜数十年的观测数据，研究了木星辐射随太阳活动的变化。分析显示木星的 Ly$\alpha$ 发射与太阳 X 射线通量密切相关，而日冕物质抛射 (CMEs) 后检测到的木星 X 射线爆发支持了 CME 驱动木星极光激发的观点。
- **PDF**: https://arxiv.org/pdf/2606.20355v1

--- 
## 📚 学科: `stat.*`
**学科总结**：本周 `stat` 领域的研究集中在强化学习与决策优化的理论前沿。研究重点包括：处理奖励非随机缺失情况下的离线策略评估方法；在匹配市场中引入累积前景理论以模拟人类偏好，并实现对抗鲁棒学习；以及提出一种无需调用求解器即可训练“预测并优化”模型的扩展方法，大幅提升了计算效率。

### Off-Policy Evaluation for Missingness-Aware Policies in MDPs with Rewards Missing Not at Random
- **分数**: 6
- **链接**: https://arxiv.org/abs/2606.20206v1
- **作者**: Ziheng Wei, Annie Qu, Rui Miao
- **备注**: Accepted at ICML 2026
- **摘要**: 在离线强化学习中，由于记录稀疏或截断，即时奖励往往无法观测。当奖励是非随机缺失 (MNAR) 时，即使在给定状态和动作的情况下也会产生选择偏误。我们引入了一个桥接函数，无需显式建模 MNAR 机制即可恢复条件平均奖励，并通过最小-最大程序进行估计以避免双重采样。我们建立了一致性和有限样本误差界限，并在模拟数据和 MIMIC-III 败血症数据上证明了方法的强劲性能。
- **PDF**: https://arxiv.org/pdf/2606.20206v1

### A Solver-Free Training Method for Predict-then-Optimize
- **分数**: 6
- **链接**: https://arxiv.org/abs/2606.19587v1
- **作者**: Beichen Wan, Mo Liu
- **备注**: Accepted by ICML 2026
- **摘要**: 我们提出了一种在“预测并优化”范式下训练预测模型的可扩展方法。现有方法在每次梯度评估时都需要调用昂贵的求解器。我们基于测度转换原理提出了一种决策聚焦的学习流程，产生了一个在训练期间完全无需优化求解器的替代损失函数。实验证明，该方法在保持竞争力的决策质量的同时，将训练时间缩短了几个数量级。
- **PDF**: https://arxiv.org/pdf/2606.19587v1

--- 
## 📚 学科: `econ.*`
**学科总结**：本周 `econ` 领域探讨了 AI 对劳动力市场的影响及复杂的策略学习理论。研究包括：针对分布值结果的 Wasserstein 策略学习框架；应用热力学原理描述全球财富不平等的普遍规律；以及关于 AI 任务链化如何重新定义工作结构和生产力增益的理论模型。

### Chaining Tasks, Redefining Work: A Theory of AI Automation
- **分数**: 3
- **链接**: https://arxiv.org/abs/2606.15960v1
- **作者**: Mert Demirer, John J. Horton, Nicole Immorlica, Brendan Lucier, Peyman Shahidi
- **备注**: Accepted to EC '26
- **摘要**: 生产是一系列步骤，可以手动执行、由 AI 增强或在被称为“链”的连续 AI 执行步骤中完全自动化。企业在专业化收益与协调成本之间权衡，将步骤打包成任务。模型揭示了 AI 质量提升带来的非线性生产力增益。实证证据支持了模型的关键预测：AI 执行的步骤倾向于在链中共同出现，且任务的邻接性会增加其被 AI 自动化的可能性。
- **PDF**: https://arxiv.org/pdf/2606.15960v1

---