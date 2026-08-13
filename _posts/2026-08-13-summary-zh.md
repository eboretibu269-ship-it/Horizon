---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> 从 31 条内容中筛选出 9 条重要资讯。

---

1. [DeepSeek V4 Pro 0813：1.7T 参数开源权重模型发布](#item-1) ⭐️ 9.0/10
2. [谷歌发布 Gemini 3.7 Flash：高性价比视觉模型](#item-2) ⭐️ 8.0/10
3. [OpenAI 与 Cerebras 推出 GPT-5.6 Sol Ultrafast，速度快约 7 倍](#item-3) ⭐️ 8.0/10
4. [DRAM 意面化：未文档化功能暴露低层攻击面](#item-4) ⭐️ 8.0/10
5. [选择无聊技术：把创新筹码花在刀刃上](#item-5) ⭐️ 8.0/10
6. [DeepSeek 推出 MIT 许可的智能体框架，实现完整会话追踪](#item-6) ⭐️ 8.0/10
7. [DeepMind 发布手语转文字模型 SL2T，落地 Pixel 11](#item-7) ⭐️ 8.0/10
8. [DeepSeek 发布开源 Harness 及 V4-Pro-0813 权重](#item-8) ⭐️ 8.0/10
9. [OpenAI 预览 Ultrafast 模式，GPT-5.6 Sol 提速 14 倍](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DeepSeek V4 Pro 0813：1.7T 参数开源权重模型发布](https://simonwillison.net/2026/Aug/12/deepseek-v4-pro-0813/) ⭐️ 9.0/10

DeepSeek 发布了 DeepSeek V4 Pro 0813，先通过 OpenRouter 以 API 形式提供；随后其开放权重也已在 Hugging Face 上发布（deepseek-ai/DeepSeek-V4-Pro-0813），参数量为 1.7T，大小为 893 GB。 这是来自头部 AI 实验室的一次重要开放权重发布，让研究人员和开发者能够使用参数量高达 1.7T 的大型模型。这很可能推动开源 AI 生态中进一步的实验、微调和应用开发。 该模型最初仅通过 API 提供，DeepSeek 没有明显的官方公告页面。早期基准测试结果先在官方 DeepSeek 微信群中分享，后被转发到 Reddit（版主以“低质内容”为由删帖），再被复制到 Hacker News 上的 ASCII 艺术表格中。

rss · Simon Willison · 8月12日 23:59

**背景**: 开放权重模型是指将训练得到的模型参数（权重）公开发布，任何人都可以下载并运行。OpenRouter 是一个统一 API 服务，通过单个端点即可访问数百个语言模型。DeepSeek 是一家中国 AI 实验室，此前已发布过 DeepSeek-V4-Pro（4 月）和 DeepSeek-V4-Flash（7 月）等开放权重模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/docs/quickstart">OpenRouter Quickstart Guide</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**社区讨论**: 社区讨论较为分散：基准数据最初在 DeepSeek 官方微信群分享，随后被发布到 r/LocalLLaMA，但版主以“低质内容”为由删除了该帖，最后被复制到 Hacker News 讨论串中，以 ASCII 艺术表格形式呈现。整体氛围偏向好奇但不算热烈，目前还没有看到广泛的争论。

**标签**: `#AI`, `#DeepSeek`, `#LLM`, `#open-weights`, `#model-release`

---

<a id="item-2"></a>
## [谷歌发布 Gemini 3.7 Flash：高性价比视觉模型](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 8.0/10

谷歌 DeepMind 发布了 Gemini 3.7 Flash，这是一个具备视觉能力、主打成本效益的多模态模型，代码性能提升明显。它在文档理解与业务流程基准上显著超过上一代 3.6 Flash：GDP.pdf 为 34.0%对 22.0%，AutomationBench 为 30.4%对 17.0%。 在模型定价和发布节奏竞争白热化的当下，这次发布巩固了谷歌 Flash 系列作为高容量、重视觉与代码工作负载首选低成本层的地位。它也引发了与 GPT-5.6 Luna 等竞品的直接对比，部分用户认为 Luna 更便宜且在关键基准上更强。 Gemini 3.7 Flash 的首发定价将于 2027 年 1 月 1 日翻倍，调整为每 100 万输入 token 1.50 美元、每 100 万输出 token 7.50 美元。谷歌表示该模型还可与 Nano Banana 配合，实时动态生成角色、物品和纹理；此外，它距 3.6 Flash 发布仅三周，这也引发了关于模型更新换代速度的质疑。

hackernews · thisisauserid · 8月13日 17:23 · [社区讨论](https://news.ycombinator.com/item?id=49289112)

**背景**: Gemini 是谷歌 DeepMind 开发的多模态大语言模型系列，包含 Pro、Flash 和 Flash Lite 等不同层级。Flash 层级专为低成本、高吞吐、低延迟的场景设计，常用于摘要、解析、格式化以及视觉密集型任务，因此是 API 开发者常用的“工兵型”模型。Gemini 3.7 Flash 延续了这一系列，同时增强了代码与文档推理能力，定位介于旗舰前沿模型与更便宜的轻量选项之间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/">Gemini 3.7 Flash: our most intelligent workhorse model</a></li>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3.7 Flash — Google DeepMind</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_2.5_Flash_Image">Gemini 2.5 Flash Image</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有测试者发现 Gemini 3.7 Flash 在图像转 HTML 方面表现出色，但 Anthropic 的 Opus 仍是标杆；也有人质疑“首发定价”将在 2027 年初翻倍，且距 3.6 Flash 发布仅三周。多名用户认为 GPT-5.6 Luna 更便宜且在 DeepSWE 1.1 上得分更高，削弱了 Flash 的性价比；另有人指出该模型更像是对标 Terra 而非 Luna。

**标签**: `#AI`, `#Gemini`, `#Google`, `#LLM`, `#pricing`

---

<a id="item-3"></a>
## [OpenAI 与 Cerebras 推出 GPT-5.6 Sol Ultrafast，速度快约 7 倍](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

OpenAI 与 Cerebras 宣布推出 GPT-5.6 Sol Ultrafast——一个由 Cerebras 驱动的全新 OpenAI API 服务层级，每秒最多可输出 750 个 token。在 frontier 基准测试上，Ultrafast 的运行速度约为标准 GPT-5.6 Sol 的 7 倍，同时保持相当的准确性；该模式最初仅向部分精选客户开放。 推理速度是许多实时和交互式 AI 应用的瓶颈，此次合作表明在提供前沿模型质量的同时不必牺牲延迟。这也验证了 Cerebras 的晶圆级技术是 AI 推理领域的重要参与者，可能重塑模型提供商和硬件厂商之间的竞争格局。 Cerebras 和 OpenAI 声称与标准模型相比没有质量折损，但并没有明确说明输出是否完全一致。根据 Artificial Analysis 报告的输出速度，Ultrafast 比 Claude Fable 5 快 11 倍，比 Fast 模式下的 Claude Opus 4.8 快 5 倍；定价细节尚未公布。

hackernews · pr337h4m · 8月13日 18:10 · [社区讨论](https://news.ycombinator.com/item?id=49289844)

**背景**: Cerebras 制造晶圆级引擎（WSE），这是一块硅晶圆大小的单芯片，集成了计算、内存和互连，最初旨在加速深度学习训练。HLE（Humanity's Last Exam）和 GPQA 等前沿基准用极其困难的推理和科学问题来衡量 LLM，常被用来比较最先进的模型。这一公告是更大趋势的一部分：推理速度（而不仅仅是原始智能）正成为 AI 服务的关键差异点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT‑5.6 Sol at up to ... - OpenAI</a></li>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT-5.6 Sol Ultrafast with OpenAI - cerebras.ai</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cerebras">Cerebras - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对这次合作和速度提升感到兴奋，有人说他们一直在期待 OpenAI 和 Cerebras 合作带来‘了不起的东西’。也有人指出，公告中没有明确说明 Ultrafast 的输出与普通 Sol 完全一致，并且没有定价信息可能意味着价格非常高昂。还有人认为速度通过实现迭代思考提高了推理质量，提到人类会多次修正自己的想法。

**标签**: `#AI`, `#LLM`, `#Inference`, `#OpenAI`, `#Cerebras`

---

<a id="item-4"></a>
## [DRAM 意面化：未文档化功能暴露低层攻击面](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 8.0/10

安全研究员 Christopher Domas（xoreaxeaxeax）发布了名为“Spaghettifying DRAM”的项目，演示了如何利用未文档化的 DRAM 功能进行底层系统访问。该工作配合一场 Black Hat 演讲，并在 GitHub 仓库中提供了攻击细节。 这项研究揭示了 DRAM 的攻击面远比通常认为的更大，可能影响游戏主机安全和可信执行环境。从 ring-0 访问“负环”功能的能力，可能破坏受影响系统的硬件安全边界。 根据 README，该攻击适用于 AMD Jaguar（AMD16h，2013 年的低功耗架构），并注释称 Zen 3 的内存控制器寄存器基地址不同。该技术允许 ring-0 root 访问隐藏功能，但仓库未说明其他哪些处理器系列也受影响。

hackernews · matt_d · 8月13日 14:17 · [社区讨论](https://news.ycombinator.com/item?id=49286341)

**背景**: DRAM（动态随机存取存储器）是计算机的主存，由内存控制器管理，通常在启动时通过专有固件进行配置。现代 DRAM 控制器非常复杂，部分操作属于未文档化或保留功能。此前的研究如 Row Hammer 已证明 DRAM 的物理行为可被利用；本项目更进一步，通过普通软件直接操纵内存控制器寄存器，暴露了作者所称的“负环”领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49286341">Spaghettifying DRAM | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Row_hammer">Row hammer - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区反应热烈，用户对 Domas 以往的演讲表示赞赏，并指出 DRAM 日益复杂的安全问题。评论者还质疑哪些较新的 CPU 受影响，一些人推测 Xbox 和 PlayStation 的安全团队可能对游戏主机破解的影响感到担忧。

**标签**: `#security`, `#hardware`, `#DRAM`, `#exploitation`, `#hacking`

---

<a id="item-5"></a>
## [选择无聊技术：把创新筹码花在刀刃上](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

丹·麦金利（Dan McKinley）2015 年的文章《选择无聊技术》认为，公司应该优先采用成熟、被充分理解的技术，并把新技术的采用视为一种稀缺资源，即“创新筹码”。这篇文章提出了一个框架，后来成为软件工程和工程管理领域被广泛引用的参考文献。 文章提出的“创新筹码”概念为工程领导者提供了一种令人印象深刻的方式，用来论证保守的技术选择并向组织上下解释权衡。在 AI 时代，它的相关性反而增强，因为评论者认为，无聊技术在大语言模型训练数据中也有更充分的体现，因此 AI 智能体处理起来也更可靠。 麦金利在 Etsy 工作期间创造了这个术语，当时该公司使用 PHP 和 MySQL 等语言。这里的“无聊”并不等于过时，而是指有大量文档、充足人才储备以及故障模式被充分理解的技术。

hackernews · tosh · 8月13日 17:48 · [社区讨论](https://news.ycombinator.com/item?id=49289512)

**背景**: 这篇文章论证，每家公司可用于采用新技术的“创新筹码”是有限的，一旦花掉，要很久才能补充。因此，大多数工程问题应该用无聊技术来解决，把创新预算留给那些真正能带来竞争优势的新颖领域。这一概念已被许多工程组织采用，并催生了相关社区和评论，包括关于将其应用于 AI 智能体的讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.peal.dev/blog/boring-technology-principle-why-we-pick-proven-tools">The Boring Technology Principle: Why We Reach for... — peal.dev</a></li>
<li><a href="https://jonathannen.com/choose-boring-technology/">Still choose boring technology</a></li>
<li><a href="https://www.growingscrummasters.com/keywords/innovation-tokens/">Managing Innovation Tokens for Strategic Technical Change : Growing Scrum Masters</a></li>

</ul>
</details>

**社区讨论**: 评论者大多称赞这一框架；NickNaraghi 称它是自己作为产品经理和工程领导者职业生涯中最有用的概念之一，theptip 则把它应用到 AI 智能体上，建议使用“分布内技术”。然而，insanitybit 提出了反驳，认为“创新筹码”很随意，“新颖”或“新”只是很弱的代理指标，iand675 也附上了一篇书面反方观点。

**标签**: `#software-engineering`, `#technology-strategy`, `#innovation`, `#engineering-management`

---

<a id="item-6"></a>
## [DeepSeek 推出 MIT 许可的智能体框架，实现完整会话追踪](https://deepseek.com/harness/en/) ⭐️ 8.0/10

DeepSeek 发布了 DeepSeek Harness 的早期开发者预览版，这是一个采用 MIT 许可证的开源智能体框架。该预览版通过只追加的事件日志提供完整的会话可追溯性，支持回放、分支、恢复和搜索。 可追溯性是一个突出的特性，因为许多商业 AI 模型对其运行轨迹进行加密或混淆，限制了透明度和可调试性。通过以 MIT 许可证开源，DeepSeek 为开发者构建和审计可靠的 AI 智能体提供了一个强大的基础。 该框架采用基于 Cordis v4 的“一切皆插件”架构，支持插件热重载和动态启用/禁用，并自动清理状态和副作用。只追加的会话日志以统一事件流的形式记录系统提示、推理过程、工具调用、子智能体调度和上下文注入。

hackernews · bjin · 8月13日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49285244)

**背景**: 智能体框架是为大型语言模型提供支撑的软件基础设施，使其能够作为 AI 智能体运行，管理工具调用、记忆、状态持久化和执行环境。DeepSeek Harness 基于这一概念构建，延续了 DeepSeek 从开源权重模型到开源基础设施的趋势。该项目仍处于早期预览阶段，作者预计会存在粗糙之处和破坏兼容性的变更。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>
<li><a href="https://www.langchain.com/blog/the-anatomy-of-an-agent-harness">The Anatomy of an Agent Harness</a></li>
<li><a href="https://www.spanchain.dev/blog/how-to-audit-ai-agents">How to Audit AI Agents: From Mutable Logs to Tamper-Evident ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极但有所保留：一位评论者称可追溯性功能是“杀手级特性”，并对比了美国模型的加密轨迹；另一位则指出底层论文有用但并非革命性。作者承认这是早期预览版并欢迎反馈，还有几位用户分析了 Cordis v4 插件系统如何实现带状态清理的热重载。也有反对的声音表示对“一切皆插件”的架构感到厌倦。

**标签**: `#AI agents`, `#DeepSeek`, `#open source`, `#traceability`, `#developer tools`

---

<a id="item-7"></a>
## [DeepMind 发布手语转文字模型 SL2T，落地 Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

Google DeepMind 于 2026 年 8 月 12 日发布了多语言手语转文字模型 SL2T。该模型已首次落地消费产品，在 Pixel 11 的 Gboard 和 Live Transcribe 中支持将美国手语（ASL）实时转为英文文字。 这是首款大规模手语 AI 真正落地消费产品，是无障碍技术的重要里程碑。它有望让手语用户在短信、字幕等日常场景中更顺畅地与外界交流，后续还将扩展到更多设备和语言。 该模型使用了超过 10 万小时、涵盖 50 多种手语的数据进行训练。在 FLEURS-ASL 基准上，其零样本得分达 70 BLEURT，远超此前的纪录。为保护隐私，它只处理手部和身体姿态关键点，不读取原始视频。

telegram · zaihuapd · 8月13日 08:55

**背景**: 手语翻译长期以来依赖规模有限的数据集，且因手语的视觉特性而面临较大挑战。FLEURS-ASL 是 FLORES/FLEURS 多语言平行基准的扩展，它把美国手语纳入大规模多语言评测集。BLEURT 是建立在 BERT 基础上的神经文本生成评估指标，通过将候选译文与人工撰写的参考译文比较来打分。SL2T 使用姿态关键点——即身体动作的轻量数值表示——因此更具隐私性且更高效。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datanorth.ai/news/google-deepmind-releases-sl2t">Google DeepMind releases SL2T sign language AI - DataNorth</a></li>
<li><a href="https://interestingengineering.com/ai-robotics/google-sign-language-model-body-landmarks">Google's new model turns sign language into text for web searches</a></li>
<li><a href="https://arxiv.org/html/2408.13585">FLEURS-ASL: Including American Sign Language in Massively...</a></li>

</ul>
</details>

**标签**: `#sign language`, `#DeepMind`, `#AI model`, `#accessibility`, `#speech recognition`

---

<a id="item-8"></a>
## [DeepSeek 发布开源 Harness 及 V4-Pro-0813 权重](https://mp.weixin.qq.com/s/mANdGRI4fO_sEbC1ECEoZQ) ⭐️ 8.0/10

DeepSeek 以 MIT 协议发布了全新的 DeepSeek Harness 应用，并在 Hugging Face 上开放了 DeepSeek-V4-Pro-0813 权重。Harness 将模型、工具、技能、会话、沙箱、存储、调度和 UI 设计为可替换插件，提供标准、PTC、极简和创造四种运行模式。 此次发布对 AI Agent 生态意义重大，为开发者构建生产级 Agent 提供了模块化的开源基础。通过同时开源 Harness 和 V4-Pro 权重，DeepSeek 降低了实验和定制的门槛，有望加速基于 Agent 的应用创新。 DeepSeek Harness 基于 Cordis 的插件系统构建，其 GitHub 仓库现已公开。V4-Pro-0813 权重的 Hugging Face 页面当晚曾短暂返回 404 错误，随后已恢复。

telegram · zaihuapd · 8月13日 12:39

**背景**: Agent Harness 是一种将 AI 模型与工具、记忆和执行环境连接起来的框架，使其能够执行超越简单文本生成的复杂任务。DeepSeek 是一家以发布开源模型而闻名的 AI 研究公司，此次推出的 Harness 采用“一切皆插件”的架构，允许开发者独立定制每个组件。源代码以开发者预览版形式提供，欢迎社区贡献和进一步开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.deepseek.com/harness/en/">DeepSeek Harness developer preview: Everything is a plugin</a></li>
<li><a href="https://github.com/deepseek-ai/deepseek-harness">GitHub - deepseek-ai/deepseek-harness: DeepSeek Harness...</a></li>
<li><a href="https://dlcmh.github.io/">DeepSeek Agent Harness: Technical deep-dive & the open-source...</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#open-source`, `#AI`, `#model release`, `#Harness`

---

<a id="item-9"></a>
## [OpenAI 预览 Ultrafast 模式，GPT-5.6 Sol 提速 14 倍](https://openai.com/index/previewing-ultrafast/) ⭐️ 8.0/10

OpenAI 预览了一项名为 Ultrafast 的全新 API 服务层级，使 GPT-5.6 Sol 的处理速度比标准模式快至 14 倍。该服务由 Cerebras 驱动，每秒最多可输出 750 个 token，目前仅向 OpenAI API 中的少数客户开放限量预览。 这大幅降低了推理延迟，使前沿 AI 模型在故障响应、金融研究、客服和电商等对时间敏感的场景中更加实用。同时，这也标志着 OpenAI 与 Cerebras 的合作深化，凸显了除传统 GPU 之外的高速 AI 推理硬件替代方案。 Ultrafast 模式由 Cerebras 的晶圆级引擎（Wafer-Scale Engine）驱动，在不牺牲质量的情况下每秒最多可输出 750 个 token。该服务目前为限量预览，OpenAI 表示将随着算力扩充逐步扩大访问范围。

telegram · zaihuapd · 8月13日 17:04

**背景**: Cerebras 的晶圆级引擎是一种单片晶圆级集成处理器，集成了计算、内存和互连结构，专为超高速 AI 训练和推理设计。GPT-5.6 Sol 是 OpenAI GPT-5.6 系列中的旗舰模型，擅长复杂推理、编程和智能体工作流，并支持高达 100 万 token 的上下文。Ultrafast 模式利用 WSE 的高 token 生成速度，使最智能的模型能够在实时、对延迟敏感的应用中发挥作用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT‑5.6 Sol at up to ... - OpenAI</a></li>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT-5.6 Sol Ultrafast with OpenAI</a></li>
<li><a href="https://techcrunch.com/2026/08/13/openai-introduces-ultrafast-a-new-mode-that-makes-gpt-5-6-sol-work-at-14x-the-speed/">OpenAI introduces 'Ultrafast,' a new mode that makes GPT-5.6 ...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-5.6`, `#Ultrafast`, `#Cerebras`, `#AI性能`

---