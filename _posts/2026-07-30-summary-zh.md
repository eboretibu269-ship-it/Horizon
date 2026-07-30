---
layout: default
title: "Horizon Summary: 2026-07-30 (ZH)"
date: 2026-07-30
lang: zh
---

> 从 37 条内容中筛选出 14 条重要资讯。

---

1. [GitHub 推出堆叠拉取请求公开预览](#item-1) ⭐️ 9.0/10
2. [Anthropic 的 AI 在 60 小时内破解 NIST 后量子候选算法 HAWK](#item-2) ⭐️ 9.0/10
3. [廉价流媒体棒预装恶意软件用于广告欺诈](#item-3) ⭐️ 8.0/10
4. [Gemini Robotics 2 实现机器人全身控制](#item-4) ⭐️ 8.0/10
5. [OpenAI 发布 GPT-5.6 Luna，价格大降 80%](#item-5) ⭐️ 8.0/10
6. [Google 通过 Age Signals API 在全球扩大安卓年龄验证](#item-6) ⭐️ 8.0/10
7. [重构的经济效益量化分析](#item-7) ⭐️ 8.0/10
8. [GCC 指导委员会通过拒绝 AI 生成贡献的政策](#item-8) ⭐️ 8.0/10
9. [教授因会议评审缺陷失去博士生候选人](#item-9) ⭐️ 8.0/10
10. [MLVC：面向真实部署的多平台学习视频编解码器](#item-10) ⭐️ 8.0/10
11. [Kimi K3 以创新技术实现前沿开源权重性能](#item-11) ⭐️ 8.0/10
12. [字节最大 To B 重组：飞书并入豆包和火山引擎](#item-12) ⭐️ 8.0/10
13. [谷歌 DeepMind 解散 AlphaFold 团队，核心成员转投 Anthropic](#item-13) ⭐️ 8.0/10
14. [欧盟启动 AI 超级工厂招标 拟撬动 300 亿欧元](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GitHub 推出堆叠拉取请求公开预览](https://github.blog/changelog/2026-07-30-stacked-pull-requests-are-now-in-public-preview/) ⭐️ 9.0/10

GitHub 现已对所有仓库开放堆叠拉取请求的公开预览，允许开发者将相互依赖的 PR 以有序堆栈的形式进行管理。 此功能通过允许对堆叠的变更进行增量式、独立的审查，显著改善了代码审查工作流，有助于提高代码质量和加快迭代速度。 堆叠 PR 需要使用特定的 CLI 工具（gh-stack），合并队列支持将在未来几周内逐步推出。已知问题包括使用压缩合并时批量合并功能失效，需要重新批准。

hackernews · tomzorz · 7月30日 16:26 · [社区讨论](https://news.ycombinator.com/item?id=49112232)

**背景**: 堆叠拉取请求是一种开发工作流，将大型功能拆分为多个相互依赖的小变更，每个变更独立审查但按顺序合并。这与传统的单个大型 PR 不同，可以减少合并冲突并加快审查周期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-07-30-stacked-pull-requests-are-now-in-public-preview/">Stacked pull requests are now in public preview - GitHub ...</a></li>

</ul>
</details>

**社区讨论**: 社区总体持积极态度，Steve Klabnik 称这是 GitHub 多年来最大的变化之一。但一些用户报告了合并和压缩合并工作流中的错误，并且关于其相比逐提交审查的优势仍存在疑问。

**标签**: `#github`, `#pull requests`, `#developer tools`, `#workflow`

---

<a id="item-2"></a>
## [Anthropic 的 AI 在 60 小时内破解 NIST 后量子候选算法 HAWK](https://startupfortune.com/claude-mythos-broke-hawk-and-the-nist-post-quantum-timeline-may-not-survive-it/) ⭐️ 9.0/10

Anthropic 宣布，其 Claude Mythos Preview AI 发现了 NIST 后量子候选算法 HAWK 的一个严重弱点，在 60 小时内将其安全裕度降低，花费了 10 万美元的 API 费用。这一发现此前两年来一直未被人类专家发现。 这展示了 AI 在识别密码学漏洞方面比人类密码分析员更快的日益增强的能力，可能加速后量子标准化进程。同时，它也凸显了密码敏捷性的迫切需要，以及应依赖现有标准而非等待完美算法。 该攻击将 HAWK-256 的有效密钥强度从 2^64 降至 2^38，但并不在多项式时间内运行，因此更大密钥仍然安全。此外，研究还包括对七轮 AES-128 的改进攻击，但完整的 10 轮 AES-128 仍未受影响。

telegram · zaihuapd · 7月30日 05:47

**背景**: HAWK 是一种基于格的数字签名方案，目前处于 NIST 后量子密码标准化过程的第三轮。Claude Mythos Preview 是 Anthropic 开发的强大 AI 模型，专为复杂的网络安全任务设计。这一发现突显了高级 AI 在防御和攻击场景中的双重用途性质。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.csoonline.com/article/4202920/mythos-takes-its-first-shot-at-post-quantum-cryptography.html">Anthropic finds weakness in Hawk post-quantum digital signature algorithm | CSO Online</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos</a></li>
<li><a href="https://www.techtimes.com/articles/322174/20260730/south-korea-certifies-hybrid-post-quantum-encryption-module-ai-breaks-hawk-algorithm-60-hours.htm">South Korea Certifies Hybrid Post-Quantum Encryption Module as AI Breaks HAWK Algorithm in 60 Hours</a></li>

</ul>
</details>

**标签**: `#AI`, `#cryptography`, `#post-quantum`, `#NIST`, `#security`

---

<a id="item-3"></a>
## [廉价流媒体棒预装恶意软件用于广告欺诈](https://krebsonsecurity.com/2026/07/read-this-before-you-buy-that-tv-streaming-stick/) ⭐️ 8.0/10

KrebsOnSecurity 报告称，许多由大型零售商销售的廉价电视流媒体棒预装了恶意软件，这些恶意软件会将设备变成住宅代理并实施广告欺诈，带来严重的安全和隐私风险。 这暴露了消费物联网设备中的普遍漏洞，可能危及数百万用户的隐私并欺诈在线广告商。它突显了大型电子商务平台对所售产品缺乏问责制。 据报道，该恶意软件用于住宅代理方案，通过设备的 IP 地址路由网络流量以冒充真实用户连接，以及广告欺诈，生成虚假点击和曝光以窃取收入。这些设备通常运行过时的 Android 版本，没有安全更新。

hackernews · speckx · 7月30日 17:04 · [社区讨论](https://news.ycombinator.com/item?id=49112744)

**背景**: 住宅代理是使用真实 ISP 分配的 IP 地址来隐藏网络流量来源的中介服务器，使其难以被检测。广告欺诈涉及创建欺诈性的在线广告互动以产生收入。廉价流媒体棒通常运行修改版的 Android 操作系统，安全实践较差，容易成为恶意软件注入的目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Residential_proxy">Residential proxy</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ad_fraud">Ad fraud</a></li>
<li><a href="https://www.cloudflare.com/learning/bots/what-is-ad-fraud/">What Is Ad Fraud? | Ad Click Fraud</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了对零售商责任的担忧，许多人认为亚马逊、百思买等应被迫为销售这些有害设备负责。用户分享了类似产品的个人经历，一些人指出即使没有故意植入恶意软件，缺乏技术维护也使这些设备容易受到攻击。

**标签**: `#security`, `#privacy`, `#IoT`, `#consumer electronics`, `#streaming devices`

---

<a id="item-4"></a>
## [Gemini Robotics 2 实现机器人全身控制](https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/) ⭐️ 8.0/10

这一进展使人形机器人更接近在制造业、物流和家庭辅助等领域的实际应用。它展示了 DeepMind 在具身智能方面的进展，可能加速多功能机器人的普及。 Gemini Robotics 2 利用空间推理和长时域规划来制定多步骤任务并实现机器人间的协作。目前仅限受信任的测试者使用，包括波士顿动力和 Agility Robotics 等公司。

hackernews · ai2027 · 7月30日 15:15 · [社区讨论](https://news.ycombinator.com/item?id=49111237)

**背景**: 早期的 Gemini Robotics 模型仅使用上身控制来专注于桌面操作。全身控制需要平衡、腿部运动以及更多自由度的协调，难度显著增加。该模型基于 Gemini 2.0 大语言模型，针对机器人场景进行了调整。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/">Gemini Robotics 2 brings whole body intelligence to robots — Google DeepMind</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_Robotics">Gemini Robotics</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/gemini-robotics-er-2/">Introducing Gemini Robotics ER 2</a></li>

</ul>
</details>

**社区讨论**: 一位 DeepMind 研究人员从内部角度称赞了该实验室在 AI 各领域的广度。评论者注意到机器人目前动作缓慢，但与早期 LLM 相类比，预测其将快速改进。也有部分人对人形硬件的局限性（如执行器）表示怀疑。

**标签**: `#robotics`, `#AI`, `#DeepMind`, `#Gemini`, `#embodied intelligence`

---

<a id="item-5"></a>
## [OpenAI 发布 GPT-5.6 Luna，价格大降 80%](https://openai.com/index/advancing-the-price-performance-frontier-with-gpt-5-6/) ⭐️ 8.0/10

OpenAI 发布了 GPT-5.6 Luna，这是其最快、最实惠的模型，价格降低了 80%，现在每百万输入令牌收费 0.10 美元，每百万输出令牌收费 0.60 美元。 这一大幅降价使高级 AI 推理对开发者和企业更加可及，可能加速采用并支持新的高容量应用，如多智能体系统。 GPT-5.6 Luna 支持 1,050,000 令牌的上下文窗口和最多 128,000 令牌的输出，同时 OpenAI 通过内核优化和效率改进降低了服务成本。

hackernews · tedsanders · 7月30日 17:15 · [社区讨论](https://news.ycombinator.com/item?id=49112867)

**背景**: GPT-5.6 Luna 是 OpenAI 的 GPT-5.6 模型家族的一部分，该家族包括旗舰模型 Sol 和平衡模型 Terra。它专为成本敏感、高负载的工作负载设计。此次降价延续了 AI 模型价格在经历一段上涨期后再次下降的趋势，Kimi K3 和 GLM 5.2 等竞争对手也在降低成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://openrouter.ai/openai/gpt-5.6-luna">GPT-5.6 Luna - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://developers.openai.com/api/docs/models/gpt-5.6-luna">GPT-5.6 Luna Model | OpenAI API</a></li>

</ul>
</details>

**社区讨论**: 社区对此反应热烈且惊讶，将此次降价比作从拨号上网到宽带的转变。用户指出运行更多并行智能体的潜力，以及决定何时使用较弱模型的挑战。一些人质疑 OpenAI 通过优化节省的成本是否每月达到数十亿美元。

**标签**: `#AI`, `#GPT-5.6`, `#OpenAI`, `#cost-efficiency`, `#model-pricing`

---

<a id="item-6"></a>
## [Google 通过 Age Signals API 在全球扩大安卓年龄验证](https://android-developers.googleblog.com/2026/07/google-play-age-signals-api-safer-experiences.html) ⭐️ 8.0/10

Google 宣布将在 2026 年底前在全球范围内扩大安卓设备的年龄验证检查，要求应用集成其 Play Age Signals API 以确定用户年龄范围。该 API 目前处于测试阶段，允许应用从 Google Family Link 请求年龄信号，从而强制执行适龄内容。 此举标志着 Google 在全球市场向监管合规迈出了重要一步，但引发了关于强制创建账号和数据集中化的隐私担忧。这将影响数百万安卓应用开发者和用户，可能重塑应用处理年龄敏感内容的方式。 Play Age Signals API 返回的年龄范围包括 0-12、13-15、16-17 和 18+，支持 Android 6.0 及以上设备。未集成该 API 的应用可能面临执法行动，但 Google 尚未披露具体处罚措施。该功能首先在巴西进行测试。

hackernews · dmantis · 7月30日 10:13 · [社区讨论](https://news.ycombinator.com/item?id=49107950)

**背景**: 移动平台上的年龄验证一直存在争议，监管机构要求加强对未成年人的保护。Google 的 Family Link 已提供家长控制功能，而 Age Signals API 将其扩展到第三方应用。开发者必须选择接入该 API，不能依赖用户自行填报的年龄。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.android.com/google/play/age-signals/use-age-signals-api">Use Play Age Signals API (beta) - Android Developers</a></li>
<li><a href="https://developer.android.com/google/play/age-signals/overview">Play Age Signals overview | Android Developers</a></li>
<li><a href="https://cybernews.com/tech/android-developers-age-verification-tool-google/">What is Google’s Android Age Signals API tool? | Cybernews</a></li>

</ul>
</details>

**社区讨论**: 评论反映出分歧：有人反对强制创建账号，担心垄断锁定；另一些人则认为仅靠家长责任不够，监管必不可少。一个值得注意的担忧是，该 API 是自愿接入的，可能导致不合规的应用仍让儿童接触不适当内容。

**标签**: `#privacy`, `#age-verification`, `#android`, `#google-play`, `#regulation`

---

<a id="item-7"></a>
## [重构的经济效益量化分析](https://martinfowler.com/articles/exploring-gen-ai/refactoring-economic-benefit.html) ⭐️ 8.0/10

本文对重构的经济效益进行了量化分析，通过提供 AI 在重构任务中性能的具体测量数据，批评了模糊的 AI 评论。 这很重要，因为它将关于 AI 在软件工程中的讨论从抽象推测转向数据驱动的证据，帮助开发者和管理者在重构和 AI 工具投资方面做出明智决策。 文章可能包括 token 消耗减少等具体指标，并认为重构能降低 token 使用量并提升 AI 推理能力，正如社区评论所指出的。

hackernews · javaeeeee · 7月30日 15:10 · [社区讨论](https://news.ycombinator.com/item?id=49111176)

**背景**: 重构是在不改变代码外部行为的情况下重组现有代码的过程，旨在提高可读性、可维护性和性能。随着 AI 编程助手的兴起，关于 AI 辅助重构的讨论很多，但往往缺乏具体证据。本文提供了数据驱动的视角。

**社区讨论**: 社区高度赞扬这篇文章的具体量化方法，将其与模糊的 AI 评论形成对比。一些评论强调重构的好处不仅限于 token 消耗，还包括更好的推理和泛化能力。另一些评论指出，在重构过程中，人工参与对于理解项目上下文仍然至关重要。

**标签**: `#refactoring`, `#AI`, `#software engineering`, `#economics`, `#code quality`

---

<a id="item-8"></a>
## [GCC 指导委员会通过拒绝 AI 生成贡献的政策](https://lwn.net/Articles/1086041/) ⭐️ 8.0/10

GCC 指导委员会已采纳 GCC AI 政策工作组的建议，拒绝任何由 AI 或 LLM 代理生成的、具有法律意义的代码贡献，该政策立即生效。 该政策为应对大量低质量 AI 生成拉取请求的开源项目树立了明确先例，有助于维护代码质量和法律清晰度，同时引发了关于 AI 在开源开发中角色的辩论。 该政策针对“具有法律意义”的贡献，如新功能或复杂补丁，而细微的修正（如拼写纠正）仍可能被接受；贡献者需证明其工作是自己的原创。

hackernews · arto · 7月30日 11:45 · [社区讨论](https://news.ycombinator.com/item?id=49108685)

**背景**: GCC（GNU 编译器套件）是一个支持多种编程语言的基石级开源编译器项目。AI 编码助手的兴起导致大量自动化拉取请求涌入，这些请求通常缺乏质量和法律来源，促使许多开源项目制定正式的 AI 贡献政策。类似举措已在 curl 等项目中出现，后者因 AI 生成的虚假报告而部分关闭了其漏洞赏金计划。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/GCC-Declining-AI-Contributions">GCC To Decline Any Significant Contributions Made Via AI/LLMs...</a></li>
<li><a href="https://itsfoss.com/news/gcc-bans-ai-code/">GCC Compiler Bans AI Code Contribution But Sensibly</a></li>

</ul>
</details>

**社区讨论**: 社区评论呈现出多种观点：一些人称赞该政策是对低质量 AI 贡献的必要防护，而另一些人则批评其过于严格，让人联想到过去有问题的禁令（如 Zig 的类似政策）。一条引人注目的评论称“AI 的真正目的是让财富获得技能，而不让技能获得财富”，反映了对公平性的深层担忧。

**标签**: `#GCC`, `#AI policy`, `#open source`, `#community guidelines`

---

<a id="item-9"></a>
## [教授因会议评审缺陷失去博士生候选人](https://www.reddit.com/r/MachineLearning/comments/1vawwb8/i_have_lost_three_and_a_half_potential_phd/) ⭐️ 8.0/10

一位早期职业助理教授报告称，他因机器学习会议评审过程的随意性和令人疲惫不堪而失去了三位半潜在的博士生。 这凸显了机器学习学术界的一个系统性问题：评审过程使有才华的年轻研究者不愿攻读博士学位，可能损害该领域的未来。 该教授的论文获得了强力评审（例如四份一致弱接收），但仍被拒稿，导致无尽的重新提交循环，每轮都会引入新的随机批评。

reddit · r/MachineLearning · /u/AffectionateLife5693 · 7月30日 15:30

**背景**: 顶级机器学习会议（如 NeurIPS、ICML、ICLR）采用每篇论文多位评审人的同行评审流程。近年来，投稿量激增，使得评审压力更大且不一致。ML 领域的“三大顶会”通常被认为是 NeurIPS、ICML 和 ICLR；有些人也将 CVPR 纳入视觉领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.roboflow.com/ai-computer-vision-conferences/">Top AI & Computer Vision Conferences in 2026</a></li>
<li><a href="https://www.academia.edu/85652368/Design_and_Analysis_of_the_NIPS_2016_Review_Process">(PDF) Design and Analysis of the NIPS 2016 Review Process</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#conference review`, `#academia`, `#PhD students`, `#research culture`

---

<a id="item-10"></a>
## [MLVC：面向真实部署的多平台学习视频编解码器](https://www.reddit.com/r/MachineLearning/comments/1vb3xwd/mlvc_multiplatform_learned_video_codec_for/) ⭐️ 8.0/10

MLVC 是一种对硬件鲁棒的神经视频编解码器，它通过超先验传输熵模型尺度参数，绕过了跨平台数值精度问题，在消费级 NPU 上对 360p/540p 视频实现了约 100 FPS 的编码/解码。 这项工作解决了学习型视频编解码器的一个关键部署障碍——跨平台不兼容性，尽管其编码效率更优，但这一问题此前阻止了它们在实际中取代 H.264 和 AV1 等传统编解码器。 MLVC 通过超先验显式传输熵模型参数，避免了在不同 NPU 上要求神经网络推理的位精确性，从而确保即使硬件数学运算不同也能正确解码。在消费级 NPU 上，该编解码器对较低分辨率视频运行速度约为 100 FPS。

reddit · r/MachineLearning · /u/tanelai · 7月30日 19:40

**背景**: 学习型视频编解码器使用神经网络压缩视频，通常能比 H.265 和 AV1 等传统编解码器获得更好的率失真性能。然而，它们依赖的熵模型要求编码器和解码器进行位精确的算术运算；不同硬件平台上的微小浮点差异可能导致灾难性的解码失败。传统编解码器之所以占主导地位，是因为它们拥有无处不在的硬件加速和明确指定的数学运算，而神经编解码器缺乏跨平台确定性和高效的部署路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2309.11276">Towards Real-Time Neural Video Codec for Cross-Platform ...[2606.28027v1] MLVC: Multi-platform Learned Video Codec for ...Towards Real-Time Neural Video Codec for Cross-Platform ...Towards Real-Time Neural Video Codec for Cross-Platform ...Towards Real-Time Neural Video Codec for Cross-Platform ...Towards Real-Time Neural Video Codec for Cross-Platform ...Cross-Platform Neural Video Coding: A Case Study - IEEE Xplore</a></li>

</ul>
</details>

**标签**: `#learned video codecs`, `#neural compression`, `#cross-platform`, `#video encoding`, `#AI deployment`

---

<a id="item-11"></a>
## [Kimi K3 以创新技术实现前沿开源权重性能](https://www.reddit.com/r/MachineLearning/comments/1vaysjf/how_kimi_k3_engineered_its_way_to_the_frontier_r/) ⭐️ 8.0/10

Moonshot AI 发布了开源权重模型 Kimi K3，在 Artificial Analysis 上排名第四，仅次于 Claude Opus 5、Fable 5 和 GPT-5.6 Sol。其 47 页技术报告和代码揭示了三大创新：Kimi Delta Attention、896 专家量级均衡以及用于强化学习的 AgentENV。 该模型证明开源权重模型能够与专有前沿模型竞争，降低了研究人员和开发者获取最先进能力的门槛。新颖的注意力机制和专家均衡技术可能影响整个行业未来的架构设计。 Kimi Delta Attention 将 93 层中 69 层的 KV 缓存替换为每个注意力头一个 128x128 矩阵，使 100 万 token 上下文内存从 104.6 GiB 降至 27.2 GiB。Quantile Balancing 直接根据路由器得分分位数计算选择偏差，以均匀加载每层 896 个专家，克服了 DeepSeek-V3 固定步长偏差调整的局限。

reddit · r/MachineLearning · /u/noninertialframe96 · 7月30日 16:37

**背景**: 大型语言模型通常使用需要大量内存存储键值缓存的注意力机制，尤其在长上下文场景下。混合专家（MoE）模型使用多个专家子网络和一个路由器为每个 token 选择子集，需要负载均衡以防止某些专家过载。面向智能体任务的强化学习训练需要隔离的沙箱来安全高效地执行动作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jianyuh.github.io/attention/2025/12/13/KDA.html">Linear Attention: Kimi Delta Attention | Jianyu Huang’s Blog</a></li>
<li><a href="https://lilting.ch/en/articles/kimi-k3-moe-experts-router-dynamic-transformer">Kimi K3's router picks 16 of 896 experts: an allocator... | lilting channel</a></li>
<li><a href="https://www.marktechpost.com/2026/07/27/kimi-ai-and-kvcache-ai-open-sources-agentenv/">Kimi AI and kvcache-ai Open Sources 'AgentENV... - MarkTechPost</a></li>

</ul>
</details>

**标签**: `#large language models`, `#attention mechanisms`, `#open-weight models`, `#model optimization`, `#Moonshot AI`

---

<a id="item-12"></a>
## [字节最大 To B 重组：飞书并入豆包和火山引擎](https://news.qq.com/rain/a/20260730A03CAP00) ⭐️ 8.0/10

字节跳动宣布自成立以来最大规模的 B 端业务重组，将飞书产品团队与豆包 AI 助手团队整合为新的“豆包产品团队”，并将飞书的市场、销售及客服团队与火山引擎合并，成立“创造力服务平台”。 此举标志着字节跳动战略性地将其领先的 AI 助手豆包与企业生产力工具深度融合，可能重塑中国企业软件市场的竞争格局。 飞书现有产品保持不变，双方团队将深化生产力场景合作；由双方共同开发的豆包企业版已在部分飞书客户中开展内测。

telegram · zaihuapd · 7月30日 02:55

**背景**: 飞书是字节跳动的企业协作套件。豆包是字节跳动基于自研大语言模型的 AI 对话助手，拥有超过 5000 万活跃用户。火山引擎是字节跳动的企业云和 AI 平台。此次重组旨在统一 AI 能力与企业服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.toolcentral.ai/ai-tools/doubao/">Doubao: ByteDance's AI Assistant for Chat & Content - ToolCentral</a></li>
<li><a href="https://aiwiki.ai/wiki/volcano_engine">Volcano Engine | AI Wiki</a></li>

</ul>
</details>

**标签**: `#ByteDance`, `#AI`, `#Feishu`, `#enterprise software`, `#restructuring`

---

<a id="item-13"></a>
## [谷歌 DeepMind 解散 AlphaFold 团队，核心成员转投 Anthropic](https://www.ft.com/content/61b2953d-ee0d-45de-af6e-a9c1cf524b33?syn-25a6b1a6=1) ⭐️ 8.0/10

谷歌 DeepMind 解散了 AlphaFold 团队，将大部分研究人员重新分配至其他项目（包括 Gemini 和 Isomorphic Labs），而三名核心成员——John Jumper、Jonas Adler 和 Alexander Pritzel——已离职加入竞争对手 Anthropic。 此次重组将资源从获得诺贝尔奖的突破性成果转移到大语言模型等其他优先事项上，标志着 DeepMind 的战略转向。核心人才流向 Anthropic 凸显了行业对 AI 研究人员的激烈竞争。 在过去一年中，大多数 AlphaFold 论文的原作者已被内部调岗至 Gemini、酶设计、核聚变和基因组学等项目，部分人转至 Alphabet 旗下的药物发现子公司 Isomorphic Labs。近四分之一的论文作者已完全离开公司。

telegram · zaihuapd · 7月30日 07:45

**背景**: AlphaFold 是由 DeepMind 开发的 AI 系统，能够高精度预测蛋白质结构，并于 2024 年获得诺贝尔化学奖。它已被广泛应用于生物学研究。Isomorphic Labs 由 DeepMind CEO Demis Hassabis 创立，是一家独立的 Alphabet 公司，专注于将 AI 应用于药物发现，其技术基于 AlphaFold。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AlphaFold">AlphaFold - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Isomorphic_Labs">Isomorphic Labs</a></li>
<li><a href="https://deepmind.google/science/alphafold/">AlphaFold — Google DeepMind</a></li>

</ul>
</details>

**标签**: `#AI`, `#DeepMind`, `#AlphaFold`, `#Anthropic`, `#talent migration`

---

<a id="item-14"></a>
## [欧盟启动 AI 超级工厂招标 拟撬动 300 亿欧元](https://www.wsj.com/world/europe/eu-opens-call-for-creation-of-local-ai-gigafactories-c286213d) ⭐️ 8.0/10

欧盟委员会正式启动人工智能超级工厂的招标程序，计划建设最多七座 AI 设施，目标撬动约 3000 亿欧元总投资，其中 100 亿欧元来自欧盟层面资金和参与成员国共同出资。 这一举措是欧盟增强自身 AI 能力、与美国等全球领导者竞争的战略行动。该投资可能大幅加速欧洲 AI 基础设施建设，影响初创企业、研究人员和各行各业。 招标分为建设选址和扩建两个阶段，投标截止日期为 11 月 12 日，中标结果预计 2027 年 7 月公布，项目须在签约后 18 个月内投入运营。

telegram · zaihuapd · 7月30日 11:50

**背景**: AI 超级工厂是大型设施，旨在处理超大规模 AI 模型的完整生命周期，从训练到部署。它们与传统数据中心不同，通过统一架构整合强大的计算资源。欧盟的高性能计算联合企业（EuroHPC JU）负责监督该计划。此举正值全球 AI 竞争加剧之际，美国和中国都在进行大量投资。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eurohpc-ju.europa.eu/ai-gigafactories_en">AI Gigafactories - The European High Performance Computing Joint...</a></li>

</ul>
</details>

**标签**: `#AI`, `#EU`, `#infrastructure`, `#investment`, `#policy`

---