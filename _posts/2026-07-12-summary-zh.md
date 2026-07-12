---
layout: default
title: "Horizon Summary: 2026-07-12 (ZH)"
date: 2026-07-12
lang: zh
---

> 从 30 条内容中筛选出 9 条重要资讯。

---

1. [vLLM v0.25.0：Model Runner V2 成为默认，PagedAttention 被移除](#item-1) ⭐️ 9.0/10
2. [GPT-5.6 一小时内证明 50 年图论猜想](#item-2) ⭐️ 9.0/10
3. [英伟达、CoreWeave 与 Nebius：GPU 繁荣中的循环融资内幕](#item-3) ⭐️ 8.0/10
4. [ClickHouse 将 PgBouncer 吞吐量提升四倍](#item-4) ⭐️ 8.0/10
5. [SQLite：建议使用严格表以确保类型安全](#item-5) ⭐️ 8.0/10
6. [U-Boot 六个漏洞可在操作系统启动前执行代码](#item-6) ⭐️ 8.0/10
7. [智谱创始人宣布‘摸高计划’追求 AGI](#item-7) ⭐️ 8.0/10
8. [xAI Grok CLI 默认上传整个代码库及密钥文件](#item-8) ⭐️ 8.0/10
9. [欧盟拟对失职保护消费者的大型科技公司罚款](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0：Model Runner V2 成为默认，PagedAttention 被移除](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 将 Model Runner V2 设为所有密集模型的默认执行路径，移除了旧的 PagedAttention 实现，并使 Transformers 建模后端的性能与原生 vLLM 持平。 此版本标志着 vLLM 的一个重要架构里程碑，简化了代码库并提高了可维护性，同时提供了与原生命内核相匹配的性能，使开发者更容易部署和定制 LLM 服务。 Model Runner V2 现在支持 EVS、实时嵌入、Mamba 混合模型的前缀缓存以及带有完整 CUDA 图的动态推测解码。Transformers 后端增加了 FP8 MoE 支持和 CUDA 图修复，PagedAttention 被完全删除。

github · khluu · 7月11日 20:06

**背景**: vLLM 是一个用于快速 LLM 服务的开源库，最初引入 PagedAttention 以使用虚拟内存分页高效管理 KV 缓存。随着时间的推移，开发团队开发了 Model Runner V2 以解决 V1 架构中的设计问题和技术债务。Transformers 后端允许用户通过利用 Hugging Face Transformers 以最少的代码更改运行模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://en.wikipedia.org/wiki/PagedAttention">PagedAttention</a></li>
<li><a href="https://docs.vllm.ai/en/stable/features/speculative_decoding/dynamic_speculative_decoding/">Dynamic Speculative Decoding - vLLM</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM serving`, `#AI infrastructure`, `#model optimization`, `#open source`

---

<a id="item-2"></a>
## [GPT-5.6 一小时内证明 50 年图论猜想](https://www.qbitai.com/2026/07/447873.html) ⭐️ 9.0/10

OpenAI 的 GPT-5.6 Sol Ultra 模型通过 64 个子代理和一个详细提示，在不到一小时内证明了图论中长达 50 年的循环双覆盖猜想。 这一成就展示了 AI 通过多代理推理解决长期数学问题的突破性能力，有望加速数学及相关领域的研究。 模型将猜想转化为有限域上的边标号和线性方程组问题：为每条边配置两个标签，使相同标签的边组成圈。OpenAI 还公布了约 700 个字符的完整提示，该提示规定了验收标准和边界条件，而非固定解题步骤。

telegram · zaihuapd · 7月12日 03:49

**背景**: 循环双覆盖猜想询问是否每个无桥无向图都存在一个圈的集合，使得每条边恰好出现两次。这是图论中一个著名的开放问题，由 Tutte、Itai 和 Rodeh、Szekeres 以及 Seymour 提出。有限域是元素个数有限的代数结构，在此用于将问题转化为代数形式。子代理是较小的 AI 助手，可被委派子任务以管理复杂性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/Finite_field">Finite field</a></li>
<li><a href="https://anthropic.skilljar.com/introduction-to-subagents">Introduction to subagents</a></li>

</ul>
</details>

**标签**: `#AI`, `#mathematics`, `#graph theory`, `#GPT-5.6`, `#reasoning`

---

<a id="item-3"></a>
## [英伟达、CoreWeave 与 Nebius：GPU 繁荣中的循环融资内幕](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 8.0/10

一项分析揭示了英伟达、CoreWeave 和 Nebius 如何通过投资和 GPU 供应协议相互关联，引发了关于这是否构成循环融资的辩论。 理解这些金融动态至关重要，因为它们支撑着蓬勃发展的 AI 基础设施市场，可能影响 GPU 定价、云竞争以及 AI 生态系统的稳定性。 英伟达向 CoreWeave 投资 20 亿美元获得 9%的股权，而 CoreWeave 计划 2026 年资本支出 350 亿美元，英伟达的投资仅覆盖一小部分。与此同时，Nebius 与 Meta 签署了 270 亿美元的 AI 基础设施协议，使用英伟达的 GPU。

hackernews · adletbalzhanov · 7月11日 17:21 · [社区讨论](https://news.ycombinator.com/item?id=48873836)

**背景**: CoreWeave 和 Nebius 是独立的 GPU 云提供商，为 AI 工作负载提供英伟达 GPU。GPU 繁荣导致了巨大的资本支出，云提供商依赖英伟达等硬件供应商的投资和 Meta 等大型科技公司的收入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.coreweave.com/products/gpu-compute">GPUs for AI Models and Innovation | CoreWeave</a></li>
<li><a href="https://nebius.com/">Nebius - The Ultimate AI Cloud</a></li>
<li><a href="https://tech-insider.org/meta-nebius-27-billion-ai-infrastructure-deal-2026/">Meta-Nebius 7B AI Infrastructure Deal Breakdown [2026]</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：一些人认为英伟达相对于 CoreWeave 资本支出的较小持股比例证明了这不是循环融资，而另一些人则关注盈利能力问题，如每 token 的 ROI 等指标。少数人讨论了 Nebius 的容量和面试经历。

**标签**: `#GPU boom`, `#Nvidia`, `#CoreWeave`, `#cloud infrastructure`, `#AI financing`

---

<a id="item-4"></a>
## [ClickHouse 将 PgBouncer 吞吐量提升四倍](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse 发布博客文章，描述了他们如何通过使用对等连接共享和启用 SO_REUSEPORT 多进程，将 PostgreSQL 连接池工具 PgBouncer 的吞吐量提升四倍。 这一优化打破了许多 PostgreSQL 部署中的常见瓶颈，使池化器饱和的系统无需扩展 Postgres 本身即可处理更多流量，展示了一种实用且低成本的数据库基础设施性能提升方法。 改进措施包括在同一主机上运行多个 PgBouncer 进程，使用 SO_REUSEPORT 共享同一端口，并启用对等通信以便取消请求能转发到正确的进程。此配置现已成为 ClickHouse Managed Postgres 的默认设置。

hackernews · saisrirampur · 7月11日 15:28 · [社区讨论](https://news.ycombinator.com/item?id=48872874)

**背景**: PgBouncer 是 PostgreSQL 的轻量级连接池工具，用于管理数据库连接以减少开销。传统上，单个 PgBouncer 进程在高并发下会成为瓶颈。对等通信允许多个 PgBouncer 进程共享连接元数据并转发取消请求，防止查询丢失。SO_REUSEPORT 允许多个进程监听同一个 TCP 端口，分散传入连接。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres">How we scale PgBouncer in ClickHouse Managed Postgres</a></li>
<li><a href="https://www.pgbouncer.org/">PgBouncer - lightweight connection pooler for PostgreSQL</a></li>
<li><a href="https://www.pgbouncer.org/config.html">PgBouncer config</a></li>

</ul>
</details>

**社区讨论**: 评论讨论了技术细节：有人质疑 PgBouncer 为何需要处理取消请求，并提到了 Odyssey 和 pgdog 等替代方案。总体情绪积极，用户注意到通过 Kubernetes 扩展的有用性，并对对等配置表现出兴趣。

**标签**: `#PostgreSQL`, `#PgBouncer`, `#performance`, `#connection pooling`, `#scalability`

---

<a id="item-5"></a>
## [SQLite：建议使用严格表以确保类型安全](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 8.0/10

Evan Hahn 发表了一篇文章，倡导在 SQLite 中使用严格表（STRICT tables）来强制执行列类型约束，以防止因类型不匹配导致的数据损坏。 这种做法通过插入时捕获类型错误而非静默损坏数据，提升了 SQLite 用户的数据完整性，特别是在多应用或生产环境中。 严格表从 SQLite 3.37.0（2021-11-27）版本引入，按表启用。但现有表无法直接通过 ALTER TABLE 转换；可使用 sqlite-utils 等工具通过复制数据来执行转换。

hackernews · ingve · 7月11日 17:33 · [社区讨论](https://news.ycombinator.com/item?id=48873940)

**背景**: 在普通 SQLite 表中，列数据类型是提示而非严格规则，允许任何类型的值存入任何列。这种灵活性称为动态类型，可能导致静默数据损坏（例如将字符串插入整数列）。严格表在数据库层面强制执行列类型，拒绝不匹配的值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sqlite.org/stricttables.html">STRICT Tables</a></li>
<li><a href="https://antonz.org/sqlite-strict-tables/">STRICT tables in SQLite</a></li>
<li><a href="https://www.sqlitetutorial.net/sqlite-strict-tables/">SQLite Strict Tables</a></li>

</ul>
</details>

**社区讨论**: 评论中既有支持也有担忧：simonw 在 sqlite-utils 中添加了转换表的功能；dfabulich 引用了官方'flextypegood'文档，反对默认启用严格模式；jll29 希望严格成为默认；ezekiel68 指出了简单性与可靠性之间的权衡；petilon 指出严格模式缺少 Date 等数据类型。

**标签**: `#SQLite`, `#databases`, `#data integrity`, `#strict tables`, `#software engineering`

---

<a id="item-6"></a>
## [U-Boot 六个漏洞可在操作系统启动前执行代码](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

固件安全公司 Binarly 披露了 U-Boot 引导程序 FIT 签名验证代码中的六个漏洞，其中两个可导致任意代码执行，四个可导致设备崩溃，影响从 U-Boot 2013.07 版本开始的设备。 这些漏洞允许攻击者在操作系统和安全软件启动之前执行恶意代码，可能禁用固件安全功能并植入持久性恶意软件，在 BMC 等系统上可实现远程利用。 漏洞位于 FIT 签名验证代码中，影响超过 50 个稳定版本及下游厂商分支；U-Boot 维护者已接受补丁，但需要硬件厂商将其集成到固件更新中才能分发。

telegram · zaihuapd · 7月11日 08:32

**背景**: U-Boot 是一种开源引导程序，广泛用于路由器、物联网设备和服务器的嵌入式设备中。FIT（扁平镜像树）是一种用于打包内核、设备树和 initramfs 的格式，通过签名验证确保完整性。BMC（基板管理控制器）是一种远程管理处理器，允许管理员通过网络更新固件，使得远程利用成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.u-boot.org/en/latest/usage/fit/signature.html">U-Boot FIT Signature Verification — Das U-Boot unknown version documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Intelligent_Platform_Management_Interface">Intelligent Platform Management Interface - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#U-Boot`, `#firmware`, `#vulnerability`, `#bootloader`

---

<a id="item-7"></a>
## [智谱创始人宣布‘摸高计划’追求 AGI](https://mp.weixin.qq.com/s/3CQSkf_kBnXiCDgS4L-Cgg) ⭐️ 8.0/10

智谱创始人唐杰发布内部信，宣布启动‘摸高计划’，规划通过长程任务、自治智能体系统、完全自我训练和极致安全治理来实现 AGI，并在机械可解释性方面进行百亿级投入。 该计划标志着中国领先 AI 公司之一选择优先追求 AGI 而非短期商业变现，强调可解释性和安全性的重要性，可能影响全球 AGI 研究方向，尤其在中国 AI 生态中。 计划将 AGI 路径概括为四座高峰：长程任务、自治智能体、完全自我训练和极致安全治理。智谱承诺投入百亿级资金研究机械可解释性，推动黑盒模型透明化。其 GLM-5.2 模型被认为接近海外最前沿模型能力，且采用开源模式。

telegram · zaihuapd · 7月11日 13:59

**背景**: AGI（通用人工智能）指能执行任何人类智力任务的人工智能系统。机械可解释性是通过逆向工程理解神经网络内部算法和电路的研究领域。自治智能体系统能独立规划并执行复杂任务，是迈向 AGI 的关键一步。智谱是以开源 GLM 系列模型著称的中国 AI 公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://en.wikipedia.org/wiki/Autonomous_agent">Autonomous agent - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AGI`, `#AI Safety`, `#Interpretability`, `#ZhiPu`, `#Open Source`

---

<a id="item-8"></a>
## [xAI Grok CLI 默认上传整个代码库及密钥文件](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 8.0/10

安全研究人员发现，xAI 的 Grok CLI 工具（版本 0.2.93）默认将整个代码仓库和 .env 等密钥文件上传至 xAI 服务器，即使关闭“改进模型”开关也无法阻止。 这对使用该工具的开发者构成了严重的隐私和安全风险，可能导致专有代码、凭证及其他敏感数据在未经用户同意或知情的情况下泄露给 xAI。 该工具通过两种渠道上传文件：文件内容嵌入模型请求并上传至 Google Cloud Storage，同时无论用户提示如何，整个仓库都以 git bundle 形式上传。测试中，一个被明确指示不要打开的文件在上传包中完整可恢复。

telegram · zaihuapd · 7月12日 04:19

**背景**: Grok CLI 是 xAI 开发的命令行工具，将 Grok 模型（如 Grok 4.5）集成到终端中辅助编程。git bundle 是一个包含完整 Git 仓库（包括所有分支和历史记录）的二进制文件。“改进模型”设置本应用于控制数据共享以训练模型，但在此处未能阻止上传。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://github.com/Norlem/grok-cli">GitHub - Norlem/grok-cli: A terminal UI for xAI's Grok models...</a></li>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git-bundle Documentation</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#xAI`, `#CLI`, `#code leakage`

---

<a id="item-9"></a>
## [欧盟拟对失职保护消费者的大型科技公司罚款](https://www.ft.com/content/25640be5-a5bd-4548-81f9-bd0e16f87f35) ⭐️ 8.0/10

欧盟司法专员 Michael McGrath 宣布，欧盟委员会将在 2025 年底前提出新立法，赋予欧盟对未能保护消费者（尤其是儿童）免受成瘾性设计、订阅陷阱和暗黑模式侵害的大型科技公司罚款的权力。 这标志着欧盟消费者保护执法的重大扩展，可能迫使主要平台重新设计界面并减少欺骗性做法。此举可能为监管暗黑模式和成瘾性设计树立全球先例。 新规则不仅涵盖已受数字法规约束的大型科技公司，还包括小型在线商家和游戏开发商。McGrath 指出，目前由成员国执行的规则从未导致罚款，缺乏威慑力。

telegram · zaihuapd · 7月12日 06:25

**背景**: 暗黑模式是一种欺骗性用户界面设计，旨在诱骗用户进行非预期操作，例如购买不必要的保险或不想要的商品。欧盟此前已颁布《数字服务法》等法规，但消费者保护执法力度薄弱。拟议立法旨在填补执法空白，赋予欧盟直接处罚系统性违规行为的权力。

**标签**: `#EU regulation`, `#consumer protection`, `#dark patterns`, `#tech policy`, `#online platform regulation`

---