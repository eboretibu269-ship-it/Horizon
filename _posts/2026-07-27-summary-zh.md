---
layout: default
title: "Horizon Summary: 2026-07-27 (ZH)"
date: 2026-07-27
lang: zh
---

> 从 32 条内容中筛选出 13 条重要资讯。

---

1. [谷歌透露 Gemini 4 为迄今最雄心勃勃的预训练项目](#item-1) ⭐️ 9.0/10
2. [Fastjson2 远程代码执行漏洞(RCE)未修复](#item-2) ⭐️ 9.0/10
3. [vLLM v0.26.0 新增 Inkling 模型家族与 DeepSeek-V4 优化](#item-3) ⭐️ 8.0/10
4. [Anthropic 明确其对开放权重模型的立场](#item-4) ⭐️ 8.0/10
5. [法官驳回谷歌利用 DMCA 阻止爬虫的尝试](#item-5) ⭐️ 8.0/10
6. [Bun 的 Rust 重写进展顺利，发布推迟](#item-6) ⭐️ 8.0/10
7. [现代电子邮件可用借来的部件构建](#item-7) ⭐️ 8.0/10
8. [月之暗面发布 Kimi-K3：2.8 万亿参数的开源模型](#item-8) ⭐️ 8.0/10
9. [独立研究：6 大前沿 LLM 均显示左倾政治偏见](#item-9) ⭐️ 8.0/10
10. [提出训练前数据确定性审计门控方案](#item-10) ⭐️ 8.0/10
11. [长鑫科技科创板首日暴涨 471%](#item-11) ⭐️ 8.0/10
12. [华为被指与昇维旭共建 DRAM 工厂](#item-12) ⭐️ 8.0/10
13. [中国开始量产国产 DUV 光刻机，今年目标约 5 台](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [谷歌透露 Gemini 4 为迄今最雄心勃勃的预训练项目](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 9.0/10

谷歌 CEO Sundar Pichai 在 Alphabet 2026 年第二季度财报电话会议上宣布，下一代大语言模型 Gemini 4 已投入训练，预计将于 2026 年底发布。 这表明谷歌致力于引领 AI 前沿，可能推动 AGI 研究，并加剧主要 AI 实验室之间的竞争。 Pichai 强调计算资源将优先用于前沿 AGI 研发，而 Gemini 3.x Flash 系列将继续以每月一次的频率更新，重点提升智能编码能力。

telegram · zaihuapd · 7月27日 04:06

**背景**: 预训练是大语言模型从海量文本数据中学习语法、事实和推理的初始阶段。这一阶段建立了通用的基础，之后可以针对特定任务进行微调。谷歌的 Gemini 4 是其迄今为止最雄心勃勃的预训练项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.entrypointai.com/blog/pre-training-vs-fine-tuning-vs-in-context-learning-of-large-language-models/">Pre-training vs Fine-Tuning vs In-Context Learning of Large Language Models | Entry Point AI</a></li>
<li><a href="https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/gemini/3-flash">Gemini 3 Flash | Gemini Enterprise Agent Platform | Google Cloud Documentation</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google Gemini`, `#Large Language Models`, `#AGI`, `#Pre-training`

---

<a id="item-2"></a>
## [Fastjson2 远程代码执行漏洞(RCE)未修复](https://mp.weixin.qq.com/s/LJaul1jNjK9pXRAkoUiMEA) ⭐️ 9.0/10

Fastjson2 2.0.62 及之前所有版本被曝存在严重远程代码执行（RCE）漏洞，项目维护者已确认，但官方补丁尚未发布，PR #7695 已关闭且未合入主分支。 Fastjson2 是 Java 生态中广泛使用的 JSON 处理库，此未修复漏洞对数千应用构成直接安全风险。鉴于这是本月 Fastjson 系列第二个严重漏洞，依赖该库的组织必须立即采取缓解措施，例如彻底禁用 AutoType。 该漏洞允许攻击者通过恶意 JSON 数据绕过 AutoType 类型校验，可能导致任意代码执行。完整漏洞细节和利用代码尚未公开，但维护者建议在修复版发布前彻底禁用 AutoType。

telegram · zaihuapd · 7月27日 10:31

**背景**: Fastjson2 是阿里巴巴开发的高性能 Java JSON 库，作为 Fastjson 1.x 的继任者。AutoType 是一种在反序列化时自动解析类型的特性，历史上一直是反序列化漏洞的常见攻击面。2026 年 7 月早些时候，Fastjson 1.x（版本 1.2.68–1.2.83）被披露存在严重 RCE 漏洞，阿里巴巴建议迁移到 Fastjson2 作为长期修复方案；然而，此次新漏洞表明 Fastjson2 本身现在也受到影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://alibaba.github.io/fastjson2/">FASTJSON2 is a Java JSON library with excellent performance.</a></li>
<li><a href="https://thehackernews.com/2026/07/fastjson-1x-rce-vulnerability-targeted.html">Fastjson 1.x RCE Vulnerability Targeted in Attacks With No Patched...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#RCE`, `#Fastjson2`, `#Java`

---

<a id="item-3"></a>
## [vLLM v0.26.0 新增 Inkling 模型家族与 DeepSeek-V4 优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 全面支持 975B 参数、1M 上下文长度的 Inkling 模型家族，并针对 DeepSeek-V4 进行了显著性能优化（包括专用路由内核和 fused_topk_bias），同时新增通过 head_dtype 实现的 fp32 lm_head 以提升精度。 此版本大幅扩展了 vLLM 的模型支持与性能能力，使从业者能够更高效、更准确地部署 Inkling 和 DeepSeek-V4 等前沿大模型，并支持 NVIDIA、AMD 和 Intel 硬件。 关键技术细节包括：Inkling 模型的分段 CUDA 图支持、Hopper FA4 相对注意力、MTP=1 推测解码、LoRA 支持以及 ModelOpt NVFP4 量化；DeepSeek-V4 方面，专用路由内核带来 2.94% 的端到端 TPOT 提升，fused_topk_bias 实现 1.5-2 倍内核加速。

github · khluu · 7月27日 01:06

**背景**: vLLM 是一个开源的高吞吐量 LLM 推理服务系统。Inkling 模型是 Thinking Machines Lab 发布的 975B 参数混合专家 transformer，具有 41B 活跃参数和 1M 令牌上下文窗口。Flash Attention 4 (FA4) 是针对 NVIDIA Hopper GPU 优化的注意力算法，NVFP4 是 NVIDIA Model Optimizer 提供的 4 位浮点量化方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://www.spheron.network/blog/tensorrt-model-optimizer-modelopt-quantization-guide/">NVIDIA TensorRT Model Optimizer (ModelOpt): FP8, INT4, and FP4 Quantization Guide (2026) | Spheron Blog</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#release notes`, `#performance optimization`, `#open-source`

---

<a id="item-4"></a>
## [Anthropic 明确其对开放权重模型的立场](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic 公开发表了对开放权重模型的立场，主张对所有足够强大的模型进行强制性安全测试，但不全面禁止，但批评者认为这实际上限制了开放模型。 这一立场对 AI 治理意义重大，它在开放性与安全性之间寻求平衡，可能为开源 AI 模型的监管开创先例，影响全球开发者和用户。 Anthropic 提议对所有有能力的模型（无论是开放还是封闭）进行强制性安全测试，但未明确由谁管理测试或承担费用，导致批评者认为这实质上等同于禁止开放权重模型。

hackernews · surprisetalk · 7月27日 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开放权重模型是指核心组件公开发布的 AI 模型，允许任何人下载、检查、修改并在自己的基础设施上运行。Anthropic 是一家领先的 AI 安全公司，其 CEO Dario Amodei 此前曾撰写过关于 AI 风险和监管的文章。争论焦点在于如何在不妨碍创新的情况下监管日益强大的开放模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>

</ul>
</details>

**社区讨论**: 社区评论大多持批评态度，用户指出 Anthropic 立场存在矛盾——例如反对全面禁令却支持芯片销售限制——并认为强制性测试可能成为高成本障碍，实质上是禁止开放模型。一些人指责 Anthropic 保护自身闭源业务利益。

**标签**: `#AI safety`, `#open weights`, `#regulation`, `#Anthropic`, `#model governance`

---

<a id="item-5"></a>
## [法官驳回谷歌利用 DMCA 阻止爬虫的尝试](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

一名法官驳回了谷歌利用 DMCA 安全港条款阻止第三方抓取其搜索结果的尝试，裁定这些数据不具有版权性，谷歌的论点不恰当。 该裁决强化了抓取公开数据通常不构成版权侵权的观点，并凸显了谷歌自身爬取网络的历史与其限制自身服务被爬取的努力之间的矛盾。 该案件涉及谷歌起诉 SerpAPI（一个抓取谷歌搜索结果的服务）。法官认为这些数据不具有版权性，谷歌的 DMCA 主张没有依据。

hackernews · cdrnsf · 7月27日 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49073513)

**背景**: DMCA 安全港条款保护在线服务提供商免受用户生成内容的版权责任，但并不能阻止抓取非版权性的事实。谷歌自身依赖网络爬虫来索引互联网。网络抓取的合法性通常取决于被抓取的数据是否具有版权或是否违反服务条款。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DMCA_safe_harbor">DMCA safe harbor</a></li>
<li><a href="https://www.quinnemanuel.com/the-firm/publications/the-legal-landscape-of-web-scraping/">The Legal Landscape of Web Scraping</a></li>
<li><a href="https://blog.apify.com/is-web-scraping-legal/">Is web scraping legal? Yes, if you know the rules.</a></li>

</ul>
</details>

**社区讨论**: 评论者指出了谷歌的虚伪，强调谷歌本身就是通过爬取开放网络建立起来的，并且其 API 的弃用迫使人们依赖第三方抓取工具。一些人表达了对 SerpAPI 的支持，并批评谷歌的强硬法律手段。

**标签**: `#legal`, `#web scraping`, `#DMCA`, `#Google`, `#tech industry`

---

<a id="item-6"></a>
## [Bun 的 Rust 重写进展顺利，发布推迟](https://lockwood.dev/ai/2026/07/27/how-is-the-bun-rewrite-in-rust-going.html) ⭐️ 8.0/10

Bun 的 Rust 重写版已在 Anthropic 的 Claude Code 工具中发布，项目负责人透露重写进展顺利，但 Bun v1.4 版本发布将推迟，直到承诺的 Node.js 兼容性测试数量达标。 这次重写旨在解决广泛使用的 JavaScript 运行时的性能和兼容性问题。发布推迟凸显了在迁移到 Rust 的同时实现完全 Node.js 兼容性的难度，影响了依赖 Bun 提升速度和稳定性的开发者。 Rust 重写版已在一个月前部署到 Claude Code 中，大多数用户并未察觉。发布推迟具体是由于项目中自定的新增 Node.js 测试通过数量指标尚未达标，所需的拉取请求仍未合并。

hackernews · tomlockwood · 7月27日 11:12 · [社区讨论](https://news.ycombinator.com/item?id=49067854)

**背景**: Bun 是一个 JavaScript 运行时，旨在作为 Node.js 的快速替代品，内置了打包器、转译器和包管理器。最初使用 Zig 编写，项目决定用 Rust 重写核心以提高性能和可维护性。Claude Code 是 Anthropic 的代理式编码工具，运行在终端中，协助代码编辑和执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: 项目负责人 Jarred 确认重写版已在 Claude Code 中发布，但版本发布推迟。评论者 SquareWheel 指出，重大重构通常会暂时放缓开发速度；benjiro29 质疑使用 LLM 进行代码翻译，认为软件的价值在于迭代开发；另一位评论者 bendmorris 提到了基于 Zig 的替代方案 buz，声称其构建时间不到一秒，暗示原版的问题可能是自身造成的。

**标签**: `#Bun`, `#Rust`, `#Node.js`, `#runtime`, `#software-engineering`

---

<a id="item-7"></a>
## [现代电子邮件可用借来的部件构建](https://en.andros.dev/blog/d7ed8b07/modern-email-can-be-built-from-borrowed-parts/) ⭐️ 8.0/10

一篇文章提出，通过复用 HTTP 和 Matrix 等现代协议的组件来重建电子邮件，而不是继续扩展 SMTP。这种概念性的转变建议用借用的技术模块化替换 SMTP 的核心功能。 如果实现，这可能使电子邮件更安全、高效和功能丰富，使其符合现代通信期望。然而，由于网络效应和根深蒂固的基础设施，大规模采用障碍意味着任何变革都将极其困难。 文章强调 SMTP 的基本设计已经过时，但社区评论指出了挑战，如垃圾邮件、向后兼容性以及大型邮件的 JSON 解析开销。值得注意的是，JMAP 和 Matrix 是现有的现代协议，可以作为构建模块。

hackernews · andros · 7月27日 08:27 · [社区讨论](https://news.ycombinator.com/item?id=49066639)

**背景**: 自 20 世纪 80 年代以来，电子邮件一直构建在 SMTP 之上，但它是为不同时代设计的，在垃圾邮件、安全性和丰富功能方面存在困难。现代协议如 JMAP（基于 JSON 的 IMAP 替代品）和 Matrix（去中心化实时通信协议）提供了已验证的组件来解决这些缺陷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JSON_Meta_Application_Protocol">JSON Meta Application Protocol - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Matrix_(protocol)">Matrix (protocol) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论意见不一：一些人引用了历史上失败的尝试（例如 1990 年代的垃圾邮件解决方案列表），而另一些人则提出了具体修复方案，如按邮件收费或需要收件人许可。还有人担心 JSON 解析需要在大规模场景下将整个邮件加载到内存中，同时强烈共识认为向后兼容性对采用至关重要。

**标签**: `#email`, `#spam`, `#SMTP`, `#protocol design`, `#network effects`

---

<a id="item-8"></a>
## [月之暗面发布 Kimi-K3：2.8 万亿参数的开源模型](https://huggingface.co/moonshotai/Kimi-K3) ⭐️ 8.0/10

月之暗面（Moonshot AI）在 HuggingFace 上发布了 Kimi-K3，这是一个约 2.8 万亿参数的开源权重模型，是目前公开可用的最大模型。该模型支持原生视觉理解和 100 万 token 的上下文窗口。 此次发布推动了开源 AI 的前沿，为开发者和企业提供了前所未有的定制能力和数据主权。同时，它也引发了关于托管万亿参数模型的经济性和实用性的重要讨论。 该模型采用 mxfp4 精度，需要约 1.5TB 显存。其许可证规定，若年度营收超过 2000 万美元，商业使用需与月之暗面另行签订协议。模型在某些回复中存在身份混淆问题。

hackernews · nateb2022 · 7月27日 06:18 · [社区讨论](https://news.ycombinator.com/item?id=49065752)

**背景**: 万亿参数级的大语言模型通常只能通过 API 访问。开源权重发布允许任何人下载、微调和自行托管模型，在此规模下极为罕见。月之暗面是一家总部位于北京的公司，以推动开源模型的规模边界而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://platform.kimi.ai/docs/models">Model List - Kimi API Platform</a></li>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI</a></li>

</ul>
</details>

**社区讨论**: 社区评论聚焦于托管成本，估计服务该模型可能需要 16 块 B200 GPU。定制化和数据主权被视为重要优势，而许可证的收入门槛则引发了对商业使用的担忧。部分用户指出该模型错误地自称 Claude。

**标签**: `#AI`, `#LLM`, `#Open Source`, `#HuggingFace`, `#Model Release`

---

<a id="item-9"></a>
## [独立研究：6 大前沿 LLM 均显示左倾政治偏见](https://www.reddit.com/r/MachineLearning/comments/1v8fnzw/evaluated_6_frontier_llms_gpt54_claude_sonnet_46/) ⭐️ 8.0/10

一项针对 6 个前沿 LLM（GPT-5.4、Claude Sonnet 4.6、Claude Opus 4.7、Gemini Pro/Flash、Grok 4.3）的独立评估，跨越 8 个偏见基准（约 20,600 个样本），发现所有模型都表现出左倾政治偏见，包括自称右倾的 Grok 在内容分类和政策问答中实际表现为左倾。 这项研究揭示了最先进 LLM 中存在系统性的政治偏见，引发了人们对用于内容审核、信息检索和决策支持的 AI 系统公平性和中立性的担忧。Grok 自称与实际行为之间的不一致进一步挑战了自我声明模型对齐的可靠性。 在 BBQ 种族数据集中，当正确答案涉及种族时，GPT-5.4 拒绝回答的比例为 20.3%，Claude Opus 4.7 为 13.8%，Grok 为 9.5%，Claude Sonnet 4.6 和 Gemini Pro 约为 5%。该研究未经同行评审，每个任务使用单一提示模板，且未进行多次运行取平均。

reddit · r/MachineLearning · /u/marggggggggg · 7月27日 22:37

**背景**: WinoBias（性别共指）、BBQ（社会刻板印象）和 SeeGULL（地域文化刻板印象）等偏见基准旨在衡量 AI 系统中的有害偏见。政治偏见基准如 Political Compass 和 Hyperpartisan News 评估模型的政治倾向。LLM 在大规模网络数据上训练，这些数据常包含政治不平衡，可能导致有偏见的输出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kaggle.com/datasets/thedevastator/winobias-coreference-dataset">WinoBias Coreference Dataset | Kaggle</a></li>
<li><a href="https://arxiv.org/abs/2110.08193">BBQ: A Hand-Built Bias Benchmark for Question Answering</a></li>
<li><a href="https://github.com/google-research-datasets/seegull">GitHub - google-research-datasets/seegull: SeeGULL is...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#AI bias`, `#political bias`, `#fairness`, `#benchmarking`

---

<a id="item-10"></a>
## [提出训练前数据确定性审计门控方案](https://www.reddit.com/r/MachineLearning/comments/1v8a3nu/training_data_needs_a_real_gonogo_gate_before/) ⭐️ 8.0/10

Reddit 用户提出一种训练前确定性门控机制，审计训练数据中的泄漏、矛盾、冗余、覆盖度、来源和证据完整性，输出可复现的裁决结果，如 PASS、WARNING、FAIL 或 FAIL_SECURITY。 这填补了 MLOps 中训练数据质量检查常为临时性的关键空白，通过一个正式且可复现的门控机制防止代价高昂的训练失败，提升模型可靠性。 该门控机制在即将使用的具体工件上本地运行，裁决由显式证据决定而非 LLM，确保确定性；它还能生成修复计划，并在批准的更改后重新审计。

reddit · r/MachineLearning · /u/jesusmjk · 7月27日 19:13

**背景**: 数据泄漏指训练数据无意中包含了测试集的信息，导致性能估计过于乐观。训练数据来源追踪数据集起源和处理历史，对治理和安全至关重要。机器学习流水线门控是在进入下一阶段前强制执行质量标准的检查点，但针对数据工件的标准化训练前审计门控此前一直缺失。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Leakage_(machine_learning)">Leakage (machine learning) - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/data-leakage-machine-learning">What is Data Leakage in Machine Learning? | IBM</a></li>
<li><a href="https://dev.to/aicryptosystems/training-data-provenance-the-manifest-diff-that-explains-the-hash-11bj">Training Data Provenance: The Manifest Diff That... - DEV Community</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#training data`, `#data quality`, `#MLOps`, `#pipeline gates`

---

<a id="item-11"></a>
## [长鑫科技科创板首日暴涨 471%](https://www.stcn.com/article/detail/4042119.html) ⭐️ 8.0/10

长鑫科技（688825.SH）于 7 月 27 日在上海科创板上市，开盘价 49.5 元，较发行价 8.66 元暴涨 471.59%。 此次破纪录的 IPO 彰显了中国本土存储芯片产业的快速成长及其在全球舞台上日益增长的竞争力，同时也创下了科创板募资新纪录。 公司本次 IPO 实际募资约 579 亿元，若全额行使超额配售权，总募资额可达 666 亿元，超过 2020 年中芯国际的 532 亿元纪录。

telegram · zaihuapd · 7月27日 01:29

**背景**: 长鑫科技是中国领先的动态随机存取存储器（DRAM）芯片制造商，DRAM 是计算机和服务器的关键部件。上海科创板于 2019 年启动，是中国版的纳斯达克，旨在以较宽松的上市条件支持科技创新企业。此次 IPO 凸显了中国推动半导体自主化的决心。

**标签**: `#IPO`, `#semiconductor`, `#Chinese tech`, `#memory`, `#STAR Market`

---

<a id="item-12"></a>
## [华为被指与昇维旭共建 DRAM 工厂](https://www.xda-developers.com/huawei-is-building-its-own-dram-fab-and-it-could-reshape-ram-prices-for-everyone/) ⭐️ 8.0/10

华为据报与深圳初创企业昇维旭（Swaysure）合作建设一座 12 英寸 DRAM 晶圆厂，规划月产能约 14 万片，但华为已否认相关说法。 如果建成，该工厂可为华为昇腾 AI 芯片系列保障内存供应，减少对外部供应商如长鑫存储的依赖，并可能影响全球 DRAM 价格。 据报该工厂将采用 12 英寸（300mm）晶圆，业界观察人士指出，即使尽快开工建设，量产仍需数年时间，因此短期内消费级 DRAM 价格不太可能受到影响。

telegram · zaihuapd · 7月27日 03:17

**背景**: DRAM（动态随机存取存储器）是一种易失性存储器，广泛用于电脑和服务器。华为的昇腾 AI 加速器基于达芬奇架构，需要高带宽内存用于 AI 工作负载。昇维旭（Swaysure）是一家 2022 年成立的深圳初创企业，具有国有背景，专注于存储芯片技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://insights.greyb.com/shenzhen-shengweixu-technology-patents/">Shenzhen Shengweixu Technology Patents – Insights and Stats...</a></li>
<li><a href="https://aiwiki.ai/wiki/huawei_ascend">Huawei Ascend | AI Wiki</a></li>
<li><a href="https://www.industryresearch.co/blog/top-dram-wafer-companies-12">DRAM Wafer Market Outlook 2026–2035 | Growth & Trends</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#DRAM`, `#Huawei`, `#AI chips`, `#supply chain`

---

<a id="item-13"></a>
## [中国开始量产国产 DUV 光刻机，今年目标约 5 台](https://www.theinformation.com/articles/china-starts-mass-producing-homegrown-duv-chipmaking-tools-advance-local-chip-industry) ⭐️ 8.0/10

中国已开始大规模生产自主研发的浸没式深紫外（DUV）光刻机，上海一家国企计划今年生产约 5 台，2027 年约 20 台，将交付中芯国际、华虹半导体等国内芯片制造商。 这标志着中国半导体自主化努力的重要突破，因为 DUV 光刻是先进芯片制造的关键。尽管国产设备在性能和可靠性上仍落后于 ASML，但产量的增加可能逐步侵蚀 ASML 在中国市场的份额，尤其是在西方出口限制收紧的情况下。 首批设备需要数月测试精度和兼容性才能投入量产线。部分关键部件仍来自日本，今年国内供应链延误已影响进度。

telegram · zaihuapd · 7月27日 14:10

**背景**: 深紫外（DUV）光刻是一种成熟技术，用于在硅晶圆上打印电路图案，通过多重图案化可实现低至 7nm 左右的节点。浸没式光刻在镜头和晶圆之间注入水层以提升分辨率，是 DUV 工具中最先进的类型。ASML 主导全球 DUV 市场，西方控制措施限制了对华出口尖端 DUV 系统，促使中国推动国产替代。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbeta.com.tw/articles/tech/1445926.htm">全新国产DUV光刻机曝光：“套刻 8nm”... - cnBeta.COM</a></li>
<li><a href="https://school.gugu.fund/ai/answer/duv和eu-2-1057457">DUV和EUV光刻機在晶片製造中的具體應用有何不同？ | AIGC</a></li>

</ul>
</details>

**标签**: `#半导体`, `#光刻机`, `#国产替代`, `#芯片制造`, `#技术突破`

---