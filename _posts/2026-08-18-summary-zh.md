---
layout: default
title: "Horizon Summary: 2026-08-18 (ZH)"
date: 2026-08-18
lang: zh
---

> 从 29 条内容中筛选出 4 条重要资讯。

---

1. [Mojo 编程语言开源，采用 Apache 2.0 许可证](#item-1) ⭐️ 9.0/10
2. [塞思·戈丁：亚马逊的搜索结果向消费者征收隐性‘税’](#item-2) ⭐️ 8.0/10
3. [Linux 7.3 提升显卡显存耗尽时的性能](#item-3) ⭐️ 8.0/10
4. [Qwen 3.8 27B 在 AI 指数上获 52 分，与更大模型持平](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Mojo 编程语言开源，采用 Apache 2.0 许可证](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 9.0/10

2026 年 8 月 18 日，Modular 在发布 Mojo 1.0 后，将 Mojo 编译器与工具链以 Apache 2.0 许可证正式开源。这兑现了该公司自 2023 年 5 月以来的开源承诺。 Mojo 是备受瞩目的编程语言，目标是结合 Python 的易用性与 C 级别性能，对 AI/ML 和系统编程具有重要意义。以宽松许可证开源编译器有望加速生态发展，使 Mojo 成为 GPU 计算领域 C++ 和 CUDA 的可行替代方案。 Mojo 最初“成为 Python 完整超集”的计划已在 2025 年 8 月左右被放弃，现在它是一种独立语言，采用类似 Python 的语法，并针对 GPU 编程优化。该语言还具备借鉴自 Rust 的静态类型和借用检查器等特性。

rss · Simon Willison · 8月18日 21:39

**背景**: Mojo 是 Modular 公司开发的系统编程语言，首次发布于 2023 年 5 月。它采用类似 Python 的语法，同时加入手动内存管理和借用检查器等底层能力，类似 Rust，但更易用。最初它被定位为 Python 的超集，后转变为专注于 GPU 与 AI 负载的独立语言。此次 1.0 发布并开源是该项目的重要里程碑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language) - Wikipedia</a></li>
<li><a href="https://www.infoworld.com/article/4081105/revisiting-mojo-a-faster-python.html">Revisiting Mojo: A faster Python? | InfoWorld</a></li>

</ul>
</details>

**标签**: `#Mojo`, `#Open Source`, `#Programming Languages`, `#AI/ML`, `#Python`

---

<a id="item-2"></a>
## [塞思·戈丁：亚马逊的搜索结果向消费者征收隐性‘税’](https://seths.blog/2026/08/the-amazon-tax/) ⭐️ 8.0/10

2026 年 8 月，塞思·戈丁发表博客文章，指出亚马逊的搜索结果已从帮助消费者找到最佳产品，转变为推销亚马逊自己想要销售的商品。他认为，这种转变以广告和操控排名的方式，向消费者征收了一种隐性‘税’。 这一批评很重要，因为它揭示了在世界上最大的电商平台上，广告驱动的搜索设计如何侵蚀消费者的信任与选择。这一讨论反映出用户对平台激励机制的认知不断增强，并可能加速用户向其他购物渠道迁移。 戈丁指出，即使亚马逊知道某个查询（如‘空气炸锅’）中评价最好、退货率最低的产品，它仍会展示广告，引导顾客选择其他选项。社区评论称，亚马逊搜索结果中大约四分之三是赞助广告，避开这些广告‘雷区’已成为一件令人头痛的事。

hackernews · herbertl · 8月18日 13:22 · [社区讨论](https://news.ycombinator.com/item?id=49345263)

**背景**: 亚马逊的产品排名由 A9 搜索算法决定，该算法优先考量销售表现和转化率，而非简单的关键词相关性。Sponsored Products（赞助商品）是出现在自然列表旁边的按点击付费广告，使得付费与自然结果之间的界限变得模糊。在此语境下，‘亚马逊税’是一个隐喻，指的是当搜索结果以亚马逊的广告收入而非消费者意图为优化目标时，消费者在金钱、时间和信任上付出的额外成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://salesduo.com/blog/amazon-a9-search-engine-guide/">Amazon A9 Algorithm: How Amazon’s Search Engine Works (2026)</a></li>
<li><a href="https://www.repricerexpress.com/amazons-algorithm-a9/">Understanding Amazon's A9 Algorithm: Boost Your Product Rankings</a></li>
<li><a href="https://advertising.amazon.com/solutions/products/sponsored-products">Sponsored Products - Help increase product sales | Amazon Ads</a></li>

</ul>
</details>

**社区讨论**: 评论普遍同意戈丁的观点，有用户指出，搜索已经从‘定位我想找的精确商品’演变为‘给我看一列语义搜索结果’，而平台正悄无声息地引导用户购买它想卖的东西。另一名用户表示，由于质量明显下滑，正在考虑注销使用了 15 年的亚马逊账户；还有用户报告称，约 75%的搜索结果都是赞助广告。也有评论者提出疑问：如果不投放广告，一款新品、高质量的空气炸锅如何脱颖而出？

**标签**: `#e-commerce`, `#search`, `#ads`, `#platform design`, `#consumer behavior`

---

<a id="item-3"></a>
## [Linux 7.3 提升显卡显存耗尽时的性能](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 8.0/10

Linux 7.3 内核版本将引入由 Valve 工程师 Natalie Vock 提交的早期 vRAM 管理代码。该工作旨在显存耗尽时更好地利用系统内存作为后备，从而提升性能。 显存耗尽在 8GB 及以下显存的 GPU 上是很常见的瓶颈，导致活动游戏数据被移到较慢的系统内存（GTT），而不是逐出后台应用。这项改进可为使用低显存 AMD GPU 的 Linux 玩家带来可观的帧率提升和更流畅的体验。 Linux 7.3 将包含这项 vRAM 管理工作的早期部分，并基于 Valve 工程师 Natalie Vock 此前改善低显存 GPU 的补丁。这些改动主要针对物理显存被超额使用的场景，相关补丁此前已提交到内核邮件列表并被接受。

hackernews · flaburgan · 8月18日 07:51 · [社区讨论](https://news.ycombinator.com/item?id=49342719)

**背景**: 视频内存（vRAM）是显卡上的专用显存，通常比系统内存快得多。当显存被占满时，内核或 GPU 驱动必须通过 GTT（图形转换表）把数据移出到系统内存，这会导致带宽更低、延迟更高。Valve 工程师 Natalie Vock 一直在改进 Linux 在 AMD GPU 上的显存管理，尤其是 8GB 及以下显存的显卡。Linux 7.3 的目标就是让这种显存耗尽的情况更平稳地降级，而不是突然掉帧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Linux-7.3-Improving-vRAM-Mgmt">Linux 7.3 To Land Initial Code Improving vRAM Management ...</a></li>
<li><a href="https://www.osnews.com/story/145846/beyond-the-limits-of-physical-vram/">Beyond the limits of physical VRAM – OSnews</a></li>
<li><a href="https://videocardz.com/newz/valve-developer-improves-linux-vram-handling-for-8gb-gpus-with-new-kernel-patches">Valve developer improves Linux VRAM handling for 8GB GPUs with new kernel patches - VideoCardz.com</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍非常兴奋，称赞这项工作令人印象深刻，并期待 Linux 7.3 的到来；也有人提到系统内存耗尽导致卡死的问题仍需要类似关注。讨论还涉及 Nvidia 缺少显存交换支持、内核侧内存碎片整理的可行性，以及应用自身更清楚哪些显存分配应该保留等观点。多位开发者对这项内核工作表示感谢。

**标签**: `#Linux`, `#kernel`, `#VRAM`, `#performance`, `#memory management`

---

<a id="item-4"></a>
## [Qwen 3.8 27B 在 AI 指数上获 52 分，与更大模型持平](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

Qwen 3.8 27B 在 Artificial Analysis Intelligence Index 上获得 52 分，与 GPT-5.6 Luna（max）持平，仅比 GLM-5.2（753B）和 DeepSeek V4 Pro 0813（1.7T）低 1 分。 这意义重大，因为一个 27B 参数的模型能取得与体积大数十甚至数百倍的前沿模型相当的成绩，凸显了模型效率和开源 AI 的快速进步。这可能使最先进的 AI 能力变得更加普及和便宜。 据 Simon Willison 称，Qwen 3.8 27B 是一款令人惊叹的模型。对比对象包括 753B 参数的 GLM-5.2 和 1.7T 参数的 DeepSeek V4 Pro 0813，而 GPT-5.6 Luna 的规模未知，但很可能远大于 27B。

rss · Simon Willison · 8月17日 23:58

**背景**: Artificial Analysis Intelligence Index 是 Artificial Analysis 发布的一项基准测试，用于评估各类 AI 模型的能力。Qwen 是由阿里巴巴开发的开源大语言模型系列，而 3.8 27B 似乎是该系列的最新版本。该指数为独立于特定任务比较模型质量提供了一种方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://artificialanalysis.ai/evaluations">Artificial Analysis</a></li>

</ul>
</details>

**标签**: `#ai`, `#llms`, `#qwen`, `#benchmarks`, `#efficiency`

---