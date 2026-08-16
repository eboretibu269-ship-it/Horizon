---
layout: default
title: "Horizon Summary: 2026-08-16 (ZH)"
date: 2026-08-16
lang: zh
---

> 从 28 条内容中筛选出 5 条重要资讯。

---

1. [Anthropic 发布 Claude 系统提示词，引发社区深度分析](#item-1) ⭐️ 8.0/10
2. [AI 模型故意变‘笨’以减少幻觉](#item-2) ⭐️ 8.0/10
3. [Cloudflare 在切换域名服务器时静默注入分析脚本](#item-3) ⭐️ 8.0/10
4. [Qwen 3.8 27B：出色的开源视觉 LLM，但默认过度思考](#item-4) ⭐️ 8.0/10
5. [Anthropic 第二季营收暴涨至 115 亿美元，增 14 倍，扭亏为盈](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic 发布 Claude 系统提示词，引发社区深度分析](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 8.0/10

Anthropic 在文档站发布了 Claude 模型所使用的详细系统提示词，前所未有地展示了模型行为的指令方式。该发布包含带版本号的更新说明，社区成员如 Simon Willison 已开始追踪 Opus 4.8 与 Opus 5 之间的变化。 这种透明度意义重大，因为系统提示词通常被 AI 实验室保密，而理解它们有助于开发者、安全研究人员和用户评估模型行为是如何被塑造的。这也引发了关于 AI 安全、提示词演变，以及这些提示词究竟体现的是“智能”还是工程约束的讨论。 提示词中的值得注意的细节包括：要求 Claude 验证图片是否真的存在，以及一条危机处理规则，即在用户处于危机时优先考虑其福祉而非完成任务。通过 git-diff 的社区分析揭示了诸如在 Opus 5 提示词中提到 'Claude Fable 5 and Claude Mythos 5' 等更新。

hackernews · tosh · 8月16日 12:48 · [社区讨论](https://news.ycombinator.com/item?id=49319556)

**背景**: 系统提示词（system prompt）是在用户查询之前发送给大语言模型的初始指令，用于定义模型的角色、行为、语气、约束和界限。它优先于用户输入，部署者用它来保证跨上下文的一致响应。提示工程（prompt engineering）就是编写和优化这些输入以获得期望输出的实践。通过发布这些提示词，Anthropic 让人们看到了对话式 AI 应用“隐形基础”的内部。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://promptengineering.org/system-prompts-in-large-language-models/">System Prompts in Large Language Models</a></li>
<li><a href="https://www.ibm.com/think/topics/prompt-engineering">What Is Prompt Engineering? | IBM</a></li>

</ul>
</details>

**社区讨论**: 社区成员对这次透明度给予了积极回应，Simon Willison 还建立了一个 git 历史追踪器来查看变化。一些评论者借此机会对平台移除负面 AI 报道表示担忧，另一些人则讨论这些提示词究竟展现了真正的智能还是仅仅只是工程护栏。

**标签**: `#AI`, `#Claude`, `#System Prompts`, `#Anthropic`, `#LLM`

---

<a id="item-2"></a>
## [AI 模型故意变‘笨’以减少幻觉](https://w4g1.dev/blog/models-are-getting-dumber-on-purpose) ⭐️ 8.0/10

这篇文章认为，AI 模型正有意从记住事实转向依赖外部工具和检索，从而在独立的基准测试中显得‘更笨’。这种设计选择以牺牲原始的召回能力为代价，换取更少的幻觉和对最新信息的更好获取。 这一趋势使评估 LLM 变得更加复杂，因为衡量内置知识的基准可能不再反映真实世界的能力。它还引发了关于推理是否能与事实基础分离的讨论，影响 AI 的部署和研究方向。 文章特别指出，将知识外包给工具可以减少幻觉，但会让评估变得更难，因为模型在 SimpleQA 等事实召回测试中的表现会变差。社区评论者也提醒，像 Gemini 2.5 Pro 这样的示例模型已经过时，而且推理通常依赖于事实。

hackernews · hruvhwe · 8月16日 19:04 · [社区讨论](https://news.ycombinator.com/item?id=49322695)

**背景**: 检索增强生成（RAG）是一种让 LLM 在回答前从外部来源获取相关信息技术，有助于减少幻觉并保持回答更新。工具增强语言模型（TALM）通过让模型调用 API 和与外部状态交互，扩展了这一思路。这些方法预示着一个未来：LLM 携带更少的静态知识，转而查询动态的外部工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval-augmented generation</a></li>
<li><a href="https://arxiv.org/abs/2205.12255">[2205.12255] TALM: Tool Augmented Language Models</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对这个论点展开讨论，有人希望未来能有可插拔的知识库，让用户能更换特定领域的模块。另一些人指出文章中的基准已过时，还有人质疑推理是否真能与事实分离，认为关于人类行为的推理需要事实依据。

**标签**: `#AI`, `#LLMs`, `#tool-use`, `#knowledge`, `#benchmarks`

---

<a id="item-3"></a>
## [Cloudflare 在切换域名服务器时静默注入分析脚本](https://news.ycombinator.com/item?id=49322107) ⭐️ 8.0/10

一位 Hacker News 用户报告称，在将域名服务器切换到 Cloudflare 以便通过自定义子域名提供 R2 存储桶内容后，Cloudflare 自动向其纯 HTML、无 JavaScript 的网站 textlog.cc 注入了 Web Analytics 脚本。该脚本只能通过手动进入 Analytics 仪表板、添加站点并禁用它来移除，而且没有任何选择加入（opt-in）的提示。 此事之所以重要，是因为一家大型 CDN 和 DNS 提供商默认启用第三方跟踪 beacon，并且采取“默认开启、需手动退出”的流程，哪怕用户只想使用 DNS 或 R2 存储。这引发了透明度和隐私方面的担忧，也可能促使网站所有者审查被注入的 HTML 或强制使用 CSP 策略。 评论中展示的注入 beacon 来自 static.cloudflareinsights.com/beacon.min.js，并带有包含版本号和 token 的 data-cf-beacon 数据。多位评论者指出，这一行为会在新域名上启用 Cloudflare Web Analytics 时出现；还有人指出，只有在 Cloudflare 代理 HTTPS 流量时才有可能注入 HTML，纯 DNS 模式下不会发生。

hackernews · stagas · 8月16日 17:49

**背景**: Cloudflare Web Analytics（又称 Real User Monitoring，RUM）是一款注重隐私的分析产品，既可以通过 JavaScript 片段安装，也可以在 Cloudflare 代理站点时自动注入。当域名切换到 Cloudflare 的域名服务器后，该区域可以被设置为“已代理（proxied）”，使 Cloudflare 位于源服务器之前，并能修改 HTTP 响应，包括插入分析 beacon。R2 是 Cloudflare 的对象存储服务，关联到存储桶的自定义域名正是通过这条代理路径来提供内容的。如果站点只用 Cloudflare 来做 DNS 而没有启用代理，通常不会收到被注入的脚本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.cloudflare.com/web-analytics/get-started/">Enabling Cloudflare Web Analytics · Cloudflare Web Analytics docs</a></li>
<li><a href="https://burgeonlab.com/blog/cloudflare-web-analytics-rum-injected-tracking-beacon-script-into-my-sites/">Cloudflare Auto Injected Tracking Scripts To My Sites</a></li>
<li><a href="https://developers.cloudflare.com/r2/buckets/public-buckets/">Public buckets · Cloudflare R2 docs</a></li>

</ul>
</details>

**社区讨论**: 评论者大多证实了这一报告并分享了缓解方法，有人建议使用只允许加载本站脚本的 Content-Security-Policy。还有人引用了 Cloudflare 的“RUM diaries”文章；另有人指出，注入现象说明用户使用了 Cloudflare 的 HTTPS 代理；还有人观察到，新添加的域名可能默认就启用了 Web Analytics。

**标签**: `#cloudflare`, `#privacy`, `#analytics`, `#javascript`, `#dns`

---

<a id="item-4"></a>
## [Qwen 3.8 27B：出色的开源视觉 LLM，但默认过度思考](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 8.0/10

阿里巴巴 Qwen 实验室发布了 Qwen 3.8 27B，这是一款采用 Apache-2.0 许可的 27B 参数视觉语言模型，据其自报基准，性能超过了 Qwen 3.6 27B 和闭权的 Qwen 3.7-Plus。该模型默认使用最高推理强度（'xhigh'），即使是简单提示也会产生极长的思考过程。 Qwen 3.8 27B 是罕见的、可运行在单张消费级 GPU 上的开源权重前沿模型，使先进的视觉语言能力可以本地使用。但其默认的'xhigh'推理模式会产生荒谬的长思考时间，凸显了推理强度默认值对实际可用性的影响。 作者通过 LM Studio 和 llama-server 测试了 17GB 的 Q4_K_M 量化 GGUF，并将上下文窗口从默认的 8,192 提高到完整的 262,144 个 token，以避免在琐碎提示上耗尽 token。一个生成的 SVG 提示花了 21 分钟，使用了 22,276 个推理 token 才生成 3,223 个输出 token。

rss · Simon Willison · 8月16日 22:00

**背景**: 视觉语言模型（VLM）是一种多模态 AI，能够理解图像和文本，扩展了传统仅文本 LLM 的能力。'开放权重（open-weight）'意味着模型的训练参数可以公开下载，不同于像 Qwen 3.7-Plus 这样内部细节保密的闭源模型。包括 Qwen 在内的许多开放权重模型提供'reasoning_effort'参数来在思考深度和速度之间取舍；Qwen 3.8 27B 莫名其妙地默认使用最高档，导致过度思考。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://www.yottalabs.ai/post/qwen-3-8-27b-specs-hardware-requirements-how-to-run-2026">Qwen 3.8 27B: Specs, Hardware Requirements, and How to Run It (2026) | Yotta Labs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vision-language_model">Vision-language model - Wikipedia</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Qwen`, `#open-source`, `#benchmarks`, `#local-AI`

---

<a id="item-5"></a>
## [Anthropic 第二季营收暴涨至 115 亿美元，增 14 倍，扭亏为盈](https://www.cnbc.com/2026/08/15/anthropic-revenue-jumps-to-over-11point5-billion-in-q2-report.html) ⭐️ 8.0/10

Anthropic 公布第二季初步营收超过 115 亿美元，同比增长逾 14 倍，并实现调整后营业利润转正。该公司正准备可能于今秋启动的 IPO。 这标志着领先 AI 公司 Anthropic 的一个重大财务里程碑，展现出超高速增长和向盈利转变的趋势。其潜在的 IPO 可能对 AI 投资格局和更广泛的科技市场产生重大影响。 这些数字为初步数据，仍可能调整。营收高于 2025 年第二季的 7.87 亿美元和 2026 年第一季的 47.3 亿美元，显示出强劲的环比加速增长。

telegram · zaihuapd · 8月16日 07:26

**背景**: Anthropic 是一家领先的 AI 研究与安全公司，以其 Claude 大语言模型而闻名。该公司与 OpenAI 等企业在快速增长的生成式 AI 市场中竞争，投资者正密切关注其在潜在 IPO 前是否展现出可持续增长和盈利能力的迹象。

**标签**: `#Anthropic`, `#AI industry`, `#Revenue`, `#IPO`, `#Business`

---