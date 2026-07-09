---
layout: default
title: "Horizon Summary: 2026-07-09 (EN)"
date: 2026-07-09
lang: en
---

> From 36 items, 13 important content pieces were selected

---

1. [Rewriting Bun in Rust](#item-1) ⭐️ 9.0/10
2. [OpenAI Launches GPT-Live Full-Duplex Voice Model](#item-2) ⭐️ 9.0/10
3. [TypeScript 7.0 Released: Go Rewrite Boosts Speed Up to 12x](#item-3) ⭐️ 9.0/10
4. [Meta to Mass-Produce In-House AI Chip Iris in September](#item-4) ⭐️ 9.0/10
5. [FTC settlement grants farmers right to repair John Deere equipment](#item-5) ⭐️ 8.0/10
6. [EU Parliament passes Chat Control 1.0, enabling warrantless message scanning](#item-6) ⭐️ 8.0/10
7. [Spider venom selectively kills varroa mites, spares bees](#item-7) ⭐️ 8.0/10
8. [xAI Releases Grok 4.5 with Improved Reasoning and Pricing](#item-8) ⭐️ 8.0/10
9. [Microsoft releases Flint, visualization language for AI agents](#item-9) ⭐️ 8.0/10
10. [OpenAI Proposes Fixes for Flawed Coding Benchmarks](#item-10) ⭐️ 8.0/10
11. [LingBot-Video: Open-Source Sparse-MoE Video Diffusion World Model](#item-11) ⭐️ 8.0/10
12. [Samsung Display Halts Vision Air Screen Development, Project Killed](#item-12) ⭐️ 8.0/10
13. [OpenAI Publishes National Security Principles, Bans Autonomous Weapons](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Rewriting Bun in Rust](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 9.0/10

Jarred Sumner, creator of the Bun JavaScript runtime, announced a full rewrite of Bun from Zig to Rust, leveraging AI coding agents to port the codebase in 11 days. This engineering shift addresses critical memory safety bugs that plagued Bun, and demonstrates that AI-assisted code rewrites can be cost-effective and reliable, potentially changing how large software projects approach language migrations. The rewrite cost approximately $165,000 in API tokens, using 5.9 billion uncached input tokens and 690 million output tokens. The new Rust version has been live in Claude Code since June 17, 2026, with 10% faster startup on Linux.

rss · Simon Willison · Jul 8, 23:57

**Background**: Bun is a high-performance JavaScript runtime and toolchain built initially in Zig, a systems language emphasizing simplicity and performance. Zig requires manual memory management, which led to bugs like use-after-free. Rust provides memory safety guarantees through its ownership system. The rewrite was enabled by Bun's comprehensive TypeScript test suite acting as a conformance suite for AI agents.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://bun.com/">Bun — A fast all-in-one JavaScript runtime</a></li>

</ul>
</details>

**Tags**: `#Bun`, `#Rust`, `#Zig`, `#JavaScript runtime`, `#software engineering`

---

<a id="item-2"></a>
## [OpenAI Launches GPT-Live Full-Duplex Voice Model](https://openai.com/index/introducing-gpt-live/) ⭐️ 9.0/10

OpenAI has launched GPT-Live, a new generation voice model that supports full-duplex real-time conversation, allowing simultaneous input and output, and is now rolling out to ChatGPT users worldwide. This marks a major advancement in voice AI, enabling more natural and interactive conversations, as users can interrupt or pause freely while the model handles complex tasks in the background using GPT-5.5. GPT-Live comes in two variants: GPT-Live-1 (for paid users) and GPT-Live-1 mini (for free users), and it includes visual cards for weather and stocks, with optimizations for background noise, but lacks video or screen sharing support.

telegram · zaihuapd · Jul 8, 17:15

**Background**: Full-duplex voice AI allows simultaneous listening and speaking, unlike traditional turn-based systems. ChatGPT's previous voice mode used an older GPT-4o model with limited capabilities. GPT-Live leverages GPT-5.5 for background reasoning, enabling richer interactions.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-live/">Introducing GPT-Live | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>

</ul>
</details>

**Discussion**: Early tester Simon Willison reported that GPT-Live is very impressive and enables hour-long conversations, but encountered a bug where the model interrupted him by laughing at non-jokes, which felt rude. He reported it and OpenAI seems to have reduced the issue.

**Tags**: `#OpenAI`, `#GPT-Live`, `#voice AI`, `#real-time dialogue`, `#ChatGPT`

---

<a id="item-3"></a>
## [TypeScript 7.0 Released: Go Rewrite Boosts Speed Up to 12x](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

Microsoft released TypeScript 7.0, a native version rewritten in Go, achieving 8-12x build speed improvements with support for shared-memory multithreading. This major performance leap significantly improves developer productivity in the JavaScript ecosystem, especially for large codebases, and sets a new standard for compiler tooling. Users can customize parallelism with --checkers and --builders flags, and a compatibility package allows coexistence with TypeScript 6; however, toolchain support for Vue and Svelte is not yet ready, requiring use of the old version.

telegram · zaihuapd · Jul 9, 04:01

**Background**: TypeScript is a typed superset of JavaScript that compiles to plain JavaScript, widely used for large-scale applications. The Language Server Protocol (LSP) standardizes communication between editors and language servers, enabling features like auto-completion; TypeScript 7.0's new language server uses LSP for editor integration.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Language_Server_Protocol">Language Server Protocol - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#TypeScript`, `#Go`, `#Performance`, `#Release`, `#Compilers`

---

<a id="item-4"></a>
## [Meta to Mass-Produce In-House AI Chip Iris in September](https://www.reuters.com/world/asia-pacific/meta-put-ai-chip-into-production-september-it-looks-double-computing-capacity-2026-07-09/) ⭐️ 9.0/10

Meta plans to start mass production of its self-developed AI chip, codenamed Iris, in September 2026, as part of its fourth-generation MTIA (Meta Training and Inference Accelerator) project, aiming to double its computing capacity by 2027. This move reduces Meta's reliance on external suppliers like Nvidia and AMD for AI chips, potentially lowering costs and increasing control over its AI infrastructure, which is critical for powering its massive AI workloads and metaverse ambitions. The Iris chip is designed in partnership with Broadcom and manufactured by TSMC, and testing took only six weeks with no major issues found. Meta plans to deploy 7 gigawatts (GW) of compute infrastructure this year and double it to 14 GW by 2027, with AI infrastructure spending expected to reach $145 billion in 2026.

telegram · zaihuapd · Jul 9, 12:37

**Background**: Meta has been developing its own AI chips under the MTIA family to optimize performance and efficiency for its unique workloads. While the Iris chip will supplement, not replace, the large volumes of GPUs Meta buys from Nvidia and AMD, it represents a strategic shift toward in-house silicon to support the company's massive data center expansion plans. The term "gigawatt" (GW) is increasingly used to describe the power capacity of hyperscale data centers, with 1 GW capable of housing around 200,000 Nvidia GB200 chips.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/09/meta-to-put-ai-chip-into-production-in-september-report.html">Meta to put AI chip into production in September as it looks to double computing capacity, Reuters reports</a></li>
<li><a href="https://ai.meta.com/blog/next-generation-meta-training-inference-accelerator-AI-MTIA/">Our next generation Meta Training and Inference Accelerator</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/meta-start-production-iris-ai-122141801.html">Meta to start production of Iris AI chip in September 2026</a></li>

</ul>
</details>

**Tags**: `#AI Chips`, `#Meta`, `#Hardware`, `#Infrastructure`, `#Semiconductors`

---

<a id="item-5"></a>
## [FTC settlement grants farmers right to repair John Deere equipment](https://apnews.com/article/john-deere-right-to-repair-agriculture-equipment-cb7514ffedb95c130a976af661f2bc02) ⭐️ 8.0/10

John Deere has settled with the Federal Trade Commission, agreeing to allow farmers and independent repair shops to repair their own equipment, ending years of restrictions. The settlement requires Deere to provide diagnostic tools, manuals, and parts to owners. This settlement sets a significant precedent for the right-to-repair movement, potentially forcing other manufacturers to follow suit. It empowers farmers who have been locked into dealer-only repairs, saving time and money, and challenges corporate control over product servicing. John Deere will pay $1 million collectively to five states for antitrust enforcement costs and be subject to strict compliance oversight for 10 years. The company faced allegations that its software restrictions forced farmers to use authorized dealers for repairs.

hackernews · djoldman · Jul 8, 23:37 · [Discussion](https://news.ycombinator.com/item?id=48838876)

**Background**: The right-to-repair movement advocates for consumers and small businesses to be able to repair products they own without being forced to use authorized service providers. In agriculture, modern tractors often contain software locks that prevent third-party repairs, and manufacturers like John Deere have been criticized for monopolizing repair services. The FTC settlement is a major victory for advocates who have pushed for legislation and enforcement actions.

**Discussion**: Commenters celebrated the settlement, with many praising activist Louis Rossmann for his work on right-to-repair. Some expressed skepticism about the small fine, noting Deere's massive profits, while others debated the broader implications for tech companies and regulatory capture.

**Tags**: `#right-to-repair`, `#antitrust`, `#consumer rights`, `#regulatory capture`, `#John Deere`

---

<a id="item-6"></a>
## [EU Parliament passes Chat Control 1.0, enabling warrantless message scanning](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 8.0/10

The EU Parliament has passed Chat Control 1.0, allowing US tech companies to scan private messages without a warrant or prior suspicion, a measure it had rejected twice earlier in March. This legislation undermines end-to-end encryption, threatening privacy rights for all EU citizens and setting a precedent for mass surveillance that could spread globally. Despite 314 MEPs voting against and only 276 in favor, the motion to reject failed because it required an absolute majority of 361 votes; the scanning is now permitted until 2028.

hackernews · rapnie · Jul 9, 11:03 · [Discussion](https://news.ycombinator.com/item?id=48843923)

**Background**: Chat Control is a series of EU proposals aimed at combating child sexual abuse material (CSAM) by requiring platforms to scan private communications. Critics argue it effectively breaks end-to-end encryption and violates fundamental privacy rights. The law targets direct messages on platforms like Instagram, Discord, Snapchat, Skype, Gmail, and iCloud.

**Discussion**: Comments express frustration with the procedural manipulation, noting that the vote was rushed under urgency procedure on the last session before summer break. Some users discuss technical workarounds like steganography to avoid detection, while others argue that this could radicalize people against the EU.

**Tags**: `#privacy`, `#EU legislation`, `#encryption`, `#surveillance`

---

<a id="item-7"></a>
## [Spider venom selectively kills varroa mites, spares bees](https://connectsci.au/news/news-parent/9703/Spider-venom-kills-varroa-mites-without-harming) ⭐️ 8.0/10

Researchers have discovered that peptides from spider venom can selectively kill Varroa destructor mites without harming honeybees, offering a promising new biological treatment for beekeepers. Varroa mites are the most devastating pest for honeybee colonies worldwide, contributing to colony collapse disorder. A selective, non-toxic treatment could reduce reliance on chemical miticides that contaminate honey and harm bees. The spider venom peptides target mite-specific ion channels, leaving honeybee physiology unaffected. Further research is needed to develop a practical formulation for hive application, but the initial results show high specificity.

hackernews · Jedd · Jul 9, 05:14 · [Discussion](https://news.ycombinator.com/item?id=48841259)

**Background**: Varroa destructor is an external parasitic mite that feeds on honeybees and transmits debilitating viruses like deformed wing virus. Without management, infested colonies typically collapse within 2–3 years in temperate climates. Current control relies on synthetic miticides, which can lead to resistance and honey contamination.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Varroa_mite">Varroa mite</a></li>

</ul>
</details>

**Discussion**: Beekeepers in the discussion emphasize that mite control is the most time-consuming aspect of modern beekeeping, and current treatments often render honey inedible. Some commenters reference alternative approaches like powdered sugar dusting and mycelium-based immune boosters, suggesting interest in integrated pest management.

**Tags**: `#biotechnology`, `#beekeeping`, `#pest control`, `#research`

---

<a id="item-8"></a>
## [xAI Releases Grok 4.5 with Improved Reasoning and Pricing](https://x.ai/news/grok-4-5) ⭐️ 8.0/10

xAI has released Grok 4.5, a large language model that claims 4x better reasoning efficiency compared to Opus, with a pricing of $2 per million input tokens and $6 per million output tokens. The model was trained on trillions of tokens of Cursor data, capturing developer-agent interactions. Grok 4.5 offers competitive performance at a significantly lower cost than many existing models, potentially accelerating adoption of AI in coding and reasoning tasks. Its training on real-world developer interactions could lead to better agentic coding workflows. Grok 4.5 is priced at $2/M input tokens and $6/M output tokens, with benchmarks suggesting performance around the level of Opus 4.7. The model was trained using a dataset from Cursor that includes trillions of tokens of developer-agent interactions.

hackernews · BoumTAC · Jul 8, 18:00 · [Discussion](https://news.ycombinator.com/item?id=48835111)

**Background**: Grok is a series of large language models developed by xAI (SpaceXAI). Reasoning efficiency refers to a model's ability to solve complex problems with minimal computational overhead. Cursor is an AI-powered code editor that captures detailed user interactions, which can be used to train models for coding tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://x.ai/">SpaceXAI — Creators of Grok, the AI Chatbot</a></li>

</ul>
</details>

**Discussion**: Comments on the release are polarized: some users highlight the model's cost-efficiency and technical gains, while others express distrust in xAI due to political alignment and concerns about CSAM. A common sentiment is a desire for more technical discussion and less political commentary.

**Tags**: `#AI`, `#Grok`, `#xAI`, `#Large Language Models`, `#Benchmarks`

---

<a id="item-9"></a>
## [Microsoft releases Flint, visualization language for AI agents](https://microsoft.github.io/flint-chart/#/) ⭐️ 8.0/10

Microsoft has released Flint, an intermediate visualization language designed to help AI agents create high-quality charts reliably by abstracting low-level visual decisions. Flint is open-source and includes an MCP server for easy integration with agent applications. Flint addresses a key limitation in AI-generated visualizations—balancing reliability and quality—by providing a high-level specification that a compiler optimizes into polished charts. This pattern of using a deterministic intermediate layer (like an IR) for LLM outputs is an emerging trend that could improve the robustness of agentic systems. Flint uses a semantic-type-based specification and includes a layout optimization engine to produce detailed, good-looking charts from simple specs. It currently does not natively support layering for multi-axis charts, but the team may consider composability in future.

hackernews · chenglong-hn · Jul 8, 17:46 · [Discussion](https://news.ycombinator.com/item?id=48834924)

**Background**: Current visualization languages like Vega or Vega-Lite are powerful but require AI agents to specify many low-level visual details, leading to either unreliable or verbose outputs. Flint serves as an intermediate language that bridges the gap between high-level user intent and low-level rendering, similar to how intermediate representations work in compilers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/research/blog/flint-a-visualization-language-for-the-ai-era/">Flint: A visualization language for the AI era - Microsoft ...</a></li>
<li><a href="https://microsoft.github.io/flint-chart/">Flint: A Visualization Language for the AI Era</a></li>
<li><a href="https://github.com/microsoft/flint-chart">GitHub - microsoft/flint-chart: Flint is a visualization ...</a></li>

</ul>
</details>

**Discussion**: Commenters appreciate Flint's approach but raise several points: some see it as simply an easy-to-generate language for charts, while others question its advantage over existing tools like Vega. Accessibility is also highlighted as an important consideration for data visualizations. There is general agreement that the deterministic intermediate layer pattern will become more common in agentic systems.

**Tags**: `#visualization`, `#AI agents`, `#Microsoft`, `#intermediate language`, `#Vega`

---

<a id="item-10"></a>
## [OpenAI Proposes Fixes for Flawed Coding Benchmarks](https://openai.com/index/separating-signal-from-noise-coding-evaluations/) ⭐️ 8.0/10

OpenAI published an analysis identifying that about 30% of tasks in SWE-Bench Pro, a popular coding benchmark, have evaluation flaws such as underspecified prompts or low-coverage tests, and proposed a methodology to mitigate these issues. Flawed benchmarks can mislead the AI industry about model capabilities and hinder progress; improving evaluation rigor helps developers and researchers trust results and build better coding agents. The analysis manually reviewed 731 public tasks from SWE-Bench Pro, finding issues like overly strict tests, misleading prompts, and incomplete fix validation; OpenAI's proposed methodology includes automatic detection and human verification to clean benchmarks.

hackernews · sk4rekr0w · Jul 8, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48837396)

**Background**: SWE-Bench is a widely used benchmark for evaluating AI coding agents by having them solve real-world GitHub issues. However, many benchmark tasks contain flaws that cause incorrect pass/fail verdicts. OpenAI's work highlights the need for careful benchmark design to ensure evaluations reflect true model performance.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/separating-signal-from-noise-coding-evaluations/">Separating signal from noise in coding evaluations - OpenAI</a></li>
<li><a href="https://news.aibase.com/news/29502">OpenAI Criticizes AI Evaluation Benchmark: 731 Questions ...</a></li>
<li><a href="https://www.bestaitools.com/new-ai-coding-benchmark-exposes-major-flaws-in-industry-standards-and-crowns-gpt-5-5-as-clear-leader/">New AI coding benchmark exposes major flaws in industry ...</a></li>

</ul>
</details>

**Discussion**: Community comments express agreement with the criticism, noting similar issues in other benchmarks like Terminal Bench 2 and call for new metrics that combine efficiency and intelligence. Some readers argue that these flaws mirror real-world software development where requirements are often ambiguous.

**Tags**: `#AI benchmarking`, `#coding evaluations`, `#machine learning`, `#software testing`, `#OpenAI`

---

<a id="item-11"></a>
## [LingBot-Video: Open-Source Sparse-MoE Video Diffusion World Model](https://www.reddit.com/r/MachineLearning/comments/1ur0bxq/lingbotvideo_sparsemoe_video_diffusion/) ⭐️ 8.0/10

LingBot-Video is an open-source video diffusion transformer with a DeepSeek-V3-style sparse mixture-of-experts (MoE) architecture, totaling 13B parameters but activating only 1.4B per step. It is post-trained with reinforcement learning using six rewards, including a physical-plausibility reward graded by a vision-language model (VLM). This work pushes the boundary of combining sparse MoE efficiency with video diffusion for world modeling, offering an open-weight alternative that could reduce computational costs for robot simulation and policy evaluation. However, the community questions whether a VLM can reliably judge physics, and whether the model truly functions as a world model rather than a sophisticated video generator. The model uses a single-stream diffusion transformer with 128 experts and top-8 routing, inspired by DeepSeek-V3. It supports an action-to-video mode for predicting robot rollouts from action and hand-pose conditions, and achieves top average scores on the RBench benchmark, though reasoning-heavy dimensions still trail closed models.

reddit · r/MachineLearning · /u/Savings-Display5123 · Jul 8, 17:58

**Background**: Sparse mixture-of-experts (MoE) is a neural network architecture that activates only a subset of its parameters per input, enabling larger total capacity with lower inference cost—DeepSeek-V3 popularized this with 671B total and 37B active parameters. Video diffusion models generate video by iteratively denoising random noise, while world models simulate environment dynamics to enable planning and policy evaluation. LingBot-Video combines these ideas with reinforcement learning to improve physical plausibility.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>
<li><a href="https://github.com/sgl-project/sglang">GitHub - sgl-project/sglang: SGLang is a high-performance ...</a></li>

</ul>
</details>

**Discussion**: The Reddit community expresses skepticism about using a VLM to judge physical plausibility, warning of Goodhart's law where the model may over-optimize for VLM scores without true physics understanding. Commenters also question the lack of closed-loop robot evaluation, arguing that without such metrics it is unclear if LingBot-Video is a genuine world model or just a high-quality video generator.

**Tags**: `#video diffusion`, `#sparse MoE`, `#world model`, `#reinforcement learning`, `#robot simulation`

---

<a id="item-12"></a>
## [Samsung Display Halts Vision Air Screen Development, Project Killed](https://finance.sina.com.cn/stock/t/2026-07-09/doc-inihczpn4610103.shtml) ⭐️ 8.0/10

Samsung Display has canceled the development of G-VR display panels for Apple's Vision Air headset, effectively ending the project. Apple is shifting its strategic focus to AI-powered smart glasses. This cancellation signals Apple's retreat from the high-end VR headset market due to poor sales of the Vision Pro. The shift to AI smart glasses indicates a major pivot in Apple's spatial computing strategy, with implications for the entire AR/VR industry. The G-VR panel was an OLED-on-glass technology with a PPI of about 1600-1700, half that of the Vision Pro's 3386 PPI, aiming to reduce costs. Mass production was planned for after 2028.

telegram · zaihuapd · Jul 9, 03:16

**Background**: OLEDoS (OLED-on-Silicon) is a microdisplay technology used in high-end VR/AR headsets, offering high brightness and resolution on a silicon substrate. The Vision Pro uses OLEDoS panels with over 3000 PPI, but its high cost and limited app ecosystem led to weak sales. The G-VR project aimed to create a cheaper alternative using a glass substrate instead of silicon.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.biggo.com/news/0a1e5d25-0d64-40df-b883-768688282ff3">Apple Pulls the Plug on Cheaper Vision Pro Display Project ...</a></li>
<li><a href="https://9to5mac.com/2026/07/08/component-development-for-cheaper-apple-vision-pro-reportedly-scrapped/">Component development for cheaper Apple Vision Pro reportedly ...</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#VR/AR`, `#Samsung Display`, `#product cancellation`, `#AI smart glasses`

---

<a id="item-13"></a>
## [OpenAI Publishes National Security Principles, Bans Autonomous Weapons](https://openai.com/index/government-national-security-partnerships/) ⭐️ 8.0/10

OpenAI has published its national security principles, explicitly prohibiting the use of its technology for mass surveillance, autonomous weapons, and high-risk automated decision-making. It also announced expanded defense collaborations with U.S. allies through the Daybreak cybersecurity program. This policy move sets clear boundaries for AI use in military and surveillance contexts, influencing global AI governance and defense partnerships. It could shape how other AI companies approach national security collaborations. The principles ban high-risk automated decision-making, which refers to AI systems used in finance, public administration, surveillance, and other domains that require stricter oversight. The Daybreak program, which includes the full version of GPT-5.5-Cyber, provides advanced defensive tools to verified defenders.

telegram · zaihuapd · Jul 9, 13:22

**Background**: National security principles for AI have become a key policy area as governments explore military AI applications. High-risk automated decision-making systems are those that could cause significant harm if erroneous, such as in medical diagnosis or autonomous driving. OpenAI's Daybreak initiative is a cybersecurity program that uses advanced AI models for vulnerability discovery and automated patching.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/daybreak/">Daybreak | OpenAI for cybersecurity</a></li>
<li><a href="https://baike.baidu.com/item/高风险人工智能系统/67234097">高风险人工智能系统 - 百度百科</a></li>
<li><a href="https://www.sohu.com/a/838817524_121798711">谷歌更新政策：引导高风险领域中的AI决策，人工监督成关键_自动化_技...</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#OpenAI`, `#national security`, `#AI safety`, `#autonomous weapons`

---