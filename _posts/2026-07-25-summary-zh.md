---
layout: default
title: "Horizon Summary: 2026-07-25 (ZH)"
date: 2026-07-25
lang: zh
---

> 从 26 条内容中筛选出 11 条重要资讯。

---

1. [vLLM v0.26.0 发布：新增 Inkling 模型家族与性能优化](#item-1) ⭐️ 9.0/10
2. [Anthropic 发布 Claude Opus 5，价格仅为 Fable 5 的一半](#item-2) ⭐️ 9.0/10
3. [SGLang v0.5.16 发布：支持 DSpark 推测解码和 Inkling 模型](#item-3) ⭐️ 8.0/10
4. [开放权重 AI 正在迎来它的 Kubernetes 时刻](#item-4) ⭐️ 8.0/10
5. [安卓可能限制设备端 ADB 使用](#item-5) ⭐️ 8.0/10
6. [Ruff v0.16.0 默认启用 413 条 lint 规则](#item-6) ⭐️ 8.0/10
7. [AMD 能否打破 CUDA 护城河？代理内核与 MI455X](#item-7) ⭐️ 8.0/10
8. [中国离岸信托个税新规：装入财产及收益须按年申报，税率 20%](#item-8) ⭐️ 8.0/10
9. [中国对携程开出 51.79 亿元反垄断罚单](#item-9) ⭐️ 8.0/10
10. [高通宣布全线产品 9 月 1 日起涨价](#item-10) ⭐️ 8.0/10
11. [微软利用 TPM 芯片封堵盗版 Windows 激活](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 发布：新增 Inkling 模型家族与性能优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 正式发布，包含来自 212 位贡献者的 411 次提交，新增对 Inkling 模型家族的支持、DeepSeek-V4 的性能优化、fp32 lm_head 支持以及可按 KV-cache 分组选择注意力后端的功能。 此版本意义重大，因为 vLLM 是广泛使用的 LLM 推理库，新功能提升了灵活性、性能和模型支持，惠及整个 LLM 服务生态系统。 关键技术细节包括 Inkling 模型的分段 CUDA graph 支持、DeepSeek-V4 的专用路由内核、以及用于 fp32 lm_head 的新 'head_dtype' 参数。现在可以每个 KV-cache 分组选择注意力后端，滑动窗口支持成为显式能力。

github · khluu · 7月25日 10:38

**背景**: vLLM 是一个用于高吞吐量 LLM 推理的开源库，支持多种模型和硬件。Inkling 模型家族是 Thinking Machines Lab 推出的多模态 MoE 模型，总参数 975B。分段 CUDA graph 通过将计算拆分为片段来提高性能，Hopper FA4 是专为 NVIDIA Hopper 架构优化的 FlashAttention-4。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://docs.sglang.io/advanced_features/piecewise_cuda_graph.html">Piecewise CUDA Graph - SGLang Documentation</a></li>
<li><a href="https://arxiv.org/html/2603.05451v1">FlashAttention-4: Algorithm and Kernel Pipelining Co-Design for Asymmetric Hardware Scaling</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#vLLM`, `#deep learning`, `#model serving`, `#GPU optimization`

---

<a id="item-2"></a>
## [Anthropic 发布 Claude Opus 5，价格仅为 Fable 5 的一半](https://simonwillison.net/2026/Jul/24/introducing-claude-opus-5/#atom-everything) ⭐️ 9.0/10

Anthropic 发布了 Claude Opus 5，这是一款接近 Claude Fable 5 前沿智能水平的新 AI 模型，但价格仅为后者的一半。该模型目前在 Artificial Analysis 排行榜上领先，甚至超越了 Fable 5。 此次发布以显著降低的价格提供了接近前沿的 AI 能力，可能会让更多开发者和企业以更低成本使用先进 AI。这也展示了大型语言模型开发的持续快速进步，加剧了供应商之间的竞争。 Claude Opus 5 的定价与其前身 Opus 4.8 相同，并提供快速模式（价格为基本模型的两倍）。它提升了网络安全漏洞检测能力，但未刻意接受利用漏洞的训练，因此更加安全。

rss · Simon Willison · 7月24日 23:48

**背景**: Anthropic 是一家领先的 AI 公司，以其 Claude 系列大型语言模型而闻名。前沿智能指的是最先进的 AI 能力，其中 Claude Fable 5 是 Anthropic 先前的最顶级模型。Artificial Analysis 排行榜根据多项基准测试的表现对模型进行排名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/leaderboards/models">LLM Leaderboard - Comparison of AI models from OpenAI, Anthropic...</a></li>
<li><a href="https://huggingface.co/spaces/ArtificialAnalysis/LLM-Performance-Leaderboard">LLM Performance Leaderboard - a Hugging Face Space by...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#language models`, `#machine learning`

---

<a id="item-3"></a>
## [SGLang v0.5.16 发布：支持 DSpark 推测解码和 Inkling 模型](https://github.com/sgl-project/sglang/releases/tag/v0.5.16) ⭐️ 8.0/10

SGLang v0.5.16 引入了基于置信度调度的推测解码算法 DSpark，并增加了对 Inkling 多模态 MoE 模型（975B 参数、1M 上下文）的支持。该版本还将 UnifiedRadixTree 设为默认缓存结构，优化了 Blackwell GPU 上的线性注意力性能，并新增了 LongCat 2.0 等模型。 DSpark 在 DeepSeek-V4-Pro 上实现了 383.7 tok/s 的速度和约 5 的接受长度，显著提升单用户生成吞吐量。对 Inkling 的支持使得 975B 多模态 MoE 模型能够得到高达 71.7k tok/s 输入和 171.0 tok/s 单用户解码的推理服务，推动了开源权重模型推理的极限。 DSpark 采用半自回归块草稿和基于置信度的验证窗口大小，通过 --speculative-algorithm DSPARK 启用。Inkling 混合了滑动窗口、完全注意力和 Mamba2 线性注意力，并包含 NVFP4 MoE，已在 Blackwell、H200 和 AMD MI350X 上验证。该版本还移除了实验性的 QServe 和 FBGEMM FP8 量化路径。

github · Qiaolin-Yu · 7月25日 00:13

**背景**: 推测解码通过使用小型草稿模型生成多个候选 token，再由目标模型验证，从而加速 LLM 推理。DSpark 通过根据草稿模型的置信度自适应调整验证窗口大小，改进了固定长度草稿方法。Inkling 是 Thinking Machines Lab 开发的 975B 参数多模态 MoE 模型，具有 1M token 上下文和包括 Mamba2 线性注意力在内的混合注意力机制。Mamba2 是一种状态空间模型，可实现线性时间序列建模，在处理长上下文时更为高效。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.05147">[2607.05147] DSpark: Confidence-Scheduled Speculative ...</a></li>
<li><a href="https://inkling-model.com/">Inkling Model: Architecture, Capabilities, Context & Access</a></li>
<li><a href="https://arxiv.org/abs/2312.00752">[2312.00752] Mamba: Linear-Time Sequence Modeling with Selective State Spaces</a></li>

</ul>
</details>

**标签**: `#sglang`, `#speculative decoding`, `#LLM serving`, `#multimodal MoE`, `#performance optimization`

---

<a id="item-4"></a>
## [开放权重 AI 正在迎来它的 Kubernetes 时刻](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

文章认为，开放权重 AI 模型有望成为类似 Kubernetes 的基础平台，推动 AI 行业的广泛采用和协作创新。 这一转变可能使 AI 开发民主化，减少对封闭模型的依赖，并促进类似 Kubernetes 在云计算领域的协作生态系统，使初创企业和企业能够基于共享的开放权重模型进行构建。 开放权重模型提供模型权重的访问权限，但不一定包括完整的训练数据或代码，这与完全开源模型不同。该类比强调，像 Kubernetes 一样，开放权重 AI 可以标准化并加速创新，同时仍然允许商业使用。

hackernews · tknaup · 7月25日 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49048034)

**背景**: Kubernetes 是一个开源容器编排平台，已成为大规模部署和管理应用程序的行业标准。类似地，开放权重 AI 模型发布训练好的神经网络权重，使其他人可以在无需从头训练的情况下进行微调、托管和构建。这种方法降低了准入门槛并促进了协作，但不同于完全开源 AI，后者还包括训练代码和数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open-weight AI : what if we finally opened the bonnet ?</a></li>
<li><a href="https://openai.com/index/introducing-gpt-oss/">Introducing gpt-oss | OpenAI</a></li>

</ul>
</details>

**社区讨论**: 社区评论者讨论了按来源禁止中国 AI 模型的可行性，指出权重只是数字，无法追溯地理位置。其他人讨论了 GPT-4 等封闭模型定价波动性，并认为开放权重模型提供了稳定的基准。还有支持类似 Linux 的协作模型开发，呼吁 OpenAI 等实验室更频繁地更新模型。

**标签**: `#open-weight AI`, `#Kubernetes`, `#AI models`, `#open source`, `#AI industry`

---

<a id="item-5"></a>
## [安卓可能限制设备端 ADB 使用](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

安卓可能对设备端 ADB（Android 调试桥）的使用实施限制，根据功能请求讨论，可能限制其可用性或要求身份验证。 这一变化可能严重影响依赖 ADB 进行调试和自定义的开发者及高级用户，同时提升普通用户的安全性。这再次引发了安全与开发者自由之间的辩论。 拟议的限制似乎针对通过 Wi-Fi 的远程 ADB，要求用户启用开发者选项和远程调试。社区对于安全收益是否超过可用性成本存在分歧。

hackernews · shscs911 · 7月25日 06:57 · [社区讨论](https://news.ycombinator.com/item?id=49045159)

**背景**: ADB 是一个命令行工具，允许开发者通过 USB 或 Wi-Fi 与 Android 设备通信，用于调试、安装应用和运行 shell 命令。设备端 ADB（Wi-Fi 无线调试）方便但可能使设备易受网络攻击。近年来，Google 一直在收紧开发者功能的安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>
<li><a href="https://www.howtogeek.com/125769/how-to-install-and-use-abd-the-android-debug-bridge-utility/">How to Install and Use ADB, the Android Debug Bridge Utility</a></li>
<li><a href="https://xdaforums.com/t/q-adb-over-wifi-security.1452999/">[Q] adb over wifi ... security | XDA Forums</a></li>

</ul>
</details>

**社区讨论**: 评论中意见不一。有人认为攻击向量极小，因为需要同时启用开发者选项和远程 ADB。另一些人则认为这是进一步限制用户控制的一步。部分开发者提出更细致的解决方案，如 IP 白名单。

**标签**: `#Android`, `#ADB`, `#Security`, `#Developer Tools`

---

<a id="item-6"></a>
## [Ruff v0.16.0 默认启用 413 条 lint 规则](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

此次默认规则的重大扩展会导致未锁定 Ruff 版本的项目出现大范围 CI 失败，迫使开发者调整其代码库。随着 Ruff 的采用率持续增长，这显著加强了整个 Python 生态系统的代码质量标准。 此次更新使规则总数从 v0.1.0 的 708 条增加到 968 条，新增默认规则包括 B（bugbear）、UP（pyupgrade）和 RUF（Ruff 特有）等类别。`ruff check . --fix --unsafe-fixes` 命令可自动修复许多问题，例如在 sqlite-utils 中修复了 1618 个错误中的 1538 个。

rss · Simon Willison · 7月25日 22:44

**背景**: Ruff 是一个用 Rust 编写的极速 Python linter 和代码格式化工具，旨在取代 Flake8、Black 和 isort 等工具。它以其速度（比现有 linter 快 10-100 倍）以及将多个工具捆绑到单个二进制文件中的能力而广受欢迎。Ruff 背后的公司 Astral 最近被 OpenAI 收购。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff">GitHub - astral-sh/ruff: An extremely fast Python linter and code formatter, written in Rust. · GitHub</a></li>
<li><a href="https://pydevtools.com/blog/ruff-0-16-0-default-rules/">Ruff 0.16.0 Enables 7x More Rules by Default | pydevtools</a></li>
<li><a href="https://docs.astral.sh/ruff/rules/">Rules | Ruff</a></li>

</ul>
</details>

**标签**: `#Python`, `#linting`, `#tooling`, `#version release`

---

<a id="item-7"></a>
## [AMD 能否打破 CUDA 护城河？代理内核与 MI455X](https://newsletter.semianalysis.com/p/can-amd-break-the-cuda-moat-amd-advancing) ⭐️ 8.0/10

Semianalysis 的一份报告分析了 AMD 通过代理内核生成和新款 Instinct MI455X GPU 打破英伟达 CUDA 垄断的策略，同时详述了严峻的生产挑战以及高达 105%的财务折扣。 如果 AMD 能够克服其软件和生产障碍，它将为英伟达 CUDA 生态系统提供可行的替代方案，从而减少 AI 开发者的锁定效应并可能降低成本。 MI455X 是采用 2nm 工艺、配备 432GB HBM4 内存的 GPU，AMD 的“代理内核生成”利用 LLM 自动优化兼容 CUDA 的内核，但内部开发集群仍不稳定，量产爬坡被形容为“地狱”。

rss · Semianalysis · 7月25日 00:33

**背景**: CUDA 是英伟达的专有并行计算平台，通过锁定开发者形成“护城河”。AMD 的开源 ROCm 平台旨在与之竞争，但历史上在软件成熟度上落后。代理内核生成（如 CUDA Agent 项目所展示）利用强化学习自动生成并优化高性能内核，有望简化从 CUDA 到 AMD 硬件的过渡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/can-amd-break-the-cuda-moat-amd-advancing">Can AMD break the CUDA Moat? AMD Advancing AI 2026</a></li>
<li><a href="https://www.phoronix.com/news/AMD-Instinct-MI455X-Helios">AMD Launches Instinct MI455X, Helios AI Rack - Phoronix</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/amd-takes-the-wraps-off-its-instinct-mi455x-ai-accelerator-cdna-5-and-helios-rack-scale-architecture-combine-to-take-the-fight-to-nvidia-in-the-data-center">AMD takes the wraps off its Instinct MI455X AI accelerator — CDNA 5 and Helios rack-scale architecture combine to take the fight to Nvidia in the data center | Tom's Hardware</a></li>

</ul>
</details>

**标签**: `#AMD`, `#CUDA`, `#GPU computing`, `#AI hardware`, `#machine learning`

---

<a id="item-8"></a>
## [中国离岸信托个税新规：装入财产及收益须按年申报，税率 20%](https://liaoning.chinatax.gov.cn/art/2026/7/24/art_5869_7823.html) ⭐️ 8.0/10

该规定封堵了富裕阶层利用离岸信托延期或逃避个税的路径，对高净值人群的跨境财富筹划和税务合规义务产生重大影响。 税率统一为 20%，仅对增值部分（现值减原值及成本）征税；2023 年至 2025 年间的应缴未缴税款及 2026 年前收益可在公告实施后 90 日内补申报，不加收滞纳金。

telegram · zaihuapd · 7月25日 00:31

**背景**: 离岸信托常被中国居民用于资产保护与财富传承，但此前税法对信托资产及收益的征税时点和方式缺乏明确规定。新规采用穿透式征税原则，将信托视为税收透明体，每年将全部经济利益归属于委托人。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://yangxiang.blog.caixin.com/archives/286129">yangxiang.blog.caixin.com/archives/286129</a></li>
<li><a href="https://www.donews.com/news/detail/8/6645794.html">donews.com/news/detail/8/6645794.html</a></li>
<li><a href="https://www.workercn.cn/c/2026-07-25/8855325.shtml">政策解读·问答｜离岸信托需缴纳个人所得税 - 经济 - 中工网</a></li>

</ul>
</details>

**标签**: `#tax regulation`, `#offshore trusts`, `#China`, `#personal finance`

---

<a id="item-9"></a>
## [中国对携程开出 51.79 亿元反垄断罚单](https://www.xinhuanet.com/fortune/20260725/693124245aa44d2bbc7520b7a0c244ea/c.html) ⭐️ 8.0/10

2026 年 7 月 25 日，国家市场监督管理总局因滥用市场支配地位对携程集团处以罚没款合计 51.79 亿元（没收违法所得 16.58 亿元，罚款 35.21 亿元），并责令其退还酒店经营者订单储备金 1.22 亿元，全面整改并落实 19 项措施。 这是中国科技公司收到的最高反垄断罚单，标志着中国新反垄断体制下监管力度的进一步加强。它为针对其他平台经济参与者的执法树立了先例，并重塑在线旅游行业的竞争格局。 罚款包含没收违法所得 16.58 亿元和罚款 35.21 亿元，合计 51.79 亿元。携程须停止独家合作协议、取消“全网最低价”要求，并彻底改革分销模式，包括下线一级委托分销（特牌）合作模式。

telegram · zaihuapd · 7月25日 02:24

**背景**: 中国《反垄断法》禁止滥用市场支配地位，例如强制交易对手进行独家交易或附加不合理交易条件。携程作为在线旅游市场的支配地位企业，被认定强制酒店进行独家合作并附加“最低价”条款，损害了市场竞争。国家市场监督管理总局近年来加强反垄断执法，尤其针对大型平台企业。

**标签**: `#antitrust`, `#regulation`, `#China`, `#Ctrip`, `#tech industry`

---

<a id="item-10"></a>
## [高通宣布全线产品 9 月 1 日起涨价](https://tw.news.yahoo.com/%E7%8D%A8%E5%AE%B6-%E9%AB%98%E9%80%9A%E6%BC%B2%E5%83%B9%E4%BF%A1%E6%9B%9D%E5%85%89-%E5%85%A8%E7%B7%9A%E7%94%A2%E5%93%819-1%E8%B5%B7%E8%AA%BF%E6%BC%B2-%E7%9B%B4%E8%A8%80-142730846.html) ⭐️ 8.0/10

2026 年 7 月 24 日，高通向客户发出价格调整通知，宣布自 2026 年 9 月 1 日起，所有出货产品价格上调。公司表示，晶圆制造、封装测试及基板材料成本持续上升，加上 AI 与数据中心需求激增挤压供应链产能。 此次涨价影响高通广泛应用于手机、PC、物联网和汽车领域的芯片，可能导致消费电子产品价格上涨或功能缩减。这标志着 AI 需求和先进封装成本驱动的半导体行业成本结构性转变。 高通未公布统一涨幅，也未列出具体产品型号，表示客户经理将逐一联系客户提供新报价。部分已下单但排在 9 月后出货的订单也可能被重新报价。

telegram · zaihuapd · 7月25日 03:01

**背景**: 先进封装技术如台积电 CoWoS 和英特尔 EMIB 越来越多用于集成多个芯片，在不完全依赖晶体管微缩的情况下提升性能。这些工艺加上基板材料成本上升，增加了半导体制造成本。高通在移动和汽车芯片领域的主导地位使其定价决策对整个行业具有影响力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Advanced_packaging_(semiconductors)">Advanced packaging (semiconductors)</a></li>
<li><a href="https://www.trendforce.com/news/2025/12/01/news-gold-and-ccl-price-surge-pressures-substrate-makers-driving-shift-toward-high-value-ai-products/">[News] Gold and CCL Price Surge Squeezes Substrate Makers as ...</a></li>

</ul>
</details>

**标签**: `#Qualcomm`, `#price increase`, `#chip shortage`, `#AI demand`, `#semiconductor industry`

---

<a id="item-11"></a>
## [微软利用 TPM 芯片封堵盗版 Windows 激活](https://www.techspot.com/news/113232-microsoft-using-tpm-chips-crack-down-pirated-windows.html) ⭐️ 8.0/10

微软宣布将在其批量激活工具 KMS 中加入基于 TPM 芯片的硬件证明机制，要求 KMS 服务器在进行批量激活前先证明其硬件身份已经微软认证且未被篡改。这一变化将从下一版 Windows Server 起成为强制要求，并自 2026 年 8 月起在 Windows Server 2025 中推送准备提示。 这一反盗版措施针对的是盗版 Windows 广泛使用的 KMS 激活漏洞，可能导致 Online KMS 等常见工具彻底失效。它对企业激活流程进行了重要加固，并可能改变微软与激活绕过开发者之间的攻防态势。 微软 2025 年已封堵了 KMS38 漏洞，而新的 TPM 证明预计将使需要每半年连接伪造服务器续期的 Online KMS 方法失效。不过，Massgrave 组织已推出 TSforge 方法，声称可绕过微软整个 DRM 激活架构，这场攻防战的结果仍有待观察。

telegram · zaihuapd · 7月25日 15:55

**背景**: KMS（密钥管理服务）是一种批量激活方法，企业可借助本地 KMS 主机在网络中批量激活 Windows 和 Office 客户端。TPM（可信平台模块）是一种硬件安全芯片，能够提供系统身份的加密证明。长期以来，盗版 Windows 激活利用伪造 KMS 服务器绕过授权，微软一直在逐步加强激活机制以应对这些攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/windows-server/get-started/kms-client-activation-keys">Key Management Services (KMS) client activation... | Microsoft Learn</a></li>
<li><a href="https://massgrave.dev/">Microsoft Activation Scripts | MAS</a></li>
<li><a href="https://github.com/massgravel/TSforge">GitHub - massgravel/TSforge: A collection of activation/evaluation...</a></li>

</ul>
</details>

**标签**: `#Windows`, `#TPM`, `#Anti-piracy`, `#KMS`, `#Software licensing`

---