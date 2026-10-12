```markdown

同步自EasyReader每周精选模块。
配合“导读+思维导图”功能阅读，效率提升80%。[立即体验EasyReader论文阅读](https://www.easyreader.com.cn/)
# 🗓️ 周报 (2026-W41)
> 更新时间: 2026-10-11

--- 
## 📚 学科: `eess.*`
**学科总结**：本周 `eess.*` 领域共推荐 4 篇论文，涵盖信号处理、无线通信与多模态感知。研究重点包括：1）在顺序蒙特卡洛中引入可微系统重采样（DSR），解决变分滤波中的梯度传导问题（NeurIPS 2026）；2）针对时钟不同步的多面板大规模MIMO提出UNILocMP统一定位框架；3）利用复数神经网络（CVNN）融合视觉与音频的虚部伴随流，推升开放词汇视听事件定位性能（BMVC 2026）；4）提出多专家融合框架CloudEar，用于生成音乐的感知与对齐评估（ISMIR 2026）。

### Differentiable Systematic Resampling for Variational Sequential Monte Carlo
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.12094v1
- **作者**: Fredrik Cumlin, Saikat Chatterjee
- **备注**: Accepted to NeurIPS 2026
- **摘要**: 粒子滤波是用于非线性状态估计的标准工具，但其重采样步骤是离散的，阻碍了变分顺序蒙特卡洛中的梯度学习。我们提出了可微系统重采样（DSR），这是一种基于温度控制的系统重采样松弛方法，在保持系统重采样的CDF排序和带状结构的同时，实现了完整的梯度流。当温度趋近于零时，DSR收敛于精确的系统重采样，并且我们证明了其诱导偏差具有点对点指数收敛速率。与基于最优传输的可微重采样相比，DSR避免了迭代求解器，计算开销显著降低。在随机动力系统和真实手写数据上的实验表明，DSR取得了相当或更优的滤波与动力学学习性能。
- **PDF**: https://arxiv.org/pdf/2610.12094v1

### Localization in Multi-Panel Massive MIMO With Clock Asynchronism: A Unified Approach
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.12178v1
- **作者**: Yuhao Zhang, Guangjin Pan, Musa Furkan Keskin, Carmen D'Andrea, Stefano Buzzi, Henk Wymeersch
- **备注**: Accepted to IEEE Globecom Workshops (GC Wkshps) 2026
- **摘要**: 本文针对时钟不同步条件下的多面板大规模MIMO系统，提出了一种名为UNILocMP的统一定位框架，将基于模型的几何方法与信道图谱（CC）相结合。得益于多面板架构，用户被分为多视距（multi-LoS）用户（与至少两个面板保持LoS链路）和单/非视距用户（仅与一个面板保持LoS或完全没有LoS链路）。针对多视距用户，开发了联合位置与时钟偏差估计方法；针对单/非视距用户，使用两阶段数据增强策略训练无监督CC模型，并引入了时钟偏差感知的不相似度度量。数值验证表明，所提UNILocMP优于基于模型和基于CC的基线，且与全监督指纹识别相比达到了可接受的性能。此外，在固定总天线数的情况下，多面板架构相比单面板基站部署显著提高了定位精度和鲁棒性，特别是在存在时钟不同步的情况下。
- **PDF**: https://arxiv.org/pdf/2610.12178v1

### Open-Vocabulary Audio-Visual Event Localization via Complex-Valued Fusion
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.11846v1
- **作者**: Anirudh Praveen, Koteswar Rao Jerripothula, Pratik Joshi, Aveen Dayal, Neela Sawant
- **备注**: Accepted to British Machine Vision Conference (BMVC) 2026
- **摘要**: 开放词汇视听事件定位（OV-AVEL）旨在为每个视频片段标注事件类别，包括训练期间未见过的类别。主流流程使用冻结的多模态基础模型（如ImageBind）将视觉帧、音频梅尔频谱图和候选类别名称嵌入到共享空间中，然后计算视觉-文本和音频-文本的两组余弦相似度。现有的方法通常在取argmax之前使用固定规则（几何平均、加权平均）将这对相似度折叠为单个标量分数。相比之下，我们计算复数相似度，并使用复数神经网络（CVNN）来学习它们的融合。每个模态的标准表示成为我们流程的实部，而配对的伴随流提供虚部。我们使用视觉模态的iHSV虚部和音频模态的CycleGAN转换相位频谱图作为这些伴随流，从而得到两个复相似度并进行融合。在保持视觉和音频编码器冻结的同时，仅训练时间注意力块和融合CVNN。这种四流复数架构在两个OV-AVEL基准测试上均创下了新的SOTA。在OV-AVEBench的开放（未见类别）划分上，达到了66.5%/59.1%/54.1%的Acc/Seg-F1/Event-F1（相比之前报道的微调基线提高了+1.6/+4.1/+6.6），已知类别也有持续提升。我们还修改了AVE数据集用于此任务，观察到我们的架构达到了60.7%/51.9%/50.4%的Acc/Seg-F1/Event-F1，同样取得了SOTA结果。我们还提出了一种双流替代方案，相比基线也有大幅改进。
- **PDF**: https://arxiv.org/pdf/2610.11846v1

### CloudEar: Integrating Perceptual, Diagnostic, and Cross-Modal Evidence for Music Evaluation
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.11672v1
- **作者**: Qiqi He, Anqi Huang
- **备注**: Accepted at the Late-Breaking/Demo session of ISMIR 2026
- **摘要**: 评估生成的音乐需要对感知质量、技术音频质量和提示词对齐进行建模。现有方法常常忽视信号层面的缺陷，产生压缩的质量分数，并且遗漏了文本提示中细粒度的音乐属性。我们提出了CloudEar，一个用于评估音乐性和提示词对齐的成对评估框架。它包含三个部分：i）用于歌曲质量评估的感知专家；ii）用于学习和信号层面质量分析的诊断专家；iii）基于音乐属性进行提示词-歌曲对齐的跨模态专家。实验表明，CloudEar在成对偏好准确率和分数相关性方面均优于对比基线。
- **PDF**: https://arxiv.org/pdf/2610.11672v1

--- 
## 📚 学科: `q-bio.*`
**学科总结**：本周 `q-bio.*` 领域推荐了 3 篇结合人工智能与生物医学前沿的高质量论文。主要探讨内容包括：1）结合确定性计算与LLM智能体推理的ARGUS框架，消除非编码变异功能解释中的幻觉（NeurIPS 2026 Workshop）；2）利用脑电（EEG）基础模型与隐状态转移图分析脑部疾病个性化模型中预测拟合与隐动力学结构的解耦现象（NeurIPS 2026 Workshop）；3）针对电影-fMRI的ADHD分类提出MovieSTAGE多尺度编码框架，通过场景对齐的功能连接提升分类能力（BIBM 2026）。

### Unlocking the Regulatory Genome by ARGUS: An Evidence-Constrained Agentic Framework for Interpreting Single Nucleotide Variants
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.12281v1
- **作者**: Pratik Dutta, Matthew B. Obusan, Max Chao, Rekha Sathian, Nimisha Papineni, Ramana V. Davuluri
- **备注**: Accepted at the NeurIPS 2026 Workshop on Agentic AI for Biological Discovery (AgenticLS). Code: https://github.com/duttaprat/ARGUS
- **摘要**: 基因组关联研究（GWAS）中超过90%的疾病相关变异位于非编码调控区，但其功能解释仍是基因组医学中的核心开放难题。大语言模型在解释此类变异时经常出现幻觉，伪造实验支持，并将统计上微不足道的信号赋予生物学意义。我们提出了ARGUS（面向不确定性感知科学家的智能体调控基因组学），严格将确定性生物计算与LLM介导的推理分离开来。ARGUS将458个基于DNABERT的转录因子（TF）结合模型封装在一个假设导向的调查循环中，规划器根据当前的不确定性选择证据源，验证器确定性地解释每个观察结果，中间结果会改变调查路径。在8q24癌症风险位点的变异rs6983267上，同一个规划器针对四个TF生成了四条不同的轨迹（FOXA1在3步内被救回；KLF6、RAD21和SP1进行不同路径的处理或弃权）。所有观察均来自真实的ADASTRA、JASPAR和ENCODE cCRE查询，无任何模拟。固定优先级与LLM介导规划的对比表明，LLM规划器通过拒绝无法解决当前待测主张的证据，用更少的工具调用达到了相同的结论。
- **PDF**: https://arxiv.org/pdf/2610.12281v1

### Similar Predictive Fit but Different Latent Dynamics: Characterizing Learned Dynamical Structure in Personalized Models of Brain Disorders
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.10850v1
- **作者**: Rita Huan-Ting Peng, Nhat Bui
- **备注**: Accepted at the World Models for High-Stakes Health (WMHS) Workshop at NeurIPS 2026
- **摘要**: 随着AI模型走向临床决策和个性化治疗，理解模型“学到了什么”比仅关注预测准确率更为重要。我们探究了个性化隐动力学是否能在预测拟合度相似的情况下揭示与临床相关的差异。一个在Temple大学脑电图语料库（TUEG）上预训练的轻量级CNN-Transformer EEG基础模型提取片段级表示。利用Temple大学癫痫语料库（TUEP），将表示映射到共享的隐状态空间，并为每个受试者独立拟合稀疏多项式逻辑转移分布（mLTD），以获得个性化的转移依赖图 $W_n$（包含198名受试者，99名癫痫/99名非癫痫）。在 $k=4$ 和 $k=6$ 时，癫痫受试者展现出明显更密集的学习依赖结构（$p=1.1\times 10^{-7}$）。来自图特征的指标在5折受试者级交叉验证下提供了中等的组间区分度（AUROC 0.68）。相比之下，组间的留一对数似然和下一状态预测几乎相同。因此，相似的预测拟合度并不意味着相似的学习动力学：各组受试者在预测性上可以相当，但个性化模型学到的内部动力学结构却存在显著差异。这一发现提示在个性化临床模型评估中应将学习到的结构与预测性能一并考量。
- **PDF**: https://arxiv.org/pdf/2610.10850v1

### MovieSTAGE: Scene, Transition, and Global Encoding for Movie-fMRI ADHD Classification
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.09306v1
- **作者**: Boseong Kim, Haejun Chung, Ikbeom Jang
- **备注**: Accepted to the 2026 IEEE International Conference on Bioinformatics and Biomedicine (BIBM 2026)
- **摘要**: 自然主义电影-fMRI为大脑动力学提供了共享的、时间上有结构的探针，但现有预测模型通常依赖于全长运行的功能连接（FC）或与叙事事件不对齐的通用时间表示。我们引入了MovieSTAGE（场景、过渡和全局编码），这是一个多尺度框架，结合了场景内超图结构化的FC特征组织、相邻场景间无符号的FC特征差异以及全电影FC。我们在来自CMI-HBN《小黄人》数据集的260名参与者上评估了病例-对照、ADHD亚型和三分类任务。MovieSTAGE分别实现了0.69、0.73和0.75的AUROC，以及67.6%、69.8%和58.3%的平衡准确率，在评估的方法中取得了最高的平均点估计。在三分类任务中，完整模型优于所有双分支变体，HGNN场景编码器在相同设定下优于MLP、GAT和BNT替代方案，且人工标注的分割优于时长匹配的随机和固定数量GSBS对照。这些受控实验结果支持了在结合全电影FC时事件对齐的场景和过渡表示带来的增量预测价值。事后模型衍生分析生成了涉及额顶叶和默认模式系统的网络级假设。
- **PDF**: https://arxiv.org/pdf/2610.09306v1

--- 
## 📚 学科: `cs.*`
**学科总结**：本周 `cs.*` 领域选录 5 篇高质量成果，涵盖多智能体系统、计算机视觉、具身智能与网络安全：1）提出具备显式二阶“心智模型”的多智能体决策框架（NeurIPS 2026）；2）FreeMatching打破传统时空先验，实现跨图像编辑与生成的高泛化密集对应匹配（NeurIPS 2026）；3）OmniCapBench诊断框架，精细化评估多模态大模型的视听字幕能力（NeurIPS 2026）；4）VersaCamVLA实现相机配置可变条件下的机器人操控策略泛化（NeurIPS 2026）；5）ORCAGen利用RAG与生成式AI编排防御恶意软件的上下文感知欺骗机制。

### Mental-Models for Multi-Agent Systems
- **分数**: 7
- **链接**: https://arxiv.org/abs/2610.12453v1
- **作者**: Hanan Gani, Lulu Shao, Manmohan Chandraker
- **备注**: Accepted at NeurIPS 2026
- **摘要**: 大基础模型加速了向通用智能体的发展，这些智能体通过语言和多模态信号与人类及其他智能体进行交互。然而，稳健的多智能体决策需要在部分可观测性下对其他智能体的已知信息、意图和可能采取的行动进行推理。现有的智能体系统通常通过提示设计、记忆或端到端行为塑造来运行，但通常不会学习可作为跨任务决策变量复用的显式伙伴状态表示。我们引入了“心智模型赋能的智能体”框架，为智能体装备其对手的隐心智模型，允许其从历史观察中推断隐藏的信念、意图和可能的反应，并利用这些推断指导动作选择。我们的方法联合学习摊销的递归心智理论（Theory-of-Mind）表示（包含一阶和二阶心智状态结构）以及一个基于信念条件的奖励模型，该奖励模型根据推断出的伙伴状态评估候选动作。随后在该信念感知信号下学习策略，使智能体在推理阶段能够独立行动，同时保留显式伙伴建模的优势。我们在纯语言和多模态基准上评估了同一框架。在这些设置中，显式心智状态建模显著提高了交互质量和Theory-of-Mind性能。
- **PDF**: https://arxiv.org/pdf/2610.12453v1

### Beyond Spatio-Temporal Priors: A Generalizable Approach for Dense Correspondence Matching
- **分数**: 7
- **链接**: https://arxiv.org/abs/2610.12421v1
- **作者**: Luping Liu, Bingyi Kang, Yifan Wang, Dong Xu
- **备注**: Accepted at NeurIPS 2026. 24 pages, 7 figures, including appendices
- **摘要**: 密集对应匹配（Dense correspondence matching）历史上一直受到平滑运动和刚体几何等简化时空先验的束缚。虽然这些假设对传统任务有效，但在图像编辑与参考引导生成（IEG）中会失效，因为在这些场景中，变换可以在保留视觉身份的同时破坏物理连续性。为了跨此类变换建立保持身份的对应关系，我们提出了FreeMatching，这是一个通用框架，结合了生成式与语义基础表示，并融合了来自传统数据集、追踪视频和合成场景的异构监督。教师引导的迭代精炼进一步改善了IEG中无需密集对应标注的匹配质量。实验表明，单模型FreeMatching极大地提升了具挑战性的IEG图像对上的匹配质量，同时在传统基准上保持了有竞争力的性能。此外，我们证明了其作为评估身份保留定量指标的实用性，其得分与人类判断高度相关。
- **PDF**: https://arxiv.org/pdf/2610.12421v1

### OmniCapBench: A Deep-Structured Evaluation Framework for Fine-Grained Audio-Visual Captioning
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.12458v1
- **作者**: Zhongyu Yang, Jiale Tao, Ruitao Chen, Zuhao Yang, Yingfang Yuan, Xueliang Zhao, Auden, Kai Wang, Shuai Shao, Biao Wang, Steve Yves, Qinglin Lu
- **备注**: Accepted by NeurIPS 2026. Code and benchmark can be found at https://01yzzyu.github.io/OmniCapBench/
- **摘要**: 多模态大语言模型（MLLM）正快速向连续视听推理演进，迫切需要能够暴露其能力极限的评估方法。视听生成字幕（Audio-visual captioning）是一个理想的诊断任务，但目前的基准面临着权衡：整体字幕打分覆盖面广但缺乏定位，局部探针有定位但缺乏覆盖，且无约束的LLM裁判会引入不稳定性。我们推出了OmniCapBench，将视听字幕评估重构为一个深层结构的诊断框架。OmniCapBench将预测目标从自由文本转变为跨实体引用、视觉镜头和音频事件三个轨道的原子化、可验证评估单元集合，通过确定性约束检查和局部基于LLM的语义比较实现可靠打分。OmniCapBench包含786个密集标注的视频，能有效区分MLLM的感知错误（包括时间定位失败、身份漂移、跨模态错位和幻觉描述）。对前沿MLLM的评估揭示了其强大的局部感知能力但在长时程视听推理上的短板（特别是在身份漂移和跨模态错位方面）。
- **PDF**: https://arxiv.org/pdf/2610.12458v1

### VersaCamVLA: Camera-Configurable VLA Policies for Robotic Manipulation
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.12451v1
- **作者**: Boyao Han, Chen Shi, Jingjing Qian, ZhuoTan Tian, Li Jiang
- **备注**: Accepted at NeurIPS 2026. Project page: https://boyaohan.github.io/VersaCamVLA.github.io/
- **摘要**: 视觉-语言-动作（VLA）模型已成为机器人操控的强大基础，但它们在训练期间对固定相机配置的依赖导致其在部署时对相机数量或位姿的变化非常脆弱。为克服这些限制，我们提出了VersaCamVLA，一个相机可配置的框架，将相机集合表示与动作学习解耦。VersaCamVLA学习了一个统一的场景Token接口，将任意、可变数量带位姿的RGB视图映射为固定大小的隐式场景Token。这通过多信号目标视图预测和利用手腕相机自然运动带来免费位姿多样性的手腕增强位姿采样（WAPS）来实现。在部署时，轻量级空间编码器将这些紧凑的场景Token作为补充视觉条件注入预训练的基座VLA，无需显式3D感知或新视图渲染。在RoboTwin、LIBERO及真实机器人平台上的实验表明，VersaCamVLA持续优于以往的VLA方法和直接多视图基线，在不同相机数量和未见过的相机位姿下均保持鲁棒性能。
- **PDF**: https://arxiv.org/pdf/2610.12451v1

### ORCAGen: Orchestrating Context-Aware Malware Deception with RAG-Guided Generative AI
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.12415v1
- **作者**: Shihab Ahmed, Md Sajidul Islam Sajid, Teryl Taylor, Frederico Araujo, Tariqul Islam
- **备注**: Accepted at 2026 IEEE 8th International Conference on Trust, Privacy and Security in Intelligent Systems, and Applications (TPS-ISA)
- **摘要**: 恶意软件防御通常尽可能快地移除或隔离可疑程序。虽然对遏制威胁有效，但这可能浪费观察攻击者行为和部署针对性反制措施的机会。ORCAGen采取了不同的方法：利用生成式AI离线构建恶意软件特定的欺骗剧本，在部署前进行验证，并在运行时仅执行经过验证的逻辑。ORCAGen结合检索增强生成（RAG）与结构化提示工程，以生成概念验证（PoC）恶意软件及相应的欺骗编排代码。由恶意软件规程和主动防御策略组成的精选知识库（KB）奠定了生成过程的基础，帮助LLM生成特定威胁且可执行的欺骗逻辑，而非通用或幻觉输出。生成的PoC恶意软件提供了一种安全且可复现的方式，用于在欺骗策略加入运行时剧本前测试其能否干扰、重定向或抑制目标恶意软件行为。我们在包含键盘记录器、信息盗取程序和勒索软件的合成及150个真实恶意软件样本上评估了ORCAGen，涵盖GPT-4o、GPT-5.5、Gemini 3.5 Flash等模型。结果表明RAG引导的结构化提示能支持可扩展、轻量且确定性的恶意软件欺骗剧本构建。
- **PDF**: https://arxiv.org/pdf/2610.12415v1

--- 
## 📚 学科: `math.*`
_本周缺少高价值论文_

---
## 📚 学科: `astro-ph.*`
**学科总结**：本周 `astro-ph.*` 领域选录 5 篇前沿天文学研究成果：1）在Parkes归档巡天数据中新发现6颗隐藏的脉冲星（包括大麦哲伦星系中最慢的脉冲星）（ApJ Letters）；2）利用TEXES长达20年的光谱数据绘制木卫一日面赤道 $SO_2$ 大气密度的完整经度分布（PSJ）；3）开发Rust语言实现的行星能量平衡模型Gen-EBM，揭示失控温室效应下的气候多稳定性（A&A）；4）MeerKAT首次在宇宙学尺度上实现中性氢21厘米自功率谱的直接强度映射测量（MNRAS）；5）利用Gaia DR3对巨型星团Westerlund 1进行二维运动学分析，首次揭示其沿银纬方向的各向异性膨胀与剪切（A&A）。

### Discovery of Hidden Extragalactic Pulsars in the Parkes Archival Data
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.12450v1
- **作者**: Rahul Sengar, Laila Vleeschower, Matthew Bailes, Fronefield Crawford, Duncan R. Lorimer, Joshua P. Ridley
- **备注**: Accepted for publication in ApJ Letters
- **摘要**: 已知无线电脉冲星群体中仅有略高于1%位于大麦哲伦星系和小麦哲伦星系（MC）。通过在高谐波折叠下折叠接近噪声水平的候选信号，我们重新处理了原始Parkes多波束MC巡天数据并发现了6颗脉冲星。其中5颗位于大麦哲伦星系（LMC），包括一颗自转周期为3.8秒的脉冲星（MC中已知最慢的脉冲星）；剩余1颗位于小麦哲伦星系方向，与银河系前景相关。新发现脉冲星中有4颗展现出闪烁现象，1颗具有明显的调零（nulling）行为。这些发现使LMC中已知的无线电脉冲星总数增加到49颗。光度函数和占空比分析表明它们与银河系规范脉冲星一致。种群合成模拟表明，基于其母体种群上限，更深度的巡天将在MC中揭示更多脉冲星（包括多达数颗毫秒脉冲星）。重新分析归档数据对提高巡天完整性和发现科学价值天体至关重要。
- **PDF**: https://arxiv.org/pdf/2610.12450v1

### Longitudinal distribution of Io's dayside atmospheric density
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.12275v1
- **作者**: R. S. Giles, J. R. Spencer, T. K. Greathouse, C. C. C. Tsang, E. Lellouch, M. A. López-Valverde
- **备注**: Accepted for publication in The Planetary Science Journal (PSJ). 16 pages, 6 figures, and 1 table
- **摘要**: 自2001年以来，我们利用NASA红外望远镜设施的TEXES高分辨率中红外光谱仪研究木卫一（Io）以 $SO_2$ 为主的大气密度。191次独立观测覆盖了530 cm$^{-1}$ 附近的多个 $SO_2$ 吸收线以及木卫一中心经度的全范围，使我们能深入研究其日面大气的经度变化。通过改进经度变化建模并采用季节模型对反演的 $SO_2$ 密度进行时间归一化，我们重建了代表近日点和远日点的木卫一赤道 $SO_2$ 柱丰度的两个完整经度分布。两者均显示出先前研究观察到的半球不对称性，最高密度出现在200W附近，最低密度出现在305W附近。远日点最大与最小密度对比约为27倍，近日点约为16倍。两种经度分布均不对称，木卫一后随半球的下降比主导半球更陡峭。与火山活动、冰不均匀性或蚀（eclipse）效应驱动的预期分布进行对比后，我们得出结论：蚀效应很重要但不足以完全解释经度变化形状，霜冻（frost）分布也可能非常关键。
- **PDF**: https://arxiv.org/pdf/2610.12275v1

### Gen-EBM: an energy balance model for terrestrial planets. Climate multistability from snowball to post-runaway greenhouse climates
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.12267v1
- **作者**: Siddharth Bhatnagar, Emeline Bolmont, Maura Brunetti, Jérôme Kasparian, Tim Kallioinen, Marine Leyvraz, Guillaume Chaverot, Yonatan Birhanu Haile, Dóra Takács
- **备注**: 18 pages, 14 figures. Accepted for publication in A&A
- **摘要**: 气候多稳定性与临界点是类地行星气候的关键属性。我们推出了日内瓦能量平衡模型（Gen-EBM），这是一个新的1维纬度EBM，用于快速探索类地行星气候，并研究行星自转、轨道偏心率和热惯性如何塑造气候吸引子和多稳定性。Gen-EBM采用Rust语言实现，合并了涵盖类地、失控温室萌发期和失控温室后期的温度相关出射长波辐射方案。我们通过模拟集合构建分叉图。引入失控温室后期状态大幅扩大了多种气候状态共存的参数空间。慢自转行星接近空间均匀极限并保持更宽的温和稳定性范围，而快自转行星产生强赤道-极地温度梯度从而收窄温和分支。在平均通量近似下，偏心率增加会增强气候变率并改变吸引子结构。温和气候消失的临界偏心率强烈依赖于热惯性，富含海洋的行星比陆地主导的行星在更大偏心率下仍能保持稳定。Gen-EBM计算效率高且具灵活性，构成了简单气候模型与3维通用循环模型（GCM）之间的重要桥梁。
- **PDF**: https://arxiv.org/pdf/2610.12267v1

### HI intensity mapping with MeerKAT: A measurement of the 21-cm auto-spectrum on cosmological scales
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.12158v1
- **作者**: MeerKLASS Collaboration, Matilde Barberi-Squarotti, José L. Bernal, Philip Bull, Stefano Camera, Isabella P. Carucci, Zhaoting Chen, Steven Cunnington, Brandon N. Engelbrecht, José Fonseca, Keith Grainge, Wenkai Hu, Melis O. Irfan, Yichao Li, Mário G. Santos, Marta Spinelli, Jingying Wang, Amadeus Witzemann, Laura Wolz
- **备注**: 34 pages, 32 figures. Accepted for publication by MNRAS on 01/10/2026
- **摘要**: 我们报道了在红移 $z = 0.42$ 处，通过强度映射技术在宇宙学尺度 $0.095\,h\,{\rm Mpc}^{-1}<k<0.245\,h\,{\rm Mpc}^{-1}$ 上对中性氢（HI）21厘米信号功率谱的直接测量。分析了 MeerKLASS 2021年观测期间在 $971.2\,{\rm MHz}<ν<1023.6\,{\rm MHz}$ 频率范围内获取的约 $236\,{\rm deg}^2$ 天区的强度图。我们将数据集划分为多个观测独立的子集，在独立执行盲污染分离后，利用内部互相关抑制仪器噪声平台并从残留系统误差中孤立出宇宙学信号。引入多子集形式学推断HI自功率谱振幅，达到了信噪比为6.2的探测。测量得出 $10^3\,Ω_{\rm HI} b_{\rm HI}=1.271^{+1.080}_{-0.598}$。这一直接测量是证明HI强度映射技术对SKAO未来巡天有效性的里程碑。
- **PDF**: https://arxiv.org/pdf/2610.12158v1

### EWOCS-XI: Anisotropic expansion and shear in the cluster Westerlund 1. A 2D kinematic analysis with Gaia DR3
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.12117v1
- **作者**: L. Prisinzano, F. Damiani, C. Ordenes-Huanca, M. Tarantino, S. Sciortino, N. J. Wright, V. Almendros-Abad, M. Andersen, A. Bayo, R. Bonito, V. Cusimano, M. Haberle, K. Mužic, I. Negueruela, E. Sabbi, A. Winter, M. G. Guarcello
- **备注**: 19 pages, 13 figures, Accepted for publication in A&A
- **摘要**: Westerlund 1 (Wd1) 是银河系中最质量巨大的年轻星团之一。利用 Gaia DR3 数据与5D聚类方法，我们确认了559个真实成员星。对524颗高精度自行恒星建模，导出了速度梯度张量，映射了膨胀、旋转与剪切。二维运动学分析揭示了显著的各向异性膨胀，优先沿银纬方向（位置角 $164^\circ\pm10.1^\circ$），并在天空平面上探测到了清晰的剪切特征。Wd1并非单一凝聚的群体，而是包含两个解耦的子系统：一个处于动力学平衡的结合核心，和一个正在逃逸的非结合包层。这种垂直于银道的各向异性膨胀运动学时间尺度（$2.08 \pm 0.44$ Myr）与星团轨道穿越银道面的时间（$2.10 \pm 0.05$ Myr）高度契合，表明膨胀的开启与穿越银道面重合，由内部动力学（如早期超新星反馈）或外部潮汐扰动触发。活跃的星团解体正在进行中，主导机制是离散的动力学抛射事件而非长期恒星蒸发。
- **PDF**: https://arxiv.org/pdf/2610.12117v1

--- 
## 📚 学科: `stat.*`
**学科总结**：本周 `stat.*` 领域选录 2 篇统计学与机器学习交叉成果：1）提出可微系统重采样（DSR）方法，解决了变分顺序蒙特卡洛中连续梯度流与低计算开销兼得的问题（NeurIPS 2026）；2）提出提示词级别的 e-过程 统计监控框架，实现大语言模型权重窃取行为的随时有效（anytime-valid）检测（NeurIPS 2026 Workshop）。

### Differentiable Systematic Resampling for Variational Sequential Monte Carlo
- **分数**: 6
- **链接**: https://arxiv.org/abs/2610.12094v1
- **作者**: Fredrik Cumlin, Saikat Chatterjee
- **备注**: Accepted to NeurIPS 2026
- **摘要**: 粒子滤波是用于非线性状态估计的标准工具，但其重采样步骤是离散的，阻碍了变分顺序蒙特卡洛中的梯度学习。我们提出了可微系统重采样（DSR），这是一种基于温度控制的系统重采样松弛方法，在保持系统重采样的CDF排序和带状结构的同时，实现了完整的梯度流。当温度趋近于零时，DSR收敛于精确的系统重采样，并且我们证明了其诱导偏差具有点对点指数收敛速率。与基于最优传输的可微重采样相比，DSR避免了迭代求解器，计算开销显著降低。在随机动力系统和真实手写数据上的实验表明，DSR取得了相当或更优的滤波与动力学学习性能。
- **PDF**: https://arxiv.org/pdf/2610.12094v1

### Anytime-valid detection of LLM weight exfiltration
- **分数**: 3
- **链接**: https://arxiv.org/abs/2610.11843v1
- **作者**: Ines Ortega-Fernandez, Mateusz Kowalczyk, Keri Warr
- **备注**: Accepted for oral presentation at the NeurIPS 2026 workshop E-Values: From Statistics to ML (Paris, December 13 2026)
- **摘要**: 受损的大语言模型推理服务器可以通过将有效载荷比特编码在看似合理的Token选择中来泄露模型权重。在受信服务器中重放相同的提示词可以暴露此类偏差，但正常的数值非确定性也会导致Token不匹配。我们引入了一种提示词层面的e-过程（e-process），它在受信良性流量上校准整篇响应的不匹配事件，并在无限监控时间线内顺序累积证据，同时在校准转移假设下控制任意假阳性的概率。与硬性单Token报警相比，e-过程跨响应融合弱证据，同时提供显式的随时有效（anytime-valid）假报警控制。
- **PDF**: https://arxiv.org/pdf/2610.11843v1

--- 
## 📚 学科: `econ.*`
_本周缺少高价值论文_
```