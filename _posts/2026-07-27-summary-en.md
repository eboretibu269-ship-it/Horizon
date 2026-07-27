---
layout: default
title: "Horizon Summary: 2026-07-27 (EN)"
date: 2026-07-27
lang: en
---

> From 32 items, 13 important content pieces were selected

---

1. [Google Teases Gemini 4 as Most Ambitious Pre-Training Yet](#item-1) ⭐️ 9.0/10
2. [Fastjson2 Remote Code Execution Vulnerability (RCE) Unpatched](#item-2) ⭐️ 9.0/10
3. [vLLM v0.26.0 Adds Inkling, DeepSeek-V4 Optimizations](#item-3) ⭐️ 8.0/10
4. [Anthropic clarifies stance on open-weights models](#item-4) ⭐️ 8.0/10
5. [Judge Rejects Google's DMCA Defense Against Scraping](#item-5) ⭐️ 8.0/10
6. [Bun's Rust Rewrite Makes Progress, Release Delayed](#item-6) ⭐️ 8.0/10
7. [Modern email can be built from borrowed parts](#item-7) ⭐️ 8.0/10
8. [Moonshot AI Releases Kimi-K3, a 2.8 Trillion Parameter Open Model](#item-8) ⭐️ 8.0/10
9. [Solo Study: All 6 Frontier LLMs Show Left-Leaning Political Bias](#item-9) ⭐️ 8.0/10
10. [Proposal for a deterministic pre-training data audit gate](#item-10) ⭐️ 8.0/10
11. [ChangXin Technology Soars 471% on STAR Market Debut](#item-11) ⭐️ 8.0/10
12. [Huawei Reportedly Building DRAM Fab with Shengweixu](#item-12) ⭐️ 8.0/10
13. [China begins mass production of domestic DUV lithography tools, targeting ~5 units this year](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Google Teases Gemini 4 as Most Ambitious Pre-Training Yet](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 9.0/10

Google CEO Sundar Pichai announced during Alphabet's Q2 2026 earnings call that Gemini 4, the next-generation large language model, is now in training and is expected to launch by late 2026. This signals Google's commitment to leading the AI frontier, potentially advancing AGI research and intensifying competition among major AI labs. Pichai emphasized that compute resources will be prioritized for frontier AGI research, and Gemini 3.x Flash models will continue monthly updates focusing on coding intelligence.

telegram · zaihuapd · Jul 27, 04:06

**Background**: Pre-training is the initial phase where large language models learn grammar, facts, and reasoning from massive text datasets. This stage establishes a versatile foundation that can later be fine-tuned for specific tasks. Google's Gemini 4 represents its most ambitious pre-training effort to date.

<details><summary>References</summary>
<ul>
<li><a href="https://www.entrypointai.com/blog/pre-training-vs-fine-tuning-vs-in-context-learning-of-large-language-models/">Pre-training vs Fine-Tuning vs In-Context Learning of Large Language Models | Entry Point AI</a></li>
<li><a href="https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/gemini/3-flash">Gemini 3 Flash | Gemini Enterprise Agent Platform | Google Cloud Documentation</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google Gemini`, `#Large Language Models`, `#AGI`, `#Pre-training`

---

<a id="item-2"></a>
## [Fastjson2 Remote Code Execution Vulnerability (RCE) Unpatched](https://mp.weixin.qq.com/s/LJaul1jNjK9pXRAkoUiMEA) ⭐️ 9.0/10

A critical remote code execution (RCE) vulnerability has been disclosed in Fastjson2 versions up to 2.0.62, affecting all currently released versions. The maintainer has acknowledged the issue but no official patch has been released yet, as pull request #7695 was closed without merging into the main branch. Fastjson2 is widely used in Java ecosystems for JSON processing, and this unpatched vulnerability poses an immediate security risk to thousands of applications. As this is the second severe Fastjson vulnerability within a month, organizations relying on the library must take urgent mitigating actions, such as disabling AutoType entirely. The vulnerability allows attackers to bypass AutoType type validation using malicious JSON data, potentially leading to arbitrary code execution. Full vulnerability details and exploit code have not been publicly disclosed, but the maintainer advises disabling AutoType completely until a fix is available.

telegram · zaihuapd · Jul 27, 10:31

**Background**: Fastjson2 is a high-performance JSON library for Java developed by Alibaba, designed as the successor to Fastjson 1.x. AutoType is a feature that allows automatic type resolution during deserialization, which has historically been a common attack surface for deserialization vulnerabilities. Earlier in July 2026, a critical RCE vulnerability in Fastjson 1.x (versions 1.2.68–1.2.83) was disclosed, and Alibaba recommended migrating to Fastjson2 as the long-term fix; however, this new vulnerability shows that Fastjson2 itself is now also affected.

<details><summary>References</summary>
<ul>
<li><a href="https://alibaba.github.io/fastjson2/">FASTJSON2 is a Java JSON library with excellent performance.</a></li>
<li><a href="https://thehackernews.com/2026/07/fastjson-1x-rce-vulnerability-targeted.html">Fastjson 1.x RCE Vulnerability Targeted in Attacks With No Patched...</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#RCE`, `#Fastjson2`, `#Java`

---

<a id="item-3"></a>
## [vLLM v0.26.0 Adds Inkling, DeepSeek-V4 Optimizations](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 introduces full support for the Inkling model family with 975B parameters and 1M token context, along with significant DeepSeek-V4 performance improvements including specialized routing kernels and fused topk bias, plus fp32 lm_head via head_dtype for improved accuracy. This release significantly expands vLLM's model support and performance capabilities, making it easier for practitioners to deploy cutting-edge large models like Inkling and DeepSeek-V4 with improved efficiency and accuracy across NVIDIA, AMD, and Intel hardware. Key technical details include piecewise CUDA graph support, Hopper FA4 relative attention, MTP=1 speculative decoding, LoRA support, and ModelOpt NVFP4 quantization for Inkling; for DeepSeek-V4, a 2.94% end-to-end TPOT improvement from a specialized routing kernel and 1.5-2x kernel speedup from fused_topk_bias.

github · khluu · Jul 27, 01:06

**Background**: vLLM is an open-source high-throughput LLM serving system. The Inkling model is a 975B parameter Mixture-of-Experts transformer with 41B active parameters and a 1M token context window, released by Thinking Machines Lab. Flash Attention 4 (FA4) is an optimized attention algorithm for NVIDIA Hopper GPUs, and NVFP4 is a 4-bit floating-point quantization method from NVIDIA Model Optimizer.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://www.spheron.network/blog/tensorrt-model-optimizer-modelopt-quantization-guide/">NVIDIA TensorRT Model Optimizer (ModelOpt): FP8, INT4, and FP4 Quantization Guide (2026) | Spheron Blog</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#release notes`, `#performance optimization`, `#open-source`

---

<a id="item-4"></a>
## [Anthropic clarifies stance on open-weights models](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic has publicly stated its position on open-weights models, advocating for mandatory safety testing for all sufficiently capable models without a blanket ban, but critics argue this effectively restricts open models. This stance is significant for AI governance as it balances openness and safety, potentially setting a precedent for regulation of open-source AI models and impacting developers and users worldwide. Anthropic proposes mandatory safety testing for all capable models, both open and closed, but does not specify who administers the tests or covers the costs, leading critics to argue it could amount to a de facto ban on open-weights models.

hackernews · surprisetalk · Jul 27, 22:03 · [Discussion](https://news.ycombinator.com/item?id=49076057)

**Background**: Open-weights models are AI models whose core components are publicly released, allowing anyone to download, inspect, modify, and run them on their own infrastructure. Anthropic is a leading AI safety company, and its CEO Dario Amodei has previously written about AI risks and regulation. The debate centers on how to regulate increasingly capable open models without stifling innovation.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>

</ul>
</details>

**Discussion**: Community comments are largely critical, with users pointing out contradictions in Anthropic's position—such as opposing bans while supporting chip sales restrictions—and arguing that mandatory testing could serve as a costly barrier that effectively bans open models. Some accuse Anthropic of protecting its own closed-source business interests.

**Tags**: `#AI safety`, `#open weights`, `#regulation`, `#Anthropic`, `#model governance`

---

<a id="item-5"></a>
## [Judge Rejects Google's DMCA Defense Against Scraping](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

A judge rejected Google's attempt to use the DMCA safe harbor to block third-party scraping of its search results, ruling that the data is not copyrightable and that Google's argument was inappropriate. This ruling reinforces that scraping publicly available data is generally not copyright infringement, and it underscores the tension between Google's own history of crawling the web and its efforts to restrict scraping of its own services. The case involved Google suing SerpAPI, a service that scrapes Google search results. The judge found that the data is not copyrightable and that Google's DMCA claim was unfounded.

hackernews · cdrnsf · Jul 27, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49073513)

**Background**: The DMCA safe harbor protects online service providers from copyright liability for user-generated content, but does not prevent scraping of non-copyrightable facts. Google itself relies on web crawling to index the internet. Web scraping legality often depends on whether the scraped data is copyrightable or if it violates terms of service.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DMCA_safe_harbor">DMCA safe harbor</a></li>
<li><a href="https://www.quinnemanuel.com/the-firm/publications/the-legal-landscape-of-web-scraping/">The Legal Landscape of Web Scraping</a></li>
<li><a href="https://blog.apify.com/is-web-scraping-legal/">Is web scraping legal? Yes, if you know the rules.</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted Google's hypocrisy, noting that Google built its business on crawling the open web and that its deprecation of APIs forces reliance on third-party scrapers. Some expressed support for SerpAPI and criticized Google's heavy-handed legal tactics.

**Tags**: `#legal`, `#web scraping`, `#DMCA`, `#Google`, `#tech industry`

---

<a id="item-6"></a>
## [Bun's Rust Rewrite Makes Progress, Release Delayed](https://lockwood.dev/ai/2026/07/27/how-is-the-bun-rewrite-in-rust-going.html) ⭐️ 8.0/10

Bun's Rust rewrite has shipped in Anthropic's Claude Code tool, and the project lead reported that the rewrite is progressing well, but the Bun v1.4 release is delayed until a promised number of Node.js compatibility tests pass. This rewrite addresses performance and compatibility issues for a widely-used JavaScript runtime. The delay underscores the difficulty of achieving full Node.js compatibility while migrating to Rust, affecting developers who depend on Bun for speed and reliability. The Rust rewrite was already deployed in Claude Code over a month ago without most users noticing. The release delay is specifically tied to meeting a self-imposed metric of newly passing Node.js tests, with the required pull requests still unmerged.

hackernews · tomlockwood · Jul 27, 11:12 · [Discussion](https://news.ycombinator.com/item?id=49067854)

**Background**: Bun is a JavaScript runtime designed as a fast drop-in replacement for Node.js, including a built-in bundler, transpiler, and package manager. Originally written in Zig, the project decided to rewrite the core in Rust to improve performance and maintainability. Claude Code is Anthropic's agentic coding tool that runs in the terminal and assists with code editing and execution.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Discussion**: Project lead Jarred confirmed the rewrite shipped in Claude Code and that the release is delayed. Commenter SquareWheel noted that a major refactor typically slows development temporarily, while benjiro29 questioned the use of LLMs for code translation, arguing that real software value comes from iterative development. Another commenter, bendmorris, pointed to a Zig-based alternative called buz that claims sub-second build times, suggesting the original issues might have been self-inflicted.

**Tags**: `#Bun`, `#Rust`, `#Node.js`, `#runtime`, `#software-engineering`

---

<a id="item-7"></a>
## [Modern email can be built from borrowed parts](https://en.andros.dev/blog/d7ed8b07/modern-email-can-be-built-from-borrowed-parts/) ⭐️ 8.0/10

An article proposes rebuilding email by reusing components from modern protocols like HTTP and Matrix, rather than continuing to extend SMTP. This conceptual shift suggests a modular replacement of SMTP's core functions with borrowed technologies. If realized, this could make email more secure, efficient, and feature-rich, aligning it with modern communication expectations. However, massive adoption barriers due to network effects and entrenched infrastructure mean any change would be extremely difficult. The article emphasizes that SMTP's fundamental design is outdated, but community comments highlight challenges such as spam, backward compatibility, and JSON parsing overhead for large emails. Notably, JMAP and Matrix are existing modern protocols that could serve as building blocks.

hackernews · andros · Jul 27, 08:27 · [Discussion](https://news.ycombinator.com/item?id=49066639)

**Background**: Email has been built on SMTP since the 1980s, but it was designed for a different era and struggles with spam, security, and rich features. Modern protocols like JMAP (a JSON-based replacement for IMAP) and Matrix (a decentralized real-time communication protocol) offer proven components that address these shortcomings.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JSON_Meta_Application_Protocol">JSON Meta Application Protocol - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Matrix_(protocol)">Matrix (protocol) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments are divided: some reference historical failed attempts (e.g., a spam solutions list from the 1990s), while others propose specific fixes like charging per email or requiring recipient permission. There is also concern about JSON parsing requiring full email loading into memory at scale, and a strong consensus that backward compatibility is essential for adoption.

**Tags**: `#email`, `#spam`, `#SMTP`, `#protocol design`, `#network effects`

---

<a id="item-8"></a>
## [Moonshot AI Releases Kimi-K3, a 2.8 Trillion Parameter Open Model](https://huggingface.co/moonshotai/Kimi-K3) ⭐️ 8.0/10

Moonshot AI released Kimi-K3 on HuggingFace, an open-weight model with approximately 2.8 trillion parameters, the largest openly available model to date. The model supports native visual understanding and a 1M-token context window. This release pushes the frontier of open-source AI, enabling unprecedented customization and data sovereignty for developers and enterprises. It also sparks critical discussions on the economics and practicality of hosting trillion-parameter models. The model uses mxfp4 precision, requiring approximately 1.5TB of VRAM. Its license mandates a separate agreement with Moonshot AI for commercial use if revenue exceeds $20 million annually. The model appears to have identity confusion in some responses.

hackernews · nateb2022 · Jul 27, 06:18 · [Discussion](https://news.ycombinator.com/item?id=49065752)

**Background**: Large language models with trillions of parameters are typically only accessible via API. An open-weight release allows anyone to download, fine-tune, and self-host the model, which is rare at this scale. Moonshot AI is a Beijing-based company known for pushing the scaling frontier of open models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://platform.kimi.ai/docs/models">Model List - Kimi API Platform</a></li>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI</a></li>

</ul>
</details>

**Discussion**: Community comments focused on hosting costs, with estimates that serving the model may require 16x B200 GPUs. Customization and IP sovereignty were highlighted as major wins, while license revenue thresholds raised concerns for commercial use. Some users noted the model incorrectly identified itself as Claude.

**Tags**: `#AI`, `#LLM`, `#Open Source`, `#HuggingFace`, `#Model Release`

---

<a id="item-9"></a>
## [Solo Study: All 6 Frontier LLMs Show Left-Leaning Political Bias](https://www.reddit.com/r/MachineLearning/comments/1v8fnzw/evaluated_6_frontier_llms_gpt54_claude_sonnet_46/) ⭐️ 8.0/10

A solo evaluation of 6 frontier LLMs (GPT-5.4, Claude Sonnet 4.6, Claude Opus 4.7, Gemini Pro/Flash, Grok 4.3) across 8 bias benchmarks (~20,600 examples) found that all models exhibit left-leaning political bias, including Grok which self-reports as right-leaning but behaves left-leaning on content classification and policy questions. This study reveals a systematic political bias in state-of-the-art LLMs, raising concerns about fairness and neutrality in AI systems used for content moderation, information retrieval, and decision support. The discrepancy between Grok's self-reported and actual behavior further challenges the reliability of self-declared model alignment. On the BBQ race dataset, GPT-5.4 refused to answer race-related questions where the correct answer involves race 20.3% of the time, while Claude Opus 4.7 refused 13.8%, Grok 9.5%, and Claude Sonnet 4.6/Gemini Pro about 5%. The study is non-peer-reviewed, uses a single prompt template per task, and lacks multi-run averaging.

reddit · r/MachineLearning · /u/marggggggggg · Jul 27, 22:37

**Background**: Bias benchmarks like WinoBias (gender coreference), BBQ (social stereotypes), and SeeGULL (geo-cultural stereotypes) are designed to measure harmful biases in AI systems. Political bias benchmarks such as the Political Compass and Hyperpartisan News assess models' political leanings. LLMs are trained on vast web data, which often contains political imbalances, potentially leading to biased outputs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kaggle.com/datasets/thedevastator/winobias-coreference-dataset">WinoBias Coreference Dataset | Kaggle</a></li>
<li><a href="https://arxiv.org/abs/2110.08193">BBQ: A Hand-Built Bias Benchmark for Question Answering</a></li>
<li><a href="https://github.com/google-research-datasets/seegull">GitHub - google-research-datasets/seegull: SeeGULL is...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#AI bias`, `#political bias`, `#fairness`, `#benchmarking`

---

<a id="item-10"></a>
## [Proposal for a deterministic pre-training data audit gate](https://www.reddit.com/r/MachineLearning/comments/1v8a3nu/training_data_needs_a_real_gonogo_gate_before/) ⭐️ 8.0/10

A Reddit user proposes a deterministic pre-training gate that audits training data for leakage, contradictions, redundancy, coverage, provenance, and evidence integrity, outputting reproducible verdicts like PASS, WARNING, FAIL, or FAIL_SECURITY. This addresses a critical gap in MLOps where training data quality checks are often ad hoc, providing a formal, reproducible gate that could prevent costly training failures and improve model reliability. The gate operates locally on the exact artifact to be used, with verdicts determined by explicit evidence rather than an LLM, ensuring determinism; it can also generate a repair plan and re-audit after approved changes.

reddit · r/MachineLearning · /u/jesusmjk · Jul 27, 19:13

**Background**: Data leakage occurs when training data inadvertently contains information from the test set, leading to overly optimistic performance estimates. Training data provenance tracks the origin and processing history of datasets, crucial for governance and security. ML pipeline gates are checkpoints that enforce quality standards before progressing to the next stage, but a standardized pre-training audit gate for data artifacts has been missing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Leakage_(machine_learning)">Leakage (machine learning) - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/data-leakage-machine-learning">What is Data Leakage in Machine Learning? | IBM</a></li>
<li><a href="https://dev.to/aicryptosystems/training-data-provenance-the-manifest-diff-that-explains-the-hash-11bj">Training Data Provenance: The Manifest Diff That... - DEV Community</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#training data`, `#data quality`, `#MLOps`, `#pipeline gates`

---

<a id="item-11"></a>
## [ChangXin Technology Soars 471% on STAR Market Debut](https://www.stcn.com/article/detail/4042119.html) ⭐️ 8.0/10

ChangXin Technology (688825.SH) made its debut on Shanghai's STAR Market on July 27, with shares opening at 49.5 yuan, a 471.59% surge from the issue price of 8.66 yuan. This record-breaking IPO underscores the rapid growth of China's domestic memory chip industry and its increasing competitiveness on the global stage, while also setting a new fundraising record on the STAR Market. The company raised approximately 57.9 billion yuan in the IPO, and if the overallotment option is fully exercised, the total could reach 66.6 billion yuan, surpassing Semiconductor Manufacturing International Corporation's (SMIC) 53.2 billion yuan record from 2020.

telegram · zaihuapd · Jul 27, 01:29

**Background**: ChangXin Technology is a leading Chinese manufacturer of dynamic random-access memory (DRAM) chips, a critical component in computers and servers. The Shanghai STAR Market, launched in 2019, is China's Nasdaq-style board designed to support tech and innovative companies with less stringent listing requirements. This IPO highlights the country's push for semiconductor self-sufficiency.

**Tags**: `#IPO`, `#semiconductor`, `#Chinese tech`, `#memory`, `#STAR Market`

---

<a id="item-12"></a>
## [Huawei Reportedly Building DRAM Fab with Shengweixu](https://www.xda-developers.com/huawei-is-building-its-own-dram-fab-and-it-could-reshape-ram-prices-for-everyone/) ⭐️ 8.0/10

Huawei is reportedly collaborating with Shenzhen-based startup Shengweixu (Swaysure) to build a 12-inch DRAM wafer fab with a planned monthly capacity of 140,000 wafers, though Huawei has denied the claims. If realized, this fab could secure memory supply for Huawei's Ascend AI chip series, reducing dependence on external suppliers like Changxin Memory Technologies, and potentially impact global DRAM prices. The reported fab would use 12-inch (300mm) wafers, and industry observers note that even if construction starts soon, mass production would take years, so near-term consumer DRAM prices are unlikely to be affected.

telegram · zaihuapd · Jul 27, 03:17

**Background**: DRAM (Dynamic Random Access Memory) is a type of volatile memory widely used in computers and servers. Huawei's Ascend AI accelerators, based on the Da Vinci architecture, require high-bandwidth memory for AI workloads. Shengweixu (Swaysure) is a Shenzhen-based startup founded in 2022 with a state-owned background, focusing on memory chip technology.

<details><summary>References</summary>
<ul>
<li><a href="https://insights.greyb.com/shenzhen-shengweixu-technology-patents/">Shenzhen Shengweixu Technology Patents – Insights and Stats...</a></li>
<li><a href="https://aiwiki.ai/wiki/huawei_ascend">Huawei Ascend | AI Wiki</a></li>
<li><a href="https://www.industryresearch.co/blog/top-dram-wafer-companies-12">DRAM Wafer Market Outlook 2026–2035 | Growth & Trends</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#DRAM`, `#Huawei`, `#AI chips`, `#supply chain`

---

<a id="item-13"></a>
## [China begins mass production of domestic DUV lithography tools, targeting ~5 units this year](https://www.theinformation.com/articles/china-starts-mass-producing-homegrown-duv-chipmaking-tools-advance-local-chip-industry) ⭐️ 8.0/10

China has started mass production of domestically developed immersion DUV lithography machines, with a state-owned enterprise in Shanghai planning to produce about 5 units this year and around 20 units by 2027. The tools will be delivered to domestic chipmakers such as SMIC and Hua Hong Semiconductor. This marks a significant breakthrough in China's semiconductor self-sufficiency efforts, as DUV lithography is critical for advanced chip manufacturing. Although the domestic tools still lag behind ASML in performance and reliability, scaling up production could gradually erode ASML's market share in China, especially if Western export restrictions tighten. The first batch of tools requires months of testing for precision and compatibility before being used in mass production lines. Some critical components still come from Japan, and domestic supply chain delays have already affected progress this year.

telegram · zaihuapd · Jul 27, 14:10

**Background**: Deep ultraviolet (DUV) lithography is a mature technology used to print circuit patterns on silicon wafers for chips at nodes down to around 7nm using multi-patterning. Immersion lithography, which uses a layer of water between the lens and wafer, improves resolution and is the most advanced type of DUV tool. ASML dominates the global DUV market, and Western controls have restricted exports of cutting-edge DUV systems to China, spurring Beijing’s push for domestic alternatives.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbeta.com.tw/articles/tech/1445926.htm">全新国产DUV光刻机曝光：“套刻 8nm”... - cnBeta.COM</a></li>
<li><a href="https://school.gugu.fund/ai/answer/duv和eu-2-1057457">DUV和EUV光刻機在晶片製造中的具體應用有何不同？ | AIGC</a></li>

</ul>
</details>

**Tags**: `#半导体`, `#光刻机`, `#国产替代`, `#芯片制造`, `#技术突破`

---