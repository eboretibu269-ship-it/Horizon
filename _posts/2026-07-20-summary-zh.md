---
layout: default
title: "Horizon Summary: 2026-07-20 (ZH)"
date: 2026-07-20
lang: zh
---

> 从 34 条内容中筛选出 13 条重要资讯。

---

1. [Sam Altman 邮件揭示发布本地 GPT-3 模型的计划](#item-1) ⭐️ 9.0/10
2. [Hugging Face 披露 AI 智能体攻击，商业大模型拒绝取证](#item-2) ⭐️ 9.0/10
3. [Fastjson 1.x 被发现无需 gadget 的严重 RCE 漏洞](#item-3) ⭐️ 9.0/10
4. [欧盟拟向美开放生物识别数据换取免签](#item-4) ⭐️ 9.0/10
5. [智谱完成国产芯片大型数据中心建设](#item-5) ⭐️ 9.0/10
6. [中国开源权重 AI 策略胜出西方闭源模型](#item-6) ⭐️ 8.0/10
7. [黑客摧毁罗马尼亚土地登记数据库](#item-7) ⭐️ 8.0/10
8. [arXiv 上 AI 写作在 ChatGPT 后激增，计算机科学领域 2026 年达 65%](#item-8) ⭐️ 8.0/10
9. [完美并非过度工程](#item-9) ⭐️ 8.0/10
10. [Kimi K3、Qwen 3.8 与 Anthropic 的（潜在）解体](#item-10) ⭐️ 8.0/10
11. [本·汤普森提议美国立法促进开放 AI 模型以对抗中国](#item-11) ⭐️ 8.0/10
12. [Kimi K3 崛起，美国或限制使用中国开放权重 AI 模型](#item-12) ⭐️ 8.0/10
13. [美军常用 App 被发现嵌入中俄代码](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Sam Altman 邮件揭示发布本地 GPT-3 模型的计划](https://simonwillison.net/2026/Jul/20/sam-altman/#atom-everything) ⭐️ 9.0/10

一封 Sam Altman 在 2022 年 10 月发给 OpenAI 董事会的邮件，在 2026 年马斯克诉 Altman 案中被曝光，详细说明了一项发布可在消费硬件上本地运行的 GPT-3 级模型的策略。其目的是阻止 Stability AI 等竞争对手，并让新项目更难获得资金。 这一揭露直接展示了 OpenAI 在开源 AI 方面的竞争策略，表明发布本地模型被视为先发制人的手段。这加剧了关于 AI 伦理、开源背后的企业动机以及开放与控制之间平衡的持续辩论。 邮件特别提到要创建一个“能力接近 GPT-3”且可本地运行的语言模型，并强调要在“Stability 或其他公司”之前完成。Altman 认为此举将“阻止其他人发布类似强大的模型”，并阻碍新竞争者获得资金。

rss · Simon Willison · 7月20日 03:47

**背景**: GPT-3 是 OpenAI 在 2020 年发布的大型语言模型，通常因其规模而通过云 API 访问。2022 年，在消费硬件上运行此类模型具有挑战性，但后来量化技术和高效架构的进步使本地部署成为可能。这封邮件早于 LLaMA 等模型的开源发布，后者引发了广泛的本地 AI 实验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://originality.ai/blog/openai-nlp-models">OpenAI NLP Models – Originality.AI</a></li>
<li><a href="https://www.computeleap.com/blog/how-to-run-ai-locally-2026/">Running LLMs on Your Own Hardware: What Actually Works in ...</a></li>

</ul>
</details>

**标签**: `#open-source`, `#openai`, `#gpt-3`, `#ai-ethics`, `#competition`

---

<a id="item-2"></a>
## [Hugging Face 披露 AI 智能体攻击，商业大模型拒绝取证](https://huggingface.co/blog/security-incident-july-2026) ⭐️ 9.0/10

Hugging Face 披露了 2026 年 7 月的一起安全事件：一个自主 AI 智能体利用数据处理流程中的两处代码执行漏洞，执行了数万次操作并窃取了内部数据和凭证。商业大模型 API 拦截了取证分析，团队转而使用本地部署的 GLM 5.2 模型分析了超过 1.7 万条攻击记录。 此事件突显了一种新型威胁：AI 驱动的自主智能体能够渗透主要平台，并揭示了依赖商业大模型进行安全事件响应的潜在风险——安全护栏可能阻碍取证工作。同时强调了开源本地模型在关键任务中的重要性。 攻击发生在周末期间，智能体横向移动至多个内部集群。Hugging Face 确认面向公众的模型、数据集及 Spaces 未被篡改，软件供应链无异常。公司已修复漏洞、重建受损节点并轮换受影响的凭证。

telegram · zaihuapd · 7月20日 10:41

**背景**: Hugging Face 是一个托管 AI 模型和数据集的主要平台。AI 智能体是使用大语言模型（LLM）自主执行任务的程序。在此事件中，攻击者使用了一个自主智能体框架（可能基于安全研究工具包），利用数据集处理流程中的代码执行漏洞。像 OpenAI 或 Anthropic 的商业 LLM 通常具有安全护栏，可能阻止涉及攻击数据的请求，因此团队转向了 GLM 5.2——来自 Z.ai（原名智谱 AI）的中国开源模型，可本地运行而无需此类限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech.ifeng.com/c/8uuiZXccGKJ">Hugging Face遭攻击取证受阻，只能靠国产GLM 5.2救场？_ 凤凰网</a></li>
<li><a href="https://en.wikipedia.org/wiki/GLM_5.2">GLM 5.2</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.2">zai-org/GLM-5.2 · Hugging Face</a></li>

</ul>
</details>

**标签**: `#AI Security`, `#Security Incident`, `#Hugging Face`, `#Supply Chain Security`, `#Incident Response`

---

<a id="item-3"></a>
## [Fastjson 1.x 被发现无需 gadget 的严重 RCE 漏洞](https://x.com/k_firsov/status/2078872293745570032) ⭐️ 9.0/10

安全研究员 Kirill Firsov 披露了 Fastjson 1.x 版本 1.2.68 至 1.2.83 中存在的高危远程代码执行漏洞，该漏洞无需开启 autoType 或依赖 classpath gadget 即可利用。 此漏洞对使用受影响 Fastjson 版本的所有应用构成严重风险，尤其因为 Fastjson 1.x 已于 2024 年 10 月停止维护，官方极有可能不发布补丁，迫使开发者立即迁移或采取缓解措施。 该漏洞可在 JDK 8、17 和 21 上利用，无需 autoTypeSupport 或特定 gadget 链，推荐的唯一缓解措施是升级到 Fastjson2 或在配置中启用 SafeMode。

telegram · zaihuapd · 7月20日 14:32

**背景**: Fastjson 是阿里巴巴开发的 Java 中常用的 JSON 解析库。历史上，许多 Fastjson 漏洞需要开启 autoType 并依赖 classpath 上的特定 gadget 链才能实现远程代码执行。SafeMode 功能从 Fastjson 1.2.68 开始引入，启用后会完全禁用 autoType，从而阻止此类利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson/wiki/fastjson_safemode_en">fastjson_safemode_en · alibaba/fastjson Wiki · GitHub</a></li>
<li><a href="https://alibaba.github.io/fastjson2/autotype_cn.html">FASTJSON 2 Autotype机制介绍 | fastjson2</a></li>

</ul>
</details>

**标签**: `#fastjson`, `#rce`, `#vulnerability`, `#java`, `#security`

---

<a id="item-4"></a>
## [欧盟拟向美开放生物识别数据换取免签](https://edri.org/our-work/the-eu-is-about-to-sell-our-most-sensitive-data-to-the-us-for-visa-free-travel/) ⭐️ 9.0/10

欧盟委员会正与特朗普政府谈判一项“增强边境安全伙伴关系”（EBSP）框架协议，该协议将允许美国访问欧盟公民的生物识别数据，以换取维持欧盟公民的免签旅行待遇。 该协议可能为大范围监控树立危险先例，并抑制政治异议，因为泄露的草案中包含基于政治观点共享“风险指标”的条款。这引发了关于隐私权以及安全与公民自由之间平衡的根本性问题。 美国已设定 2026 年 12 月 31 日为完成 EBSP 协议的最后期限，从 2027 年起参与将成为签证豁免计划（VWP）的强制要求。欧洲数字权利组织（EDRi）警告称，生物识别数据和基于政治观点的风险指标可能被系统性地传输给美国当局。

telegram · zaihuapd · 7月20日 15:08

**背景**: 美国签证豁免计划允许参与国公民赴美旅行最多 90 天而无需签证。2022 年，华盛顿要求加强数据共享作为继续给予欧盟公民免签待遇的条件。增强边境安全伙伴关系（EBSP）是美国寻求访问欧盟成员国指纹及其他生物识别数据库以进行筛查和身份验证的框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.europarl.europa.eu/RegData/etudes/BRIE/2026/785725/EPRS_BRI(2026)785725_EN.pdf">Negotiating the Enhanced Border Security Partnership: Balancing...</a></li>
<li><a href="https://www.euractiv.com/news/eu-countries-gear-up-to-let-us-tap-their-citizens-biometrics/">EU countries gear up to let US tap their citizens’ biometrics | Euractiv</a></li>
<li><a href="https://www.atlanticcouncil.org/in-depth-research-reports/issue-brief/negotiating-an-eu-us-biometric-information-sharing-agreement/">Negotiating an EU-US biometric information-sharing agreement</a></li>

</ul>
</details>

**标签**: `#privacy`, `#biometric data`, `#EU-US relations`, `#data protection`, `#civil liberties`

---

<a id="item-5"></a>
## [智谱完成国产芯片大型数据中心建设](https://www.bloomberg.com/news/articles/2026-07-20/z-ai-completes-giant-data-center-with-chinese-chips-to-train-ai) ⭐️ 9.0/10

智谱人工智能公司建成了一座全部采用国产芯片的 1 吉瓦数据中心，并已开始部分运营。 这一成就标志着中国 AI 基础设施自主化的重要里程碑，展示了在克服美国出口限制方面的进展。 该设施功率达 1 吉瓦（足以满足 75 万户家庭用电），是中国 AI 实验室建造的最大规模设施之一，将用于支持智谱的 GLM 大语言模型训练。

telegram · zaihuapd · 7月20日 15:43

**背景**: 智谱 AI 是中国领先的人工智能公司，开发了 GLM 系列大语言模型，并于 2025 年 1 月被列入美国实体清单。受美国出口管制影响，中国 AI 实验室被迫依赖国产芯片建设大规模计算基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zhipu_AI">Zhipu AI</a></li>

</ul>
</details>

**标签**: `#AI`, `#China`, `#chips`, `#data center`, `#geopolitics`

---

<a id="item-6"></a>
## [中国开源权重 AI 策略胜出西方闭源模型](https://werd.io/american-ai-is-locked-down-and-proprietary-its-losing/) ⭐️ 8.0/10

一篇分析文章指出，中国的开放权重 AI 模型凭借更低成本和更高可及性，正在市场主导地位上超越 OpenAI 和 Anthropic 等西方专有模型。 这一转变可能重塑全球 AI 格局，使先进 AI 更易负担和普及，同时挑战西方领先 AI 公司的商业模式。 开放权重模型并非完全开源，它们缺少训练代码和数据，但允许任何人下载和微调权重，从而实现广泛部署和定制。

hackernews · benwerd · 7月20日 14:21 · [社区讨论](https://news.ycombinator.com/item?id=48979269)

**背景**: 开放权重 AI 模型将训练后的参数（权重）公开，允许用户下载、运行和微调，这与封闭的专有模型不同。这种开放性降低了准入门槛，促进了快速迭代和采用。成本优势显著，因为用户可自行托管或使用第三方服务商，避免支付专有供应商高昂的推理费用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://callsphere.ai/blog/open-weight-models-vs-proprietary-2026-enterprise-comparison">Open-Weight Models vs Proprietary: A 2026 Comparison ...</a></li>

</ul>
</details>

**社区讨论**: 评论者以 PC 取代小型机、Linux 击败 UNIX 作历史类比，认为开放权重模型最终将主导。有人质疑文章称 80%初创公司使用中国模型的说法，引用自身经历表示美国模型更常见。还有人指出，开放权重模型仍需支付高昂的 GPU 租赁费用。

**标签**: `#AI`, `#open-source`, `#China`, `#machine learning`, `#industry analysis`

---

<a id="item-7"></a>
## [黑客摧毁罗马尼亚土地登记数据库](https://news.risky.biz/risky-bulletin-hacker-wipes-romanias-entire-land-registry-database/) ⭐️ 8.0/10

一名黑客入侵了罗马尼亚土地登记机构（ANCPI）并清空了整个数据库，但离线备份可能避免了灾难性数据丢失。ANCPI 现正从头重建网络并迁移至政府云。 这一事件凸显了国家关键基础设施易受网络攻击的脆弱性，以及保留离线备份的极端重要性。若没有离线备份，证明土地所有权将给罗马尼亚带来社会混乱。 安全公司 KELA 确认攻击者为阿尔及利亚的 Zakaria Mahdjoub，他声称也删除了备份。但 ANCPI 似乎已有一份离线副本。该机构宣布完全重建网络并迁移至罗马尼亚政府云，由特别电信服务（STS）协调，预计于 7 月 22 日完成。

hackernews · speckx · 7月20日 13:28 · [社区讨论](https://news.ycombinator.com/item?id=48978605)

**背景**: 土地登记数据库包含土地所有权、边界和抵押等官方记录。离线备份（又称气隙备份）是指存储在未连接任何网络的介质上的副本，因此能免受远程擦除攻击。若无此类备份，此类攻击可能导致永久性数据丢失，因为在线或网络连接的备份也可能被破坏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.howtogeek.com/818193/why-you-need-an-offline-backup/">Why You Need an Offline Backup - How-To Geek</a></li>

</ul>
</details>

**社区讨论**: 评论者担心 IT 承包中的腐败导致安全性差，亲信获得合同却未实施真正的保护措施。其他人确认了黑客身份并指出罗马尼亚与阿尔及利亚之间有引渡条约。还有评论将其与韩国政府数据中心因缺少备份而由火灾导致数据丢失的事件相比较。

**标签**: `#cybersecurity`, `#data breach`, `#critical infrastructure`, `#Romania`, `#hacktivism`

---

<a id="item-8"></a>
## [arXiv 上 AI 写作在 ChatGPT 后激增，计算机科学领域 2026 年达 65%](https://unslop.run/blog/measuring-ai-writing-on-arxiv) ⭐️ 8.0/10

一项针对 arXiv 论文的分析使用调校过的 AI 检测器发现，被标记为机器写的论文比例从 ChatGPT 前的 0.4%上升到 2026 年 1 月的总体 39%，计算机科学领域达到 65%。 这种急剧增长引发了对科学文献完整性和同行评审可靠性的担忧，因为 AI 生成的内容可能微妙地改变研究的传播与评估。 检测器被特意调校以减少误报，ChatGPT 前基线仅为 0.4%。值得注意的是，数学论文变化极小，被标记比例仅约 0.7%。

hackernews · dopamine_daddy · 7月20日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=48981206)

**背景**: arXiv 是一个免费开放获取的学术预印本仓库，涵盖物理学、数学和计算机科学等领域，拥有数百万篇文章。AI 生成文本检测使用计算方法区分人类与机器写作，但仍不完善，因为相同的文本可能由两者产生。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ArXiv">ArXiv</a></li>
<li><a href="https://arxiv.org/abs/2601.03812">[2601.03812] AI Generated Text Detection</a></li>
<li><a href="https://guides.library.ttu.edu/artificialintelligencetools/detection">AI Detection - Artificial Intelligence Tools for Detection, Research and Writing - Guides at Texas Tech University</a></li>

</ul>
</details>

**社区讨论**: 评论者对检测可靠性表示怀疑，一位用户发现其 2015 年前的论文被高比例标记（27-74%），质疑是自己写得像 LLM 还是 LLM 从自己身上学习。其他人指出，当输出可能完全相同时，区分人类和 AI 文本具有挑战性。

**标签**: `#AI detection`, `#arXiv`, `#academic publishing`, `#LLMs`, `#scientific integrity`

---

<a id="item-9"></a>
## [完美并非过度工程](https://var0.xyz/posts/perfection-is-not-over-engineering.html) ⭐️ 8.0/10

一篇新文章认为，在软件中追求完美是一种合理的工艺选择，而非过度工程，挑战了常见的格言'完美是好的敌人'。 这场辩论影响着软件团队如何平衡质量、技术债和务实主义，进而影响工程文化和产品成果。 作者将完美定义为精确满足严格需求，并区分了它和解决错误问题的过度工程。文章认为，否定完美可能导致草率的工作和低质量系统。

hackernews · var0xyz · 7月20日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48979120)

**背景**: 在软件工程中，常使用'完美是好的敌人'这句话来鼓励快速交付和迭代。然而，它有时被误用来为糟糕的设计或技术债辩护。这篇文章反驳了这一点，倡导在适当的情况下追求工艺和高标准。

**社区讨论**: 评论者反应不一：一些人同意这句格言被过度使用来为糟糕的软件辩护，而另一些人则警告说，真正的完美主义可能导致过度工程和浪费精力。少数人指出，这句话仅是为了避免对罕见边缘情况过早优化，而非为草率辩护。

**标签**: `#software engineering`, `#craftsmanship`, `#technical debt`, `#code quality`

---

<a id="item-10"></a>
## [Kimi K3、Qwen 3.8 与 Anthropic 的（潜在）解体](https://www.emergingtrajectories.com/lh/frontier-lab-economics/) ⭐️ 8.0/10

分析近期开源权重大语言模型发布、Anthropic 可能面临的解体以及 Figma 争议，突显专用 ASIC 领域的竞争。

hackernews · cl42 · 7月20日 15:13 · [社区讨论](https://news.ycombinator.com/item?id=48980019)

**标签**: `#AI`, `#LLMs`, `#Open Source`, `#Anthropic`, `#Industry Trends`

---

<a id="item-11"></a>
## [本·汤普森提议美国立法促进开放 AI 模型以对抗中国](https://simonwillison.net/2026/Jul/20/afraid-of-chinese-models/#atom-everything) ⭐️ 8.0/10

本·汤普森提议美国立法，明确将 AI 训练数据收集归类为合理使用，并禁止禁止模型蒸馏的服务条款，旨在帮助美国开放模型与中国同行竞争。他还指出，阿里巴巴决定以开放权重形式发布 Qwen 3.8 Max，可能受到习近平 2026 年 7 月鼓励开源开放合作的演讲影响。 该提议可能重塑美国 AI 政策，解决企业在使用未经授权数据训练模型的同时却限制模型蒸馏的矛盾，从而加速创新并增强美国在全球 AI 竞赛中与中国的竞争力。 模型蒸馏是指利用大型模型的输出训练小型模型，通常通过 API 查询实现，且难以阻止。汤普森认为，既然美国实验室已经在合理使用下利用未经授权数据进行训练，他们也应允许他人蒸馏其模型以促进更广泛的创新。

rss · Simon Willison · 7月20日 17:09

**背景**: 模型蒸馏是一种将大型强大模型的知识迁移到更小、更高效模型的技术，通常通过查询大型模型的 API 实现。在 AI 领域，“合理使用”是美国版权法中的一项法律原则，允许未经许可有限使用受版权保护的材料，AI 公司以此为依据对公开数据进行模型训练。开放权重模型发布训练好的参数，但不提供训练代码或数据，这与完全开源模型不同。关于蒸馏和合理使用的争论是中美 AI 模型竞争的核心，因为中国实验室经常发布开放权重模型并受益于蒸馏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_distillation">Model distillation</a></li>
<li><a href="https://www.linkedin.com/posts/irina-foret-4a6b79263_fair-use-triangle-activity-7381648994852229121-eO_d">Fair Use Triangle | Irina Foret</a></li>
<li><a href="https://www.linkedin.com/pulse/frontier-ai-models-closed-vs-open-weight-source-varadaraj-pandurangan-yrdue">Frontier AI Models: Closed vs Open Weight vs Open Source</a></li>

</ul>
</details>

**标签**: `#AI`, `#copyright`, `#distillation`, `#open models`, `#policy`

---

<a id="item-12"></a>
## [Kimi K3 崛起，美国或限制使用中国开放权重 AI 模型](https://www.axios.com/2026/07/20/ai-us-china-open-source-kimi) ⭐️ 8.0/10

据报道，由于 Moonshot AI 的 Kimi K3 模型表现强劲，特朗普政府正考虑采取新措施，限制美国企业使用中国的开放权重 AI 模型。 这一政策转变可能重塑全球 AI 格局，限制美国企业获取性价比高的中国模型，从而可能削弱竞争并减缓美国公司的创新步伐。 政府可能不会直接封禁，而是通过采购规则、实体清单威胁和舆论施压等手段实施‘软封锁’。白宫 AI 顾问 David Sacks 批评 OpenAI 和 Anthropic 试图借助政府之手消灭开源竞争。

telegram · zaihuapd · 7月20日 11:49

**背景**: 开放权重 AI 模型公开其训练后的参数，允许开发者下载、微调和部署。Kimi K3 由中国初创公司 Moonshot AI 开发，是全球首个开放的 3T 参数模型，在编程和推理方面具有前沿性能，支持 100 万 token 的上下文窗口。美国官员此前曾对中国 AI 能力表示担忧，但被主张放松监管的官员阻止。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(chatbot)">Kimi (chatbot) - Wikipedia</a></li>
<li><a href="https://medium.com/thought-vector/open-weight-llms-a-strategic-advantage-for-enterprise-ai-1c4859ea6885">Open-Weight LLMs: A Strategic Advantage for Enterprise AI | Medium</a></li>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#open-source models`, `#US-China tech competition`, `#Kimi K3`

---

<a id="item-13"></a>
## [美军常用 App 被发现嵌入中俄代码](https://www.wired.com/story/apps-marketed-to-us-troops-are-shipping-chinese-and-russian-code/) ⭐️ 8.0/10

普渡大学等机构的研究人员发现，面向美军人员推广的 220 多款应用中，近三分之二嵌入了来自中国、俄罗斯、伊朗或朝鲜的第三方代码，其中包括已被美国政府列为国家安全威胁的华为软件开发工具包（SDK）。 军事应用中嵌入的外国代码可能引发数据泄露或监视风险，潜在地危及部队位置和行动安全，这对国家安全构成了重大威胁。这类应用在军人中的广泛使用进一步放大了这种威胁。 虽然尚未观察到数据实际流向华为服务器，但该 SDK 可随时远程更新，潜伏代码有被激活的风险。在对 103 名军人关联人员的调查中，76%至 83%的人对应用包含敌对国家代码表示极度不安。

telegram · zaihuapd · 7月20日 13:42

**背景**: 软件开发工具包（SDK）是一套工具和代码，开发者将其集成到应用中，以添加分析或身份验证等功能。当应用包含来自外国实体的 SDK 时，可能会无意中授予远程访问或数据收集的能力。美国国防部此前曾报告，对手利用商业位置数据监视中东地区的美军人员。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.huawei.com/consumer/en/">HUAWEI Developers</a></li>
<li><a href="https://documentation.onesignal.com/docs/en/huawei-sdk-setup">OneSignal Huawei SDK Setup Guide for Android Studio.</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#national security`, `#Huawei`, `#SDK`, `#app security`

---