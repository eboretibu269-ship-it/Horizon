---
layout: default
title: "Horizon Summary: 2026-07-10 (ZH)"
date: 2026-07-10
lang: zh
---

> 从 38 条内容中筛选出 13 条重要资讯。

---

1. [OpenAI 发布 GPT-5.6，在 ARC-AGI-3 上达到最优](#item-1) ⭐️ 9.0/10
2. [欧盟议会批准 Chat Control 1.0，允许无证扫描私人消息](#item-2) ⭐️ 8.0/10
3. [Mitchell Hashimoto 谈 Ghostty、Zig 与 Rust 文化](#item-3) ⭐️ 8.0/10
4. [Lisp 的持久魅力与社区辩论](#item-4) ⭐️ 8.0/10
5. [Meta 发布 Muse Spark 1.1 代理模型](#item-5) ⭐️ 8.0/10
6. [内部 TLS 证书最佳实践引发热议](#item-6) ⭐️ 8.0/10
7. [Meta 超级智能进展更新](#item-7) ⭐️ 8.0/10
8. [Meta 自研 AI 芯片'Iris'将于 9 月量产](#item-8) ⭐️ 8.0/10
9. [OpenAI 发布国家安全原则，禁止自主武器和大规模监控](#item-9) ⭐️ 8.0/10
10. [中国法院裁定游戏账号可继承，平台禁止条款无效](#item-10) ⭐️ 8.0/10
11. [Anthropic 网页抓取与导流比例达 2800:1](#item-11) ⭐️ 8.0/10
12. [长征十号乙完成全球首次网系火箭一子级海上回收](#item-12) ⭐️ 8.0/10
13. [OpenAI 和 Google 被指通过新加坡向黑名单中国公司提供 AI 服务](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-5.6，在 ARC-AGI-3 上达到最优](https://openai.com/index/gpt-5-6/) ⭐️ 9.0/10

OpenAI 发布了 GPT-5.6 系列模型，包括旗舰版 Sol、平衡版 Terra 和低成本版 Luna，在 ARC-AGI-3 基准测试中以 7.8%的得分创下新纪录。该模型还引入了改进的意图理解和原始图像细节保留功能。 此次发布标志着 AI 智能体能力的重要进步，GPT-5.6 Sol 是首个通过验证解决 ARC-AGI-3 游戏的前沿模型。改进的意图理解和图像处理能力有望提升开发者生产力，并实现更自然的人机交互。 开发者指南强调，GPT-5.6 无需显式逐步指令即可推断用户意图，但重要约束仍需明确说明。该模型保留发送图像的原始尺寸，Sol 版本使用 max/ultra 推理和多智能体协作。

hackernews · logickkk1 · 7月9日 17:04 · [社区讨论](https://news.ycombinator.com/item?id=48849066)

**背景**: ARC-AGI-3 是一个交互式推理基准，测试 AI 智能体在新颖的回合制环境中探索、推断目标和规划的能力。它在 ARC-AGI-1 和 2 的静态网格任务基础上引入了部分可观测性和多轮动态。7.8%的得分代表了显著进步，但人类表现仍接近 100%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">ARC-AGI-3: A New Challenge for Frontier Agentic IntelligenceARC-AGI-3: A New Challenge for Frontier Agentic IntelligenceARC-AGI-3 Quickstart - ARC-AGI-3 DocsARC-AGI-3: The New Interactive Reasoning Benchmark - DataCampGPT 5.6 Sol Tops ARC-AGI 3 With 7.8%, Becomes First Model To ...ARC-AGI-3: Interactive AGI Benchmark - emergentmind.com</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：有人称赞 ARC-AGI-3 的 SOTA 结果和详细的开发者指南，也有人指出 GPT-5.6 的编码性能与 GPT-5.5 相似且落后于 Sonnet 5。还有讨论关于 Fable 5 因拒答行为被排除在某些基准之外，以及 Codex 与 Claude Code 的比较。

**标签**: `#AI`, `#GPT-5.6`, `#OpenAI`, `#language models`, `#benchmark`

---

<a id="item-2"></a>
## [欧盟议会批准 Chat Control 1.0，允许无证扫描私人消息](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 8.0/10

欧洲议会批准了 Chat Control 1.0 临时法规，允许 Instagram、Discord、Gmail 等主要科技平台在没有搜查令或事先怀疑的情况下扫描私人消息以检测儿童性虐待内容。 这一决定实际上重新授权了对私人通信的大规模监控，削弱了整个欧盟的数字隐私和加密保护，并为未来的监控立法树立了令人担忧的先例。 该法规尽管遭到多数投票议员反对（314 票反对，276 票赞成），但由于否决动议未能达到所需的 361 票绝对多数，因此获得通过；该法规有效期至 2028 年 4 月 3 日。

hackernews · rapnie · 7月9日 11:03 · [社区讨论](https://news.ycombinator.com/item?id=48843923)

**背景**: Chat Control 1.0 是一项临时措施，为科技公司自愿扫描用户聊天内容以发现已知和未知的儿童性虐待材料提供法律保护。它最初在 2026 年 3 月被议会两次否决，但欧盟委员会拒绝撤回提案，迫使进入二读。批评者认为，检测未知儿童性虐待材料的技术不可靠，并会对隐私和加密构成风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://www.euronews.com/next/2026/07/10/chat-control-10-passed-the-european-parliament-through-the-back-door">Why Chat Control 1.0 is the EU's most Orwellian law yet</a></li>
<li><a href="https://www.theregister.com/security/2026/07/09/meps-fail-to-prevent-chat-control-snoopfest-revival/5269379">EU 'Chat Control' snoopfest returns after vote to kill it falls short</a></li>

</ul>
</details>

**社区讨论**: 评论者对允许该法规在多数反对下通过的议会策略表示愤慨，称其不民主。有人指出投票恰在暑假前举行，导致出席人数减少，且默认通过。另一些人注意到该法规仍允许自愿扫描，但批评其对隐私权的侵蚀。

**标签**: `#privacy`, `#surveillance`, `#EU regulation`, `#chat control`, `#encryption`

---

<a id="item-3"></a>
## [Mitchell Hashimoto 谈 Ghostty、Zig 与 Rust 文化](https://alexalejandre.com/programming/interview-with-mitchell-hashimoto/) ⭐️ 8.0/10

Ghostty 的创建者 Mitchell Hashimoto 在一次访谈中解释了为何选择用 Zig 构建终端模拟器，并阐述了他对 Rust 社区文化的批评。 此次访谈揭示了 Zig 与 Rust 在系统编程领域的持续争论，凸显了社区文化和工程务实主义如何影响语言的采用。 Hashimoto 强调 Ghostty 使用了平台原生 UI 和 GPU 加速来实现高性能，并指出分叉项目需要承担与上游变更同步的负担。

hackernews · veqq · 7月9日 17:17 · [社区讨论](https://news.ycombinator.com/item?id=48849292)

**背景**: Ghostty 是一个快速的跨平台终端模拟器，使用 GPU 加速和原生 UI。Zig 是一种系统编程语言，旨在替代 C，注重简洁性和性能。访谈对比了 Zig 与 Rust 的文化，Hashimoto 表达了对 Rust 社区态度不适。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ghostty.org/">Ghostty</a></li>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: 👻 Ghostty is a fast, feature-rich, and cross-platform terminal emulator that uses platform-native UI and GPU acceleration.</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**社区讨论**: 评论对 Hashimoto 对 Rust 文化的批评展开了辩论，有用户指出在 Rust 和 Zig 社区中都有负面体验。另一位用户赞赏务实工程思维，并表示受到访谈激励。还有评论讨论了分叉开源项目的挑战，认同同步工作的负担很大。

**标签**: `#Zig`, `#Rust`, `#terminal emulator`, `#software engineering culture`, `#open source`

---

<a id="item-4"></a>
## [Lisp 的持久魅力与社区辩论](https://scotto.me/blog/2026-07-09-why-lisp/) ⭐️ 8.0/10

一篇名为《通向 Lisp 之路：为什么是 Lisp》的反思性文章探讨了 Lisp 的独特特性（如宏）以及程序员自由与安全之间的张力，并伴随着 Hacker News 上关于其学习曲线和 AI 时代未来的高参与度讨论。 这场讨论凸显了 Lisp 作为一种优先考虑表达性和元编程的语言的持久魅力，与当前强调安全性和工具化的趋势形成对比，并提出了 AI 对编程语言演化影响的问题。 该帖本身是一篇反思性文章而非技术教程，但社区评论提到了最近的工具改进，如 Mine（完整的 Lisp 环境）和 Olive（VSCode 插件），以及影响语法高亮的网站 Bug。

hackernews · silcoon · 7月9日 13:06 · [社区讨论](https://news.ycombinator.com/item?id=48845209)

**背景**: Lisp 是最古老的编程语言之一，以其宏系统著称，该系统允许将代码作为数据进行操作（同像性），使开发者能够扩展语言语法。这种宏功能提供了极大的灵活性，但也导致了陡峭的学习曲线，如讨论中所述。评论者 davidpapermill 表达了长久以来的梦想——Lisp 会成为主流，但也怀疑 AI 是否会让这个梦想过时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lisp-journey.gitlab.io/blog/common-lisp-macros-by-example-tutorial/">Common Lisp Macros By Example Tutorial</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍表达了对 Lisp 哲学的欣赏，例如安全与权力之间的“光明面与黑暗面”张力。一些用户指出了陡峭的学习曲线和生态系统挑战，而另一些用户如 vindarel 则强调了 Lisp 工具（如 Mine、Olive）的最新改进。总体而言，这场讨论展现了一个热情但小众的社区在思考 Lisp 的未来相关性。

**标签**: `#Lisp`, `#programming languages`, `#macros`, `#software engineering`, `#AI`

---

<a id="item-5"></a>
## [Meta 发布 Muse Spark 1.1 代理模型](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta 于 2026 年 7 月 9 日发布了其首个付费代理 AI 模型 Muse Spark 1.1，通过 Meta Model API 向美国开发者提供公开预览，同时也可在 Meta AI 应用的“思考”模式中使用。 此次发布标志着 Meta 战略转向对其前沿 AI 模型收费，直接与 Anthropic 和 OpenAI 竞争，但该模型在基准测试方法上受到社区批评。 定价为每百万 token 输入/输出 1.25/4.5 美元，缓存输入 0.15 美元；Terminal-Bench 2.1 评估报告使用了仅 bash 工具的环境，限制 6 个 CPU 核心和 8GB 内存，部分社区成员认为这因资源覆盖而无效。

hackernews · ot · 7月9日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48846184)

**背景**: 代理 AI 是指能够规划、使用工具并自主行动以完成任务的系统，不同于传统聊天机器人。Muse Spark 是 Meta 超级智能实验室开发的专有大型语言模型，于 2026 年 4 月首次发布，1.1 版本引入了代理能力和付费 API。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacamp.com/blog/muse-spark-1-1">Muse Spark 1.1: Meta's Agentic Model and API | DataCamp</a></li>
<li><a href="https://www.digitalapplied.com/blog/meta-muse-spark-1-1-agentic-model-api-2026">Meta Muse Spark 1.1: Meta's First Paid Agent Model</a></li>
<li><a href="https://grokipedia.com/page/Muse_Spark_AI_model">Muse Spark (AI model)</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：部分人批评基准测试方法因资源限制而无效，其他人则称赞其有竞争力的定价和易用性。Simon Willison 创建了 LLM 插件，还有人建议 Meta 应专注于模型商品化而非正面竞争。

**标签**: `#meta`, `#ai`, `#muse-spark`, `#agentic-model`, `#benchmarking`

---

<a id="item-6"></a>
## [内部 TLS 证书最佳实践引发热议](https://tuxnet.dev/posts/tls-for-internal-services/) ⭐️ 8.0/10

一篇关于内部服务 TLS 证书的博客文章引发讨论，批评分裂视域 DNS，并倡导使用 DNS-01 验证和 ACME 协议来签发证书。 这场讨论凸显了使用 TLS 保护内部服务的复杂性和权衡，影响着组织管理证书和 DNS 基础设施的方式。 社区成员批评分裂视域 DNS 会增加复杂性和静默偏差，建议使用 Let's Encrypt 的 DNS-01 挑战，并将内部 IP 放在公共区域但通过 VPN 限制访问。

hackernews · mrl5 · 7月9日 14:57 · [社区讨论](https://news.ycombinator.com/item?id=48846995)

**背景**: 分裂视域 DNS 根据请求者的源地址提供不同的 DNS 响应，常用于保持内部服务名称的私密性。ACME（自动证书管理环境）是一种自动化证书签发和验证的协议，常用于 Let's Encrypt。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Split-horizon_DNS">Split-horizon DNS</a></li>
<li><a href="https://en.wikipedia.org/wiki/ACME_protocol">ACME protocol</a></li>
<li><a href="https://tailscale.com/learn/why-split-dns">What is Split DNS & Why Should You Use It?</a></li>

</ul>
</details>

**社区讨论**: 评论者强烈反对分裂视域 DNS，称之为“分裂脑”，并倡导基于 ACME 的 DNS 验证。还有人指出在不同编程语言中配置信任存储的困难，并建议使用公共 DNS 区域配合 VPN 限制内部 IP。

**标签**: `#TLS`, `#certificates`, `#DNS`, `#internal services`, `#security`

---

<a id="item-7"></a>
## [Meta 超级智能进展更新](https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence) ⭐️ 8.0/10

一家新的强化学习环境初创公司悄然诞生，Meta 正在执行我们前所未见的最激进的算力扩展计划，通过跨尺度网络跨越 2000 多公里。该更新还为 Google DeepMind 提供了战略建议。 这标志着 AI 基础设施投资的重大加速，可能为实现超级智能级别的模型铺平道路。给 DeepMind 的建议则凸显了领先 AI 实验室之间的竞争态势。 此次算力扩展涉及跨 2000 多公里的跨尺度网络连接集群，该技术通常用于高带宽的跨数据中心互联。这家 RL 环境初创公司据称是由 Yann LeCun 创立的 AMI Labs，专注于世界模型。

rss · Semianalysis · 7月9日 19:16

**背景**: 跨尺度网络是一种网络架构，用于连接数据中心内或跨数据中心的多个横向扩展集群，以实现高性能 AI 训练。强化学习环境是模拟环境，智能体通过交互进行学习；世界模型旨在理解物理和真实世界动态，而不仅仅是语言。Meta 的超级智能工作包括内部实验室和外部投资。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence">The Future of Meta Superintelligence: A 1 Year Progress Update</a></li>
<li><a href="https://builtin.com/artificial-intelligence/meta-superintelligence-labs">Meta Superintelligence Labs: What We Know So Far | Built In</a></li>
<li><a href="https://www.broadcom.com/topics/what-is-scale-across-networking-for-ai-clusters">Scale-across Networking | AI Clusters | AI Infrastructure</a></li>

</ul>
</details>

**标签**: `#AI`, `#superintelligence`, `#Meta`, `#compute`, `#reinforcement learning`

---

<a id="item-8"></a>
## [Meta 自研 AI 芯片'Iris'将于 9 月量产](https://www.reuters.com/world/asia-pacific/meta-put-ai-chip-into-production-september-it-looks-double-computing-capacity-2026-07-09/) ⭐️ 8.0/10

Meta 计划从今年 9 月开始量产自研 AI 芯片'Iris'，目标是到 2027 年将计算能力翻倍。该芯片属于 MTIA 四代项目，由博通协助设计、台积电制造。 此举降低了 Meta 对英伟达、AMD 等外部 GPU 供应商的依赖，标志着 AI 计算市场的战略转变。这也反映了科技巨头为 AI 工作负载构建定制硬件的趋势。 Meta 预计今年部署 7 吉瓦计算基础设施，2027 年翻倍至 14 吉瓦。公司已与三星、闪迪和住友电工签订长期供应协议，保障内存、闪存和光纤设备供应。

telegram · zaihuapd · 7月9日 12:37

**背景**: Meta 的 MTIA（Meta 训练与推理加速器）是一系列定制 AI 加速器，用于处理推荐系统和生成式 AI 任务。'Iris'芯片是最新迭代，经过仅六周的测试且未发现重大问题。Meta 今年计划在 AI 基础设施上投入高达 1450 亿美元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aichipfront.com/market-analysis/meta-self-developed-ai-chip-mtia">Meta自研AI芯片MTIA路线图深度解析：摆脱英伟达依赖的算力之战</a></li>
<li><a href="https://news.qq.com/rain/a/20240902A00ROW00">2024 Hot Chips ｜Meta 下一代MTIA：专用于推荐推理的AI处理器</a></li>
<li><a href="https://storagereview.com/zh-CN/news/meta-unveils-next-gen-meta-training-and-inference-accelerator-mtia">Meta 推出下一代元训练和推理加速器 (MTIA) - StorageReview.comTop StoriesMeta 自研 AI 推理芯片：四代路线图深度解读_腾讯新闻Meta自研AI芯片“Iris”即将投产，2027年算力目标翻倍至14GWMeta推出4款MTIA芯片，专注于高性能推理_部署_torch_带宽Meta自研AI芯片将于9月开始量产，剑指降低GPU成本</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#Meta`, `#computing infrastructure`, `#hardware`, `#semiconductor`

---

<a id="item-9"></a>
## [OpenAI 发布国家安全原则，禁止自主武器和大规模监控](https://openai.com/index/government-national-security-partnerships/) ⭐️ 8.0/10

OpenAI 公布了其国家安全原则，明确禁止将其技术用于大规模国内监控、自主武器系统和高风险自动化决策。公司还扩大了与多个美国盟友的 Daybreak 网络防御计划合作。 这标志着 AI 治理的重大政策转变，为军事和监控应用设定明确界限，同时加强与盟友的防御合作。这可能影响全球 AI 伦理标准，并塑造其他 AI 公司处理国家安全合作的方式。 这些原则禁止将 OpenAI 技术用于‘大规模国内监控’、‘自主武器系统’和‘高风险自动化决策’。Daybreak 计划现已包括与澳大利亚、加拿大、日本、韩国、法国、德国、波兰、荷兰及欧盟机构的合作。

telegram · zaihuapd · 7月9日 13:22

**背景**: 自主武器，又称致命性自主武器系统（LAWS），能够独立搜索和打击目标而无需人类干预，引发伦理担忧。OpenAI 的 Daybreak 计划是一项网络防御倡议，将 AI 整合到安全平台中以优先处理威胁并生成防御。这些发展反映了在 AI 创新与安全和伦理约束之间取得平衡的持续讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Autonomous_weapons">Autonomous weapons</a></li>
<li><a href="https://www.cybersecuritydive.com/news/OpenAI-Daybreak-cyber-threats/820122/">OpenAI launches Daybreak to combat cyber threats | Cybersecurity Dive</a></li>
<li><a href="https://www.prnewswire.com/news-releases/cato-advances-enterprise-defense-joining-the-openai-daybreak-cyber-partner-program-302805920.html">Cato Advances Enterprise Defense, Joining the OpenAI Daybreak Cyber Partner Program</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI ethics`, `#national security`, `#AI policy`, `#international relations`

---

<a id="item-10"></a>
## [中国法院裁定游戏账号可继承，平台禁止条款无效](https://www.tomshardware.com/tech-industry/big-tech/chinese-courts-allow-heirs-to-inherent-accounts-of-deceased-gamers-multiple-cases-spanning-years-establish-precedent-for-digital-ownership-of-games-in-game-items-and-microtransactions) ⭐️ 8.0/10

中国法院在多起跨年案件中裁定，游戏账号、装备道具、加密货币等虚拟资产具有财产属性，可继承，平台禁止继承的条款无效。 这一里程碑式的法律先例确认了用户的数字继承权，可能迫使全球平台修改其服务条款。 法院明确指出，聊天记录等纯个人隐私内容不可继承，由平台归档保存；平台可收取合理费用协助转移账号。

telegram · zaihuapd · 7月10日 02:56

**背景**: 数字继承是指人死后数字资产的转移。传统上，许多服务协议以隐私和安全为由禁止将账户访问权授予继承人。中国法院的这些裁决通过承认虚拟资产具有经济价值的财产属性，挑战了此类条款。

**标签**: `#digital inheritance`, `#virtual assets`, `#Chinese courts`, `#property rights`, `#gaming`

---

<a id="item-11"></a>
## [Anthropic 网页抓取与导流比例达 2800:1](https://www.businessinsider.com/anthropic-web-bots-crawling-referrals-cloudflare-distillation-2026-7) ⭐️ 8.0/10

Cloudflare 数据显示，在 7 月 1 日至 7 日期间，Anthropic 的网页抓取机器人每抓取约 2800 个网页才向原网站导流一次，该比例在主要 AI 公司中最高。 这种不平衡凸显了 AI 公司在提取网页内容用于训练的同时，仅提供极少导流量的伦理问题，可能削弱内容创作者的积极性。 该比例较 4 月初约 8800:1 有所下降，在 5 月首周一度达到 24700:1。Anthropic 质疑 Cloudflare 的统计方法，称无法验证相关计算，并表示新搜索功能正在增加网站访问量。

telegram · zaihuapd · 7月10日 04:25

**背景**: Cloudflare 利用机器学习和行为分析，追踪占全球互联网流量 20%的 AI 爬虫活动。“抓取与导流比”衡量公司机器人抓取网页次数与回传导流量的比例，是评估 AI 时代数据使用伦理的指标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.businessinsider.com/anthropic-web-bots-crawling-referrals-cloudflare-distillation-2026-7">Anthropic Treats the Web Like an All-You-Can-Eat Buffet - Business Insider</a></li>
<li><a href="https://www.businessinsider.com/anthropic-bot-crawlers-feast-on-web-give-little-back-ranking-2025-9">Anthropic Bot Crawlers Feast on the Web and Give Little Back: Ranking - Business Insider</a></li>
<li><a href="https://developers.cloudflare.com/ai-crawl-control/features/analyze-ai-traffic/">Analyze AI traffic · Cloudflare AI Crawl Control docs</a></li>

</ul>
</details>

**标签**: `#AI ethics`, `#web scraping`, `#Anthropic`, `#Cloudflare`, `#content attribution`

---

<a id="item-12"></a>
## [长征十号乙完成全球首次网系火箭一子级海上回收](https://weibo.com/7340734455/R814of1Ki) ⭐️ 8.0/10

这一里程碑展示了中国在可重复使用火箭技术方面的能力，有望降低发射成本并提高发射频率，对未来的太空任务和商业发射至关重要。 网系回收方式类似于航空母舰上的阻拦索系统，下降中的一子级被海上平台上的网系装置捕获。这与 SpaceX 猎鹰 9 号使用的着陆腿方式不同。

telegram · zaihuapd · 7月10日 04:36

**背景**: 火箭级回收旨在重复使用昂贵部件，大幅降低单次发射成本。传统回收方式采用带着陆腿的动力垂直着陆，而网系捕获提供了一种替代方案，可能降低复杂性。长征十号乙是中国航天工业正在开发的部分可重复使用运载火箭。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.news.cn/20260710/ba0ac14f31dd492aaf918e7a86ac844a/c.html">长征十号乙首飞成功 我国运载火箭首次实现可控回收-新华网</a></li>
<li><a href="https://h5.ifeng.com/c/vivoArticle/v0026U0p1yEaP670syi0cuThLxSHZRUClOnfql0NufHtc7Y__?isNews=1&showComments=0">长征十号乙月底发射，再次验证海上网系回收</a></li>

</ul>
</details>

**标签**: `#aerospace`, `#rocket recovery`, `#space technology`, `#China`

---

<a id="item-13"></a>
## [OpenAI 和 Google 被指通过新加坡向黑名单中国公司提供 AI 服务](https://www.ft.com/content/5d6aafa1-5d47-4585-aa95-6ec06a6cd20f) ⭐️ 8.0/10

OpenAI 和 Google 被指通过新加坡子公司向阿里巴巴、百度和腾讯提供先进 AI 服务，尽管这些中国母公司在五角大楼的 1260H 名单上。 这重新引发了美国对 AI 软件实施更严格出口管制的呼声，因为现行法规并未广泛限制中国公司在海外获取先进 AI 模型。该问题凸显了 AI 技术国家安全监管的漏洞。 OpenAI 上月在发现疑似模型蒸馏行为后，暂停了阿里巴巴关联用户的 API 访问权限并上报美国政府。相比之下，Anthropic 执行更严格的政策，全面禁止中国公司及其海外实体访问其前沿 AI 模型。

telegram · zaihuapd · 7月10日 09:59

**背景**: 1260H 名单是美国国防部列出的涉嫌与中国军方有关联的实体名单。模型蒸馏是一种将大型 AI 模型的知识转移到小型模型的技术，可用于复制能力。美国目前对 AI 软件的出口管制主要针对从美国进行的物理出口，而未涵盖外国子公司提供的服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1260H_list">1260H list</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_distillation">Model distillation</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#export controls`, `#OpenAI`, `#Google`, `#China`

---