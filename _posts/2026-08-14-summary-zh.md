---
layout: default
title: "Horizon Summary: 2026-08-14 (ZH)"
date: 2026-08-14
lang: zh
---

> 从 34 条内容中筛选出 8 条重要资讯。

---

1. [GLM-5.3：前沿编码与突现网络能力并进](#item-1) ⭐️ 9.0/10
2. [将《毁灭战士》渲染器编译成 210 亿参数 Transformer，无需训练](#item-2) ⭐️ 9.0/10
3. [Qwen 3.8 27B 开源权重模型在本地硬件上表现惊艳](#item-3) ⭐️ 8.0/10
4. [RustDesk 为 Wayland 带来真正的无人值守远程访问](#item-4) ⭐️ 8.0/10
5. [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](#item-5) ⭐️ 8.0/10
6. [美国法官责令谷歌取消第三方应用商店安装障碍](#item-6) ⭐️ 8.0/10
7. [PostgreSQL 修复 to_char 高危堆溢出漏洞，可致任意代码执行](#item-7) ⭐️ 8.0/10
8. [苹果联手阿里训练中国专属 AI 大模型](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GLM-5.3：前沿编码与突现网络能力并进](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

Z.ai 发布了旗舰模型 GLM-5.3，它在 GLM-5.2 基础模型之上通过后训练改进，声称在 Z.ai Code Bench 上比 GLM-5.2 提升 50%，并在 Terminal-Bench 3.0 和 Agents' Last Exam (CLI) 上达到开源 SOTA。该模型还展现出突现的网络能力，包括自动化漏洞扫描和红队执行。 此次发布把开源权重模型推向编码与攻防安全的前沿，可能重塑漏洞发现方式以及 AI 智能体在真实软件环境中的运作模式。它也加剧了大模型厂商之间的竞争，社区成员报告称已用 GLM-5.3 取代其他订阅用于安全研究。 GLM-5.3 使用与 GLM-5.2 相同的基础模型，全部提升来自后训练。Z.ai 报告称，该模型在 269 个项目中发现了 2,436 个真实漏洞，并维护公开的 CVD 台账；部分漏洞已被 MITRE、FreeBSD 和 Red Hat 认可并归功于该模型。

hackernews · pella · 8月14日 05:19 · [社区讨论](https://news.ycombinator.com/item?id=49294997)

**背景**: GLM 是 Z.ai（智谱 AI）开发的开源权重大型语言模型系列，定位为中国对 OpenAI、Anthropic、Google 等前沿模型的替代方案。“前沿编码（frontier coding）”指在软件工程和智能体编码基准上达到最先进水平。“突现网络能力（emergent cyber capabilities）”指大型模型中自动漏洞扫描、红队测试等技能，这些技能可能是自然涌现或被刻意训练出来的；对它们的验证很重要，因为可能改变安全编码实践和威胁格局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://codersera.com/blog/glm-5-3-cyber-capabilities-explained-2026/">GLM-5.3 Cyber Capabilities: Real, Verified or Hype?</a></li>
<li><a href="https://kie.ai/blog/what-is-glm-5-3">What Is GLM-5.3? Z.ai's Next Open-Weight Model</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体热烈但保持审慎。用户报告 GLM-5.3 在红队和漏洞研究中的真实成功，包括发现 WordPress 插件 0-day、RCE 和内核漏洞利用改编；但也有评论认为它在某些利用链基准上仍略逊于 Sol、Fable 等模型，且权重尚未开源。还有人赞赏 Z.ai 的研究者式文风，另一些人则质疑大规模漏洞扫描的成本与披露流程。

**标签**: `#AI`, `#LLM`, `#cybersecurity`, `#coding`, `#GLM`

---

<a id="item-2"></a>
## [将《毁灭战士》渲染器编译成 210 亿参数 Transformer，无需训练](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 9.0/10

作者使用自定义编译器，将《毁灭战士》的渲染算法转换为标准的 210 亿参数 Transformer 检查点，全程无需训练。该模型通过根据 3614 个 token 的提示生成 53747 个 token 级绘图指令来渲染经典 E1M1 关卡，在 NVIDIA B200 上每帧约需 40 分钟。 这项研究表明，复杂的命令式程序可以通过编译而非基于梯度的学习直接嵌入 Transformer 权重，为机制可解释性和算法权重复制编程开辟了新途径。它也挑战了人们对 Transformer 计算能力的假设，尽管最终速度远慢于原生执行。 该检查点完全兼容 Hugging Face Transformers 库，无需 trust_remote_code；一个 43 行的 Python 宿主程序即可加载模型、执行生成并将绘图指令解析为可见帧。计算图源码已在 GitHub 上公开，所用的编译器为 TorchWright，它可将符号图转换为嵌入、注意力、前馈和写回权重。

reddit · r/MachineLearning · /u/notforrob · 8月14日 15:50

**背景**: Transformer 通常通过梯度下降在海量数据集上训练，但最近诸如 TorchWright 等项目直接将 Python 定义的计算图编译为 Transformer 权重，相当于手工“编程”模型。《毁灭战士》引擎的软件渲染器是 1993 年游戏中著名的实时 3D 光栅化器；证明这一算法可以编码为发射 token 的 Transformer，展示了基于注意力的计算的普适性。作者此前两篇帖子正是在为这一最终结果做铺垫。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://towardsdatascience.com/i-built-a-tiny-computer-inside-a-transformer/">I Built a Tiny Computer Inside a Transformer | Towards Data Science</a></li>
<li><a href="https://github.com/Percepta-Core/transformer-vm">GitHub - Percepta-Core/transformer-vm: Compile programs directly into transformer weights. Includes a 2D convex-hull KV cache with O(log n) inference. · GitHub</a></li>

</ul>
</details>

**标签**: `#transformer`, `#compiler`, `#interpretability`, `#doom`, `#mechanistic`

---

<a id="item-3"></a>
## [Qwen 3.8 27B 开源权重模型在本地硬件上表现惊艳](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 8.0/10

Qwen 3.8 27B 是阿里巴巴 Qwen 团队新发布的开源权重语言模型，现已可在 Hugging Face 上获取。社区用户报告其在本地设备上表现出色，一位用户指出它在 DeepSWE 基准测试上超越了 Claude Opus 4.7。 该发布表明高性能推理模型可以在本地运行，为昂贵的专有服务提供了高性价比的替代方案。社区基准测试的强劲结果表明，开源权重模型对爱好者和企业而言正变得越来越有竞争力。 该模型拥有 270 亿参数，隐藏维度为 5120，并在回答前会生成显式的推理轨迹。用户指出，其 VRAM 使用效率不如 Gemma 4 等同类模型，在解决一个私人基准测试时消耗了更多 token 和时间，但最终还是成功完成。

hackernews · erdaltoprak · 8月14日 15:00 · [社区讨论](https://news.ycombinator.com/item?id=49299605)

**背景**: Qwen 是阿里巴巴开发的一系列大语言模型，涵盖密集型（dense）和混合专家（MoE）架构。开源权重模型将训练好的参数公开可供下载，用户可以在自己的硬件上运行，这与封闭 API 不同。Qwen3 是最新一代，其中的推理优先模型默认会输出结构化的“思考”轨迹。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://ollama.com/library/qwen3:30b-a3b-thinking-2507-q8_0">qwen3:30b-a3b-thinking-2507-q8_0</a></li>
<li><a href="https://openrouter.ai/qwen/qwen3-next-80b-a3b-thinking/pricing">Qwen: Qwen3 Next 80B A3B Thinking – Effective Pricing | OpenRouter</a></li>

</ul>
</details>

**社区讨论**: 评论区用户分享了实际操作测试：Simon Willison 称赞了它绘制“骑自行车的鹈鹕”的能力，另一位用户则表示它是第二款通过其私人基准测试的本地模型。还有用户与 Claude Opus 进行了对比，指出本地模型的成本效益更高，也有人希望看到更多诸如 35B A3B 的 MoE 模型。

**标签**: `#AI`, `#Machine Learning`, `#Language Model`, `#Qwen`, `#Open Source`

---

<a id="item-4"></a>
## [RustDesk 为 Wayland 带来真正的无人值守远程访问](https://rustdesk.com/blog/unattended-remote-access-wayland/) ⭐️ 8.0/10

RustDesk 宣布在 Wayland 上支持真正的无人值守远程访问，并支持多显示器。目前提供面向 x86_64 Debian/Ubuntu 系统的预览构建版本。 Wayland 的安全模型使无人值守远程访问变得困难，因此该功能填补了 Linux 用户面临的一个重要空白。它使 RustDesk 成为 TeamViewer 和 AnyDesk 等专有工具更具竞争力的开源替代方案。 预览版面向 x86_64 Debian/Ubuntu 系统。社区成员指出，自托管连接仍不支持加密（GitHub issue #3714），而且客户端向主机传递麦克风输入的功能尚未实现。

hackernews · rustdesk · 8月14日 16:12 · [社区讨论](https://news.ycombinator.com/item?id=49300759)

**背景**: Wayland 是一种旨在取代 X Window System 的显示服务器协议；它采用合成器（compositor）模型，出于安全原因对屏幕捕获进行限制，因此实现远程桌面更为复杂。无人值守远程访问是指无需有人在场接受会话即可连接到计算机。RustDesk 是一款开源的远程桌面应用，设计用于自托管，可替代 TeamViewer 和 AnyDesk 等专有工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rustdesk.com/blog/unattended-remote-access-wayland/">Unattended Remote Access on Wayland with RustDesk — RustDesk</a></li>
<li><a href="https://en.wikipedia.org/wiki/Wayland_(display_server_protocol)">Wayland (display server protocol)</a></li>
<li><a href="https://github.com/rustdesk/rustdesk">GitHub - rustdesk/rustdesk: An open-source remote desktop application designed for self-hosting, as an alternative to TeamViewer. · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论主要指出仍存在的缺口：自托管连接仍缺少加密（GitHub issue #3714），且缺少客户端到主机的麦克风透传。还有用户询问 RustDesk 与 VNC 或基于 SSH/Tailscale 的 Remmina 相比如何，也有人希望了解 RustDesk 与 VNC 的基本区别。

**标签**: `#remote-desktop`, `#wayland`, `#rustdesk`, `#open-source`, `#linux`

---

<a id="item-5"></a>
## [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

小红书 dots 实验室开源了 dots3-note 的开放权重预览版，这是一个 280B 参数的混合专家模型，每次仅激活 16B 参数，支持 512K 上下文窗口，并可处理文本、图片、视频和音频输入。此次发布还引入了 TEMPO 强化学习方法以及两个真实场景智能体基准 VibeSearchBench 和 VibeLifeBench。 这是一次重要的开源发布，因为它将一个前沿规模的 MoE 模型和全新的强化学习训练方法带给了社区，有望加速长程智能体 AI 的研究。同时发布的真实场景基准有助于弥合基准分数与实际智能体性能之间的差距，惠及从事 AI 智能体开发的开发者和研究人员。 dots3-note 模型采用 TEMPO 强化学习训练，该方法利用自批判和测试时价值估计来训练长程智能体。开放权重已在 Hugging Face 上发布，配套的 VibeSearchBench 和 VibeLifeBench 基准旨在真实、多轮场景下评估智能体表现。

telegram · zaihuapd · 8月14日 08:27

**背景**: 混合专家（MoE）是一种神经网络架构，其中每个 token 只激活一部分参数（称为专家），从而在保持较低推理成本的同时实现较大的总参数规模。总参数需要加载到内存中，而激活参数才是实际参与计算的参数。TEMPO 是一种面向长程任务的新型强化学习方法，新发布的基准则聚焦于主动搜索和日常生活等智能体场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://osfoundry.io/articles/mixture-of-experts-explained">Mixture of Experts Explained: Total vs Active Parameters ...</a></li>
<li><a href="https://arxiv.org/html/2605.27882v2">VibeSearchBench: Benchmarking Long-horizon Proactive Search ...</a></li>
<li><a href="https://www.alphaxiv.org/overview/2510.27329">Reinforcement Learning for Long-Horizon Unordered... | alphaXiv</a></li>

</ul>
</details>

**标签**: `#MoE`, `#open-source`, `#reinforcement-learning`, `#multimodal`, `#large-language-models`

---

<a id="item-6"></a>
## [美国法官责令谷歌取消第三方应用商店安装障碍](https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/) ⭐️ 8.0/10

美国地区法官 James Donato 下令谷歌在一周内简化 Play Store 中安装第三方应用商店的流程，删除多余的警告弹窗与步骤。该命令源自 Epic Games 诉谷歌反垄断案。 该裁决直接削弱了谷歌对安卓应用分发的控制，可能让竞争性应用商店更容易触达用户。它还为其他平台处理应用侧载和第三方市场的方式确立了法律先例。 法官认定，这种“先查看再安装”的多步骤提示是蓄意设计的反竞争摩擦，目的是吓退普通用户。谷歌必须让安装第三方商店的过程与安装普通安卓应用一样直接，并须在一周内完成修改。

telegram · zaihuapd · 8月14日 09:55

**背景**: 侧载（sideloading）是指通过官方应用商店之外的渠道安装应用，通常是下载 APK 文件。安卓在技术上允许侧载，但 Google Play 历来会设置警告和额外步骤。该命令源于 Epic Games 诉谷歌案，陪审团在该案中裁定谷歌在安卓应用分发上构成非法垄断。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Google">Epic Games v. Google - Wikipedia</a></li>
<li><a href="https://www.howtogeek.com/773639/what-is-sideloading-and-should-you-do-it/">What Is Sideloading, and What Are the Risks? - How-To GeekHow to Sideload Apps on Android after April 2026? (Google's ...What is sideloading? [Android A to Z] | Android CentralWhat is sideloading on Android: history, methods, pros, and risksSideloading on Android: what it is and why it's so relevantHow to Sideload Apps on Android (And What You Need to Know in ...</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#Android`, `#Google`, `#app stores`, `#regulation`

---

<a id="item-7"></a>
## [PostgreSQL 修复 to_char 高危堆溢出漏洞，可致任意代码执行](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL 披露并修复了 CVE-2026-14669，这是 to_char(timestamptz) 在处理超长 POSIX 时区缩写时出现的堆缓冲区溢出漏洞。已认证的低权限数据库用户可利用该漏洞，以 PostgreSQL 服务进程的操作系统权限执行任意代码；修复版本为 18.6、17.11、16.15、15.19 和 14.24。 由于 PostgreSQL 是全球部署最广泛的数据库之一，核心格式化函数中可执行任意代码的严重漏洞急需修复。该漏洞仅需低权限数据库账户即可利用，因此多租户或共享的 PostgreSQL 部署在升级前都可能面临风险。 受影响的版本为 18.5、17.11、16.15、15.19 和 14.24 之前的 PostgreSQL；但由于 18.5 因回归问题未正式发布，18 系列用户应直接升级至 18.6。此次小版本更新无需转储数据库或运行 pg_upgrade，只需替换程序文件并重启服务，该漏洞 CVSS 评分为 8.8。

telegram · zaihuapd · 8月14日 14:35

**背景**: to_char 是 PostgreSQL 的数据类型格式化函数，用于按指定格式将时间戳、时间间隔和数字转换为字符串。POSIX 时区规范是类似 'EST5EDT' 的字符串，用于定义与 UTC 的标准时差及可选的夏令时规则；PostgreSQL 会在相关上下文中接受这种字符串，并在格式化时展开时区缩写。该漏洞正是由于超长的 POSIX 时区缩写导致格式化过程中发生堆缓冲区溢出。由于该函数运行在数据库服务进程内，成功利用可将 SQL 层面的访问权限提升为操作系统层面的任意代码执行权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/functions-formatting.html">PostgreSQL: Documentation: 18: 9.8. Data Type Formatting Functions</a></li>
<li><a href="https://postgrespro.com/docs/postgrespro/9.6/datetime-posix-timezone-specs">Postgres Pro Standard : Documentation: 9.6: B.5. POSIX Time Zone...</a></li>
<li><a href="https://www.postgresql.org/docs/current/pgupgrade.html">PostgreSQL: Documentation: 18: pg_upgrade</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#CVE`, `#Security`, `#Vulnerability`, `#Patch`

---

<a id="item-8"></a>
## [苹果联手阿里训练中国专属 AI 大模型](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 8.0/10

据报道，苹果正在阿里巴巴的支持下，专门为中国市场训练一个大语言模型，标志着其不再依赖第三方模型。Apple Intelligence 预计在未来数月内通过 iOS 更新在中国上线。 如果成功，苹果可能成为首个获准在中国提供自有 AI 模型的外国公司，从而更好地掌控其设备上的 AI 体验，并增强在中国市场的竞争力。这也标志着中国 AI 监管对外国企业可能出现的开放。 苹果自研模型将使其更好地掌控 AI 用户体验，中国网信办已于上月对其生成式 AI 服务进行备案。关于该模型的具体技术细节尚未披露。

telegram · zaihuapd · 8月14日 14:47

**背景**: Apple Intelligence 是苹果于 2024 年 6 月发布的 AI 功能套件，集成在 iOS、iPadOS 和 macOS 中，结合了端侧和服务器处理。阿里巴巴开发了通义千问（Qwen）系列大语言模型，在中国被众多企业客户使用。根据中国监管规定，生成式 AI 服务需要获得当局批准或备案，外国公司此前面临障碍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AI`, `#China`, `#Alibaba`, `#LLM`

---