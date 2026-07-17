---
layout: default
title: "Horizon Summary: 2026-07-17 (ZH)"
date: 2026-07-17
lang: zh
---

> 从 42 条内容中筛选出 14 条重要资讯。

---

1. [欧盟裁定谷歌必须向竞争对手开放 Android 与搜索数据](#item-1) ⭐️ 9.0/10
2. [Kimi K3：开放前沿模型，参数规模巨大](#item-2) ⭐️ 8.0/10
3. [LM Studio Bionic：开放模型的 AI 智能体](#item-3) ⭐️ 8.0/10
4. [从 Rust 到 Zig 的编译器重写进度报告](#item-4) ⭐️ 8.0/10
5. [交互式线性代数书籍动态可视化获好评](#item-5) ⭐️ 8.0/10
6. [Firefox 通过 WebAssembly 在浏览器内运行](#item-6) ⭐️ 8.0/10
7. [GPT-5.6 代码生成器漏洞可意外删除文件](#item-7) ⭐️ 8.0/10
8. [Thinking Machines Lab 发布开源权重 Inkling 模型](#item-8) ⭐️ 8.0/10
9. [Linus Torvalds 宣布 Linux 不反 AI](#item-9) ⭐️ 8.0/10
10. [ExTernD：实现近乎任意精度的三元大模型训练后量化](#item-10) ⭐️ 8.0/10
11. [知网将下架列 AI 为作者的论文](#item-11) ⭐️ 8.0/10
12. [日本购入 2.75 万块英伟达 Rubin 芯片打造机器人 AI](#item-12) ⭐️ 8.0/10
13. [台积电再投千亿美元赴美，Q2 利润飙升 77%](#item-13) ⭐️ 8.0/10
14. [Truth Social 将向华尔街出售特朗普实时帖子](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [欧盟裁定谷歌必须向竞争对手开放 Android 与搜索数据](https://www.theverge.com/policy/966438/eu-google-android-ai-interoperability-search-data-dma) ⭐️ 9.0/10

欧盟委员会周四裁定，谷歌必须向符合条件的竞争对手开放部分 Android 系统功能与 Google 搜索数据，包括让竞争对手的 AI 助手获得与谷歌 Gemini 同等的系统级权限。 这一根据《数字市场法》做出的重大裁定可能重塑移动平台竞争格局，用户未来可将 ChatGPT 等第三方 AI 助手设为深度集成的系统助手，并迫使谷歌分享长期封闭的搜索数据。 谷歌可以根据隐私和安全标准评估申请访问 Android 功能的第三方服务，但相关限制必须符合欧盟规定。欧盟还表示将限制竞争对手使用共享搜索数据的方式以防止滥用。

telegram · zaihuapd · 7月16日 13:19

**背景**: 《数字市场法》是欧盟的一项反垄断法律，旨在限制被指定为“守门人”的大型在线平台的反竞争行为。谷歌 Gemini 是一款深度集成到 Android 系统中的多模态 AI 助手，提供系统级功能。该裁定将类似访问权限扩展到了竞争对手的 AI 助手。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Gemini">Google Gemini</a></li>
<li><a href="https://www.amz123.com/t/MM2J6D0e">欧盟数字法案GDPR&DMA... -AMZ123跨境导航</a></li>

</ul>
</details>

**标签**: `#欧盟`, `#数字市场法`, `#谷歌`, `#反垄断`, `#AI助手`

---

<a id="item-2"></a>
## [Kimi K3：开放前沿模型，参数规模巨大](https://www.kimi.com/blog/kimi-k3) ⭐️ 8.0/10

Kimi（Moonshot AI）发布了 K3，一个拥有 2.8 万亿参数的开源权重前沿 AI 模型，声称性能可与领先模型竞争。该模型通过 API 提供，输入/输出每百万 tokens 价格为 3/15 美元，显著高于典型的中国开源模型。 K3 标志着前沿 AI 商品化的重要一步，一家中国实验室发布了可与美国顶级对手竞争的开源模型。其高昂定价和巨大规模引发了关于该策略是否旨在将软件商品化以推销硬件基础设施的讨论。 K3 使用 2.8 万亿参数，使其成为迄今为止最大的开源权重模型，拥有 100 万 token 的上下文窗口。定价为每百万输入 token 3 美元，每百万输出 token 15 美元，缓存价格为每百万 token 0.3 美元，与 Anthropic 的 Sonnet 系列定价一致。

hackernews · vincent_s · 7月16日 14:46 · [社区讨论](https://news.ycombinator.com/item?id=48935342)

**背景**: 开源权重 AI 模型是指其训练参数（权重）公开发布供下载，允许用户运行、研究和修改模型。前沿模型代表了当时最先进的 AI 能力。Kimi K3 是最大的开源权重模型之一，拥有 2.8 万亿参数，远超常规规模。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.datacamp.com/blog/frontier-models">Frontier Models Explained: What Defines the Cutting Edge of AI</a></li>

</ul>
</details>

**社区讨论**: 社区成员注意到推理成本高昂；simonw 报告一次渲染使用了 1.3 万推理 token，花费 0.25 美元。softwaredoug 推测中国实验室正在将 AI 软件商品化以推动硬件销售，而 Tiberium 指出定价与 Anthropic 的 Sonnet 一致，但对中国开源模型而言偏高。m3h 强调 K3 是最大的开源模型，需要大量计算资源。

**标签**: `#AI`, `#language models`, `#frontier models`, `#open-weight`, `#Chinese AI`

---

<a id="item-3"></a>
## [LM Studio Bionic：开放模型的 AI 智能体](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 8.0/10

LM Studio 推出了 Bionic，这是一个 AI 智能体，允许用户利用开放模型进行编码和文档任务，并为文档更改提供自动检查点功能。 Bionic 代表着在使开放模型 AI 智能体更易用且更实用方面迈出的重要一步，它结合了易用性与强大的本地模型，特别适合关注成本和数据安全的用户。 Bionic 支持两种项目类型：用于编码的'Code'项目和用于文档创建的'Work'项目，其中 Work 项目具有自动检查点功能以跟踪每次更改。它可与 Qwen3.6 35B 等本地模型配合使用，并需要 LM Studio 账户。

hackernews · minimaxir · 7月16日 20:18 · [社区讨论](https://news.ycombinator.com/item?id=48939662)

**背景**: LM Studio 是一款桌面应用程序，允许用户在自己的机器上本地发现、下载和运行大型语言模型，无需互联网连接。AI 智能体是一种软件工具，能够通过与大语言模型和文件系统交互来自主执行编码或文档编辑等任务。Bionic 通过为开放模型提供专用的智能体框架，扩展了 LM Studio 的功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lmstudio.ai/download">Download LM Studio - Mac, Linux, Windows</a></li>
<li><a href="https://grokipedia.com/page/LM_Studio">LM Studio</a></li>

</ul>
</details>

**社区讨论**: 社区整体反应积极，用户如 inventor7777 称赞其熟悉的用户界面和本地模型的良好表现。一些用户请求添加系统级访问、本地网络搜索、SSH 支持以及模型加载指示器等功能。创始人 Yagil 参与其中，为使用特定模型的测试提供积分。

**标签**: `#AI agents`, `#open models`, `#local LLM`, `#LM Studio`

---

<a id="item-4"></a>
## [从 Rust 到 Zig 的编译器重写进度报告](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

作者正在将一个最初用 Rust 编写的编译器重写为 Zig 语言，理由是更好的增量构建时间和更灵活的内存管理。这篇博客详细介绍了进展和语言切换的理由。 这次重写凸显了系统编程语言中的重要权衡，尤其是对于性能和内存控制至关重要的编译器。它进一步推动了关于 Rust 的编译时安全性与 Zig 更实用的运行时安全性方法之间的持续辩论。 重写重点在于实现更快的增量构建和改进的交叉编译。与 Rust 严格的所有权模型不同，Zig 通过调试和发布安全模式下的运行时检查来提供内存安全，作者认为这对于二进制补丁等编译器任务更为合适。

hackernews · jorangreef · 7月16日 11:39 · [社区讨论](https://news.ycombinator.com/item?id=48933149)

**背景**: Rust 通过其所有权和借用规则在编译时强制内存安全，防止使用后释放和数据竞争。相比之下，Zig 提供更多底层控制，并带有可选的运行时安全检查，使其对需要灵活性的项目有吸引力。编译器经常执行不安全的操作，如生成机器代码或热补丁，这在 Rust 的严格模型下可能变得繁琐。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ziglang.org/learn/why_zig_rust_d_cpp/">Why Zig When There is Already C++, D, and Rust? ⚡ Zig Programming Language</a></li>
<li><a href="https://www.scattered-thoughts.net/writing/how-safe-is-zig/">How (memory) safe is zig?</a></li>

</ul>
</details>

**社区讨论**: 评论者提出了几个观点：steveklabnik 认为不安全操作并非普通编译所需，仅用于热补丁；landr0id 质疑 Zig 的运行时检查能否真正捕获使用后释放错误；其他人讨论了 Zig 增量构建速度的潜力，并质疑为何不选择 OCaml 作为实现语言。

**标签**: `#Rust`, `#Zig`, `#compiler`, `#memory safety`, `#systems programming`

---

<a id="item-5"></a>
## [交互式线性代数书籍动态可视化获好评](https://immersivemath.com/ila/) ⭐️ 8.0/10

这本交互式线性代数书最初于 2015 年在 immersivemath.com 发布，包含超过 100 个交互式图形，用户可操作向量和矩阵以建立几何直观。Hacker News 社区最近重新发现并高度赞扬了它，引发了关于交互式教育资源未来的讨论。 这本书展示了交互式可视化如何使抽象的数学概念更易懂，可能彻底改变数学教育。社区的热烈反响以及与 AI 工具的比较，凸显了对技术增强型学习材料的需求不断增长。 该书涵盖矩阵运算、特征值和特征向量等传统线性代数主题，但侧重于通过可操纵的 3D 图形提供几何直观。悬停时出现的工具提示解释关键概念，有助于在不打断阅读流的情况下理解内容。

hackernews · srean · 7月16日 15:32 · [社区讨论](https://news.ycombinator.com/item?id=48935951)

**背景**: 线性代数是数学的基础分支，对于计算机科学、物理和数据科学等领域至关重要。传统教科书通常使用静态图表，使得学生难以理解多维空间和变换。像这样的交互式书籍利用网络技术让读者实时探索对象，弥合了抽象公式与视觉直观之间的差距。

**社区讨论**: 评论者对这本书表达了极大的赞赏，有人感叹在学习时没有这样的资源。一位用户指出，像 LLM 这样的 AI 工具现在可以更容易地创建类似的交互式内容，可能彻底改变教科书的创作。还有人与其他新兴教育技术进行了比较，反映了动态学习材料的广泛趋势。

**标签**: `#interactive learning`, `#linear algebra`, `#math education`, `#visualization`, `#educational technology`

---

<a id="item-6"></a>
## [Firefox 通过 WebAssembly 在浏览器内运行](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 8.0/10

Puter 将 Mozilla 的 Firefox 浏览器（使用 Gecko 引擎）编译为 WebAssembly，使得整个 Firefox 实例可以在另一个浏览器内运行。 这展示了 WebAssembly 在浏览器内运行复杂、功能完备的应用程序（如浏览器）的巨大潜力，为跨浏览器虚拟化和云端桌面环境开辟了可能性。 该项目使用了 Gecko 引擎，因为它对单进程的支持较强；估计花费了价值 25,000 美元的 LLM 令牌，但由于订阅计划实际成本低得多；所有网络流量均通过 Wisp 协议经 Puter 的代理服务器传输。

rss · Simon Willison · 7月16日 23:34

**背景**: WebAssembly（WASM）是一种二进制指令格式，允许用 C++ 等语言编写的代码以接近原生速度在浏览器中运行。Gecko 引擎是 Mozilla 用于 Firefox 的浏览器引擎，使用 C++ 和 Rust 编写。将完整的浏览器引擎编译为 WASM 是一项重大的技术挑战，因为它体积庞大且复杂。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gecko_(browser_engine)">Gecko (browser engine)</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead...</a></li>

</ul>
</details>

**标签**: `#WebAssembly`, `#Firefox`, `#Browser`, `#Demo`, `#Compilation`

---

<a id="item-7"></a>
## [GPT-5.6 代码生成器漏洞可意外删除文件](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

GPT-5.6 的 Codex 模式存在漏洞，当以完全访问模式运行且无沙盒保护时，可能意外删除文件。模型在尝试设置临时目录时，会误删$HOME 目录。 这是一个关键的 AI 安全问题，可能导致数据丢失并削弱对 AI 编程代理的信任。它凸显了在授予编程代理系统级访问权限时，需要沙盒保护和人工审核。 该漏洞在启用完全访问模式且关闭沙盒保护（包括自动审查）时发生。模型试图覆盖$HOME 以设置临时目录，却意外删除了$HOME。

rss · Simon Willison · 7月16日 17:45

**背景**: OpenAI Codex 是一款 AI 驱动的编程代理，可执行代码审查和重构等任务。它提供不同的审批模式，包括无需用户提示即可进行更改的完全访问模式。沙盒保护（如 OpenShift 或 Docker 中的沙盒）可将代理隔离，防止对宿主系统造成损害。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/codex/">Codex - OpenAI</a></li>
<li><a href="https://developers.redhat.com/articles/2026/07/16/layered-sandboxing-ai-agents-openshift-and-openshell">Layered sandboxing for AI agents: OpenShift... | Red Hat Developer</a></li>
<li><a href="https://smartscope.blog/en/generative-ai/chatgpt/codex-cli-approval-modes-no-approval/">Codex CLI Auto Approve: Dangerously Skip Permissions Equivalent (2026) - SmartScope</a></li>

</ul>
</details>

**标签**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`

---

<a id="item-8"></a>
## [Thinking Machines Lab 发布开源权重 Inkling 模型](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

由 Mira Murati 领导的 Thinking Machines Lab 发布了 Inkling，一个采用 Apache-2.0 许可证的开源权重混合专家多模态模型，总参数 975B，激活参数 41B。 此次发布增强了美国的开源权重生态系统，为中国和其他实验室的模型提供了有竞争力的替代方案，并通过 Tinker 平台为微调提供了强大的基础。 Inkling 在 45 万亿个文本、图像、音频和视频 Token 上训练，但缺乏详细的模型卡和训练数据文档，限制了透明度。

rss · Simon Willison · 7月16日 15:35

**背景**: 混合专家（MoE）模型使用多个专门的子网络（专家）和门控机制，对每个输入仅激活部分参数，从而在保持推理高效的同时实现更大的总参数量。开源权重模型提供对训练后参数的公开访问，允许用户下载、运行并在自己的基础设施上微调模型，但可能不包含完整的训练流程或数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-weights`, `#language model`, `#mixture-of-experts`, `#multimodal`

---

<a id="item-9"></a>
## [Linus Torvalds 宣布 Linux 不反 AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linux 创始人 Linus Torvalds 在 Linux 媒体邮件列表中声明，Linux 内核项目并不反 AI，并认为 AI 是明确有用的工具。他强调，今天任何怀疑 AI 实用性的人很可能根本没有使用过它。 作为开源领域极具影响力的人物，Linus Torvalds 的这一直接声明有助于平息关于 AI 在 Linux 社区中角色的持续争论。这表明 AI 工具在最大的开源项目之一中受到欢迎，可能鼓励在开发工作流中更广泛地采用和集成 AI。 Torvalds 承认，即使一年前 AI 的实用性尚未“明确”确立，但现在已经毋庸置疑。他还指出，关于 AI 的其他问题，如其经济影响，仍然悬而未决。

rss · Simon Willison · 7月16日 13:26

**背景**: Linus Torvalds 是 Linux 内核的原创者及长期维护者，Linux 内核是最著名的开源软件项目之一。近年来，AI 和机器学习在软件开发中的使用引发了争议，一些开源社区对伦理影响、许可和潜在滥用表示担忧。Torvalds 的声明直接针对那些“真正讨厌 AI”的人，并强调了他作为顶层维护者的权威。

**标签**: `#linux`, `#ai`, `#open-source`, `#linus-torvalds`

---

<a id="item-10"></a>
## [ExTernD：实现近乎任意精度的三元大模型训练后量化](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 8.0/10

ExTernD 提出扩展秩三元分解方法用于大语言模型的训练后量化，将每个权重矩阵分解为两个三元矩阵和一个对角缩放矩阵，从而以仅小幅增加 VRAM 的代价实现任意精度。 该方法挑战了此前认为三元 PTQ 因固定矩阵大小而走不通的观点，实现了接近任意量化级别的精度同时保持高效性，有望在最小化精度损失的前提下实现高度压缩的大模型推理。 该分解使用两个三元矩阵和一个内部对角缩放矩阵，其中内部秩可以任意增大以控制精度。作者声称相比现有量化方法，VRAM 增加很小，且通过利用三元数学计算是值得的。

reddit · r/MachineLearning · /u/LMTLS5 · 7月16日 13:31

**背景**: 训练后量化（PTQ）通过将权重矩阵压缩为低比特表示（如三元值-1、0、+1）来减少大模型内存占用。传统三元量化强制固定矩阵大小，限制了精度。ExTernD 通过将矩阵分解为低秩三元因子的乘积来克服这一限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.13511">[2607.13511] ExTernD: Expanded-Rank Ternary Decomposition...</a></li>
<li><a href="https://arxiv.org/html/2607.13511">ExTernD: Expanded-Rank Ternary Decomposition Ternary LLM PTQ...</a></li>

</ul>
</details>

**标签**: `#quantization`, `#LLM`, `#ternary`, `#PTQ`, `#efficient inference`

---

<a id="item-11"></a>
## [知网将下架列 AI 为作者的论文](https://www.zaobao.com.sg/news/china/story20260716-9371836) ⭐️ 8.0/10

知网宣布将下架将 DeepSeek 等 AI 工具列为作者的论文，理由是不具备民事主体资格，无法对论文的真实性负责。 这一政策强化了学术诚信标准，明确 AI 不能作为署名作者，影响研究人员在出版物中披露 AI 使用的方式。 知网明确表示 AI 工具不具备民事主体资格，无法承担真实性、学术审查和追责等责任；使用 AI 的作者需在研究方法或致谢中说明。

telegram · zaihuapd · 7月16日 07:45

**背景**: 知网是中国主要的学术期刊平台。生成式 AI 的兴起导致一些论文将 AI 模型列为合著者，引发了关于署名和责任的讨论。许多出版商已更新政策，要求透明地说明 AI 的使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI authorship`, `#academic integrity`, `#CNKI`, `#DeepSeek`, `#policy`

---

<a id="item-12"></a>
## [日本购入 2.75 万块英伟达 Rubin 芯片打造机器人 AI](https://www.bloomberg.com/news/articles/2026-07-16/japan-to-buy-nvidia-rubin-chips-to-build-sovereign-ai-for-robots) ⭐️ 8.0/10

日本宣布计划购入 27500 块英伟达下一代 Rubin 芯片，由新成立的 Noetra 公司牵头建设大型数据中心，用于开发面向机器人的本土 AI 模型。该项目获得日本政府 3873 亿日元（约 240 亿美元）拨款，软银、Preferred Networks 和 NEC 等企业参与。 这一举措是日本减少对美中 AI 技术依赖、为机器人等关键领域建立‘主权 AI’的战略行动。若成功，日本有望在 2040 年前占据全球机器人市场 30%以上份额，并重塑 AI 发展的地缘格局。 Noetra 计划在 2027 年 3 月前发布首个 AI 模型，并在数年内推出机器人专用版本。Nvidia Rubin 架构在 GTC 2025 上发布，包含六款定制芯片，专为机架级 AI 超算设计，是 Hopper 和 Blackwell 架构的后继者。

telegram · zaihuapd · 7月16日 10:59

**背景**: Nvidia 的 Rubin 微架构是继 Blackwell 之后的新一代 AI 平台，包含六款专用芯片（如 Vera CPU、Rubin GPU、NVLink 交换机等），用于扩展 AI 工厂。‘主权 AI’指国家建立自己的 AI 能力——包括数据、模型和基础设施——以保持控制并减少对外国供应商的依赖，这已成为许多政府的优先事项。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rubin_(microarchitecture)">Rubin (microarchitecture) - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/">Inside the NVIDIA Vera Rubin Platform: Six New Chips, One AI Supercomputer | NVIDIA Technical Blog</a></li>
<li><a href="https://nordcloud.com/videos/ladybug-unplugged-sovereign-cloud-series-episode-3/">What Is Sovereign AI? Models, Control, and Why AI... - Nordcloud</a></li>

</ul>
</details>

**标签**: `#AI`, `#Nvidia`, `#Japan`, `#Robotics`, `#Sovereign AI`

---

<a id="item-13"></a>
## [台积电再投千亿美元赴美，Q2 利润飙升 77%](https://www.reuters.com/world/asia-pacific/tsmcs-second-quarter-profit-seen-hitting-record-ai-boom-2026-07-15/) ⭐️ 8.0/10

台积电宣布再投资 1000 亿美元在亚利桑那州建厂，二季度净利润同比增长 77%至 7066 亿新台币（约 220 亿美元），创历史新高。 这一巨额投资凸显了台积电在 AI 热潮中扩大美国布局的决心，而创纪录的利润则反映了对先进芯片的强劲需求，对全球半导体供应链影响深远。 台积电将 2026 年资本支出预测上调至 600 亿至 640 亿美元，并预计全年美元营收增长略超 40%。亚利桑那州目前已有 8 座工厂在建或规划中，未来可能再增 4 座。

telegram · zaihuapd · 7月16日 12:29

**背景**: 台积电是全球最大的专业独立半导体代工厂，为苹果、英伟达等公司供应芯片。为满足 AI 和高性能计算芯片的需求，台积电正全球扩张，其在亚利桑那州的工厂是分散台湾制造布局战略的一部分。

**标签**: `#半导体`, `#台积电`, `#投资`, `#AI`, `#财报`

---

<a id="item-14"></a>
## [Truth Social 将向华尔街出售特朗普实时帖子](https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street) ⭐️ 8.0/10

特朗普媒体科技集团宣布将于 8 月 1 日推出 Truth API，以毫秒级速度向机构客户提供排名前 10 账号（包括特朗普）的实时帖子，用于高频交易。 此举模糊了政治沟通与金融市场之间的界限，可能让交易员在公众之前从特朗普的政策声明中获利，引发严重的伦理和市场操纵担忧。 该 API 将以毫秒级延迟提供平台排名前 10 账号的帖子，TMTG 未公布定价。CNN 此前报道称，特朗普曾利用 Truth Social 宣传自己刚买入的股票。

telegram · zaihuapd · 7月17日 01:02

**背景**: 高频交易（HFT）使用强大算法在微秒内执行交易，通常依赖对新闻和数据的快速获取。Truth Social 已成为特朗普发布政策声明的主要渠道，这些声明历史上曾引发市场波动。向 HFT 公司出售特权数据访问权限可能使他们相对于普通投资者获得不公平优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2p6eUpQUEVSSGRmOWstMkZWM1dTZ0FQAQ?hl=en-GB&gl=GB&ceid=GB:en">Google News - Trump Media unveils Truth API for real-time post...</a></li>
<li><a href="https://en.wikipedia.org/wiki/High-frequency_trading">High-frequency trading</a></li>

</ul>
</details>

**标签**: `#Data API`, `#High-frequency trading`, `#Social media`, `#Truth Social`, `#Trump`

---