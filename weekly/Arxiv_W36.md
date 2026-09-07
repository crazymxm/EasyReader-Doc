# 🗓️ 周报 (2026-W36)

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
> 更新时间: 2026-09-06

--- 
## 📚 学科: `eess.*`
### ToolDF: Tool-Integrated Reasoning for Mixed-Authenticity Audio Deepfake Detection
- **分数**: 6
- **链接**  https://arxiv.org/abs/2609.03620v1
- **作者**: Taewoo Kim, Young Han Lee, Nam In Park, Chanwoo Kim
- **备注**: To appear in Findings of the Association for Computational Linguistics: EMNLP 2026
- **摘要**: 语音深度伪造检测通常被表述为单域音频的剪辑级二分类任务。然而，现实世界中的篡改音频往往表现出混合的真实性，即真实和篡改的线索跨越时间过渡、重叠声源或两者并存。这种设置不仅需要检测篡改的音频，还需要定位为决策提供证据的组件。我们提出了 ToolDF，一个用于混合真实性音频伪造检测的工具集成推理框架。ToolDF 采用音频大语言模型作为协调器，并使用监督工具使用轨迹进行训练。它能自适应地分析音频场景，选择性地进行声源分离，将各个组件路由到特定领域的专家模块，并将它们的证据聚合为一个具有可解释性的判定。我们进一步引入了一个涵盖时间过渡、声学重叠和混合物合流的混合真实性音频伪造检测基准。实验结果表明，ToolDF 在复合类型检测上取得了最佳的综合性能，相比于最强的单体基线和固定流水线，其 macro-F1 分数分别提升了 3.72 和 14.39，同时还能提供定位到具体时间区域和声源的可解释证据。我们的源代码和数据集已在网上公开。
- **PDF**: https://arxiv.org/pdf/2609.03620v1

### Geometry-Aware Graph Construction via Adaptive Spectral Bandwidth Control
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.03306v1
- **作者**: Ecem Bozkurt, Antonio Ortega
- **备注**: Accepted at IEEE MLSP 2026. 6 pages, 4 figures
- **摘要**: 使用高斯核的核化图方法（如谱聚类、扩散映射和稀疏核回归图）依赖于高斯带宽参数 $\sigma$ 的选择，该参数决定了局部核算子的谱特征。当 $\sigma$ 过小时，核函数会高估局部复杂度，并将每个样本视为独立方向；而当 $\sigma$ 过大时，核函数会将多个方向折叠在一起，导致条件数发散，丢失所有的几何鉴别能力。我们提出了一种尺度选择方法，使核的谱复杂度与底层流形的固有复杂度相一致。我们提出了一种基于单节点的带宽标准，通过联合匹配核的有效秩与通过最小生成树估计的局部内在维度来实施这一原则，从而将搜索锚定在与流形一致的双对数缩放区间内。我们在 CIFAR-100 上评估了来自六个编码器的自监督学习（SSL）嵌入，结果表明，与固定带宽方法和竞争的自适应方法相比，自适应带宽一致地提高了留一法（LOO）分类和标签传播（LP）的准确率。
- **PDF**: https://arxiv.org/pdf/2609.03306v1

### Coupling-Aware Aggregation of Multi-Zone HVAC Loads under Uncertainty: A Two-level Framework
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.03253v1
- **作者**: Jingguan Liu, Han Jiang, Xiaomeng Ai, Shengshi Wang, Xizhen Xue, Shichang Cui, Jinming Hou, Jiakun Fang, Jinyu Wen
- **备注**: Published in: IEEE Transactions on Smart Grid (vol. 17, no. 3, pp. 2077-2091, 2026)
- **摘要**: 聚合建筑暖通空调（HVAC）负荷可为电力系统释放巨大的需求侧灵活性。然而，多区域耦合带来了复杂的相互依赖性和不确定性传播，使得量化聚合灵活性变得异常困难。为了解决这个问题，本文提出了一种耦合感知的两级聚合框架。在建筑级别，采用定制的高斯消元法和坐标变换技术，将高维热动力学重新表述为等效的低维解析表达式。该表达式通过以下方式简化了后续的聚合器级别阶段：（i）阐明了区域级不确定性向建筑级接口的传播路径；（ii）将建筑内部的多区域耦合与建筑间的聚合进行解耦；（iii）提供了全维度的建筑级灵活性集合，以实现易于处理的重构。在聚合器级别，通过新开发的矩阵变换技术推广了现有的几何聚合方法。该技术有效地构建了不同维度多胞体之间的内逼近，从而在电力子空间中生成高维多区域 HVAC 灵活性的闭式图像。随后，所得的内逼近被重构为一个定制的可分离线性规划，以高效确定最佳聚合参数。案例研究验证了我们框架的有效性，突出了其准确性、可靠性和可扩展性。
- **PDF**: https://arxiv.org/pdf/2609.03253v1

### Preference-Oriented Aggregation of Heterogeneous Distributed Energy Resources for Reserve Dispatch
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.03252v1
- **作者**: Jingguan Liu, Xiaomeng Ai, Shichang Cui, Xizhen Xue, Shengshi Wang, Jiakun Fang, Wei Yao, Jinyu Wen
- **备注**: Published in: IEEE Transactions on Smart Grid (vol. 17, no. 2, pp. 1264-1279, 2026)
- **摘要**: 聚合分布式能源（DERs）旨在将其集体灵活性编码为一个单一集合，以便进行高效的电网调度。然而，由于两个主要挑战，现有的聚合方法对于异构 DER 而言过于保守：1）维度异构性，这使跨不同时间维度的灵活性结合变得复杂；2）类型异构性，多样且不规则的 DER 曲线阻碍了准确的近似，导致显著的灵活性损失。为了解决这些挑战，本文提出了一种新型的面向偏好的备用调度聚合方法。针对维度异构性，我们通过使用矩阵变换技术将闵可夫斯基和重构为多胞体投影问题，从而扩展了现有技术。通过在高维空间中统一 DER 并将其投影回聚合可行域，所提技术有效地聚合了维度异构的 DER。针对类型异构性，我们进一步开发了一个分布式聚合-调度协调框架，将备用调度偏好纳入聚合中。该框架有效地捕捉了在最佳备用调度中优先考虑的关键、主动的聚合灵活性，从而显著减少了聚合类型异构 DER 时的灵活性损失。数值测试验证了我们方法在解决这两种异构性方面的有效性，并突出了其在具有高备用需求电力系统中的应用潜力。
- **PDF**: https://arxiv.org/pdf/2609.03252v1

### Modulation Analysis with Higher-Order Spectra
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.03172v1
- **作者**: Christopher K. Kovach, Sukhbinder Kumar
- **备注**: 42 pages, 10 figures. A previous version of this preprint was published under the title "A Slice of Trispectrum for Patterns of Modulation" at https://doi.org/10.36227/techrxiv.21401703.v1
- **摘要**: 在生理信号分析中，经常需要识别频谱功率的调制。通过滤波和包络提取来估计相关频带中的功率存在若干局限性：滤波器的选择可能会使所得估计产生偏差，而加性高斯噪声由于包络计算的非线性会变得非高斯。本工作探讨了高阶累积量的谱分解（高阶谱，HOS）如何避免这些限制，重点是利用三重谱（trispectrum）来识别调制振荡。具体而言，本文展示了：1）通过将三重谱视为 Wigner-Ville 分布的互谱，可以将其解释为跨频率功率线性依赖关系的度量。2）三重谱的一个特定二维子域有助于识别调制载波，在恢复调制信号和载波信号的关键谱特性的同时，避免了完整三重谱估计的三次方复杂度。该子域的一种表示形式——调制图（modulogram），被证明是识别和区分不同调制形式的有用工具。3）作为一种由累积量推导出的度量，调制图不会受到加性高斯噪声的干扰。4）调制图的相位保留了可用于识别调制时间模式的信息。5）最近提出的一种高阶谱加性分解方法（HOSD）在应用于三重谱时，能进一步辅助识别。我们通过盲检测啮齿动物和人类局部场电位记录中的 $\beta$ 爆发（beta bursts）阐明了这些进展。最后，我们探讨了本方法与先前通过矩最大化进行盲识别（BI）的技术（包括盲解卷积和独立成分分析）之间的关系。
- **PDF**: https://arxiv.org/pdf/2609.03172v1

### 学科总结
本期 `eess.*` 领域的论文主要聚焦于信号处理、图学习以及智能电网中的资源聚合优化。具体研究包括：利用语音大模型进行混合真实性语音伪造检测的 ToolDF 框架；通过自适应谱量化控制来优化图构建的几何感知方法；针对多区域暖通空调（HVAC）负荷和异构分布式能源（DER）的电力系统聚合与灵活调度策略；以及利用高阶谱分析生理信号功率调制的理论与应用。这些工作展示了信号分析与控制优化在安全、能源及生物医学领域的深度融合。

--- 
## 📚 学科: `q-bio.*`
### SimpleDesign: A Joint Model for Protein Sequence and Structure Codesign
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.03377v1
- **作者**: Jiarui Lu, Yuyang Wang, Yizhe Zhang, Jiatao Gu, Navdeep Jaitly, Joshua M. Susskind, Miguel Ángel Bautista
- **备注**: Published in Transactions on Machine Learning Research (TMLR), 2026. https://openreview.net/forum?id=wPfw7GkMns
- **摘要**: 蛋白质是生物学过程的基础，其功能由氨基酸序列与三维结构之间复杂的相互作用所决定。开发能够理解这种本质上多模态关系的生成模型，对于药物发现和蛋白质工程等领域至关重要。现有的模型通常依赖于多阶段训练过程：第一阶段训练自编码器将数据标记为潜在表示；第二阶段在自编码器的潜在表示上训练生成模型，即在潜在空间中进行生成建模。我们假设，获得高性能的协同设计模型并不一定需要这种多阶段训练，因此提出了 SimpleDesign——一个直接在数据空间中进行训练的高效多模态蛋白质设计模型。SimpleDesign 采用单阶段端到端目标，将用于序列的离散交叉熵与用于结构的回归目标结合起来。为了有效地对序列和结构模态的差异进行建模，我们开发了一种 Mixture-of-Transformer 架构，该架构在允许进行模态专属处理的同时，保持对两种模态的全局自注意力。我们在超过 200 万个“序列-结构”对上训练了 SimpleDesign，在协同设计和无条件序列/结构生成基准测试中均取得了强劲的表现。
- **PDF**: https://arxiv.org/pdf/2609.03377v1

### A mechanistic modeling framework to interpret ACTH stimulation tests across HPA axis adaptation states and glucocorticoid feedback dynamics
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.01684v1
- **作者**: Mamta Yadav, Phool Singh
- **备注**: 11 pages, 1 Table, 6 Figures; Matches the version published in Computers in Biology and Medicine
- **摘要**: 下丘脑-垂体-肾上腺（HPA）轴是协调对生理和心理压力产生内分泌反应的关键调节系统。虽然促肾上腺皮质激素（ACTH）刺激测试仍是评估肾上腺功能的基石，但其解释因慢性压力暴露下 HPA 轴的动态和自适应特性而变得复杂。特别是，长期压力会诱导腺体塑造、糖皮质激素受体（GR）抵抗和延迟的反馈恢复，所有这些都可能改变测试结果，而并不表明原发性肾上腺功能衰竭。在本研究中，我们提出了一个结合了激素动力学、反馈抑制以及促皮质激素和肾上腺区域功能质量适应的机制建模框架。我们模拟了涵盖基线、慢性压力和恢复三个阶段的 180 天 HPA 轴过程，同时引入了随时间变化的 GR 抵抗函数，以模拟反馈脱敏及其消退。使用该框架，我们评估了不同生理阶段的低剂量（$1\ \mu\text{g}$）和高剂量（$250\ \mu\text{g}$）ACTH 刺激测试。我们的模拟结果表明，皮质醇反应对压力暴露的幅度和时机都高度敏感，且 ACTH 的反应性具有阶段依赖性，由于持续的反馈抵抗，在恢复期往往会变弱。低剂量 ACTH 测试能更可靠地反映部分肾上腺适应，而高剂量测试由于超生理驱动，存在掩盖功能障碍的风险。这些结果突出了静态测试范式的局限性，并表明在应激相关或治疗引起的肾上腺疾病中，考虑腺体可塑性和 GR 反馈动力学对于有效的内分泌诊断至关重要。
- **PDF**: https://arxiv.org/pdf/2609.01684v1

### 学科总结
本期 `q-bio.*` 领域选入了两篇结合人工智能与机制建模的高水平论文。第一篇提出了 SimpleDesign，一个用于蛋白质序列和结构协同设计的端到端单阶段生成模型，避免了传统的多阶段潜在空间训练，提升了多模态蛋白质设计的效率。第二篇则针对人体内分泌系统，构建了 HPA 轴在慢性压力与恢复期下的机制数学模型，系统评估了不同剂量 ACTH 刺激测试的诊断可靠性，为应激相关内分泌疾病的临床诊断提供了新的计算生理学支持。

--- 
## 📚 学科: `cs.*`
### The Shape of Time: Video-Token Contrast for Temporal Understanding in VideoLMs
- **分数**: 7
- **链接**  https://arxiv.org/abs/2609.04110v1
- **作者**: Yumeng Shi, Quanyu Long, Yin Wu, Wenya Wang
- **备注**: Accepted to EMNLP 2026 (main)
- **摘要**: 按顺序观看视频帧并不等同于表征时间。现代视频大语言模型（VideoLMs）接收有序的视频流，但其主要监督信号作用于生成的文本，而非最先涌现事件动力学的视频 Token 表征。这种不匹配使得模型可以通过物体、场景和语言先验等快捷方式来学习时间维度的答案，而无需其内部视频表征去捕获事件的发展过程。为了解决这一问题，我们为 VideoLM 提出了一种表征级的时间反事实目标 VT-Contrast。该设计探究了时间监督应该在何处起作用，以及它应该揭示何种时间差异。VT-Contrast 监督选定的深层最后一帧视频 Token（这些 Token 在语言生成前被预期用于整合时间信息），并将保持顺序的视图与按肯德尔等级相关系数（Kendall tau）距离分级的同视频重排序反事实视图进行对比。它不需要改变模型架构，兼容于多种 VideoLM 训练任务，并提升了跨时间理解基准的整体性能。我们的代码可在 https://github.com/ANDgate99/VT-Contrast 获得。
- **PDF**: https://arxiv.org/pdf/2609.04110v1

### Seeing Before Synthesizing: VLM-Guided Transition Event Discovery for Weakly-Supervised Dense Video Captioning
- **分数**: 6
- **链接**  https://arxiv.org/abs/2609.04183v1
- **作者**: Ye-Chan Kim, Seunghee Choi, SeungJu Cha, Si-Woo Kim, Hwiseon Kim, Hyungee Kim, Dong-Jin Kim
- **备注**: Accepted to EMNLP 2026 (main, long)
- **摘要**: 弱监督密集视频字幕生成（Weakly-Supervised Dense Video Captioning）旨在仅给定每个视频的一组有序事件级字幕的前提下，定位并描述未剪辑视频中的多个事件。最近的研究通过大语言模型（LLM）合成辅助过渡字幕来提供额外的视觉-语言对齐，但这些字幕缺乏视觉接地（visual grounding），并且以固定的位置和时长僵硬地分配给每个事件间隔。为了解决这些问题，我们提出了“先看后合成”（Seeing Before Synthesizing, SBS）框架，它能够仅在有理论依据的地方自适应地提供基于视觉接地的语言引导。利用视觉语言模型（VLM），我们为事件之间的间隔生成帧级叙事，并从这些叙事的语义变化中检测过渡。对于识别出的过渡，我们通过融合时间中点与语义变化点，并选择使视觉-语言对齐最大化的宽度，来细化事件间的时间掩码。在 ActivityNet Captions 和 YouCook2 上的实验表明，该方法在字幕生成和定位方面都达到了最先进的性能。
- **PDF**: https://arxiv.org/pdf/2609.04183v1

### Knowledge Acquisition During Pre-training? Large Language Models Learn Better With Auxiliary Views
- **分数**: 6
- **链接**  https://arxiv.org/abs/2609.04180v1
- **作者**: Joseph Lee, Yidi Huang, Dokyoon Kim, Shu Yang, Li Shen
- **备注**: Accepted to Findings of EMNLP 2026
- **摘要**: 在我们理解大语言模型（LLM）如何在预训练期间获取知识方面仍存在空白。我们假设，辅助视图（即知识的重新表述）在因果上有助于学习。我们设计了对照实验来分离这一效应。首先，我们证实了重复对于知识获取是必要的，并阐明了改写仅在较小批次大小时有帮助。其次，在保持 Token 预算固定的情况下，将用于文档重复的 Token 分配给辅助视图，反直觉地提高了学习效果，即使对于事实性回忆也是如此。第三，辅助视图的有效性并不取决于生成它们的教师模型的强弱。第四，我们确定了在存在先验知识差距的情况下有助于学习的知识形式（上下文知识和基础知识）。最后，我们通过层级偏差和压缩机制研究了这些效应。我们的发现共同表明，预训练语料库中自然产生的知识辅助表示是预训练成功的关键因素，并为为什么数据多样性如此重要提供了一个合理解释。
- **PDF**: https://arxiv.org/pdf/2609.04180v1

### Compile by Training: Turning Natural-Language Specifications into Local Neural Functions
- **分数**: 4
- **链接**  https://arxiv.org/abs/2609.04199v1
- **作者**: Yuntian Deng, Pengyu Nie, Stuart Shieber
- **备注**: EMNLP 2026 System Demonstrations. Demo: https://programasweights.com
- **摘要**: 许多循环文本功能很容易用自然语言描述，但很难用规则来实现；而为每个输入调用远程大模型则会带来重复的成本、延迟以及对服务提供商的依赖。我们提出了“通过训练进行编译”（compile by training）方法，将自然语言规范转化为可重用的本地神经网络函数。在编译时，教师模型生成特定任务的示例，用于为紧凑的解释器训练一个小适配器。生成的神经函数在没有教师模型的情况下也可以运行，并且可以像普通软件一样进行存储、版本控制和组合。在 FuzzyBench-Hard（Program-as-Weights 快速编译器无法产生精确匹配的子集）上，“通过训练进行编译”达到了 83.6% 的语义准确率。这种更高的准确率伴随着更高的编译成本：快速编译器仅需几秒钟，而本方法大约需要一分钟。我们在公共互动服务中部署了该编译器，并在多站点网站助手、语言控制的 3D 虚拟化身以及双向英文-克劳德语（Claudish）翻译器中展示了编译后的神经函数。
- **PDF**: https://arxiv.org/pdf/2609.04199v1

### BooM-VVT: Boosting Mask-Free Video Virtual Try-On with Image-Level Pseudo Data
- **分数**: 4
- **链接**  https://arxiv.org/abs/2609.04120v1
- **作者**: Wei Zhang, Xin Li, Peishu Shi, Jialin Gao, Xuekang Peng, Zhichao Lian, Yeying Jin
- **备注**: 23 pages, 18 figures, 8 tables. Accepted to ACM Multimedia 2026 (MM '26)
- **摘要**: 视频虚拟试衣（VVT）旨在生成一个人穿着目标衣服的真实视频。最近的方法利用关键帧驱动的视频生成范式来提高野外环境下的表现，但它们仍然依赖掩码（masks）来定位试衣区域，这使它们在面对大幅度动作和严重遮挡时显得十分脆弱。虽然无掩码的基于图像的试衣方法通过利用大规模伪数据取得了令人满意的效果，但将这一范式扩展到视频仍然很困难，因为构建视频级的伪数据成本高昂。此外，粗糙的关键帧采样和多视角试衣数据的匮乏，限制了现有的关键帧驱动方法在保持衣服一致性和处理多样化试衣任务方面的能力。为了应对这些挑战，我们提出了 BooM-VVT，一个基于关键帧驱动范式构建的无掩码 VVT 框架。为了实现无掩码 VVT，我们引入了一种多阶段训练策略，该策略利用图像级伪数据进行无掩码定位学习，从而大幅减少了对高成本视频级伪数据的需求。为了提高衣服一致性，我们提出了衣服敏感关键帧采样（Garment-Sensitive Keyframe Sampling），它根据与衣服相关的身体区域选择关键帧，以更好地捕捉衣服的外观。我们进一步引入了帧共享 3D 旋转位置编码（Frame-Shared 3D-RoPE），以在关键帧和目标视频帧之间建立时空对应关系，从而实现精确的衣服细节迁移。最后，我们构建了 OmniView，一个大规模多视角试衣数据集，以支持在复杂摄像机视角和多样化试衣任务下生成可靠的试衣视频。大量实验表明，BooM-VVT 相比现有方法实现了更优的时间一致性和衣服保真度。项目页面：https://boomvvt.github.io/boomvvt。
- **PDF**: https://arxiv.org/pdf/2609.04120v1

### 学科总结
本期 `cs.*` 领域的论文聚焦于多模态大模型（VLM/VideoLM）、大模型预训练机制、本地模型蒸馏以及视频虚拟试衣等前沿方向。研究涵盖：通过表征级时间对比（VT-Contrast）提升视频大模型的时间理解能力；基于 VLM 引导的过渡事件发现（SBS）优化弱监督密集视频字幕生成；深入探索预训练中“辅助视图”对大语言模型知识获取的促进作用；提出“编译即训练”框架，将自然语言规范高效转化为可离线运行的本地微型神经函数；以及提出 BooM-VVT 框架，攻克了视频虚拟试衣中大动作和遮挡导致掩码失效的难题。

--- 
## 📚 学科: `math.*`
_本周缺少高价值论文_

### 学科总结
本周在 `math.*` 学科下未筛选出符合高质量要求的推荐论文。

--- 
## 📚 学科: `astro-ph.*`
### Low-angular-momentum accretion shocks can power weak-to-moderate X-ray flares from SgrA*
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.04145v1
- **作者**: Samik Mitra, Bożena Czerny, Michal Zajaček, Zach Sumners
- **备注**: 12 pages, 4 figures. Accepted for publication in The Astrophysical Journal
- **摘要**: 来自人马座 A*（Sgr A*）的 X 射线耀斑在持续时间、流亮度和光度上跨越了很宽的范围，但其起源仍无定论。我们测试了低角动量磁化吸积流中的驻波激波（standing shocks）是否能提供一个可行的能量储库来解释这些事件。使用半解析的跨磁声激波解，我们估算了下游激波后流中可用的动能，并将其与 25 年的钱德拉（Chandra）X 射线耀斑目录进行了对比。对于每一个理论解，我们计算了所需的效率 $\epsilon = E_{\text{data}}/E_{\text{sh}}$，其中 $E_{\text{data}}$ 是观测到的每个耀斑的辐射能量，而 $E_{\text{sh}}$ 是激波流中的可用能量。值得注意的是，弱耀斑需要 $\epsilon \sim 10^{-3}$ 到 $10^{-2}$，而中等强度的耀斑需要百分之几。我们对弱自转和高自转的情况都进行了分析，发现得到的弱到中等耀斑能量收支保持不变。对于基准吸积率和玻色修正，驻波激波中的动能储库足以解释观测到的弱到中等耀斑群体，而最强烈的事件可能需要更高的效率，这可以通过额外的磁能释放通道来介导。
- **PDF**: https://arxiv.org/pdf/2609.04145v1

### Absolute Motion of the Infrared Counterpart to Sagittarius A* in the Gaia Celestial Reference Frame 3 and Limits on an Intermediate-mass Black Hole Companion
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.04077v1
- **作者**: Rebecca A. Lewis-Merrill, Tuan Do, Matthew W. Hosek, Gregory David Martinez, Shoko Sakai, Kelly Kosmo O'Neil, Grant Weldon, Abhimat Gautam, Zoë Haggard, Andrea M. Ghez, Jessica R. Lu, Keith Matthews
- **备注**: 22 pages, 10 figures, Accepted to ApJ
- **摘要**: 我们报告了在 Gaia 天球参考系 (Gaia-CRF3) 中，对我们星系中心超大质量黑洞人马座 A* 的红外对应体 (Sgr A*-IR) 的首次自行和加速度测量。该参考系实现了国际天球参考系统 (ICRS)，这是一个由类星体定义的绝对参考坐标系。结合使用 Gaia 和哈勃空间望远镜的数据，将凯克（Keck）自适应光学（AO）观测数据转换到了 Gaia-CRF3 中。我们开发了一种选择参考星的方法，该方法可最大限度地减少天体测量转换误差（统计误差 $= 0.10 - 0.63\text{ mas}$）和坐标系统的漂移（系统误差 $\sim 0.01\text{ mas/yr}$）。我们发现 Sgr A*-IR 在 Gaia-CRF3 中的自行为 $\mu_{\alpha^{*}} = -3.093 \pm 0.085\text{ mas yr}^{-1}$ 和 $\mu_\delta = -5.62 \pm 0.13\text{ mas yr}^{-1}$，其在元期 $t_{0} = 2016.0$ 的初始位置为赤经（R.A.）$= 266.41680848 \pm 0.00000029$ 度，赤纬（DEC）$= -29.00783947 \pm 0.00000050$ 度，这转换后的精度在 R.A. 方向为 $1.05\text{ mas}$，DEC 方向为 $1.79\text{ mas}$。这与 Xu 2022 年对 Sgr A* 无线电对应体的天体测量结果一致。我们还对 Sgr A*-IR 在天球上的加速度给出了 $2\sigma$ 的上限约束，即 $0.061\text{ mas yr}^{-2}$。这一加速度限制排除了在 $\sim 0.01\text{ pc}$ 距离内存在任何质量大于 $4\times 10^{4}\ M_{\odot}$ 的中等质量黑洞伴星，这与先前的研究一致。随着 Gaia Data Release 4 的发布，我们预测这些限制将提高至少两倍。
- **PDF**: https://arxiv.org/pdf/2609.04077v1

### Two sets of potential-density basis pairs for the study of radial perturbations in collisionless spherical stellar systems
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.04012v1
- **作者**: E. V. Polyachenko, I. G. Shukhman
- **备注**: 6 pages, 3 figures. Accepted for publication in MNRAS
- **摘要**: Kalnajs 矩阵方法是研究无碰撞恒星系统全局线性稳定性和可能的朗道阻尼的广泛使用框架。然而，对于具有无限边界的三维球对称模型中的径向微扰（$l=0$），标准的双正交集（例如 Clutton-Brock 基）通常收敛缓慢。这源于一个物理约束：质量守恒的径向模式迫使扰动势在无穷远处比点质量衰减得更快，而单个 Clutton-Brock 元素带有虚假的净质量，并且仅按 $\mathcal{O}(1/r)$ 衰减，从而产生非物理的渐近尾翼。我们构建了两个新的势-密度基对系列，在构建上就消除了这些尾翼。第一个系列修改了 Clutton-Brock 集合：通过相邻元素的特定线性组合在解析上抵消了主导的 $\mathcal{O}(1/r)$ 项，使得势能按 $\mathcal{O}(1/r^3)$ 衰减，密度按 $\mathcal{O}(1/r^5)$ 衰减。这打破了严格的双正交性，但产生了一个紧凑的三对角格拉姆（Gram）矩阵，可以以微不足道的额外计算成本进入响应方程。第二个系列由雅可比多项式构建，在保留严格的对角双正交性的同时，直接在构建中嵌入了所需的 $\mathcal{O}(1/r^2)$ 势能衰减。数值测试表明，这两种展开式在半径上都具有一致的收敛性：当展开势的渐近尾翼与基元素的奇偶性匹配时，截断误差呈指数级下降，否则呈代数级下降。这两种基底都减少了给定精度所需的响应矩阵的维数，适合研究开放恒星系统中的径向微扰。
- **PDF**: https://arxiv.org/pdf/2609.04012v1

### Detection of hydrocarbons in Titan using high-resolution cross-correlation spectroscopy
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.03975v1
- **作者**: Maria Coelho, Rafael Rianço-Silva, Diogo Gonçalves, Pedro Machado, Zita Martins
- **备注**: Accepted for publication in RAS Techniques and Instruments on August 2026
- **摘要**: 高分辨率交叉相关光谱法（HRCCS）是一种探测分子强有力的技术，这些分子的单条谱线可能太弱而无法直接识别，但该技术的灵敏度受到高分辨率不透明度数据可用性和质量的限制。许多在生物和天体生物学上具有重要意义的分子缺乏完整的谱线列表，从而限制了传统的基于模板的搜索。在这项工作中，我们以土卫六（Titan）作为对照测试平台，开发并验证了一种基于截面（cross-section）的高分辨率交叉相关光谱（HRCCS）模板构建新方法。我们分析了土卫六在 K 波段（1.99 - 2.48 $\mu\text{m}$）的 CRIRES+ 观测数据，并分别使用逐线（line-by-line）和基于截面的模板计算了交叉相关函数。我们的分析恢复了已知的碳氢化合物，如甲烷（CH4）和乙炔（C2H2），并首次通过高分辨率交叉相关光谱（HRCCS）探测到了乙烷（C2H6），其信噪比峰值为 $\text{SNR}_{\text{peak}} = 5.17 \pm 0.07$。乙烷的探测完全是通过基于截面的模板实现的，因为目前该分子不存在高分辨率的谱线列表。这些结果表明，基于截面的模板构建对于将 HRCCS 扩展到目前缺乏可靠谱线列表的分子是一种实用且强大的策略，并将土卫六确立为标定分子探测技术的一个基准，该技术可推广应用于太阳系和系外行星大气层。未来将这种方法应用到其他地面高分辨率光谱仪，以及詹姆斯·韦布空间望远镜（JWST）的最高分辨率模式和极大望远镜（ELT）等下一代设施，可显著扩大在行星大气中可探测到的分子名录。
- **PDF**: https://arxiv.org/pdf/2609.03975v1

### Interferometric Survey of Stellar Parameters: Mass of the metallic A-type binary $β$ Aur
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.03886v1
- **作者**: J. Jonák, D. Mourard, J. D. Monnier, S. Hoin, M. Brož, A. Oplištilová, K. A. Kubiak, N. Ebrahimkutty, R. V. Ibañez-Bustos, H. Nowacki, M. Vrard, M. Bailleul, P. Bério, J. Dejonghe, R. Ligi, F. Morand, N. Nardetto, D. Salabert, S. Deheuvels, A. Domiciano de Souza, A. Meilland, K. Perraut, M. Wittkowski, S. Kraus, N. Anugu, M. Gutierrez
- **备注**: 17 pages, 9 figures, accepted for publication in Astronomy & Astrophysics
- **摘要**: 借助新型 CHARA/SPICA 可见光仪器和 CHARA 的多光谱波段运行能力，我们的目标是解析短周期双星的轨道，并开发一个将干涉测量、光谱测量和光度测量观测融合进单一一致模型的健壮框架。对于我们的目标样本，我们根据 CHARA/SPICA 仪器的预期性能，基于亮度、角距离和轨道特性选择合适的双星。作为案例研究，我们分析了明亮的食双星御夫座 $\beta$（$\beta$ Aurigae），它由两颗轻微演化的 A1 型恒星组成。我们将使用 CHARA/SPICA、MIRC-X 和 MYSTIC 获得的 $\beta$ Aur 的全新干涉观测数据与历史 MIRC 数据、径向速度以及光变曲线结合起来。我们首先从干涉测量可观测值中推导出天体测量位置，并计算出轨道解。随后，我们实现了一个统一模型，该模型能够将干涉建模与 ellc 代码相结合，利用马尔可夫链蒙特卡罗（MCMC）抽样同时拟合所有可观测值。我们对每个数据集的噪声统计进行了详细分析，最后采用了轮廓似然法（profile likelihood approach）来处理被低估的噪声和系统误差。我们通过联合建模推导出了 $\beta$ Aur 的一致轨道及物理学解。干涉测量数据的引入极大地约束了半长轴角距离和倾角。利用轮廓似然法处理本质上完全不同的可观测值之间不同水平的内在不确定性，我们得出了两颗恒星的质量，分别为 $M_1 = 2.359 \pm 0.005\ M_{\odot}$ 和 $M_2 = 2.293 \pm 0.004\ M_{\odot}$，它们的半径为 $R_1 = 2.752 \pm 0.002\ R_{\odot}$ 和 $R_2 = 2.622 \pm 0.002\ R_{\odot}$，以及到该双星系统的距离 $d = 24.30 \pm 0.05\text{ pc}$。
- **PDF**: https://arxiv.org/pdf/2609.03886v1

### 学科总结
本期 `astro-ph.*` 领域的论文主要涉及银河系中心黑洞、恒星双星系统物理特性、恒星动力学理论以及行星大气探测。研究包括：通过低角动量吸积激波模型解释人马座 A*（Sgr A*）的 X 射线耀斑机制；在 Gaia 参考系下首次精确测量 Sgr A* 红外对应体的绝对自行，并对可能的中等质量黑洞伴星给出严格限制；构建新型势-密度基对以高效研究无碰撞球状恒星系统的径向微扰；利用高分辨率交叉相关光谱在土卫六（Titan）大气中首次探测到乙烷；以及通过干涉测量联合建模，高精度确定了双星系统 $\beta$ Aur 的质量和半径。

--- 
## 📚 学科: `stat.*`
### Unifying Conformal Language Tasks with In-Context Ensembles
- **分数**: 4
- **链接**  https://arxiv.org/abs/2609.03005v1
- **作者**: Xiao Shi Huang, Chen-Yuan Lin, Bruce Kuwahara, Kin Kwan Leung, Jesse C. Cresswell
- **备注**: Findings of EMNLP 2026. Code is available at https://github.com/layer6ai-labs/conformal-relevance
- **摘要**: 许多自然语言处理（NLP）任务（如摘要生成和抽取式问答）都可以简化为在两个约束条件下从文档中检索相关内容：覆盖率（保留足够的关键信息以实现某种目标）和简明度（尽可能多地去除无关信息）。符合预测（Conformal prediction）方法已被用于确保覆盖率，且必须通过设计评分函数来优化简明度。目前最先进的评分函数采用人工设计的大模型（LLM）提示词，要求模型评估内容的重要性，但人工提示词工程既耗费人力又具有特定任务局限性。我们引入了 Conformal Relevance 框架，它利用上下文学习样本整理和集成方法来创建一个评分函数，在保持覆盖率的同时，以最少的人工输入提高简明度。我们展示了该框架在七个 NLP 任务中的应用，并从理论上研究了集成符合得分多样性的影响，给出了一个表征集成何时能改善最坏情况下句子得分的互补条件，以及集成改进的饱和边界。
- **PDF**: https://arxiv.org/pdf/2609.03005v1

### Comment on: "The Two Cultures of Prevalence Mapping: Small Area Estimation and Model-Based Geostatistics"
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.03805v1
- **作者**: Emanuele Giorgi, Claudio Fronterre, Peter Diggle
- **备注**: To appear on the journal "Statistical Science". Comment on arXiv:2110.09576
- **摘要**: 小区域估计（SAE）和基于模型的地统计学（MBG）为流行率制图提供了互补的方法，它们的相对优势取决于推断目标和可用数据的特征。我们认为，更全面的比较应该考虑模型的可解释性、流行病学相关协变量的作用、区域级预测之外的推断目标、不同空间划分和调查数据的整合以及特定任务的模型验证。特别地，我们质疑，当调查设计变量的作用可以通过可测量的环境和社会经济风险因素介导时，是否应例行地将其纳入 MBG 模型。我们进一步指出，与传统的交叉验证相比，针对流行率制图的实际操作目标定制的基于模拟的验证能够对模型性能提供更有信息量的评估。
- **PDF**: https://arxiv.org/pdf/2609.03805v1

### Spectral characteristics of autoencoder parameters as a vector representation of data
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.03495v1
- **作者**: Maria Nikitina, Anton Bishuk, Oleg Bakhteev
- **备注**: 13 pages, 6 figures. This is a shortened (theorem proofs are skipped) and translated version of the paper published in a Russian-language peer-reviewed journal, the citation is in the paper footnote
- **摘要**: 本文探讨了自编码器模型的参数与它们所训练的数据的统计属性之间的关系。自编码器被定义为具有编码器-解码器架构的模型，训练它们旨在通过压缩的潜在表示重建输入数据。我们提出，模型参数可以被视为相应样本的密集向量表示。为了验证这一假设，我们进行了一项理论和实验研究，其中基于自编码器参数矩阵的谱特征来构建向量表示。理论分析表明，模型参数矩阵的奇异值与训练数据协方差矩阵的特征值有关，从而确保了数据空间和参数空间之间的信息传递。在 CIFAR-10 和 FashionMNIST 数据集上的实验结果证实，所得到的向量表示能够以很高的精确度区分在不同数据子集上训练的模型，而无需借助复杂的向量生成算法或使用原始样本。这些结果表明，训练好的自编码器的参数可以被视为样本的表示形式。
- **PDF**: https://arxiv.org/pdf/2609.03495v1

### Evaluating Graph Neural Networks for Change-Criticality Classification in Maritime Navigation Charts
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.02996v1
- **作者**: Abhishek Potnis, Jacob Arndt
- **备注**: Accepted at IEEE International Geoscience and Remote Sensing Symposium (IGARSS) 2026
- **摘要**: 图神经网络（GNNs）是一类适用于在图结构数据上进行学习的神经网络。它们在空间数据上的应用是一种自然的扩展，然而，目前尚不清楚哪种消息传递操作、架构配置和图表示方法最适合分类电子航海图（ENCs，用于海上航行的地理空间矢量数据集）中对象的变更。维护这些数据集是一项挑战，而根据对象变化对航海安全的重要性进行分类尤为关键。在此，我们建议将这些矢量航海数据集表示为图结构，其中空间对象作为节点，它们的空间和语义关系构成边。我们将旧的 ENC 数据集和新的 ENC 数据集编码为一对图，并将该任务表述为图对（graph-pair）分类问题。基于这种表示，我们研究了使用 GNN 架构来分类编码图是否构成了航海安全的严重或非严重风险。我们在由海事专家审查过的 ENC 变更上训练和评估了若干种 GNN 架构和模型配置。我们的结果表明，基于图的表示方法能够提高 ENC 更新的分类效果，为自动化或改进 ENC 维护工作流程提供了一种可扩展的方法。
- **PDF**: https://arxiv.org/pdf/2609.02996v1

### A simple derivation of the Kalman filter
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.02332v1
- **作者**: Marco Chiani, Giovanni Petris, Moe Z. Win
- **备注**: To be published in IEEE Signal Processing Magazine
- **摘要**: 在本篇讲义中，我们提供了一种简明且自包含的离散时间卡尔曼滤波方程推导，这仅需要对最小二乘估计有基本的了解。推导的设计旨在最大限度地减少数学上的繁琐度，同时保留其严谨性和通用性。
- **PDF**: https://arxiv.org/pdf/2609.02332v1

### 学科总结
本期 `stat.*` 领域的论文涵盖了符合性预测、空间统计、自编码器表征、图神经网络应用及经典算法推导。研究具体包括：基于上下文学习集成的 Conformal Relevance 框架，用于优化 NLP 任务中的符合预测；针对流行率制图中 SAE 和 MBG 两大流派的深度学术评论；探讨自编码器参数的谱特征作为数据集向量表征的理论与实验；利用图神经网络（GNN）对电子海图的变更关键性进行风险分类；以及一份面向信号处理的高校教学材料，提供了卡尔曼滤波器的简明、严谨推导。

--- 
## 📚 学科: `econ.*`
### Robust Variance Estimation in Linear Regression: A Projection-Geometry Perspective
- **分数**: 3
- **链接**  https://arxiv.org/abs/2609.01804v1
- **作者**: Yanping Chen
- **备注**: 79 pages. Accepted at North American Summer Meeting 2026
- **摘要**: 线性回归中的推断通常将普通最小二乘（OLS）残差视为未观测误差的替代。当回归投影相对于误差依赖结构是非局部的时，这种近似可能会失效。残差化随后会在观测值和聚类之间转移协方差信息，而传统的异方差稳健（HC）和聚类稳健方差估计器（CRVE）仅保留对角或聚类内的残差矩，因此可能会低估抽样不确定性。本文开发了一个用于稳健方差估计的投影几何框架。OLS 估计器的方差被精确地表示为潜在协方差块的 Riesz 泛函，而可观测的残差矩通过由完整回归投影确定的线性算子与目标联系起来。这一表述将方差估计简化为一个线性逆问题。我提出了一种结合了聚类内和聚类间残差矩的 Riesz 方差估计器。传统的 HC 和 CRVE 作为受限的近似出现，其有效性取决于微不足道的投影溢出效应。当特定聚类的杠杆矩阵是奇异的时，该估计器仍然定义良好，并通过避免显式矩阵求逆的迭代算法进行计算。模拟表明，在存在投影溢出的情况下，传统方法会出现严重的覆盖不足，而所提估计器则能恢复接近名义水平的覆盖。在关于殖民地总督晋升的实际应用中，该修正改变了所报告的五个系数中四个的显著性。
- **PDF**: https://arxiv.org/pdf/2609.01804v1

### 学科总结
本期 `econ.*` 领域选入了一篇发表于北美计量经济学夏季会议的重量级计量经济学方法论论文。该研究从投影几何的角度出发，指出了传统线性回归中异方差稳健（HC）和聚类稳健方差估计（CRVE）在面对“非局部投影”时容易低估抽样不确定性的理论缺陷。作者提出了一种新型的 Riesz 方差估计器，有效结合了聚类内与聚类间的残差矩，并在模拟及历史应用数据中证实，该估计器能显著修正因常规方法失效而导致的系数显著性偏误。