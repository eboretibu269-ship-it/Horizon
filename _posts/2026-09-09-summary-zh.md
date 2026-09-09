---
layout: default
title: "Horizon Summary: 2026-09-09 (ZH)"
date: 2026-09-09
lang: zh
---

> 从 37 条内容中筛选出 10 条重要资讯。

---

1. [OpenAI 声称在纳维-斯托克斯千禧年难题上取得突破](#item-1) ⭐️ 10.0/10
2. [AlphaGenome Atlas：人类 DNA 单碱基变异影响图谱](#item-2) ⭐️ 9.0/10
3. [Qwen3.8 27B 量化基准测试：4-bit 表现稳定，1-bit 性能崩溃](#item-3) ⭐️ 8.0/10
4. [Copperhead 将 Cursor 式 AI 辅助带入电路板设计](#item-4) ⭐️ 8.0/10
5. [NeurIPS 用有缺陷的 AI 检测器拒稿 178 篇，连主席自己的论文也被误判](#item-5) ⭐️ 8.0/10
6. [马来西亚拟用华为昇腾 910C 芯片建设主权 AI 项目](#item-6) ⭐️ 8.0/10
7. [库克缺席 9 月 9 日发布会视频，新 CEO 特纳斯主推折叠 iPhone](#item-7) ⭐️ 8.0/10
8. [ASML 与台积电合作，推动 High NA EUV 转向 12 英寸光掩模](#item-8) ⭐️ 8.0/10
9. [中国计划到 2030 年将智能算力提升至 9800 EFLOPS](#item-9) ⭐️ 8.0/10
10. [OpenAI 发布 ChatGPT Images 2.5 图像模型，更快更精细](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 声称在纳维-斯托克斯千禧年难题上取得突破](https://www.reddit.com/r/MachineLearning/comments/1wavdi7/openal_says_it_has_cracked_one_of_maths/) ⭐️ 10.0/10

2026 年 9 月，OpenAI 宣布，一个未发布的内部模型生成了对纳维-斯托克斯存在性与光滑性问题这一千禧年大奖难题的解决方案。该结论声称，在光滑外力作用下的三维不可压缩光滑有限能量流动会在有限时间内形成奇点，从而对该问题给出否定答案。 如果得到验证，这将是首个由 AI 生成的千禧年大奖难题证明，可能深刻改变基础数学的研究方式。与此同时，围绕优先权的争议以及 OpenAI 可能在训练中使用人类研究人员私人会话的指控，也引发了关于 AI 伦理和研究署名的紧迫问题。 OpenAI 表示，在一系列智能体运行约 88 小时、消耗约 1300 亿输出 token 后得出了该结论，随后又用 GPT-6 Astra 花费 17 小时在 Lean 中完成形式化验证。纽约大学数学家 Tristan Buckmaster 指控 OpenAI 使用了其与 Levent Alpöge 的私人 Codex 会话；OpenAI 回应称无法排除经去标识化的用户数据对其模型产生帮助的可能性。

reddit · r/MachineLearning · /u/Shizuka_Kuze · 9月8日 17:42

**背景**: 纳维-斯托克斯方程描述粘性流体的运动，但在三维空间中，光滑整体解是否始终存在仍未得到证明。2000 年，克莱数学研究所将其列为七个千禧年大奖难题之一，每题奖金一百万美元；到目前为止，只有庞加莱猜想被正式解决。OpenAI 的这项声明尚未经过克莱研究所或更广泛数学界的验证，据称其方法基于 2023 年 Diego Córdoba 与 Luis Martínez Zoroa 提出的爆破证明技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier-Stokes_existence_and_smoothness_problem">Navier-Stokes existence and smoothness problem</a></li>
<li><a href="https://en.wikipedia.org/wiki/Millennium_Prize_Problems">Millennium Prize Problems</a></li>

</ul>
</details>

**社区讨论**: 社区评论对该事件被指涉及的知识产权窃取行为表达了强烈怀疑和愤怒。一条高赞评论列出了指控时间线，指出 Buckmaster 和 Alpöge 在八月已经就相关问题取得突破，而 OpenAI 是在得知消息后才启动研究。另一条评论引述 Buckmaster 的说法称，当他拒绝 OpenAI 的提议时，对方问他“你为什么要毁掉自己的职业生涯？”。许多评论者认为，OpenAI 无法排除用用户数据训练模型的可能性，这从根本上削弱了其辩解的正当性。

**标签**: `#OpenAI`, `#Mathematics`, `#Navier-Stokes`, `#Millennium Problems`, `#AI Research`

---

<a id="item-2"></a>
## [AlphaGenome Atlas：人类 DNA 单碱基变异影响图谱](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/) ⭐️ 9.0/10

谷歌 DeepMind 发布了 AlphaGenome Atlas，这是一个预测整个人类基因组中 90 亿个可能单核苷酸变异分子效应和 AVI 分数的目录。它被描述为一幅高分辨率图谱，展示单字母 DNA 变化可能如何影响基因组功能。 AlphaGenome Atlas 让全基因组范围内的变异解读向 AlphaFold 在蛋白质科学中的影响力又迈进了一步，因为它不仅针对已在患者中观察到的变异，而是为每一个单碱基 DNA 变化提供效应预测。这有助于临床医生和科学家区分无害变异与致病变异，从而加速罕见病诊断、个性化医疗和功能基因组学研究。 与只对蛋白质编码基因中的变异评分不同，Atlas 提供编码区和非编码区 DNA 中单核苷酸变异的效应预测。它是谷歌 DeepMind AlphaGenome 平台的一部分，可通过公开网页界面查询，且据用户反馈无需任何单位隶属信息即可访问。

hackernews · utiiiD · 9月8日 14:55 · [社区讨论](https://news.ycombinator.com/item?id=49611251)

**背景**: 单核苷酸变异（SNV）是指基因组中某个位置上单个 DNA 碱基的替换；这种变化可能是无害的，也可能增加疾病风险或直接导致疾病。因为许多变异发生在非编码 DNA 中，预测其效应非常困难，而实验室里的饱和突变实验只能覆盖局部区域。变异效应预测器（VEP）是一类计算工具，用来估算基因突变可能产生的功能影响，AlphaGenome Atlas 正是这样一个由深度学习驱动、覆盖全基因组的效应预测目录。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/alphagenome-atlas-a-predictive-map-of-every-possible-dna-letter-change-in-the-human-genome/">AlphaGenome Atlas: Molecular predictions for 9 Billion human DNA ...</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/">Introducing AlphaGenome Atlas - The Keyword</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11098935/">Variant effect predictors: a systematic review and practical guide</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论气氛积极但带有技术上的保留态度。一些评论者质疑 Atlas 是否只是提前计算好的 AlphaGenome API 结果、并未提供新信息，另一些人则询问，尽管声称覆盖非编码 DNA，启动子序列是否真的被纳入。还有人提出实际问题，例如能否用 23andMe 的个人基因组数据查找致病变异；一名评论者则确认，无需任何单位隶属信息即可访问该网络门户。

**标签**: `#genomics`, `#deepmind`, `#ai`, `#health`, `#bioinformatics`

---

<a id="item-3"></a>
## [Qwen3.8 27B 量化基准测试：4-bit 表现稳定，1-bit 性能崩溃](https://quesma.com/blog/qwen38-27b-quantizations-benchmarked/) ⭐️ 8.0/10

对 Qwen3.8 27B 各量化版本的基准测试显示，4-bit 量化保持了模型性能，而 1-bit 量化性能急剧下降。结果还呈现了直至 2-bit 水平的逐级性能变化。 这为开发者在受限 GPU 硬件上运行 Qwen3.8 27B 提供了实用参考，帮助选择能平衡显存、速度与输出质量的量化等级。同时说明，对于这类模型，极限的 1-bit 压缩目前仍不实用。 根据该基准测试，4-bit 版本与全精度模型几乎没有差别，2-bit 版本得分略低，而 1-bit 版本性能崩溃。评论区也指出，KV cache 量化、16GB 以下显存场景以及长上下文表现尚未被测试。

hackernews · stared · 9月8日 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49611128)

**背景**: 量化通过将大语言模型的权重从高精度数值转换为低精度数值来压缩模型，从而降低显存占用并加快推理速度。Qwen3.8-27B 是阿里巴巴 Qwen 团队发布的、采用 Apache-2 许可的紧凑型视觉-语言模型，旨在实现易于部署的多步推理任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/quantization-for-large-language-models">Quantization for Large Language Models (LLMs): Reduce AI Model Sizes Efficiently | DataCamp</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen</a></li>

</ul>
</details>

**社区讨论**: 评论者提出了几个后续问题：有人指出 Wilson 置信区间并不能反映多次运行间的波动，还有人认为 Qwen3.8 27B 更多的“思考”可以部分抵消低量化带来的质量损失。多位用户希望补充 KV cache 量化、16GB 以下显存范围，以及端到端质量衡量（而非只比较 token 预测差异）的基准测试。

**标签**: `#LLM`, `#quantization`, `#Qwen`, `#benchmark`, `#AI`

---

<a id="item-4"></a>
## [Copperhead 将 Cursor 式 AI 辅助带入电路板设计](https://copperhead.sh/) ⭐️ 8.0/10

Copperhead 是一款 AI 驱动的印刷电路板（PCB）设计工具，为硬件工程师带来类似 Cursor 的生成、布局和导出体验。它以 Show HN 形式发布后，在 Hacker News 上迅速获得 198 分和 77 条评论。 这反映了将 AI 编程智能体技术应用于硬件设计的趋势，可能降低 PCB 布局的技能门槛。该工具对电子爱好者、专业硬件工程师以及观望行业变革的传统 EDA 工具厂商都会产生影响。 宣传功能包括一键 Gerber、DXF/STEP、渲染和 BOM 导出，云计划还提到在 KiCad 之外支持 Altium。社区在桌面 Chrome/macOS 上测试时发现创建板卡流程存在无法输入的 bug，也有用户质疑在存在本地导出方案时为何要使用托管版本。

hackernews · animeshchouhan · 9月8日 13:26 · [社区讨论](https://news.ycombinator.com/item?id=49610059)

**背景**: Cursor 是 2022 年推出的 AI 编程智能体与开发环境，允许开发者通过自然语言指令生成和修改代码，并迅速增长至 293 亿美元估值和超过 30 亿美元年度经常性收入。Copperhead 把这一模式应用于印刷电路板（PCB）设计；传统流程依赖 KiCad、Altium 等 EDA 工具，需要手工放置元件和布线。通过将版图设计变成类似对话的任务，Copperhead 这类工具希望让硬件迭代像 Cursor 时代改代码一样快速和易用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>

</ul>
</details>

**社区讨论**: 评论者认为该领域正在升温，提到 Flux.ai、Silixon、Quilter、DeepPCB 和 Astra 等竞争对手，也有人将 Copperhead 与 KiCad 工作流进行比较。同时出现了一些实际顾虑：一名 macOS Chrome 用户报告无法在创建板卡的弹窗中输入文字，另一人询问该工具能否直接交付组装好的板子，还有人质疑在存在本地导出时托管版本的价值。

**标签**: `#PCB design`, `#AI tools`, `#hardware engineering`, `#EDA`, `#KiCad`

---

<a id="item-5"></a>
## [NeurIPS 用有缺陷的 AI 检测器拒稿 178 篇，连主席自己的论文也被误判](https://www.reddit.com/r/MachineLearning/comments/1wakf62/neurips_deskrejected_178_papers_for_being/) ⭐️ 8.0/10

NeurIPS 使用专有 AI 检测器 Pangram 对 Position Paper Track 的投稿进行了桌拒（desk rejection），共拒绝 178 篇论文，占全部投稿的 18.4%，且没有人工评审或申诉程序。独立测试显示，同一检测器将三位轨道主席自己近期的论文标记为 24%到 69%的 AI 生成内容，按照他们自己的执行规则，这些主席本人也会面临被拒风险。 这一争议引发了人们对在学术评审中使用黑箱 AI 检测器的公平性和可靠性的严重担忧，尤其是在没有申诉程序的情况下。它可能会不成比例地伤害非英语母语（ESL）研究者，损害 NeurIPS 等顶级会议的公信力，并为自动化学术诚信执法开创一个令人不安的先例。 据报道，Pangram 的默认设置最初标记了该轨道约 42.7%的论文，近一半投稿被评为 90-100%的 AI 生成内容；组织者只是通过缩小文本窗口才将标记率降至 12.7%。有 22 篇论文因检测得分高于 0.5 而被拒，尽管作者明确否认使用了 AI；帖子中引用的斯坦福研究还发现，61.22%由人类撰写的 TOEFL 作文会被误判为 AI 生成，因为非母语者的正式英语在结构上较为刻板。

reddit · r/MachineLearning · /u/tughanbulut · 9月8日 10:19

**背景**: NeurIPS 是世界上最顶级的机器学习会议之一，而“桌拒”指的是论文在同行评审之前就被组织者直接拒绝。Pangram 这类 AI 检测器并不会验证文档是否与已知的 AI 输出相匹配，而是通过寻找 AI 生成文本与人类写作之间的模式差异，对作者身份进行统计性猜测。这类工具以产生误报而闻名，尤其是在正式、结构化或非母语英语写作中，因此被批评为助长“猎巫”式指控，而非提供可靠的检测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pangram_(AI_detector)">Pangram (AI detector)</a></li>
<li><a href="https://timrequarth.substack.com/p/why-you-shouldnt-trust-ai-detector">The Problem with AI Detector Companies - by Tim Requarth</a></li>

</ul>
</details>

**标签**: `#AI detection`, `#NeurIPS`, `#academic publishing`, `#ethics`, `#machine learning`

---

<a id="item-6"></a>
## [马来西亚拟用华为昇腾 910C 芯片建设主权 AI 项目](https://www.businesstimes.com.sg/international/malaysia-eyes-huawei-chips-ai-project-despite-us-warning) ⭐️ 8.0/10

马来西亚正在评估以华为昇腾 910C 芯片作为 20 亿令吉（约 4.94 亿美元）主权 AI 项目的核心。若项目落地，这将成为外国政府首次正式选择中国 AI 加速器而非美国产品的案例。 这可能是 AI 地缘政治中的一个标志性事件，表明美国出口管制未必能阻止各国政府采用中国 AI 硬件。这也可能鼓励其他美国盟友国家在本国主权 AI 计划中考虑使用中国芯片。 马来西亚将采购多少枚芯片尚未公布。据报道，特朗普政府曾警告使用华为 AI 加速器可能违反美国出口规定，而马方认为相关决定纯属商业性质。根据已披露的规格，昇腾 910C 的 FP16 算力约为 800 TFLOPS、内存带宽约 3.2 TB/s，性能大致与 Nvidia H100 相当。

telegram · zaihuapd · 9月8日 03:35

**背景**: 主权 AI（sovereign AI）指允许一个国家按照自身条件部署 AI 系统所需的产品、技术栈和工具，而不是依赖外部供应商。华为昇腾 910C 是在美国制裁背景下研发的中国国产 AI 加速器，据媒体报道其部分性能指标接近 Nvidia H100。这一背景之所以重要，是因为美国一直试图限制中国的先进芯片能力，而出口管制正是这一竞争中的核心工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huaweicentral.com/huawei-ascend-910c-alleged-specs-suggest-it-a-tough-rival-to-nvidia-h100/">Huawei Ascend 910C alleged specs suggest it a tough rival to ...</a></li>
<li><a href="https://www.redhat.com/en/topics/ai/sovereign-ai">What is sovereign AI?</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#Huawei`, `#geopolitics`, `#export controls`, `#sovereign AI`

---

<a id="item-7"></a>
## [库克缺席 9 月 9 日发布会视频，新 CEO 特纳斯主推折叠 iPhone](https://www.macrumors.com/2026/09/07/tim-cook-wont-appear-apple-sept-9-event-video/) ⭐️ 8.0/10

苹果 9 月 9 日“Surprise and Shine”活动的视频中将不会出现蒂姆·库克，他已于 9 月 1 日卸任 CEO、转任执行董事长。新任 CEO 约翰·特纳斯将主持折叠 iPhone 的发布介绍。 这标志着苹果一场精心安排的领导层交接，让特纳斯在多年来最受瞩目的产品发布会上成为焦点。这一决定表明，苹果希望消费者和投资者把下一阶段的发展——以及折叠屏产品的推进——与新 CEO 联系起来。 据彭博社 Mark Gurman 报道，库克本周三会出席活动的放映会，但不会出现在活动视频本片中。据报道，苹果刻意安排这一交接，让特纳斯成为折叠 iPhone 及后续新品的门面，因为库克若现身反而会削弱这一效果。

telegram · zaihuapd · 9月8日 05:03

**背景**: 发布会视频是苹果精心制作的产品展示，因此选择让谁出现在其中既是实际安排，也是传递信号的决策。库克从 CEO 转任执行董事长是一种常见的继任结构，既能让资深领导者继续参与公司治理，又能让新 CEO 接管日常运营。折叠 iPhone 对苹果而言将是一个重要的新品类，它采用可弯曲屏幕，让手机可以展开成更大的屏幕。

**标签**: `#Apple`, `#CEO transition`, `#foldable iPhone`, `#tech news`

---

<a id="item-8"></a>
## [ASML 与台积电合作，推动 High NA EUV 转向 12 英寸光掩模](https://www.nrc.nl/nieuws/2026/09/08/asml-gaat-samenwerken-met-taiwanese-chipgigant-tsmc-om-zijn-nieuwste-chipmachines-te-upgraden-a4936073) ⭐️ 8.0/10

2026 年 9 月 7 日，ASML 与台积电宣布合作，推动 High NA EUV 光刻从 6 英寸光掩模转向 12 英寸规格。双方计划在 2031 年建成 12 英寸光掩模试产线，并于 2033 年将相关系统用于先进制程大规模量产；台积电拟从 2030 年开始将 High NA 用于先进节点的大规模制造。 这次合作为 High NA EUV 制定了明确的产业路线图，意义重大，因为 12 英寸掩模可提高晶圆厂生产率、降低芯片制造成本，并消除当前限制图形尺寸的拼接约束。这一举措将影响下一代先进芯片制造，并波及更广泛的半导体生态，包括台积电的竞争对手和 ASML 的其他客户。 High NA EUV 仍将首先使用现有的 6 英寸掩模投入生产，向 12 英寸掩模过渡是后续步骤。12 英寸规格要求整个行业开发新的掩模基础设施，包括掩模基板、图形制作设备和量测工具，以支撑计划中的 2031 年试产线及 2030 年代初的量产时间表。

telegram · zaihuapd · 9月8日 06:55

**背景**: High NA EUV 是下一代极紫外光刻技术，利用 13.5nm 波长的光在先进芯片上打印最小特征。更高的数值孔径（NA）能打印更精细的图形，但光刻曝光场受到物理尺寸限制，因此芯片上更大的图形目前需要通过多次曝光“拼接”而成。从 6 英寸切换到 12 英寸光掩模可扩大有效曝光场、减少拼接需求，从而提升生产率并降低成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.asml.com/en/news/press-releases/2026/tsmc-and-asml-announce-industry-transition-to-large-format-photomasks-for-high-na-euv">TSMC and ASML Announce Initiative to Pioneer Industry Transition to Large-Format Photomasks for High NA EUV</a></li>
<li><a href="https://www.asml.com/en/company/stories/2024/5-things-high-na-euv">5 things you should know about High NA EUV lithography - ASML</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#EUV lithography`, `#ASML`, `#TSMC`, `#chip manufacturing`

---

<a id="item-9"></a>
## [中国计划到 2030 年将智能算力提升至 9800 EFLOPS](https://www.scmp.com/tech/policy/article/3366733/china-targets-fourfold-boost-ai-computing-capacity-2030-major-tech-push) ⭐️ 8.0/10

中国工业和信息化部发布未来五年产业规划，提出到 2030 年将智能算力提升至 9800 EFLOPS，并计划在 2026 至 2030 年间累计投入 3.8 万亿元用于信息基础设施建设。规划还要求有序部署万卡级及 10 万卡以上的智能计算集群，并加强基础设施与国产算力芯片的适配。 该政策标志着中国以国家力量大幅扩张 AI 算力基础设施，可能重塑全球硬件供应链，并加剧与美国的科技竞争。如此规模的投资与增长目标表明，AI 算力将成为国家战略重点，对芯片厂商、云服务商和 AI 开发者都将产生深远影响。 截至今年 6 月底，中国智能算力已达 2185 EFLOPS，同比增长 177%，这意味着要实现 2030 年目标，算力规模需在此基础上增长至 4 倍以上。规划还强调部署万卡级与 10 万卡级智能计算集群，并推动基础设施与国产算力芯片的适配，显示供应链自主化的持续推进。

telegram · zaihuapd · 9月8日 11:23

**背景**: EFLOPS（每秒百亿亿次浮点运算）是衡量计算性能的单位，等于每秒 10^18 次浮点运算。美国 Frontier 和 El Capitan 等顶级超级计算机在基准测试中的性能约为 1 EFLOPS，这有助于理解中国 9800 EFLOPS 目标的庞大规模。国家级智能计算计划通常将专用 AI 芯片、大型数据中心集群和软件生态系统相结合，以训练和运行大规模 AI 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/每秒浮點運算次數">每秒浮点运算次数 - 维基百科，自由的百科全书</a></li>
<li><a href="https://blog.csdn.net/qq_16498553/article/details/123491738">什么是EFLOPS？-CSDN博客</a></li>

</ul>
</details>

**标签**: `#China`, `#AI infrastructure`, `#EFLOPS`, `#policy`, `#computing`

---

<a id="item-10"></a>
## [OpenAI 发布 ChatGPT Images 2.5 图像模型，更快更精细](https://openai.com/index/introducing-chatgpt-images-2-5/) ⭐️ 8.0/10

9 月 8 日，OpenAI 发布 ChatGPT Images 2.5 图像模型，细节更清晰、编辑更精准，生成延迟较 GPT-Image-2 最高降低 50%。该模型已向 ChatGPT、ChatGPT Work 和 Codex 全平台用户推出，API 同步上线 GPT-Image-2.5 Flare 和 Sunburst 两款模型。 此次发布显著提升了 AI 图像生成的质量、速度和编辑可靠性，惠及数百万 ChatGPT 用户及创意工作者和普通用户。Flare 与 Sunburst 两款 API 模型的推出，也为开发者提供了高质量生成与精细编辑的灵活选择，进一步巩固了 OpenAI 在多模态 AI 领域的领先地位。 ChatGPT 新增了手绘(Sketch)引导、模板、图片评论和提示词分享等功能。GPT-Image-2.5 Flare 在保持与旗舰版相同质量、编辑和速度改进的同时，延迟降低 50%；GPT-Image-2.5 Sunburst 则为精细创作任务提供更高的精度。

telegram · zaihuapd · 9月8日 18:45

**背景**: ChatGPT Images 是 OpenAI 集成在 ChatGPT 中的文本生成图像系统，用户可通过自然语言创建和编辑图像。前代模型 GPT-Image-2 奠定了图像质量和速度的基准。2.5 版在此基础上降低了延迟并提升了编辑精准度。API 访问使开发者能够将图像生成能力嵌入第三方应用中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-chatgpt-images-2-5/">Introducing ChatGPT Images 2.5 - OpenAI</a></li>
<li><a href="https://x.com/OpenAIDevs/status/2097399255975813387">OpenAI Developers on X: "Meet GPT-Image-2.5 Flare and ...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Image Generation`, `#ChatGPT`, `#AI Model Release`, `#API`

---