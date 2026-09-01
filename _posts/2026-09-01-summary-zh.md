---
layout: default
title: "Horizon Summary: 2026-09-01 (ZH)"
date: 2026-09-01
lang: zh
---

> 从 37 条内容中筛选出 6 条重要资讯。

---

1. [库克卸任苹果 CEO，特努斯接棒主推 AI](#item-1) ⭐️ 9.0/10
2. [谷歌移除 MV2 扩展，uBlock Origin 等遭下架](#item-2) ⭐️ 8.0/10
3. [NAT：互联网中心化的原罪](#item-3) ⭐️ 8.0/10
4. [滑动窗口注意力在长上下文推理上胜过线性注意力](#item-4) ⭐️ 8.0/10
5. [SynthFin-AML：新基准揭示图神经网络的时间泄漏问题](#item-5) ⭐️ 8.0/10
6. [DeepSeek 发布 V4 系列首款多模态模型 V4-Flash-Vision-Exp](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [库克卸任苹果 CEO，特努斯接棒主推 AI](https://www.bloomberg.com/news/articles/2026-08-30/apple-s-new-ceo-john-ternus-takes-reins-from-tim-cook-focusing-on-ai) ⭐️ 9.0/10

库克于 2026 年 8 月 31 日正式卸任苹果 CEO，约翰·特努斯于 9 月 1 日接任，库克留任执行主席。特努斯的首要任务是加快 AI 落地，补齐 Siri 升级延期等短板，9 月 9 日发布会上预计将亮相首款折叠屏 iPhone。 这次领导层交接标志着苹果这家全球最具影响力的科技公司之一正在经历代际更替，也表明其战略重心转向 AI。新 CEO 的聚焦方向以及即将发布的折叠屏 iPhone 将决定苹果在与三星、谷歌等对手竞争中的地位。 51 岁的特努斯是硬件工程老将，自 2021 年起负责硬件设计，并在 Apple silicon Mac 的研发中发挥了关键作用。据称首款折叠屏 iPhone 将配备 12 GB 内存，并深度整合 Siri AI，可结合屏幕、日历与相机理解现实场景。

telegram · zaihuapd · 8月31日 10:21

**背景**: Apple Intelligence 是苹果于 2024 年 6 月推出的 AI 功能套件，结合设备端和服务器端处理，随 iOS 18、iPadOS 18 和 macOS Sequoia 发布，适用于 Apple silicon 设备及新 iPhone。约翰·特努斯此前担任苹果硬件工程高级副总裁，负责 Mac、iPad 和 iPhone 等产品的设计与开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/John_Ternus">John Ternus</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence</a></li>

</ul>
</details>

**标签**: `#Apple`, `#CEO transition`, `#AI`, `#Tim Cook`, `#John Ternus`

---

<a id="item-2"></a>
## [谷歌移除 MV2 扩展，uBlock Origin 等遭下架](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

Google 已执行其 Manifest V3 迁移计划，将 Chrome 网上应用店中所有 Manifest V2 扩展下架，其中包括 uBlock Origin 等广受欢迎的隐私和广告拦截工具。这一移除使得用户更难在 Chrome 上安装这些扩展。 这标志着 Chrome 扩展一个时代的结束，迫使隐私工具用户转向 Firefox 等替代方案，或接受功能较弱的 uBlock Origin Lite。此举也引发了人们对单一公司控制用户屏蔽广告和保护隐私方式的担忧。 Manifest V3 用更有限的 declarativeNetRequest 模型取代了早期允许深度、动态网络拦截的扩展 API，这移除了 uBlock Origin 此前依赖的能力。完整版 uBlock Origin 仍可在继续支持更宽松的 WebExtensions API 的 Firefox 中运行。

hackernews · twapi · 8月31日 21:10 · [社区讨论](https://news.ycombinator.com/item?id=49514878)

**背景**: Chrome 扩展基于清单版本定义的一组能力构建。Manifest V2（MV2）多年来一直是标准，但 Google 在 2020 年推出了 Manifest V3（MV3），以改善隐私、安全性和性能。到 2025 年，MV2 在大多数 Chrome 用户中实际上已被淘汰，而 Chrome 网上应用店现在已完全移除 MV2 扩展。uBlock Origin 等广告拦截器之所以受影响，是因为 MV3 限制了以 MV2 所允许的灵活方式拦截网络请求的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V3 | Chrome for Developers</a></li>
<li><a href="https://www.pcworld.com/article/3160794/the-last-lifeline-for-ublock-origin-in-chrome-is-almost-gone-for-good.html">The last lifeline for uBlock Origin in Chrome is almost gone for good | PCWorld</a></li>
<li><a href="https://factually.co/fact-checks/technology/manifest-v3-impact-ublock-origin-chromium-blocking-workarounds-4c8757">How Does Manifest V3 Change What uBlock Origin Can Blo...</a></li>

</ul>
</details>

**社区讨论**: 新闻评论者对 Google 的决定普遍持批评态度。许多人建议改用 Firefox，指出 uBlock Origin 在那里一直运行得最好；还有人表达了对 Google 掌控网络的不满，并表示即使 Firefox 市场份额萎缩也会继续使用它或其分支。一些评论者强调，广告拦截如今已成为安全问题，尤其是对容易点击恶意广告、不太懂技术的用户而言。

**标签**: `#Chrome`, `#Manifest V3`, `#ad blocking`, `#privacy`, `#web extensions`

---

<a id="item-3"></a>
## [NAT：互联网中心化的原罪](https://dreamstation.systems/personal/ntppost.html) ⭐️ 8.0/10

一篇论文认为，NAT（网络地址转换）不仅是后来的因素，而是互联网中心化的一个根本原因，它削弱了自托管能力，并使客户端-服务器模式成为常态。该文将地址稀缺重新定义为塑造人们对互联网认知的关键力量。 该观点重新定义了互联网中心化的叙事，将对中心化的责任归于大多数用户甚至不知道的早期技术产物。这对于关心自托管、网络中立性以及用户与大型云平台之间权力平衡的人们来说意义重大。 作者称 NAT 为原罪，并指出它让人们习惯了客户端-服务器模式，而这种模式本是 IPv4 地址稀缺的产物。文章还提到，在 NAT 普及之前，架设服务器曾经是轻而易举的事情。

hackernews · robinpie · 8月31日 02:23 · [社区讨论](https://news.ycombinator.com/item?id=49504905)

**背景**: NAT（网络地址转换）将多个私有 IP 地址映射到一个公共 IP 地址，使许多设备可以共享一个公共地址，这一技术被广泛采用以节省有限的 IPv4 地址资源。客户端-服务器模型是一种计算架构，客户端从中心化服务器请求资源，而点对点或自托管模式中每个节点都可以同时作为提供者和消费者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Network_address_translation">Network address translation - Wikipedia</a></li>
<li><a href="https://www.cisco.com/site/us/en/learn/topics/networking/what-is-network-address-translation-nat.html">What Is Network Address Translation (NAT)? - Cisco</a></li>
<li><a href="https://www.geeksforgeeks.org/system-design/client-server-architecture-system-design/">Client-Server Architecture - System Design - GeeksforGeeks</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一。Linux NAT 实现者 RustyRussell 道歉称，当前的 NAT 系统削弱了公共端点的能力。其他人则认为 NAT 并非原罪，运营商级 NAT（CGNAT）才是真正的问题，而普通 NAT 是可管理的，并且保护了许多不安全设备免于暴露。

**标签**: `#NAT`, `#networking`, `#internet architecture`, `#centralization`, `#history`

---

<a id="item-4"></a>
## [滑动窗口注意力在长上下文推理上胜过线性注意力](https://www.reddit.com/r/MachineLearning/comments/1w3j1vw/slidingwindow_attention_beats_linear_on/) ⭐️ 8.0/10

一篇新的 arXiv 预印本（2608.28444）报告称，带注意力汇的滑动窗口注意力在 Needle-in-a-Haystack 和 BABILong 长上下文推理基准上，性能比线性注意力高出 2 到 10 倍。作者认为，后训练转线性模型的路线没有与更简单的基线进行充分比较，并建议改用 SWA。 这一发现挑战了近期业界投入大量后训练算力将大语言模型转换为线性注意力以提高效率的研究方向。如果 SWA 无需任何后训练就能达到或超过这些模型的表现，可能会让研究重点回归更简单、更廉价的基线，并重塑长上下文 LLM 的设计思路。 报告称差距巨大：在选定的基准测试（包括 Needle-in-a-Haystack 和 BABILong）上，SWA 的性能比线性注意力高出 2 到 10 倍。作者承认，线性注意力“可能显示出一些前景，但很可能需要从头训练或大量后训练才能达到甚至接近 SWA 的水平。”论文的建议是改用 SWA，而不是对线性模型进行后训练。

reddit · r/MachineLearning · /u/Justgototheeffinmoon · 8月31日 16:35

**背景**: 标准 Transformer 的注意力随序列长度呈二次方增长，使得长上下文推理在内存和计算上开销很大。线性注意力变体试图通过核近似或循环公式将其复杂度降到线性，但通常需要对现有 LLM 进行后训练才能适配。滑动窗口注意力（SWA）将每个 token 的注意力限制在一个固定局部窗口内，也能以更简单的方式实现线性扩展，而加入“注意力汇”有助于稳定训练。BABILong 是一个长上下文推理基准，用来测试模型在超长文档中跨分散事实进行推理的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.28444">[2608.28444] Sliding-window beats linear attention - arXiv.org</a></li>
<li><a href="https://arxiv.org/abs/2406.10149">[2406.10149] BABILong: Testing the Limits of LLMs with Long ...BABILong: Testing the Limits of LLMs with Long Context ...BABILong Benchmark - emergentmind.comRMT-team/babilong · Datasets at Hugging FaceBABILong Benchmark Scores & AI Model Leaderboard | BenchmarkListCogniFold/benchmarks/babilong/README.md at main - GitHub</a></li>
<li><a href="https://www.digitalocean.com/community/tutorials/sliding-window-attention-efficient-long-context-models">Sliding Window Attention: Efficient Long-Context Modeling | DigitalOcean</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#attention mechanisms`, `#long-context reasoning`, `#linear attention`, `#LLM efficiency`

---

<a id="item-5"></a>
## [SynthFin-AML：新基准揭示图神经网络的时间泄漏问题](https://www.reddit.com/r/MachineLearning/comments/1w3imxy/your_gnn_is_probably_just_an_overcomplicated_mlp/) ⭐️ 8.0/10

作者发布了 SynthFin-AML v10.0，一个包含 10 万节点、120 万边的合成基准，用于在动态图评估中强制执行严格的因果边界。他们证明标准的直推式随机划分会把未来边泄漏到 GNN 训练中，并提出一种 3 快照的时间点划分方法来修复该问题。 这解决了动态图研究中一个关键的评估缺陷——模型可以通过看到未来信息来作弊，从而虚报性能。该基准已提交给 PyTorch Geometric，可能成为因果评估的标准，并帮助反洗钱社区可靠地比较 GNN 与更简单基线的表现。 3 快照架构使用截至第 7 天的训练图边、截至第 8 天的验证边和截至第 10 天的测试边，从物理上限制了 GNN 的感受野。作者还通过让欺诈交易与零售交易金额服从相同的对数正态分布（μ=8.517, σ=0.8），消除了“金额划分作弊”。

reddit · r/MachineLearning · /u/Glabmayt2075 · 8月31日 16:21

**背景**: 动态图建模不断演变的关系，例如随时间产生边的金融交易网络。GNN 通过聚合邻居信息来计算节点嵌入；如果训练时使用包含未来边的静态快照，模型就能访问预测时无法获得的信息。这种时间泄漏会虚增性能，而标准随机划分对金融交易图尤其成问题。SynthFin-AML 是一个旨在防止此类泄漏的合成基准，它延续了早期合成 AML 数据集（如基于真实银行数据构建的 SynthAML）的思路。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nature.com/articles/s41597-023-02569-2">A synthetic data set to benchmark anti-money laundering methods | Scientific Data</a></li>
<li><a href="https://arxiv.org/html/2509.23631v2">Leakage-Free Evaluation and Distribution-Robust Spatio-Temporal Graph ...</a></li>
<li><a href="https://deepwiki.com/2024SIG/SIG/7.3-data-leakage-prevention">Data Leakage Prevention | 2024SIG/SIG | DeepWiki</a></li>

</ul>
</details>

**标签**: `#graph neural networks`, `#temporal leakage`, `#anti-money laundering`, `#benchmark`, `#causality`

---

<a id="item-6"></a>
## [DeepSeek 发布 V4 系列首款多模态模型 V4-Flash-Vision-Exp](https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-Vision-Exp) ⭐️ 8.0/10

DeepSeek 发布了 DeepSeek-V4-Flash-Vision-Exp，这是 V4-Flash 的实验性多模态版本，通过持续训练加入了视觉模块。在 ApexBench 多模态 agent 基准上，相比 V4-Flash-0731，成绩从 26.2 提升至 36.5，而文本 agent 表现基本持平。 这是 DeepSeek 首款 V4 代多模态模型，ApexBench 上的大幅跃升表明其多模态 agent 能力显著增强。这巩固了 DeepSeek 在开源权重大模型竞争格局中的地位，也为 agentic AI 开发提供了强力基线。 该模型基于 V4-Flash-0731 架构，新增了视觉模块并进行了持续训练。它在 ApexBench 上多模态 agent 任务取得 10.3 分的提升（从 26.2 到 36.5），同时文本 agent 性能基本持平，表明训练针对性很强。

telegram · zaihuapd · 8月31日 11:41

**背景**: 多模态模型结合了文本与视觉理解能力，使 agent 能够感知图像、截图或 UI 布局，同时进行推理和行动。像 ApexBench 这样的基准测试会在海报编辑、代码重构和知识工作等长周期、贴近真实场景的任务中评估 AI agent，因此对 agentic AI 系统具有参考价值。DeepSeek 的 V4 系列是其最新一代开源权重模型，此次实验性发布为现有 V4-Flash 产品线新增了视觉能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/apex-bench">APEX-Bench: High-Fidelity Benchmarking</a></li>
<li><a href="https://www.mercor.com/apex/">APEX Benchmarks: AI Productivity Index Leaderboards | Mercor</a></li>
<li><a href="https://link.springer.com/article/10.1007/s11390-025-4802-8">Multimodal Agent AI: A Survey of Recent Advances and Future ...</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#multimodal`, `#model release`, `#AI`, `#LLM`

---