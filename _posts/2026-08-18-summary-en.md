---
layout: default
title: "Horizon Summary: 2026-08-18 (EN)"
date: 2026-08-18
lang: en
---

> From 29 items, 4 important content pieces were selected

---

1. [Mojo programming language goes open source under Apache 2.0](#item-1) ⭐️ 9.0/10
2. [Seth Godin: Amazon's Search Imposes a Hidden 'Tax' on Shoppers](#item-2) ⭐️ 8.0/10
3. [Linux 7.3 Boosts Performance When GPU VRAM Runs Out](#item-3) ⭐️ 8.0/10
4. [Qwen 3.8 27B Scores 52 on AI Index, Matching Much Larger Models](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Mojo programming language goes open source under Apache 2.0](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 9.0/10

On August 18, 2026, Modular released the Mojo compiler and toolchain under the Apache 2.0 license, following last week's Mojo 1.0 release. This fulfills a long-standing open-source promise first made in May 2023. Mojo is a high-profile programming language aimed at combining Python's usability with C-level performance, making it highly relevant for AI/ML and systems programming. Open-sourcing the compiler under a permissive license could accelerate ecosystem growth and position Mojo as a viable alternative to C++ and CUDA for GPU computing. Mojo's original plan to be a full superset of Python was abandoned around August 2025; it is now its own language with Python-inspired syntax optimized for GPU programming. The language also includes Rust-inspired features such as static typing and a borrow checker.

rss · Simon Willison · Aug 18, 21:39

**Background**: Mojo is a systems programming language developed by Modular, first announced in May 2023. It uses a Python-like syntax while adding lower-level capabilities such as manual memory management and a borrow checker, similar to Rust but with greater ease of use. It was originally intended as a Python superset but shifted to a standalone language that prioritizes GPU and AI workloads. The recent 1.0 release and open-sourcing mark a major milestone for the project.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language) - Wikipedia</a></li>
<li><a href="https://www.infoworld.com/article/4081105/revisiting-mojo-a-faster-python.html">Revisiting Mojo: A faster Python? | InfoWorld</a></li>

</ul>
</details>

**Tags**: `#Mojo`, `#Open Source`, `#Programming Languages`, `#AI/ML`, `#Python`

---

<a id="item-2"></a>
## [Seth Godin: Amazon's Search Imposes a Hidden 'Tax' on Shoppers](https://seths.blog/2026/08/the-amazon-tax/) ⭐️ 8.0/10

In August 2026, Seth Godin published a blog post arguing that Amazon's search results have shifted from helping consumers find the best product to pushing what Amazon wants to sell. This shift, he argues, imposes a hidden 'tax' on consumers in the form of ads and manipulated rankings. This critique matters because it highlights how ad-driven search design can erode consumer trust and choice on the world's largest e-commerce platform. The discussion reflects a growing user awareness of platform incentives and may accelerate migrations to alternative shopping channels. Godin notes that even when Amazon knows the best-reviewed, least-returned product for a query like 'air fryer', it still shows ads to steer customers toward other options. Community comments report that roughly three out of four search results on Amazon can be sponsored ads, and that trying to avoid these ad 'minefields' has become a headache.

hackernews · herbertl · Aug 18, 13:22 · [Discussion](https://news.ycombinator.com/item?id=49345263)

**Background**: Amazon's product ranking is determined by the A9 search algorithm, which prioritizes sales performance and conversion rates over simple keyword relevance. Sponsored Products are cost-per-click ads that appear alongside organic listings, blurring the line between paid and organic results. The 'Amazon tax' in this context is a metaphor for the extra cost in money, time, and trust that consumers pay when search results are optimized for Amazon's ad revenue rather than customer intent.

<details><summary>References</summary>
<ul>
<li><a href="https://salesduo.com/blog/amazon-a9-search-engine-guide/">Amazon A9 Algorithm: How Amazon’s Search Engine Works (2026)</a></li>
<li><a href="https://www.repricerexpress.com/amazons-algorithm-a9/">Understanding Amazon's A9 Algorithm: Boost Your Product Rankings</a></li>
<li><a href="https://advertising.amazon.com/solutions/products/sponsored-products">Sponsored Products - Help increase product sales | Amazon Ads</a></li>

</ul>
</details>

**Discussion**: Comments generally agree with Godin, with one user noting that search has mutated from 'locate the exact item' to 'show me a list of semantic search results' that nudge users toward what the platform wants to sell. Another user says they are considering deleting their 15-year Amazon account due to painful quality degradation, while a third reports that roughly 75% of search results are sponsored ads. A commenter also raises the question of how a new, high-quality product could break through without buying ads.

**Tags**: `#e-commerce`, `#search`, `#ads`, `#platform design`, `#consumer behavior`

---

<a id="item-3"></a>
## [Linux 7.3 Boosts Performance When GPU VRAM Runs Out](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 8.0/10

Linux 7.3, the next kernel release, is set to introduce initial vRAM management code based on patches by Valve engineer Natalie Vock. The work is designed to improve performance when GPU memory is exhausted by making better use of system memory as a fallback. VRAM exhaustion is a common bottleneck on GPUs with 8GB or less, causing active games to be moved to slower system memory (GTT) instead of evicting background apps. The improvement could deliver meaningful frame-rate gains and a smoother experience for Linux gamers on low-VRAM AMD GPUs. Linux 7.3 will include the initial pieces of this VRAM-management work, building on earlier patches from Valve engineer Natalie Vock that improve low-VRAM GPUs. The changes focus on situations where physical VRAM is overcommitted, and the earlier patches were submitted to the kernel mailing lists before being accepted.

hackernews · flaburgan · Aug 18, 07:51 · [Discussion](https://news.ycombinator.com/item?id=49342719)

**Background**: Video RAM (VRAM) is dedicated memory on a graphics card and is usually much faster than system RAM. When VRAM is full, the kernel or GPU driver must move data out to system memory through the GTT (Graphics Translation Table), which causes lower bandwidth and higher latency. Valve engineer Natalie Vock has been improving Linux's VRAM handling on AMD GPUs, especially for cards with 8GB or less. Linux 7.3 aims to make these out-of-memory situations degrade more gracefully rather than causing a sudden performance collapse.

<details><summary>References</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Linux-7.3-Improving-vRAM-Mgmt">Linux 7.3 To Land Initial Code Improving vRAM Management ...</a></li>
<li><a href="https://www.osnews.com/story/145846/beyond-the-limits-of-physical-vram/">Beyond the limits of physical VRAM – OSnews</a></li>
<li><a href="https://videocardz.com/newz/valve-developer-improves-linux-vram-handling-for-8gb-gpus-with-new-kernel-patches">Valve developer improves Linux VRAM handling for 8GB GPUs with new kernel patches - VideoCardz.com</a></li>

</ul>
</details>

**Discussion**: Commenters are broadly enthusiastic, calling the work impressive and eagerly awaiting Linux 7.3; some note that system-RAM exhaustion and freezing still need similar attention. There is also discussion of Nvidia's lack of VRAM paging support, the possibility of kernel-side memory defragmentation, and how applications themselves know which VRAM allocations should be kept. Several developers express gratitude for the kernel work.

**Tags**: `#Linux`, `#kernel`, `#VRAM`, `#performance`, `#memory management`

---

<a id="item-4"></a>
## [Qwen 3.8 27B Scores 52 on AI Index, Matching Much Larger Models](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

Qwen 3.8 27B scored 52 on the Artificial Analysis Intelligence Index, matching GPT-5.6 Luna (max) and trailing only one point behind GLM-5.2 (753B) and DeepSeek V4 Pro 0813 (1.7T). This is significant because a 27B-parameter model is achieving scores comparable to frontier models that are tens or hundreds of times larger, highlighting rapid progress in model efficiency and open-source AI. It could make state-of-the-art AI capabilities much more accessible and affordable. The Qwen 3.8 27B is a truly astonishing model according to Simon Willison. The comparison includes GLM-5.2 at 753B parameters and DeepSeek V4 Pro 0813 at 1.7T parameters, while GPT-5.6 Luna's size is unknown but presumably much larger than 27B.

rss · Simon Willison · Aug 17, 23:58

**Background**: The Artificial Analysis Intelligence Index is a benchmark from Artificial Analysis that evaluates AI models across various capabilities. Qwen is a family of open-source large language models developed by Alibaba, and the 3.8 27B model appears to be a recent release in that series. The index provides a way to compare model quality independently of specific tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://artificialanalysis.ai/evaluations">Artificial Analysis</a></li>

</ul>
</details>

**Tags**: `#ai`, `#llms`, `#qwen`, `#benchmarks`, `#efficiency`

---