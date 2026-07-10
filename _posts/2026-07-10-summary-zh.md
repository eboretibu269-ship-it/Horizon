---
layout: default
title: "Horizon Summary: 2026-07-10 (ZH)"
date: 2026-07-10
lang: zh
---

> 从 38 条内容中筛选出 11 条重要资讯。

---

1. [欧盟议会通过 Chat Control 1.0，程序性操作引发争议](#item-1) ⭐️ 9.0/10
2. [OpenAI 发布 GPT-5.6，提升效率并创 ARC-AGI-3 新纪录](#item-2) ⭐️ 9.0/10
3. [用 Rust 重写的 Postgres 通过全部回归测试](#item-3) ⭐️ 9.0/10
4. [TypeScript 7.0 发布：Go 重写带来最高 12 倍速度提升](#item-4) ⭐️ 9.0/10
5. [蚂蚁灵波开源 LingBot-Video，全球首个 MoE 具身视频基模](#item-5) ⭐️ 9.0/10
6. [美军后勤脆弱性威胁未来战争胜利](#item-6) ⭐️ 8.0/10
7. [Meta 发布 Muse Spark 1.1，开始对 Agentic AI 收费](#item-7) ⭐️ 8.0/10
8. [Meta 超级智能更新：强化学习初创公司与大规模算力](#item-8) ⭐️ 8.0/10
9. [大疆 EV50 无人机飞越珠峰 8861 米](#item-9) ⭐️ 8.0/10
10. [Meta 自研 AI 芯片 9 月投产](#item-10) ⭐️ 8.0/10
11. [OpenAI 发布国家安全原则，禁止自主武器和大规模监控](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [欧盟议会通过 Chat Control 1.0，程序性操作引发争议](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 9.0/10

欧盟议会于 2025 年 7 月 10 日通过了 Chat Control 1.0 的一年延期，允许美国科技公司在无搜查令的情况下扫描私人消息中的儿童性虐待内容，有效期至 2028 年。 该法律削弱了加密和反大规模监控的保护，影响 Instagram、Discord 和 Gmail 等平台的数十亿用户。这一有争议的议会程序（要求绝对多数才能否决）引发了对欧盟民主合法性的严重质疑。 在 607 名投票的议员中，314 票反对、276 票赞成、17 票弃权，但反对动议未达到 361 票（全体议员的绝对多数）而被否决。投票在暑假前的最后一次会议日进行，有 113 名议员缺席。

hackernews · rapnie · 7月9日 11:03 · [社区讨论](https://news.ycombinator.com/item?id=48843923)

**背景**: Chat Control 是欧盟于 2022 年 5 月首次提出的法规，旨在打击网络上的儿童性虐待内容。它要求平台主动扫描私人消息，但批评者认为这实际上终结了端到端加密。1.0 版本是一项临时措施，曾过期；尽管此前被否决，其延期仍获批。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://www.techtimes.com/articles/320010/20260709/eu-parliament-passes-chat-control-default-314-meps-couldnt-block-scanning-law.htm">EU Parliament Passes Chat Control by Default: 314 MEPs Couldn ...</a></li>

</ul>
</details>

**社区讨论**: 评论者压倒性地批评这一议会把戏，称其为“对民主的嘲弄”，并指出欧盟“正走向威权政府”。一些人强调，314 名议员反对该法律，但因程序性规则（需绝对多数才能否决）而未能成功阻止。

**标签**: `#privacy`, `#surveillance`, `#EU law`, `#democracy`, `#chat control`

---

<a id="item-2"></a>
## [OpenAI 发布 GPT-5.6，提升效率并创 ARC-AGI-3 新纪录](https://openai.com/index/gpt-5-6/) ⭐️ 9.0/10

OpenAI 发布了 GPT-5.6 系列模型，包括旗舰模型 Sol 以及 Terra 和 Luna 级别，改进了 token 效率，将上下文窗口扩展到 353k token，并在 ARC-AGI-3 基准测试上取得了 7.8%的新最高分。 此次发布标志着 AI 模型效率和推理能力的重大飞跃，能够以更少的 token 和更低的成本完成更复杂的任务，并为智能体智能基准测试树立了新标准。 GPT-5.6 系列包括三个级别：Sol（最强能力）、Terra（平衡性能与成本）和 Luna（高吞吐低延迟）。上下文窗口从 258k 扩展到 353k token，模型支持 max/ultra 推理、多智能体协作和 Programmatic Tool Calling 等新功能。

hackernews · logickkk1 · 7月9日 17:04 · [社区讨论](https://news.ycombinator.com/item?id=48849066)

**背景**: ARC-AGI-3 是一个用于评估智能体智能的交互式推理基准测试，AI 智能体必须探索新环境、推断目标并在没有明确指令的情况下规划行动。它建立在以前的 ARC-AGI 基准测试之上，专注于流体自适应效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">Arc-agi-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence</a></li>

</ul>
</details>

**社区讨论**: 社区赞扬了对 token 效率的关注，用户 joerawr 表示希望'每 token 最聪明'成为趋势。其他人注意到扩展的上下文窗口和 ARC-AGI-3 结果，而一些用户在讨论模型切换的实际好处和成本影响。

**标签**: `#OpenAI`, `#GPT`, `#AI`, `#language model`, `#benchmark`

---

<a id="item-3"></a>
## [用 Rust 重写的 Postgres 通过全部回归测试](https://github.com/malisper/pgrust) ⭐️ 9.0/10

这一实验展示了大语言模型自动化大规模软件重写的潜力，可能降低成本和实现遗留系统的现代化。同时，它也证明了 Rust 在构建健壮数据库系统方面的可行性。 这个名为 pgrust 的重写版本在不到一个月内生成了超过 7100 个提交，但审查此类 AI 生成的代码仍然颇具挑战。项目还将许可证从 PostgreSQL 许可证改为 AGPL-3.0。

hackernews · SweetSoftPillow · 7月9日 06:18 · [社区讨论](https://news.ycombinator.com/item?id=48841676)

**背景**: PostgreSQL 是一个有着 30 年历史的广泛使用的开源关系型数据库。Rust 是一种以内存安全和性能著称的系统编程语言。利用大语言模型将遗留代码库翻译成现代语言是一个新兴的研究与开发领域。

**社区讨论**: 社区讨论呈现出不同反应。作者解释了正在进行的 pgrust 改进。一些用户建议通过镜像查询来测试两个数据库，而另一些用户则质疑如何审查 AI 生成的代码。许可证从 PostgreSQL 改为 AGPL-3.0 也引起了关注，存在兼容性方面的担忧。

**标签**: `#Rust`, `#PostgreSQL`, `#LLM`, `#Database`, `#Rewrite`

---

<a id="item-4"></a>
## [TypeScript 7.0 发布：Go 重写带来最高 12 倍速度提升](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

微软正式发布 TypeScript 7.0，这是用 Go 语言重写的原生版本，完整构建速度比旧版快 8 到 12 倍，并支持共享内存多线程。 这一重大版本升级显著提升了开发者的生产力和工具性能，尤其对于大型代码库，并为在编译器基础设施中使用 Go 树立了新标杆。 用户可通过 npm 直接安装 TypeScript 7.0，主流编辑器通过 LSP 支持新语言服务器；新版本引入了 --checkers 与 --builders 参数以自定义并行度，并提供兼容包实现与 TypeScript 6 并存。

telegram · zaihuapd · 7月9日 04:01

**背景**: TypeScript 是 JavaScript 的超集，添加了静态类型，广泛用于大型 Web 应用。之前的版本由 TypeScript 自身编写，编译时存在性能瓶颈。通过用 Go（一种以快速执行和高效并发著称的语言）重写编译器，微软实现了显著的性能提升。

**标签**: `#TypeScript`, `#compiler performance`, `#Go`, `#Microsoft`, `#programming languages`

---

<a id="item-5"></a>
## [蚂蚁灵波开源 LingBot-Video，全球首个 MoE 具身视频基模](https://www.qbitai.com/2026/07/446458.html) ⭐️ 9.0/10

蚂蚁灵波开源了全球首个基于混合专家（MoE）架构的具身智能视频生成基础模型 LingBot-Video，采用 Apache 2.0 许可证。该模型总参数 30B，激活参数仅 3B，推理效率是同等规模稠密模型的 3 倍，在机器人视频评测基准 RBench 上得分为 0.620，超越了 Wan2.6、Seedance1.5 Pro 等模型。 这标志着具身智能和视频生成领域的重大突破，是首个针对机器人视频任务的开源 MoE 模型。其高效率和优异性能有望加速机器人动作预测、仿真数据生成和世界模型等方向的研究，惠及整个具身智能社区。 LingBot-Video 采用 DiT+MoE 架构实现容量与成本的平衡，并使用包含 7 万小时多样化交互数据的专属具身数据引擎。其训练引入多维强化学习奖励系统，在美学和运动一致性之外，重点关注物理合理性和任务完成度。

telegram · zaihuapd · 7月9日 04:30

**背景**: DiT（扩散变换器）是一种基于 Transformer 架构的扩散模型，广泛用于图像和视频生成。MoE（混合专家）是一种神经网络设计，每次输入仅激活部分参数，从而在规模扩大时保持高效率。具身智能（Embodied AI）聚焦于通过与物理世界交互来学习的智能体，通常涉及机器人操作。RBench 是近期提出的用于评估面向机器人的视频生成模型的基准，涵盖多种机器人形态和任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://encord.com/blog/diffusion-models-with-transformers/">Diffusion Transformer (DiT) Models: A Beginner’s Guide</a></li>
<li><a href="https://arxiv.org/abs/2601.15282">[2601.15282] Rethinking Video Generation Model for the ...RBench: New Robotics Video Generation Benchmark - YouTubeDAGroup-PKU/RBench · Datasets at Hugging FaceRBench Leaderboard - a Hugging Face Space by DAGroup-PKURethinking Robotic Video Generation - emergentmind.comGitHub - DAGroup-PKU/ReVidgen: [ICML 2026 ]Rethinking Video ...</a></li>

</ul>
</details>

**标签**: `#MoE`, `#具身智能`, `#视频生成`, `#开源`, `#机器人`

---

<a id="item-6"></a>
## [美军后勤脆弱性威胁未来战争胜利](https://mwi.westpoint.edu/the-glass-backbone-why-the-armys-logistics-will-break-in-the-next-war/) ⭐️ 8.0/10

《现代战争研究所》最近一篇文章指出，美军后勤系统脆弱，由于过度依赖准时化精确供应链，将在未来冲突中失败。 这一分析凸显了美军战备中的关键脆弱性，因为现代战争需要韧性供应链，失败可能导致作战失利。 文章批评了过时的‘牙齿与尾巴比’概念，呼吁重新调整现代化优先事项以支持后勤。历史上，陆军预算请求中对后勤的投入一直低于作战系统。

hackernews · baud147258 · 7月9日 13:24 · [社区讨论](https://news.ycombinator.com/item?id=48845442)

**背景**: 准时化物流是一种在需要时准时交付物资的供应链策略，能降低库存成本但增加对中断的脆弱性。在军事环境中，受争议的后勤承认供应链将受到攻击。‘牙齿与尾巴比’衡量作战部队（牙）与支援部队（尾）的比例，低比例常被视为高效但可能脆弱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dla.mil/About-DLA/News/News-Article-View/Article/4361608/just-enough-logistics-shifts-paradigm-in-military-supply-chain-readiness/">‘Just enough logistics’ shifts paradigm in military supply ...</a></li>
<li><a href="https://www.linkedin.com/pulse/supply-chain-fragility-why-logistics-constraints-new-boardroom-jsxxf">Supply Chain Fragility: Why Logistics Constraints Are the New ...</a></li>
<li><a href="https://www.army.mil/article/292788/army_and_industry_make_significant_strides_on_building_supply_chain_resiliency">Army and industry make significant strides on building supply ...</a></li>

</ul>
</details>

**社区讨论**: 评论者基本同意文章观点，引用从汉尼拔到二战的历史案例说明后勤决定成败。有人称 SpaceX 的 StarFall 等新技术可能缓解问题，但另一些人仍持怀疑态度。

**标签**: `#logistics`, `#military`, `#systems`, `#supply chain`, `#vulnerability`

---

<a id="item-7"></a>
## [Meta 发布 Muse Spark 1.1，开始对 Agentic AI 收费](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta 于 2026 年 7 月 9 日公开发布了 Muse Spark 1.1，这是一款面向编程的 agentic 多模态 AI 模型，并开始对 API 访问收费，价格为每百万输入 token 1.25 美元。 这标志着 Meta 进入竞争激烈的 AI 编程助手市场，以商业模型挑战 OpenAI 和 Anthropic，并表明 Meta 的策略从开源免费转向 AI 变现。 在 DeepSWE 1.1 基准测试中，Muse Spark 1.1 得分为 53.3%，落后于 GPT-5.5（67.0%）和 Claude Opus 4.8（59.0%），但其使用的 bash 工具专用测试环境设置了 6 核 CPU 和 8GB RAM 的资源上限，一些批评者认为这导致结果无效。

hackernews · ot · 7月9日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48846184)

**背景**: Agentic AI 模型是能够自主使用工具、规划并采取行动以实现目标的系统。Muse Spark 是 Meta 面向编程任务的 agentic 模型系列，1.1 版本是首个收费访问的版本，标志着 Meta 此前开源策略的转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/09/meta-enters-the-crowded-ai-coding-battle-with-muse-spark-1-1/">Meta enters the crowded AI coding battle with Muse Spark 1.1</a></li>
<li><a href="https://www.reuters.com/business/meta-debuts-muse-spark-11-with-preview-open-developers-2026-07-09/">Meta debuts Muse Spark 1.1 model with preview open to ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论对评估方法表示担忧，用户 GodelNumbering 指出资源上限违反了 Terminal-Bench 规则。开发者 simonw 分享了用于 LLM 的插件来使用 Muse Spark，而其他人则注意到定价相比竞争对手偏高，并讨论了 Meta 将编程模型商品化的策略。

**标签**: `#AI`, `#Meta`, `#Muse Spark`, `#agentic-model`, `#open-source`

---

<a id="item-8"></a>
## [Meta 超级智能更新：强化学习初创公司与大规模算力](https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence) ⭐️ 8.0/10

该通讯披露了一家新兴的强化学习环境初创公司，以及前所未有的算力扩展：采用 2000 公里以上的跨数据中心互联（scale-across），同时还为 Google DeepMind 提供了战略建议。 Scale-across 方法通过超高速光网络互连地理上分布的数据中心，克服了单一站点的电力限制。该强化学习环境初创公司（可能是 Surge 或 Mercor）专门构建用于训练 AI 代理的任务和环境。

rss · Semianalysis · 7月9日 19:16

**背景**: 训练前沿 AI 模型需要超过 100MW 的算力，这促使将工作负载分布到多个数据中心。RL 环境是 AI 代理通过试错学习的模拟世界，初创公司正在为前沿实验室提供这些环境。Meta 正在大力投资 Prometheus 和 Hyperion 等超级集群，以实现工业级算力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence">The Future of Meta Superintelligence: A 1 Year Progress Update</a></li>
<li><a href="https://techcrunch.com/2025/09/21/silicon-valley-bets-big-on-environments-to-train-ai-agents/">Silicon Valley bets big on 'environments' to train AI agents | TechCrunch</a></li>
<li><a href="https://medium.com/@aicplight888/the-evolution-of-ai-computing-power-from-scale-up-and-scale-out-to-scale-across-a3a59b3b5c5e">The Evolution of AI Computing Power: From Scale-Up and Scale-Out to Scale-Across | by AICPLIGHT | Medium</a></li>

</ul>
</details>

**标签**: `#Meta`, `#superintelligence`, `#reinforcement learning`, `#compute infrastructure`, `#AI`

---

<a id="item-9"></a>
## [大疆 EV50 无人机飞越珠峰 8861 米](https://www.163.com/dy/article/L1CUCV940514R9OJ.html) ⭐️ 8.0/10

大疆尚未发布的 EV50 垂直起降运载无人机在珠峰北坡成功飞越 8861 米，创下公开测试中垂直起降无人机的最高飞行升限世界纪录，并获取了 8000 米以上海拔的真实大气剖面数据。 这一成就展示了大疆在极端高海拔环境下的先进无人机工程技术，为在常规无人机无法到达的高度进行物流、科学研究和应急救援开辟了道路。 EV50 是一款混合固定翼垂直起降无人机，可垂直起降并在起飞后切换到固定翼巡航。在为期 12 天的任务中，它完成了 32 架次起降，累计爬升 3730 米，返程时仍剩余 30%电量。

telegram · zaihuapd · 7月9日 06:00

**背景**: 垂直起降固定翼无人机结合了多旋翼的垂直机动性和固定翼飞机的长续航能力。8000 米以上的高海拔飞行因空气稀薄、低温和强风而面临极端挑战，需要专门的动力和空气动力学设计。大疆 EV50 专为百公里级货物运输和低空物流场景而设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sina.cn/news/detail/5318723679290091.html">大疆EV50飞越珠峰|大疆|ev50|无人机|采集大气数据_新浪新闻</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/2058534660083282326">大疆EV50发布：当无人机不再只是“飞”，而是“运” - 知乎</a></li>

</ul>
</details>

**标签**: `#drone`, `#DJI`, `#high altitude`, `#logistics`, `#record`

---

<a id="item-10"></a>
## [Meta 自研 AI 芯片 9 月投产](https://www.reuters.com/world/asia-pacific/meta-put-ai-chip-into-production-september-it-looks-double-computing-capacity-2026-07-09/) ⭐️ 8.0/10

Meta 计划于 2026 年 9 月开始量产其自研 AI 芯片“Iris”，该芯片属于 MTIA 第四代项目，旨在到 2027 年将计算能力翻倍。 此举减少了 Meta 对外部供应商如英伟达和 AMD 的依赖，可能重塑 AI 硬件市场。Meta 今年高达 1450 亿美元的基础设施投资标志着其向拥有自有 AI 堆栈的战略转变。 Iris 芯片由博通协助设计、台积电制造，仅用六周完成测试且未发现重大问题。Meta 还与三星、闪迪和住友电工签订了长期供应协议，以确保内存、闪存和光纤设备的供应。

telegram · zaihuapd · 7月9日 12:37

**背景**: Meta 的 MTIA（Meta 训练与推理加速器）是专为 AI 工作负载设计的定制芯片系列。通过自研芯片，Meta 旨在针对自身需求优化性能和成本，减少对通用 AI 加速器的依赖。公司计划今年部署 7 吉瓦计算基础设施，到 2027 年翻倍至 14 吉瓦，凸显了其在 AI 领域的激进扩张。

**标签**: `#Meta`, `#AI chip`, `#hardware`, `#computing infrastructure`, `#semiconductor`

---

<a id="item-11"></a>
## [OpenAI 发布国家安全原则，禁止自主武器和大规模监控](https://openai.com/index/government-national-security-partnerships/) ⭐️ 8.0/10

OpenAI 公布了其国家安全原则，明确禁止将其 AI 技术用于自主武器、大规模监控和高风险自动化决策。该公司还宣布通过 Daybreak 网络防御计划，扩大与盟友国家的防御合作。 这标志着 AI 治理的一个重要里程碑，为国家安全领域的 AI 使用设定了明确的道德边界，并可能影响全球政策。此举有助于塑造其他 AI 公司和政府处理军事及监控应用的方式，强化负责任的创新。 原则明确禁止将 OpenAI 技术用于“开发或控制自主武器系统”和“大规模国内监控”，并支持通过立法设立安全保障措施。OpenAI 的 Daybreak 计划涉及与澳大利亚、加拿大、日本、韩国、法国、德国、波兰、荷兰及欧盟机构的合作，以加强网络防御。

telegram · zaihuapd · 7月9日 13:22

**背景**: OpenAI 的 Daybreak 计划整合了 GPT-5.5-Cyber 等前沿 AI 模型和 Codex Security 工作流，帮助防御者比攻击者更快地发现、验证和修复漏洞。这一政策转变正值 AI 在军事领域的双重用途潜力引发广泛辩论之际，此前的一些限制如今被正式化并扩展到包括盟友合作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/daybreak/">Daybreak | OpenAI for cybersecurity</a></li>
<li><a href="https://openai.com/index/daybreak-securing-the-world/">Daybreak: Tools for securing every organization in the world</a></li>

</ul>
</details>

**标签**: `#AI governance`, `#OpenAI`, `#national security`, `#autonomous weapons`, `#ethics`

---