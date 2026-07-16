---
layout: default
title: "Horizon Summary: 2026-07-16 (ZH)"
date: 2026-07-16
lang: zh
---

> 从 33 条内容中筛选出 11 条重要资讯。

---

1. [xAI 因隐私事件开源 Grok Build](#item-1) ⭐️ 9.0/10
2. [Claude web_fetch 漏洞导致记忆泄露](#item-2) ⭐️ 9.0/10
3. [xAI 起诉用户用 Grok 生成儿童虐待深度伪造](#item-3) ⭐️ 9.0/10
4. [Inkling：最大的开放权重音频模型发布](#item-4) ⭐️ 8.0/10
5. [在 13 年前 CPU 上以 5 tok/s 运行 Gemma 4 26B](#item-5) ⭐️ 8.0/10
6. [通过哈达玛乘积聚类解耦卷积神经元](#item-6) ⭐️ 8.0/10
7. [T4 比 A100 慢 170 倍：PyTorch 模型中的 4D 相关性瓶颈](#item-7) ⭐️ 8.0/10
8. [Google Play 将从 7 月 22 日起托管第三方应用商店](#item-8) ⭐️ 8.0/10
9. [DeepSeek 完成首轮融资，腾讯成第一大外部股东](#item-9) ⭐️ 8.0/10
10. [Telegram 推出机器人后端无服务器平台](#item-10) ⭐️ 8.0/10
11. [长鑫存储 2026 年产能将追平美光，中国成第二大 DRAM 产地](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [xAI 因隐私事件开源 Grok Build](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 9.0/10

由于 Grok CLI 工具存在严重隐私漏洞——会将整个目录上传至 Google Cloud 存储——引发社区强烈抗议后，xAI 已将整个 Grok Build 代码库以 Apache 2.0 许可证开源。 该事件凸显了 AI 驱动的开发者工具存在的严重隐私风险，并表明开源可以成为重建用户信任的战略举措，为 AI 编程助手市场的透明度树立了先例。 Grok Build 代码库包含 844,530 行 Rust 代码，其中仅有约 3% 是第三方依赖，并以单个提交发布，没有开发历史。仓库中包含一个自包含的 Mermaid 图表终端渲染器，以及受其他编码代理启发的工具实现。

rss · Simon Willison · 7月15日 23:59

**背景**: Grok CLI 是一款利用 xAI Grok 4 模型在终端中直接协助开发者完成编程任务的命令行工具。在开源之前，该工具为闭源软件，并存在一个漏洞：在某个目录下运行它时，会将整个目录（包括 SSH 密钥、密码管理器数据库等敏感文件）上传至 xAI 的 Google Cloud 存储桶。这引发了严重的隐私担忧，促使 xAI 删除了所有保留的用户数据并禁用了上传功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lalatenduswain.medium.com/automate-your-terminal-with-grok-cli-a-developers-guide-to-xai-s-ai-powered-tool-eb8e2b0460bf">Automate Your Terminal with Grok CLI: A Developer’s Guide... | Medium</a></li>
<li><a href="https://cloud.google.com/storage">Cloud Storage | Google Cloud</a></li>

</ul>
</details>

**社区讨论**: 社区成员反应不一：有人称赞代码质量和模型性能（例如优于 Opus 4.8），也有人批评数据泄露不可接受。迅速出现了多个分支项目，例如一个面向隐私的分支去除了遥测并阻止自动更新，表明用户希望有更值得信赖的替代方案。一些人认为开源是战术性举动，而非真正的隐私承诺。

**标签**: `#security`, `#open source`, `#AI`, `#CLI tool`, `#privacy`

---

<a id="item-2"></a>
## [Claude web_fetch 漏洞导致记忆泄露](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 9.0/10

安全研究员 Ayush Paul 发现 Anthropic 的 Claude web_fetch 工具存在绕过漏洞，攻击者通过构建蜜罐网站，诱使 AI 沿 URL 链导航，从而窃取用户私人数据（记忆），包括姓名、所在城市和雇主信息。 此次攻击展示了将私有用户数据访问与网页浏览功能相结合的 AI 助手存在的严重安全风险，损害了用户信任，并凸显了加强针对提示注入和数据窃取防护的必要性。 该漏洞利用了 web_fetch 工具能够跟随已获取页面中链接的功能；Anthropic 在披露前已通过移除该能力修补了漏洞，但拒绝支付漏洞奖金，因为他们声称内部已首先发现。

rss · Simon Willison · 7月15日 14:21

**背景**: Claude 的 web_fetch 工具设计为仅能获取用户明确提供或由配套 web_search 工具返回的 URL，以防止动态构建 URL 进行数据窃取。'致命三重奏'（lethal trifecta）指的是处理不可信输入、拥有私有数据访问权限以及具备外部数据外泄能力三者的结合。在此次攻击中，攻击者托管了一个蜜罐网站，该网站向 Claude 发出指令，导航到泄露数据的个性化 URL。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Sep/10/claude-web-fetch-tool/">Claude API: Web fetch tool</a></li>
<li><a href="https://www.osohq.com/learn/lethal-trifecta-ai-agent-security">Understanding the Lethal Trifecta of AI Agents</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论表达了对 AI 安全以及防止此类攻击难度的担忧；一些用户就 Anthropic 的漏洞奖励政策是否公平展开了辩论，而另一些用户则建议采取更广泛的缓解措施，例如限制网页工具的使用。

**标签**: `#AI Security`, `#Vulnerability`, `#Data Exfiltration`, `#Claude`, `#Prompt Injection`

---

<a id="item-3"></a>
## [xAI 起诉用户用 Grok 生成儿童虐待深度伪造](https://www.reuters.com/legal/litigation/musks-xai-sues-grok-user-over-sexualized-deepfakes-2026-07-15/) ⭐️ 9.0/10

xAI 对南卡罗来纳州男子 Terry Harwood 提起诉讼，指控其滥用 Grok AI 聊天机器人生成儿童性虐待材料和非自愿成人深度伪造，违反了服务条款。 这是首批 AI 公司因用户生成色情深度伪造而起诉用户的案件之一，为 AI 问责制和安全树立了重要的法律先例。 xAI 已暂停 52,222 个账户，向国家失踪与受虐儿童中心举报 73,604 次，促成至少 244 人被捕；诉讼要求赔偿并永久禁止 Harwood 使用 Grok。

telegram · zaihuapd · 7月16日 01:45

**背景**: Grok 是由埃隆·马斯克领导的 xAI 开发的 AI 聊天机器人。深度伪造是由 AI 生成的合成媒体，可以描绘真实人物在虚假场景中。该诉讼突显了生成式 AI 被用于非法内容以及 AI 提供商的法律责任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Deepfake">Deepfake - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#deepfakes`, `#legal precedent`, `#child protection`, `#xAI`

---

<a id="item-4"></a>
## [Inkling：最大的开放权重音频模型发布](https://thinkingmachines.ai/news/introducing-inkling/) ⭐️ 8.0/10

Thinking Machines Lab 发布了 Inkling，这是一个支持音频并通过 Tinker 平台进行微调的开放权重多模态模型，号称是目前最大的开放权重音频模型。 此次发布推动了音频领域的开放权重 AI，使企业能够以更低成本定制特定任务的模型，可能让先进的多模态 AI 更加普及。 Inkling 并非总体最强的模型，但因其多模态能力、高效推理以及可在 Tinker 上微调，非常适合作为定制化的基础。它支持音频输入，这在开放权重模型中较为罕见。

hackernews · vimarsh6739 · 7月15日 18:12 · [社区讨论](https://news.ycombinator.com/item?id=48924912)

**背景**: 开放权重模型意味着其核心组件公开发布，任何人可以下载、运行、研究和修改。多模态模型整合并处理多种数据类型，如文本、音频和图像，从而实现更全面的理解。Inkling 的发布结合了这些方面，提供了一个支持音频的开放权重多模态模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our open-weights model - Thinking Machines Lab</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Inkling 的音频能力表示兴趣，部分人分享了本地运行的链接。提供强大基础模型进行微调的业务模式受到称赞，但也有评论指出其在整体性能上落后于前沿模型。一位评论者希望开源模型最终能胜出。

**标签**: `#open-weights`, `#multimodal`, `#AI`, `#machine learning`, `#audio`

---

<a id="item-5"></a>
## [在 13 年前 CPU 上以 5 tok/s 运行 Gemma 4 26B](https://www.neomindlabs.com/2026/06/08/running-gemma-4-26b-at-5-tokens-sec-on-a-13-year-old-xeon-with-no-gpu/) ⭐️ 8.0/10

一位开发者展示了仅使用 13 年前的双路 Xeon CPU（无 GPU 加速），以每秒 5 个 token 的速度运行 Google 的 Gemma 4 26B MoE 模型进行推理。 这一演示表明大语言模型可以在非常旧的硬件上运行，挑战了本地推理必须使用 GPU 的假设，并可能降低实验和隐私敏感应用的门槛。 Gemma 4 26B（A4B）模型每个 token 仅激活 4B 参数，使其对 CPU 推理高效。在这样的旧硬件上达到 5 tok/s 很可能需要激进量化（例如 4 位）和优化软件。

hackernews · neomindryan · 7月15日 15:34 · [社区讨论](https://news.ycombinator.com/item?id=48922434)

**背景**: 大语言模型传统上由于计算需求而需要 GPU。然而，混合专家（MoE）、量化以及 CPU 优化的推理引擎等技术使得在 CPU 上运行模型成为可能，尽管速度较慢。Gemma 4 是 Google 最新的开放权重模型系列，包含多模态能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ollama.com/library/gemma4">gemma4</a></li>
<li><a href="https://insiderllm.com/guides/cpu-only-llms-what-actually-works/">CPU-Only LLMs: What Actually Works | InsiderLLM</a></li>
<li><a href="https://www.medoid.ai/blog/a-hands-on-walkthrough-on-model-quantization/">A Hands-On Walkthrough on Model Quantization - Medoid AI</a></li>

</ul>
</details>

**社区讨论**: 评论者就成本效益展开辩论，指出对于低速 CPU，云推理可能比本地电力成本更便宜。一些人分享了在旧硬件上以类似速度运行其他模型的经验，并预测更大的 MoE 模型很快将在消费级设备上运行。

**标签**: `#machine learning`, `#model optimization`, `#hardware`, `#inference`, `#cost analysis`

---

<a id="item-6"></a>
## [通过哈达玛乘积聚类解耦卷积神经元](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 8.0/10

一种新方法利用神经元感受野与其权重的哈达玛乘积进行聚类，揭示了 InceptionV1 中单个 1x1 卷积神经元检测到的模式，得到了清晰的单语义簇，如汽车、猫和狗。 这项工作通过提供卷积神经元的更细粒度分解推进了机制可解释性，帮助研究人员理解视觉模型如何编码概念。它还揭示了梯度下降如何有意抑制低激活模式，为模型行为提供了洞见。 该方法对输入感受野与神经元权重向量的逐元素乘积进行聚类，每个神经元产生多个单语义簇。低激活簇（如字母）显示从属神经元的正负权重平衡，表明梯度下降的主动抑制。

reddit · r/MachineLearning · /u/narang_27 · 7月15日 06:59

**背景**: 机制可解释性旨在通过分析神经网络内部结构来逆向工程，类似于理解传统软件。哈达玛乘积（逐元素乘法）在此用于计算神经元“看到”的内容。单语义性指神经元检测单个可解释概念。先前关于单语义性的工作主要集中在语言模型上，本研究将其扩展到卷积神经网络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hadamard_product_(matrices)">Hadamard product (matrices) - Wikipedia</a></li>
<li><a href="https://transformer-circuits.pub/2024/scaling-monosemanticity/">Scaling Monosemanticity: Extracting Interpretable Features from Claude 3 Sonnet</a></li>

</ul>
</details>

**社区讨论**: Reddit 帖子表达了对社区对卷积神经元可解释性兴趣不大的失望，作者表示可能转向语言模型。未提供具体评论，但整体情绪是参与度有限。

**标签**: `#mechanistic interpretability`, `#convolutional neural networks`, `#neuron analysis`, `#monosemanticity`, `#interpretability`

---

<a id="item-7"></a>
## [T4 比 A100 慢 170 倍：PyTorch 模型中的 4D 相关性瓶颈](https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/) ⭐️ 8.0/10

用户报告称，在纯 FP32 模式下运行一个使用 4D 相关体积和变换器的点跟踪模型时，NVIDIA T4 GPU 相比 A100 GPU 慢了 170 倍。 这一极端性能差距揭示了 GPU 代际迁移中一个关键且不易察觉的瓶颈，很可能源于内存带宽差异以及 T4 缺乏针对 FP32 操作的 Tensor Core。 模型在 T4 上的 GPU 利用率达到 99%，排除了利用不足的可能，且两个独立的 T4 机器上均出现相同的减速。其架构包括构建局部 4D 相关体积（帧间密集匹配）和后续的变换器层。

reddit · r/MachineLearning · /u/Future-Structure-296 · 7月15日 13:44

**背景**: 4D 相关体积存储两个特征图之间所有网格位置对的相似性分数，支持光流和点跟踪等任务的密集匹配。T4 GPU 缺少针对 FP32 的 Tensor Core（仅支持 FP16/INT8），而 A100 拥有专用的 FP32 Tensor Core，且 A100 还提供更高的内存带宽（1.5 TB/s 对比 300 GB/s），这对相关体积计算至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://discuss.pytorch.org/t/could-pytorch-provide-correlation-operator/84030">Could pytorch provide correlation operator? - vision - PyTorch Forums</a></li>
<li><a href="https://arxiv.org/html/2507.06233">AnthroTAP: Learning Point Tracking with Real-World Motion</a></li>

</ul>
</details>

**标签**: `#PyTorch`, `#GPU performance`, `#A100`, `#T4`, `#hardware bottlenecks`

---

<a id="item-8"></a>
## [Google Play 将从 7 月 22 日起托管第三方应用商店](https://www.theverge.com/policy/965792/google-epic-withdraw-injunction-third-party-app-stores-coming-google-play) ⭐️ 8.0/10

Google 与 Epic Games 已共同撤回修改反垄断禁令的动议，Google 将于 2026 年 7 月 22 日起在 Google Play 中托管第三方应用商店。 这标志着因反垄断诉讼，Google 应用商店政策发生重大转变，可能重塑 Android 应用分发格局，并为用户提供更多选择。 第三方应用商店需每年支付 5000 美元的安全审查费，仅限美国地区，并需满足对开发者开放、明确的信任与安全政策等要求。

telegram · zaihuapd · 7月15日 11:15

**背景**: 这一变化源于 Epic Games 诉 Google 反垄断案，法院要求 Google 允许竞争性应用商店在其平台上运营。Google 最初上诉，但后来与 Epic 达成和解，导致即将实施的这一政策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://9to5google.com/2026/07/15/google-play-store-third-party-android-app-store-changes-july/">Google opens the floodgates to third-party app stores on Android</a></li>
<li><a href="https://www.engadget.com/2215452/google-allow-third-party-app-stores-android-july-22/">Google Will Allow Third-Party App Stores On Android Next Week</a></li>
<li><a href="https://www.cnet.com/tech/google-play-third-party-app-stores-android/">Google Play Opens the Door to Third-Party App Stores... - CNET</a></li>

</ul>
</details>

**标签**: `#Google Play`, `#Epic Games`, `#antitrust`, `#app stores`, `#Android`

---

<a id="item-9"></a>
## [DeepSeek 完成首轮融资，腾讯成第一大外部股东](https://www.cls.cn/detail/2427193) ⭐️ 8.0/10

深度求索关联公司近日完成工商变更，新增腾讯等投资者，腾讯成为第一大外部股东。公司同时宣布将于本月中旬推出完整版 DeepSeek-V4 模型。 腾讯通过持股平台合计持有超 33%份额，成为第一大外部股东；其他投资者包括蔚来、京东、IDG 以及国家人工智能产业投资基金。深度求索还启动了大规模招聘，涵盖 Agent、代码智能体和底层算力框架等方向。

telegram · zaihuapd · 7月15日 12:56

**背景**: DeepSeek 是一家于 2023 年 7 月由梁文锋创立的中国 AI 公司，由对冲基金幻方量化所有。该公司因发布低成本开源模型（如 DeepSeek-R1）而受到关注，其训练成本远低于 GPT-4 但性能相当。公司采用专家混合等技术，并在出口限制下使用性能较弱的 AI 芯片，但仍实现了具有竞争力的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>
<li><a href="https://www.deepseek.com/en/">DeepSeek</a></li>
<li><a href="https://api-docs.deepseek.com/news/news260424/">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>

</ul>
</details>

**标签**: `#AI`, `#DeepSeek`, `#Funding`, `#Tencent`, `#Large Language Models`

---

<a id="item-10"></a>
## [Telegram 推出机器人后端无服务器平台](https://core.telegram.org/bots/serverless) ⭐️ 8.0/10

Telegram 推出无服务器平台，允许开发者将机器人和 Mini App 的后端代码直接部署在 Telegram 的基础设施上，无需自行管理服务器。该平台使用 V8 沙箱执行代码，并内置 SQLite 数据库。 这极大简化了机器人开发流程，降低了运维负担，可能吸引更多开发者加入 Telegram 生态系统。同时顺应了无服务器计算的行业趋势，使 Telegram 在与 Discord 和 Slack 等平台的竞争中更具优势。 部署只需一条命令 'npx tgcloud push'，使用标准 JavaScript 模块。代码在紧邻 Bot API 的隔离 V8 沙箱中运行，每个机器人自带内置 SQLite 数据库。

telegram · zaihuapd · 7月15日 16:00

**背景**: 无服务器计算允许开发者运行代码而无需配置或管理服务器，由云服务商负责扩展和维护。Telegram 的新平台使用 V8 沙箱隔离技术，该技术以安全执行不受信任的 JavaScript 代码而闻名。这与 Cloudflare Workers 等其他无服务器平台的运作方式类似，但直接集成到 Telegram 的机器人生态中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.generative.inc/ai-agent-sandboxes-the-infrastructure-layer-every-builder-needs-to-understand">AI Agent Sandboxes: Infrastructure Guide 2026 | Generative, Inc.</a></li>
<li><a href="https://www.ftandy.dev/posts/system-design-liteweight-lambda">System Design Look Back - Serverless and Sandbox</a></li>

</ul>
</details>

**标签**: `#Telegram`, `#Serverless`, `#机器人`, `#云平台`

---

<a id="item-11"></a>
## [长鑫存储 2026 年产能将追平美光，中国成第二大 DRAM 产地](https://www.tomshardware.com/pc-components/dram/cxmt-close-to-matching-microns-memory-capacity-in-2026-research-claims-would-put-china-on-track-to-become-worlds-second-largest-dram-producer) ⭐️ 8.0/10

Citrini Research 预测，长鑫存储（CXMT）将在 2026 年底达到约 35 万片/月的 DRAM 产能，逼近美光的 37.5 万片/月，届时中国将成为全球第二大 DRAM 生产基地。 这一变化可能重塑全球 DRAM 供应格局，减少对三星、SK 海力士和美光的依赖，并可能稳定价格。然而，浸没式 DUV 光刻设备的出口限制构成了重大瓶颈。 如果所有规划中的扩产（包括昇维旭、晋华集成和 XMC）都实现，中国 DRAM 总产能（不含外资工厂）可达 60 万片/月。MATCH 法案可能阻止先进浸没式 DUV 出口，阻碍短期增长。

telegram · zaihuapd · 7月16日 02:30

**背景**: DRAM（动态随机存取存储器）是用于计算机、服务器和移动设备的关键存储芯片。浸没式 DUV 光刻通过在镜头和晶圆之间加液体层实现更精细的图案，对于先进 DRAM 节点至关重要。MATCH 法案是美国旨在堵住对华半导体出口管制漏洞的法案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.asml.com/en/products/duv-lithography-systems">DUV lithography systems | Products</a></li>
<li><a href="https://cryptobriefing.com/cxmt-us-export-control-challenges/">Changxin Memory Technologies faces US export control challenges...</a></li>
<li><a href="https://nltimes.nl/2026/06/24/dutch-government-irritated-us-plans-new-asml-export-restrictions">Dutch government irritated by U.S. plans for new ASML export...</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#semiconductor`, `#China`, `#memory manufacturing`, `#geopolitics`

---