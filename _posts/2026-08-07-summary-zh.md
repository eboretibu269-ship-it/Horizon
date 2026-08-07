---
layout: default
title: "Horizon Summary: 2026-08-07 (ZH)"
date: 2026-08-07
lang: zh
---

> 从 28 条内容中筛选出 13 条重要资讯。

---

1. [DeepSeek V4 Flash 0731 在 ARC-AGI 上表现强劲且速度快](#item-1) ⭐️ 9.0/10
2. [OpenAI 称 Astra 模型或达「关键」网络攻击能力，或致发布推迟](#item-2) ⭐️ 9.0/10
3. [甲骨文禁止向 OpenJDK 贡献 AI 生成代码](#item-3) ⭐️ 8.0/10
4. [用 Rust 查询引擎让 Postgres 分析性能提升 300 倍](#item-4) ⭐️ 8.0/10
5. [AI 与 HBM 需求推动 2027 年内存产能售罄](#item-5) ⭐️ 8.0/10
6. [150 万页网站对抗爬虫的一年](#item-6) ⭐️ 8.0/10
7. [新墨西哥州法院判 Meta 赔偿 5.67 亿美元 涉儿童心理健康伤害](#item-7) ⭐️ 8.0/10
8. [Show HN：Wyzer 语言欲防分布式死锁与内存错误](#item-8) ⭐️ 8.0/10
9. [Token 末日来临：企业纷纷设法削减 AI Token 开销](#item-9) ⭐️ 8.0/10
10. [SemiAnalysis：SpaceX 2027 年实现 10GW 空间太阳能或带来 3000 亿美元年收入](#item-10) ⭐️ 8.0/10
11. [Gemini 长期困境，Google Cloud 短期获益](#item-11) ⭐️ 8.0/10
12. [美国调查中国 AI 企业海外获取英伟达芯片渠道](#item-12) ⭐️ 8.0/10
13. [SK 海力士确认 V10 NAND 为 375 层堆叠，采用晶圆键合技术](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DeepSeek V4 Flash 0731 在 ARC-AGI 上表现强劲且速度快](https://arcprize.org/results/deepseek-v4-flash-0731) ⭐️ 9.0/10

DeepSeek 发布了 V4 Flash 0731，这是 V4 Flash 模型的更新版本，在 ARC-AGI 基准测试上展现出强大的性能和速度。该版本因其高性价比和本地运行能力而引发社区广泛关注。 此次发布意义重大，因为它表明一家重要的开源模型开发商以远低于前沿系统的成本提供了具有竞争力的推理性能，使先进 AI 更加普及。同时，它也凸显了 ARC-AGI 这类基准在评估真实世界智能体能力方面日益重要的地位。 0731 版本相比早期 V4 Flash 预览版是一次重大更新，用户反馈质量明显跃升。在本地双 RTX Pro 6000 Blackwell GPU 上，用户观察到预填充速度约 8k tok/s，单流生成速度约 250 tok/s，但部分用户也报告了工具调用时出现死循环和令牌浪费等回归问题。

hackernews · tosh · 8月7日 17:56 · [社区讨论](https://news.ycombinator.com/item?id=49214008)

**背景**: ARC-AGI（面向通用人工智能的抽象与推理语料库）是一种通过新颖的人类式推理任务来衡量通用智能进展的基准测试。运营该基准的 ARC Prize 基金会还推出了 ARC-AGI-3，这是一个交互式基准，用于在全新环境中测试智能体智能。DeepSeek V4 Flash 在该基准上的结果表明，开源权重模型正在推理密集型任务上缩小与前沿系统的差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi">ARC Prize - What is ARC-AGI?</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极，用户称赞该模型的高性价比（每天多会话运行成本低于 5 美元）以及在本地硬件上的速度。但部分用户报告与上一版本相比出现回归，包括模型在不执行工具调用的情况下自言自语、陷入死循环并浪费令牌的问题。

**标签**: `#AI`, `#DeepSeek`, `#LLM`, `#ARC-AGI`, `#Machine Learning`

---

<a id="item-2"></a>
## [OpenAI 称 Astra 模型或达「关键」网络攻击能力，或致发布推迟](https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/) ⭐️ 9.0/10

2026 年 8 月 7 日，OpenAI 披露其即将推出的 Astra 模型在内部评估中显示出代理编码和网络安全方面的重大进展，初步结果强到无法排除达到「关键」网络能力阈值的可能性。此前 GPT-5.6-Sol 等模型在同一评估中仅被评为「高」。 这标志着前沿 AI 模型可能具备在无需人工干预的情况下自主发现和利用加固真实系统中零日漏洞的能力，从而大幅降低复杂网络攻击的门槛。扩大安全测试并可能推迟发布，为 AI 实验室如何应对关键风险模型树立了重要先例，影响整个 AI 与网络安全领域。 OpenAI 已暂停不符合强化安全要求的 Astra 相关内部活动，并实施了隔离测试环境、加密增强和通用监控等措施。据报道，公司还将与政府机构和 AI 安全组织合作开展第三方测试。

telegram · zaihuapd · 8月7日 16:44

**背景**: OpenAI 的预备框架（Preparedness Framework）是其跟踪和防范前沿 AI 能力可能带来灾难性风险的结构化流程，网络安全是其核心追踪类别之一。根据该框架，达到「关键」阈值意味着模型能够自主发现并利用加固真实系统中的零日漏洞，或仅凭高层目标规划和执行端到端的新型网络攻击。代理编码（agentic coding）是指自主 AI 代理在极少人工干预下规划、编写、测试和修改代码的能力，这与进攻性网络操作直接相关。近期真实案例，例如 Google 披露的用 AI 开发的绕过双因素认证的零日漏洞，也说明为何这类阈值会得到认真对待。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/updating-our-preparedness-framework/">Our updated Preparedness Framework | OpenAI</a></li>
<li><a href="https://cdn.openai.com/pdf/18a02b5d-6b67-4cec-ab64-68cdfbddebcd/preparedness-framework-v2.pdf">Preparedness Framework Version 2. Last updated: 15th April, 2025</a></li>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/ai-vulnerability-exploitation-initial-access">Adversaries Leverage AI for Vulnerability Exploitation, Augmented Operations, and Initial Access | Google Cloud Blog</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#cybersecurity`, `#OpenAI`, `#frontier AI`, `#model release`

---

<a id="item-3"></a>
## [甲骨文禁止向 OpenJDK 贡献 AI 生成代码](https://app.dealroom.co/news/feed/oracle-bans-ai-generated-code-from-openjdk-despite-ellison-s-claim-oracle-isn-t-writing-its-own-code) ⭐️ 8.0/10

甲骨文发布了一项临时政策，禁止向 OpenJDK 贡献由生成式 AI 工具生成的代码。该政策发布在 openjdk.org/legal/ai，将在甲骨文法务团队制定最终版本之前持续有效。 OpenJDK 是 Java 的参考实现，支撑着庞大的企业生态系统，因此该政策可能影响其他开源项目如何应对 AI 生成代码。它凸显了 AI 辅助开发给软件供应链带来的日益增长的法律和来源风险。 临时政策发布在 openjdk.org/legal/ai 上，甲骨文的律师正在起草最终版本。其理由包括规避代码来源方面的法律责任，以及避免给本已有限的人工审阅者时间增加过多负担。

hackernews · delduca · 8月7日 17:36 · [社区讨论](https://news.ycombinator.com/item?id=49213754)

**背景**: 代码来源（code provenance）指代码来源的可验证、可审计历史，包括谁编写以及如何修改。在生成式 AI 出现后，来源变得更加模糊，因为 AI 输出可能源自受版权或许可保护的代码，带来法律不确定性。OpenJDK 是一个重要的开源项目，甲骨文的举措反映了业界对 AI 生成代码、许可和软件供应链透明度的广泛担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fortegrp.com/insights/understanding-code-provenance">Understanding Code Provenance in The Age of Generative AI</a></li>
<li><a href="https://www.gitclear.com/help/technical/code_provenance">What is "code provenance" and why does it matter? - GitClear</a></li>
<li><a href="https://jfrog.com/learn/grc/software-provenance/">What Is Software Provenance? | Secure Supply Chain Practices | JFrog</a></li>

</ul>
</details>

**社区讨论**: 对该新闻的评论意见不一。一些人认为，鉴于 Java 历史上的版权纠纷，这一政策是明智的风险管理决策；另一些人则质疑甲骨文作为 AI 领域的重要玩家，能否始终如一地执行该政策。几位评论者指出，甲骨文一边大力投入 AI 一边禁止 AI 代码具有讽刺意味，并强调核心问题是来源与法律责任，而非拒绝 AI 工具本身。

**标签**: `#OpenJDK`, `#AI-generated code`, `#Oracle`, `#open source`, `#legal policy`

---

<a id="item-4"></a>
## [用 Rust 查询引擎让 Postgres 分析性能提升 300 倍](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/) ⭐️ 8.0/10

这篇文章详细介绍了基于 Rust 的查询引擎 pgrust 如何通过批处理、算子融合和 SIMD 使 Postgres 分析查询速度提升数百倍（最高 300 倍）。作者还表示，已通过形式化验证和差分模糊测试覆盖超过 1000 个用户可见函数，以确保与 Postgres 的逻辑一致性。 这项工作展示了一条在不改变 SQL 语义的前提下大幅提升 Postgres 分析型负载性能的可信路径，可能对分析型数据库市场产生影响。它还证明了自适应规划以及基于 Rust 的重新实现方案在 Postgres 生态系统中的可行性。 这些优化重点在于减少 CPU 和内存带宽占用，采用每次操作 1024 行以上的向量化批处理、避免中间结果物化的算子融合以及 SIMD 指令。主文章还包含正确性证明目录和差分模糊测试，并且该引擎被设计为 Postgres 查询执行器的可直接替代品。

hackernews · poly2it · 8月7日 11:00 · [社区讨论](https://news.ycombinator.com/item?id=49208535)

**背景**: 传统 Postgres 采用火山模型逐行执行查询，这对分析型负载效率低下。向量化执行以列式批量处理数据，摊薄了解释器开销并启用 SIMD 指令。算子融合将多个查询算子合并以减少数据物化，DuckDB 和 ClickHouse 等现代引擎也采用类似技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/">Rebuilding Postgres for 300x faster analytics: batching, operator...</a></li>
<li><a href="https://clickhouse.com/resources/engineering/vectorized-query-execution">What is vectorized query execution? - clickhouse.com</a></li>
<li><a href="https://arxiv.org/pdf/1610.09166">Push vs. Pull-Based Loop Fusion in Query Engines</a></li>

</ul>
</details>

**社区讨论**: 作者（malisper）强调正确性是第一优先级，并谈及形式化验证和差分模糊测试。评论者 sgt 反驳说，对官方 Postgres 团队的信任比性能更重要，因此 pgrust 的采用可能受限。其他评论者对自适应规划的前景以及将 pgrust 嵌入为 SQLite/Turso 替代方案表示赞赏。

**标签**: `#postgres`, `#rust`, `#query-engine`, `#performance`, `#simd`

---

<a id="item-5"></a>
## [AI 与 HBM 需求推动 2027 年内存产能售罄](https://www.ign.com/articles/ramageddon-continues-another-year-as-2027-memory-capacity-is-reportedly-sold-out) ⭐️ 8.0/10

据报道，2027 年的内存产能已被订满，原因是 HBM（高带宽内存）生产占用了越来越多晶圆产能，而 AI 需求加剧了供应短缺。 这意味着内存短缺将持续下去，推高 DDR5 及其他 DRAM 产品的价格，影响消费者、PC 组装者和数据中心。同时也凸显出 AI 基础设施需求正在重塑整个半导体供应链。 HBM 与 DDR5 的晶圆产能换算关系约为 3 比 1：在相同技术节点下，生产同等位数 HBM3E 所需晶圆供应约为 DDR5 的三倍。因此，HBM 扩产直接限制了非 HBM 内存产品的供应增长。

hackernews · inigyou · 8月7日 07:58 · [社区讨论](https://news.ycombinator.com/item?id=49207236)

**背景**: HBM 是一种 3D 堆叠 DRAM 架构，专为高带宽、低功耗运行而设计，广泛应用于 AI 加速器和高性能计算。随着 AI 需求激增，内存厂商优先生产利润率较高但占用晶圆面积更大的 HBM，从而挤压了通用 DDR5 内存的产能，并推动价格上涨。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.micron.com/products/memory/hbm">High-bandwidth memory (HBM) | Micron Technology Inc.</a></li>
<li><a href="https://www.rambus.com/blogs/hbm3-everything-you-need-to-know/">High Bandwidth Memory (HBM): Everything You Need to Know - Rambus</a></li>

</ul>
</details>

**社区讨论**: 评论者对 HBM 挤占 DDR5 晶圆产能表示担忧，并提到 3 比 1 的产能换算关系，认为消费设备将面临更大涨价压力。还有人希望出现类似 USB 的标准化可升级内存接口，也有人表示内存紧张使他们对采用 AI 持观望态度。

**标签**: `#memory`, `#HBM`, `#AI`, `#supply chain`, `#semiconductors`

---

<a id="item-6"></a>
## [150 万页网站对抗爬虫的一年](https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/) ⭐️ 8.0/10

一位站长发布了一篇详细文章，讲述了他与占网站流量 99%的爬虫机器人进行的一年斗争，其中一个月成本飙升了约 500%。他分享了反爬虫的经验教训，而评论者们则讨论了使用 Cloudflare 的利弊以及类似工作量证明等替代方案。 这对网站运营者来说是一个高度相关的实战案例，凸显了机器人流量如何悄然推高成本并迫使人们做出艰难取舍。社区讨论提出了关于将访问决策外包给 Cloudflare 的质疑，以及激进的反爬策略是否会损害开放互联网的重要问题。 站长提到他平时每月 90 美元的账单在流量高峰期上涨了约 500%，并承认自己的网站也抓取公开文档，“一个爬虫写博客抱怨爬虫”。在评论中，其他人分享说 Claude-searchbot 在 72 小时内抓取了约 20.5 万个页面，而工作量证明工具 Anubis 能有效拦截伪造用户代理的机器人。

hackernews · petercooper · 8月7日 14:51 · [社区讨论](https://news.ycombinator.com/item?id=49211386)

**背景**: 爬虫是自动化的程序，系统性地爬取并提取网站数据，即使不是恶意的，也可能压垮网站资源。许多站长转而使用 Cloudflare 等服务来过滤机器人流量，但这意味着该企业实际上决定了谁能访问网站。工作量证明是一种替代性的反爬技术，要求客户端完成一个小的计算难题以证明自己是真实浏览器，而不是廉价的自动化爬虫。当前的对抗也因 AI 公司而加剧，它们的爬虫（如 Claude-searchbot）为训练或检索而抓取海量页面。

**社区讨论**: 评论者普遍表示同情，但对解决方案存在分歧：一些人担心默认使用 Cloudflare 会把网站访问权外包给一家公司，而另一些人则推荐 Anubis 的工作量证明工具，或者干脆放弃 D1 改用静态网站。一位评论者分享，Claude-searchbot 在 72 小时内抓取了约 20.5 万个页面，但只带来 1 次推荐，感觉被 AI 爬虫“欺骗”了。站长对自己也是爬虫的自嘲式承认引来了会意的认同。

**标签**: `#web scraping`, `#bot detection`, `#cloudflare`, `#cost optimization`, `#site reliability`

---

<a id="item-7"></a>
## [新墨西哥州法院判 Meta 赔偿 5.67 亿美元 涉儿童心理健康伤害](https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta) ⭐️ 8.0/10

2026 年 8 月 6 日，新墨西哥州一家法院裁定 Meta 支付 5.67 亿美元（另有报道称 9.42 亿美元），用于青少年心理健康项目，并要求其为未成年用户做出改变。该裁决源于一项诉讼，指控 Meta 的社交媒体平台对儿童心理健康造成伤害。 这是一项具有里程碑意义的法律裁决，依据公共妨害法认定大型社交媒体公司对未成年人算法伤害负有责任，可能促使其他州提起类似诉讼。按新墨西哥州人口计算，这笔罚金的规模相当可观，即便相对于 Meta 的全球收入而言并不算大。 法院认定 Meta 违反了新墨西哥州公共妨害法（NMSA 1978 § 30-8-1），该法针对损害公共卫生、安全、道德或福利的行为。不同媒体对赔偿金额的报道不一致——5.67 亿美元与 9.42 亿美元——可能反映了不同的损失计算方式或报道误差。新墨西哥州人口仅略超 200 万，因此人均判赔金额非常高。

hackernews · boplicity · 8月7日 00:06 · [社区讨论](https://news.ycombinator.com/item?id=49204352)

**背景**: Meta 是 Facebook、Instagram 和 WhatsApp 的母公司。在美国，许多州政府和学区已对社交媒体公司提起诉讼，称无限滚动和个性化推荐等算法功能损害青少年的心理健康。公共妨害法为州政府提供了法律依据，以制止影响公众健康、安全或福祉的行为。此案是科技公司因青少年心理健康、成瘾性设计和平台责任而面临更广泛监管与法律压力的部分体现。

**社区讨论**: 评论者讨论这笔罚金是否只是‘不痛不痒’的处罚——就全球范围而言——但对新墨西哥州这样的小州来说却非常巨大，有人指出该金额超过了按收入比例推算的预期。还有人分享了 Instagram Reels 和 TikTok 让人感觉像上瘾物质的亲身经历，批评评论区充满‘脑腐’式重复言论；也有人讨论这可能对 Meta 股价和算法设计产生的影响。

**标签**: `#legal`, `#social-media`, `#mental-health`, `#regulation`, `#Meta`

---

<a id="item-8"></a>
## [Show HN：Wyzer 语言欲防分布式死锁与内存错误](https://github.com/Wyzer-Lang/wyzer) ⭐️ 8.0/10

一位开发者推出了 Wyzer——一种新的静态类型、编译型、面向资源的编程语言，将编排编程与 Perceus 内存模型相结合；0.1.0 版本即将发布。 它将编译期安全从内存管理扩展到分布式协调，直接处理 Rust 未覆盖的分布式死锁和跨服务协议不匹配问题。如果成功，它可能为多服务系统的正确性保障提供新方向。 Wyzer 使用线性/仿射类型和 Perceus 引用计数，而不是 Rust 的借用检查器和生命周期，作者表示这对 LSP 等工具的静态分析更简单。该项目仍处于早期阶段，作者在约五个月研究和几周开发后即将发布 0.1.0。

hackernews · v0id_isgood · 8月7日 12:28 · [社区讨论](https://news.ycombinator.com/item?id=49209385)

**背景**: 编排编程是一种面向分布式系统的编程范式，程序以多个参与者间的单一交互写成；由于每次发送都对应一次接收，从而保证无死锁。Perceus 是一种带重用的精确引用计数算法，用于 Koka 等语言，可无需垃圾回收器直接编译。资源导向计算则把计算视为程序通过执行上下文管理资源，这与 Wyzer 的设计密切相关。Wyzer 借鉴学术研究，将这些理念推广为一种实用的高级语言。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Choreographic_programming">Choreographic programming</a></li>
<li><a href="https://www.microsoft.com/en-us/research/publication/perceus-garbage-free-reference-counting-with-reuse/">Perceus: Garbage Free Reference Counting with... - Microsoft Research</a></li>
<li><a href="https://en.wikipedia.org/wiki/Resource-oriented_computing">Resource-oriented computing - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞其雄心和 README 结构清晰，但认为真正新颖的想法难以找到，需要更多示例。也有人质疑在具体编排中如何保证无死锁，例如如何拒绝跨参与者的循环等待。

**标签**: `#programming-languages`, `#distributed-systems`, `#memory-safety`, `#choreographic-programming`, `#rust`

---

<a id="item-9"></a>
## [Token 末日来临：企业纷纷设法削减 AI Token 开销](https://simonwillison.net/2026/Aug/7/pdfs-are-terrible/#atom-everything) ⭐️ 8.0/10

404 Media 于 6 月 24 日的报道依据泄露的埃森哲（Accenture）会议音频指出，消耗 token 的主要是非工程师，而将 PDF 转成图片再转成 markdown 是最耗 token 的操作之一。Simon Willison 转发了这一事件，并补充说 PDF 是一种糟糕的信息传递媒介。 这件事很重要，因为 AI token 成本正在成为企业的主要运营负担，而一些隐蔽、不易察觉的工作流会悄悄推高账单。它表明，成本优化——而不只是模型能力——已成为实际部署 LLM 的核心问题。 Token 消耗是每次 API 调用中输入和输出 token 的总和；PDF 之所以昂贵，是因为内容可能被转换成图片、markdown 等中间格式，从而使 token 数量成倍增加。从业者表示，将文件转换为干净的 markdown 可在不损失内容质量的情况下减少 65%–90% 的 token 用量。

rss · Simon Willison · 8月7日 16:18

**背景**: LLM API 按 token 计费，token 通常是小于一整个词的文本块，因此工作流消耗的 token 越多，成本就越高。PDF 以“吃 token”著称，因为其排版、图片和格式往往需要多模态或冗长的文本转换，而纯 markdown 则高效得多。该事件还涉及 agentic AI——一种能够感知、推理并自主行动的系统——它随着这类智能体在企业中自动化更多任务，可能使 token 支出成倍增加。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mindstudio.ai/blog/convert-files-markdown-reduce-ai-tokens">How to Convert Files to Markdown to Reduce AI Token Usage by Up to 90% | MindStudio</a></li>
<li><a href="https://iternal.ai/token-usage-guide">Token Usage Guide 2026: How Many Tokens AI Really Uses</a></li>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained | MIT Sloan</a></li>

</ul>
</details>

**标签**: `#AI`, `#Token Costs`, `#Enterprise AI`, `#LLM`, `#Cost Optimization`

---

<a id="item-10"></a>
## [SemiAnalysis：SpaceX 2027 年实现 10GW 空间太阳能或带来 3000 亿美元年收入](https://newsletter.semianalysis.com/p/spacex-10gw-in-2027-why-its-real) ⭐️ 8.0/10

SemiAnalysis 发布深度分析，认为 SpaceX 在 2027 年前向地球传输 10GW 空间太阳能的目标是现实的，并可能带来 3000 亿美元的年经常性收入（ARR）。报告还称，微软将成为这一轨道电力的最大承购方，推动 Azure 实现三位数增长。 如果实现，这将从根本上重塑 AI 基础设施、能源供应和云计算经济，使大规模 AI 计算摆脱地面电网限制。微软作为锚定买家的潜在角色，将为 SpaceX 提供可信的收入路径，同时帮助 Azure 突破电力瓶颈。 该分析假设推理工作负载每吉瓦每年可处理约 1000 亿个 token，并提到微软“2026 年 10GW 觉醒”作为需求催化剂。然而，2027 年的时间表是前瞻性的、未经证实的；目前的空间太阳能示范（如加州理工学院的 MAPLE）仅向地球传输了微瓦级功率。

rss · Semianalysis · 8月7日 20:08

**背景**: 空间太阳能（SBSP）是指在轨道上收集太阳能——那里阳光不受大气衰减——并以微波或激光形式传输到地球。承购协议（offtake agreement）是一种长期合同，买方承诺购买项目未来的产出，常用于为大型基础设施项目融资。随着 AI 对电力需求快速增长，轨道 AI 数据中心和空间太阳能的提议近期受到关注，但在吉瓦级空间电力可行之前，仍存在重大技术和经济障碍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Space-based_solar_power">Space-based solar power</a></li>
<li><a href="https://en.wikipedia.org/wiki/Offtake_agreement">Offtake agreement</a></li>
<li><a href="https://www.cnbc.com/2026/06/21/do-space-based-ai-data-centers-make-economic-sense.html">Do space-based AI data centers make economic sense?</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#AI infrastructure`, `#Microsoft`, `#energy`, `#data centers`

---

<a id="item-11"></a>
## [Gemini 长期困境，Google Cloud 短期获益](https://newsletter.semianalysis.com/p/gemini-is-cooked-but-gcp-is-cooking) ⭐️ 8.0/10

SemiAnalysis 发布分析文章，指出 DeepMind 在 Gemini 上的长期困境反而可能在短期内为 Google Cloud 带来机遇。文章将 Gemini 的挫折重新解读为 GCP 的潜在收入驱动力。 该分析提供了对 Alphabet 内部战略动态的细致观察，影响 AI 基础设施与云计算竞争格局。云客户、投资者和 AI 开发者可能需要调整对谷歌 AI 发展路线的预期。 文章可能指出，无论 Gemini 长期成败如何，DeepMind 对算力的巨大消耗都会为 Google Cloud 带来收入。短期内，GCP 可能因内部资源重新调配或吸引对 DeepMind 方向不满的客户而获益。

rss · Semianalysis · 8月7日 02:32

**背景**: DeepMind 是 Alphabet 旗下的 AI 研究部门，负责构建与 OpenAI 的 GPT 竞争的 Gemini 大语言模型。Google Cloud Platform（GCP）向外部客户销售包括 TPU 和 GPU 在内的云基础设施。两者存在复杂的内部关系：DeepMind 消耗 GCP 资源，但如果其模型表现不佳，GCP 可能通过重新分配容量或为寻求替代方案的外部客户提供服务而获益。

**标签**: `#AI`, `#Google Cloud`, `#DeepMind`, `#Gemini`, `#Cloud Computing`

---

<a id="item-12"></a>
## [美国调查中国 AI 企业海外获取英伟达芯片渠道](https://www.bloomberg.com/news/articles/2026-08-07/us-reviews-china-s-offshore-access-to-nvidia-chips-after-ai-breakthroughs) ⭐️ 8.0/10

美国商务部工业与安全局（BIS）正系统审查中国 AI 企业如何在海外获取和使用英伟达芯片，包括远程租用算力和壳公司安排。此前月之暗面发布 Kimi K3 模型，白宫官员指控其通过泰国远程访问非法获取英伟达芯片。 此次调查可能重塑全球 AI 格局，检验美国出口管制能否覆盖海外云端算力访问。这将影响月之暗面、阿里巴巴等中国 AI 企业，以及反对扩大管制的英伟达等美国科技公司。 BIS 正在整理两份国家名单：涉嫌走私受限芯片进入中国的黑市所在地，以及中国企业远程租用芯片的国家。由于远程访问本身并不违法，美国众议院已通过两党法案拟明确授权 BIS 监管，但预计会遭到英伟达等公司反对。报道还称，阿里巴巴通过开曼实体控制的新加坡壳公司，经 Megaspeed 使用位于马来西亚的英伟达芯片。

telegram · zaihuapd · 8月7日 11:18

**背景**: 自 2022 年以来，美国限制英伟达先进芯片对华出口，但中国企业通过海外云服务租用算力等方式绕开限制。Kimi K3 是月之暗面发布的开源权重模型，拥有 2.8 万亿参数和 100 万 token 上下文窗口，其性能接近美国同行，加剧了美方对出口管制有效性的担忧。BIS 此次审查意在堵住这些海外安排可能存在的漏洞，尽管目前这些行为可能尚未违反法律条文。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(AI)">Kimi (AI) - Wikipedia</a></li>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3">moonshotai/Kimi-K3 · Hugging Face</a></li>
<li><a href="https://www.msn.com/en-us/money/general/bis-targets-legal-cloud-compute-as-china-ai-firms-bypass-export-controls/ar-AA29Cltq">BIS targets legal cloud compute as China AI firms bypass export...</a></li>

</ul>
</details>

**标签**: `#AI`, `#semiconductors`, `#export controls`, `#US-China tech`, `#Nvidia`

---

<a id="item-13"></a>
## [SK 海力士确认 V10 NAND 为 375 层堆叠，采用晶圆键合技术](https://www.gelonghui.com/live/2599953) ⭐️ 8.0/10

SK 海力士在 FMS 2026 上确认，其下一代 V10 NAND 闪存采用 375 层堆叠，并首次在其 NAND 产品中使用晶圆键合技术。该公司宣称 V10 的每瓦性能是上一代 V9 的 2.5 倍。 这标志着 3D NAND 层数提升和功耗效率方面的重要里程碑，对存储能效要求日益严苛的人工智能数据中心尤为有利。同时表明 SK 海力士正在追赶铠侠和长江存储等竞争对手，这些厂商已在 NAND 量产中采用晶圆键合技术。 V10 是 321 层 V9“4D NAND”的后续产品，也是 SK 海力士首款采用晶圆键合技术的 NAND 产品。其 2.5 倍的每瓦性能提升专为需要兼顾高能效与高性能的 AI 基础设施环境而优化。

telegram · zaihuapd · 8月7日 12:19

**背景**: NAND 闪存是一种非易失性存储，常用于固态硬盘。为了提升容量和降低成本，厂商将存储单元垂直堆叠成 3D NAND，层数大致决定密度。晶圆键合是另一种制造方式：将 CMOS 逻辑晶圆和存储阵列晶圆分开制造后再键合，从而提升密度和性能。铠侠的 CBA 和长江存储的 Xtacking 就是已量产的晶圆键合 NAND 技术，SK 海力士也在 V10 中采用了类似工艺。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.digitimes.com/news/a20250714PD212/kioxia-ymtc-nand-cmos-wafer.html">Kioxia, YMTC jump ahead with wafer-bonded NAND in volume production</a></li>
<li><a href="https://www.eetimes.com/high-density-3d-flash-memory-using-high-precision-wafer-bonding-brings-new-value-to-storage/">KIOXIA: Features of BiCS FLASH 3D Flash Memory - EE Times</a></li>

</ul>
</details>

**标签**: `#NAND`, `#SK Hynix`, `#semiconductor`, `#wafer bonding`, `#AI storage`

---