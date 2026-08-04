---
layout: default
title: "Horizon Summary: 2026-08-04 (ZH)"
date: 2026-08-04
lang: zh
---

> 从 41 条内容中筛选出 10 条重要资讯。

---

1. [Keyv 及相关 npm 包遭受活跃的 Shai-Hulud 供应链攻击](#item-1) ⭐️ 9.0/10
2. [用简单算法与颜色空间生成多样化肤色](#item-2) ⭐️ 8.0/10
3. [Waymo 在达拉斯全面推出无人驾驶网约车](#item-3) ⭐️ 8.0/10
4. [联邦快递式合法邮件助长钓鱼攻击：Troy Hunt 揭示原因](#item-4) ⭐️ 8.0/10
5. [Xbox 宕机致光盘游戏无法游玩，引发所有权之争](#item-5) ⭐️ 8.0/10
6. [系统性地改进 AI 智能体的外围框架以实现自我提升](#item-6) ⭐️ 8.0/10
7. [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资机器](#item-7) ⭐️ 8.0/10
8. [特朗普政府拟禁止进口中国新型光模块](#item-8) ⭐️ 8.0/10
9. [我国发布首部 L3/L4 自动驾驶强制性国标](#item-9) ⭐️ 8.0/10
10. [白宫开源 AI 政策急转弯，硅谷分歧加剧](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Keyv 及相关 npm 包遭受活跃的 Shai-Hulud 供应链攻击](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 9.0/10

Keyv 及相关多个 npm 包在代号为 'Shai-Hulud' 的活跃供应链攻击中被攻陷，该攻击已影响数百个 npm 包。攻击仍在进行中，开发者被敦促检查其依赖。 此事意义重大，因为 Keyv 是 Node.js 生态中广泛使用的键值存储库，供应链攻击可能危及数千个下游项目。该攻击凸显了 npm 依赖管理中的系统性漏洞以及安装时执行代码的危险性。 Shai-Hulud 攻击家族此前已攻陷数百个 npm 包并窃取开发者凭据。社区成员建议在 '.npmrc' 中添加 'min-release-age=5'，并对任何新增的预安装或后安装钩子保持极度警惕。

hackernews · cimi_ · 8月4日 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**背景**: 供应链攻击是指将恶意代码注入合法包中，然后传播到每个依赖该包的项目。npm 生态尤为脆弱，因为包可以通过预安装和后安装钩子在安装期间执行任意脚本。Shai-Hulud 一直是个持续威胁，其变体如 'Mini Shai-Hulud' 曾针对 Mistral AI SDK 和 TanStack Router 等流行包。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wiz.io/blog/shai-hulud-npm-supply-chain-attack">Shai-Hulud npm Supply Chain Attack | Wiz Blog</a></li>
<li><a href="https://www.hexnode.com/blogs/mini-shai-hulud-supply-chain-attack/">Mini Shai-Hulud Supply Chain Attack Hits Mistral AI, TanStack, and...</a></li>
<li><a href="https://www.npmjs.com/package/keyv">keyv - npm</a></li>

</ul>
</details>

**社区讨论**: 社区情绪紧迫且沮丧。有人呼吁暂停新增预安装/后安装钩子，也有人分享实用的缓解措施，如设置最小发布年龄和检查 node_modules 中的受感染迹象。人们还对这种 '玻璃下巴' 式的依赖系统表示更广泛的担忧，该系统使这类攻击如此有效且难以清理。

**标签**: `#supply-chain-security`, `#npm`, `#nodejs`, `#malware`, `#dependency-management`

---

<a id="item-2"></a>
## [用简单算法与颜色空间生成多样化肤色](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 8.0/10

一位开发者发布了一个交互式取色器和程序化生成算法，基于一个新定义的颜色空间来创建多样化且逼真的肤色。项目页面包含公式、交互式演示以及“未来工作”（Future Work）部分。 这为艺术家和游戏开发者提供了一种实用的方式来避免狭窄、刻板的肤色配色，支持更具包容性的角色设计。它也促进了关于颜色空间和算法如何模拟人类感知的持续讨论。 该颜色空间将人类肤色映射到一个新月形区域，评论者指出这与感知均匀的 Oklab 颜色空间中观察到的分布类似。作者承认方法论“可能不太严谨”，并在“未来工作”部分列出了改进方向，包括对函数拟合的进一步优化。

hackernews · automatoney · 8月4日 15:16 · [社区讨论](https://news.ycombinator.com/item?id=49170165)

**背景**: 颜色空间是一种用数学方式组织颜色、使颜色能在不同设备上一致表示和再现的方法，sRGB 和 Adobe RGB 是常见例子。程序化生成（Procedural generation）是利用算法而非手动编辑来创建纹理、游戏资产等内容。肤色尤其难以建模，因为感知到的颜色取决于光照、人类感知和文化背景，因此专门的颜色空间和工具很有价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Color_space">Color space</a></li>
<li><a href="https://en.wikipedia.org/wiki/Procedural_generation">Procedural generation</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了这项工作和手工拟合函数的方法，并指出该方法与 PCA 和 Oklab 存在联系；一位评论者建议作者参考 Pantone SkinTones，另一位观察到各种族肤色在高饱和下都会偏向橙色。还有少数用户表示某些生成的色块看起来偏绿、偏蓝或偏紫，说明模型仍存在一些边界情况。

**标签**: `#color-space`, `#algorithm`, `#digital-art`, `#skin-tones`, `#procedural-generation`

---

<a id="item-3"></a>
## [Waymo 在达拉斯全面推出无人驾驶网约车](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo 宣布将其完全无人驾驶的网约车服务扩展到达拉斯，并向所有用户开放。此举使达拉斯成为美国最新一个可使用 Waymo 自动驾驶汽车的大型都市区。 此次扩展标志着自动驾驶汽车在达拉斯-沃斯堡这样地广人稀、高度依赖汽车的地区部署的重要里程碑。它可能重塑低密度城市的出行方式与安全性，同时也引发了关于住房政策等更广泛社会影响的讨论。 该服务完全无人驾驶，方向盘后没有安全驾驶员。达拉斯的服务区域地图可通过 Google 支持页面查看，显示了乘客的服务范围。

hackernews · xnx · 8月4日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=49172836)

**背景**: Waymo 前身是 Google 自动驾驶汽车项目，是一家开发完全自动驾驶汽车的公司，旨在无需人工干预即可运送乘客。自动驾驶通常按 SAE 等级从 0 到 5 划分；Waymo 运营在最高级别，无需人工干预。达拉斯扩展是 Waymo 在美国多城市推广的一部分，此前已在旧金山和洛杉矶等地部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Waymo">Waymo - Wikipedia</a></li>
<li><a href="https://newatlas.com/sae-autonomous-levels-definition-self-driving/49947/">Self-driving vehicles: What are the six levels of autonomy?</a></li>

</ul>
</details>

**社区讨论**: 社区评论者的态度总体正面，称赞 Waymo 的安全记录和相比人类驾驶员的可预测性。一位评论者强调无人驾驶汽车是一种有效的可负担住房政策，其他人则对在达拉斯-沃斯堡这样的汽车主导都市区推出该服务表示欢迎；还有人分享了达拉斯服务区域地图的链接。

**标签**: `#autonomous-vehicles`, `#Waymo`, `#ride-hailing`, `#urban-mobility`, `#transportation`

---

<a id="item-4"></a>
## [联邦快递式合法邮件助长钓鱼攻击：Troy Hunt 揭示原因](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 8.0/10

在 2024 年的一篇博文中，安全研究员 Troy Hunt 以联邦快递的通知邮件为例，说明正规公司会发送与钓鱼模式高度相似的邮件。他认为这会让用户习惯性地怀疑一切，同时让真正的钓鱼攻击更难被识破。 这件事很重要，因为钓鱼攻击之所以仍然有效，部分原因正是正规机构的行为与钓鱼者相似，耗尽用户辨别真伪的能力。它说明仅靠技术性的邮件认证无法解决钓鱼识别的核心可用性问题。 这篇帖子属于 Hunt 的“Thanks [公司]”系列，并引发读者分享类似经历：联邦快递的报关通知以个人名义发送并附带 PDF 附件，Google 存储空间警告使用了难以验证的 c.gle 链接，而 IRS 电话系统的语音与诈骗电话相同。

hackernews · stymaar · 8月4日 21:09 · [社区讨论](https://news.ycombinator.com/item?id=49175192)

**背景**: 钓鱼攻击是一种社会工程学手法，攻击者冒充可信机构，诱导用户泄露敏感信息或点击恶意链接。SPF、DKIM 和 DMARC 等邮件认证标准可以帮助验证邮件确实来自其声称的域名，但它们并不能让用户轻松区分合法邮件与仿冒的钓鱼邮件。这正是连 Troy Hunt 这样的安全专家也会发现官方通知酷似“用户应警惕”的钓鱼模式的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DMARC">DMARC</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sender_Policy_Framework">Sender Policy Framework - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/DKIM">DKIM</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认同 Hunt 的观点，并举出官方信息看起来像诈骗的实例：联邦快递由个人发送的报关 PDF、无法成功 whois 查询的 Google c.gle 链接，以及与诈骗电话难以区分的 IRS 语音系统。还有人指出，.xyz 等大量新通用顶级域（gTLD）让非技术用户更难判断链接真伪。

**标签**: `#phishing`, `#security`, `#email`, `#user-education`, `#troy-hunt`

---

<a id="item-5"></a>
## [Xbox 宕机致光盘游戏无法游玩，引发所有权之争](https://birchtree.me/blog/xbox-goes-down-you-cant-play-games-you-own-on-disc/) ⭐️ 8.0/10

最近的一次 Xbox 宕机导致用户无法游玩甚至包括已拥有的光盘版游戏，原因是权利验证无法连接到微软服务器。此次故障影响了登录、商店、Game Pass 游戏、向下兼容游戏以及部分光盘游戏。 这一事件凸显了实体游戏光盘仍然依赖在线服务器进行权利验证，表明“拥有”游戏并不保证能随时游玩。它加剧了关于 DRM、始终在线要求和游戏行业消费者所有权的持续争论。 当 Xbox Series X 将光盘数据复制到内置硬盘后，通常需要在线检查才能开始游玩；此次宕机导致这一权利验证失败。微软曾在 2022 年放宽了多数跨世代游戏的这项检查，但向下兼容游戏和其他部分光盘游戏仍需要此步骤。

hackernews · surprisetalk · 8月4日 12:01 · [社区讨论](https://news.ycombinator.com/item?id=49167448)

**背景**: 数字版权管理（DRM）通过技术手段限制对受版权保护的数字内容的使用。在 Xbox 上，光盘游戏通常需要进行在线检查以确认用户有游玩权限，即使游戏数据就在光盘上。这引发批评，认为消费者并未真正拥有游戏，因为服务器故障可能导致访问被中断。这一争论也延伸至电视、电影和音乐等媒体，这些行业已大量转向流媒体和授权模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_rights_management">Digital rights management - Wikipedia</a></li>
<li><a href="https://arstechnica.com/gaming/2021/05/these-offline-disc-based-games-require-an-online-check-in-on-xbox-series-x/">These offline, disc-based games require an online check-in on Xbox Series X - Ars Technica</a></li>
<li><a href="https://www.theverge.com/2022/9/19/23356855/xbox-series-x-game-disc-drm-online-check-in">Microsoft eased up on one DRM hurdle for disc games on Xbox | The Verge</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体上是沮丧与怀旧。评论者指出，像 GameCube 或 PS3 这样的老主机可以让光盘游戏无限期离线游玩，而现代系统将光盘游玩与在线服务器绑定。许多人认为真正的问题是所有权——无论何种格式，购买者都应该能保留、转售和传承游戏。

**标签**: `#Xbox outage`, `#digital ownership`, `#DRM`, `#gaming`, `#always-online`

---

<a id="item-6"></a>
## [系统性地改进 AI 智能体的外围框架以实现自我提升](https://lilianweng.github.io/posts/2026-07-04-harness/) ⭐️ 8.0/10

Lilian Weng 的新博文《Harness engineering for self-improvement》探讨了如何系统地改进 AI 智能体的外围框架（harness）——包括提示词、工具和技能——以提升性能和效率。文章将智能体质量改善的重点从模型权重转向模型周边的工程基础设施。 这篇文章切中了一个新兴且实用的领域：智能体 harness 工程，它往往决定了 LLM 智能体能否在生产环境中真正好用。对这一领域的系统性改进，可以帮助开发者构建更可靠、高效的智能体，并推动 AI 开发从以模型为中心转向以基础设施为中心。 文章将提示词、工具和技能视为要优化的主要 harness 组件；配套讨论提出的实操要点包括：为代码库建立可靠的适应度函数（fitness function）、基于生产 trace 进行自动研究、让 Agent 自己编写工具。同时需要注意，必须有评估集和验证/测试集划分，否则 Agent 会投机取巧地优化目标。

hackernews · tosh · 8月4日 06:17 · [社区讨论](https://news.ycombinator.com/item?id=49164896)

**背景**: 智能体 harness（外围框架）是大型语言模型周围的软件基础设施，负责管理工具调用、记忆、状态持久化、执行环境和反馈循环，不同于模型自身的推理能力。随着 LLM 智能体从演示走向生产环境，harness 往往决定了实际性能、延迟和成本。因此，如何优化 harness——包括让智能体自己设计实验、检查 trace 来改进自身配置的自动化研究方式——正在成为热门的工程课题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>
<li><a href="https://harness-engineering.ai/blog/agent-harness-complete-guide/">The Complete Guide to Agent Harness: What It Is and Why It ...</a></li>
<li><a href="https://github.com/karpathy/autoresearch">GitHub - karpathy/autoresearch: AI agents running research on single-GPU nanochat training automatically · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者的态度积极且务实，有人分享了具体成果：通过让 Agent 基于生产 trace 做自动研究、自己编写工具，把加载上下文的 token 消耗从 20k 降到 800；另有人指出，为代码库建立可靠、通用的 fitness function 是第一步。也有评论提出大胆问题：harness 何时能自己生成 RLHF/DPO 训练集，然后用 LoRA 微调自身模型；此外还有轻松玩笑和对“提示词与代码训练范式”的猜想。

**标签**: `#AI agents`, `#LLMs`, `#software engineering`, `#machine learning`, `#agent harness`

---

<a id="item-7"></a>
## [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资机器](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

谷歌悄然搭建了规模约 2000 亿美元的基础设施融资架构，用于向 Anthropic 交付超过 1500 亿美元的 AI 芯片。相关合同总额约 2000 亿美元，约八成与芯片直接挂钩，参与方包括博通、阿波罗、黑石、摩根士丹利及多家加密矿企。 这是史上最大规模的基础设施融资架构之一，采用类似飞机租赁的厂商融资模式，将风险分散到华尔街各方。它可能重塑 AI 算力的融资方式，让没有信用评级的 Anthropic 得以扩张，同时避免数百亿美元硬件压在单一资产负债表上。 今年 6 月，特殊目的载体 Compute SPV 完成了首批交易，购入约 350 亿美元硬件，约合 1 吉瓦算力、100 万颗 TPU。各方分担风险：谷歌担保数据中心，博通购买并协助融资芯片，阿波罗与黑石购买硬件后回租给 Anthropic。

telegram · zaihuapd · 8月4日 10:52

**背景**: 特殊目的载体(SPV)是为实现狭窄、特定目标而设立的法律实体，常用于持有资产、管理风险或筹集资金，并将财务风险隔离。厂商融资模式由波音、通用电气在飞机和发动机销售中推广，让制造商通过融资支持销售，同时不必将大额资产放在自家资产负债表上。谷歌的 TPU 是为加速机器学习工作负载而设计的定制专用集成电路(ASIC)。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Special-purpose_entity">Special-purpose entity - Wikipedia</a></li>
<li><a href="https://www.investopedia.com/terms/s/spv.asp">Special Purpose Vehicle (SPV): Definition and Reasons Companies Use Them</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tensor_Processing_Unit">Tensor Processing Unit - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Google`, `#Anthropic`, `#Financing`, `#Compute`

---

<a id="item-8"></a>
## [特朗普政府拟禁止进口中国新型光模块](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 8.0/10

特朗普政府正在起草一项禁令，拟禁止进口新型中国光模块和数据中心设备，美国联邦通信委员会(FCC)正在推进该措施，目标是今年内发布并生效。该禁令针对支撑人工智能热潮的关键组件。 此举可能扰乱全球人工智能和数据中心供应链，因为中际旭创等中国企业在光模块市场占据主导地位——在全球 800G 光模块市场占有超过 40%的份额，在 1.6T 细分市场估计占 50%至 70%。运营商可能需要寻找替代供应商或加速本土生产。 据四位知情人士透露，该提案尚未最终确定，仍有可能修改或搁置。此前 FCC 已对中国无人机、路由器、机器人和逆变器实施类似限制，中国驻美使馆表示将采取一切必要措施维护自身利益。

telegram · zaihuapd · 8月4日 11:29

**背景**: 光模块是将电信号转换为光信号的电子设备，能够通过光纤电缆实现高速数据传输，是数据中心和电信网络中的关键组件。FCC 根据《安全设备法案》有权限制对美国国家安全构成风险的通信设备进口，并建立“覆盖清单”。中国在光模块领域的主导地位源于制造规模、成本优势以及与北美科技巨头在下一代产品上的紧密合作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ascentoptics.com/blog/everything-you-need-to-know-about-optical-modules/">Everything You Need to Know About Optical Modules</a></li>
<li><a href="http://www.china.org.cn/2026-06/07/content_118535139.shtml">From optical modules to chips -- China's tech supply... - China.org.cn</a></li>
<li><a href="https://www.fcc.gov/faqs-recent-updates-fcc-covered-list-regarding-routers-produced-foreign-countries">FAQs on Recent Updates to FCC Covered List Regarding Routers Produced in Foreign Countries | Federal Communications Commission</a></li>

</ul>
</details>

**标签**: `#trade policy`, `#optical modules`, `#AI infrastructure`, `#regulation`, `#supply chain`

---

<a id="item-9"></a>
## [我国发布首部 L3/L4 自动驾驶强制性国标](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

2026 年 7 月 30 日，工业和信息化部发布强制性国家标准 GB 44721—2026《智能网联汽车 自动驾驶系统安全要求》，将于 2027 年 7 月 1 日起实施。这是我国首部针对 L3 级有条件自动驾驶和 L4 级高度自动驾驶系统的强制性国标。 该标准将 L3/L4 自动驾驶安全从推荐性文件升级为强制法规，为车企和科技公司确立了明确的监管基线。这将加速中国自动驾驶汽车的安全商业化进程，并可能影响全球相关法规的制定。 该标准适用于搭载 L3 或 L4 级系统的 M 类（载客）和 N 类（载货）车辆，但不适用于自动泊车系统。标准从企业全生命周期安全保障、系统动态驾驶能力、人机交互与用户告知、多维度检验检测四个维度构建安全要求体系，要求自动驾驶系统安全水平至少达到合格且专注驾驶人的水平。

telegram · zaihuapd · 8月4日 13:06

**背景**: L3 级自动驾驶允许车辆在特定条件下自主行驶，但驾驶员必须保持接管能力；L4 级可在限定场景内无需人工干预完成全部驾驶任务。在中国，M 类车辆为载客车辆，N 类为载货车辆，强制性国家标准（GB）经国家市场监督管理总局批准后具有法律效力。新标准是对 2024 年推荐性国标的升级，反映了我国自动驾驶技术的快速发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html">《智能网联汽车 自动驾驶系统安全要求》强制性国家标准正式发布</a></li>
<li><a href="https://news.cctv.com/2026/08/04/ARTI9262heSw0hbsjizKtt1j260804.shtml">《智能网联汽车 自动驾驶系统安全要求》强制性国家标准正式发布_新闻...</a></li>

</ul>
</details>

**标签**: `#autonomous-driving`, `#regulation`, `#safety-standards`, `#china`, `#AI`

---

<a id="item-10"></a>
## [白宫开源 AI 政策急转弯，硅谷分歧加剧](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 8.0/10

白宫在对中国开源 AI 模型的限制政策上急转弯，转向发布前安全审查框架。8 月 4 日白宫邀请科技公司商议新框架，拟在模型发布前审查网络安全。 这一转变重塑了美国对开源 AI 的竞争政策，并反映出顶尖科技公司在国家安全与开放生态之间的深刻分歧。结果可能影响全球开源 AI 模型的发布方式，波及全球开发者与企业。 政策转变前，白宫幕僚长 Susie Wiles 与财长 Scott Bessent 曾考虑制裁、贸易黑名单甚至禁止美企与中国公司合作。导火索是中国开源模型 Kimi K3 部分性能比肩 OpenAI 顶级模型；Nvidia、Meta 及黄仁勋组建的 230 余家成员安全联盟反对限制，而 OpenAI 与 Anthropic 则推动限制。

telegram · zaihuapd · 8月4日 15:22

**背景**: 开源 AI 模型指权重向公众开放的 AI 系统，任何人都可以使用、研究并修改它们。总部在北京的月之暗面（Moonshot AI）于 2026 年 7 月发布了 Kimi K3，据称是全球最大的开源 AI 模型，缩小了美国企业的领先优势。美国政府内部一直在争论，限制这类中国开源模型到底是为了国家安全，还是会损害美国自身的开源生态和竞争力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(AI)">Kimi (AI) - Wikipedia</a></li>
<li><a href="https://www.nytimes.com/2026/07/17/business/china-ai-moonshot-kimi.html">China’s Moonshot AI Unveils Kimi Model, Threatening America’s Lead - The New York Times</a></li>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#open source`, `#US policy`, `#China`, `#tech industry`

---