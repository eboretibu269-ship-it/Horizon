---
layout: default
title: "Horizon Summary: 2026-07-09 (EN)"
date: 2026-07-09
lang: en
---

> From 35 items, 12 important content pieces were selected

---

1. [Spider venom selectively kills varroa mites, spares honeybees](#item-1) ⭐️ 9.0/10
2. [Rewriting Bun in Rust: A Historic Migration](#item-2) ⭐️ 9.0/10
3. [TypeScript 7.0 with Go-based native rewrite released, up to 12x faster](#item-3) ⭐️ 9.0/10
4. [Ant Group LingBot Open-Sources World's First MoE Embodied Video Foundation Model](#item-4) ⭐️ 9.0/10
5. [Meta's Self-Developed AI Chip 'Iris' to Enter Production in September](#item-5) ⭐️ 9.0/10
6. [John Deere Settles FTC Right-to-Repair Case](#item-6) ⭐️ 8.0/10
7. [EU Parliament passes Chat Control 1.0 allowing warrantless message scanning](#item-7) ⭐️ 8.0/10
8. [OpenAI Exposes Flaws in Coding Benchmarks](#item-8) ⭐️ 8.0/10
9. [OpenAI Launches GPT-Live Voice Mode with GPT-5.5 Delegation](#item-9) ⭐️ 8.0/10
10. [Samsung Display Cancels Apple Vision Air Panel; Project Ends](#item-10) ⭐️ 8.0/10
11. [National Supercomputing Internet Core Node Launches in Zhengzhou with 100,000+ Domestic AI Cards](#item-11) ⭐️ 8.0/10
12. [OpenAI Releases National Security Principles](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Spider venom selectively kills varroa mites, spares honeybees](https://connectsci.au/news/news-parent/9703/Spider-venom-kills-varroa-mites-without-harming) ⭐️ 9.0/10

Researchers have discovered that peptides derived from spider venom can selectively kill varroa mites without harming honeybees, offering a novel approach to controlling one of the most destructive pests in beekeeping. Varroa mites are a major cause of honeybee colony collapse worldwide, threatening pollination and agriculture. A selective, bee-safe treatment could reduce colony losses and lessen reliance on traditional miticides that often contaminate honey or face resistance issues. The spider-venom peptides specifically target varroa mites while leaving bees unharmed, potentially avoiding the honey contamination common with current treatments. Further research is needed to develop a practical formulation for beekeepers.

hackernews · Jedd · Jul 9, 05:14 · [Discussion](https://news.ycombinator.com/item?id=48841259)

**Background**: Varroa destructor is an external parasitic mite that feeds on honeybees and transmits debilitating viruses, leading to colony collapse if left untreated. Current chemical miticides can be toxic to bees, leave residues in honey, and face increasing resistance. Spider venom peptides have long been studied as bioinsecticides due to their potent and selective insecticidal activity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Varroa_mites">Varroa mites</a></li>
<li><a href="https://cen.acs.org/articles/95/i11/Spider-venom-insecticide-whose-time.html">Spider venom: An insecticide whose time has come? - C&EN</a></li>

</ul>
</details>

**Discussion**: Commenters expressed cautious optimism, with many beekeepers noting that mite control is currently labor-intensive and treatments often make honey inedible. Some questioned the cost compared to existing methods like powdered sugar dusting, while others recommended related research on mycelium-based bee immune boosters and discussed the potential of using native bees instead of honeybees.

**Tags**: `#bee conservation`, `#varroa mites`, `#spider venom`, `#pest control`, `#agriculture`

---

<a id="item-2"></a>
## [Rewriting Bun in Rust: A Historic Migration](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 9.0/10

Jarred Sumner, creator of the Bun JavaScript runtime, documented the complete rewrite of Bun from Zig to Rust, citing improved memory safety and stability. The rewrite was largely automated using AI coding agents and cost approximately $165,000 in API tokens. This rewrite demonstrates that large-scale, high-stakes software migrations previously considered impossible can now be executed with the help of advanced AI agents. It also strengthens Bun's reliability, potentially accelerating its adoption as a Node.js alternative. The rewrite took 11 days of agentic work, consuming 5.9 billion uncached input tokens and 690 million output tokens. The new Rust-based Bun has been deployed in Claude Code since June 17, 2026, and shows 10% faster startup on Linux.

rss · Simon Willison · Jul 8, 23:57

**Background**: Bun is a JavaScript runtime, bundler, and package manager created by Jarred Sumner, originally written in Zig. Zig is a systems language that requires manual memory management, which led to bugs like use-after-free errors. Rust offers memory safety guarantees through its ownership model and RAII patterns, making it a compelling choice for a runtime handling mixed garbage-collected and manually-managed memory.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>

</ul>
</details>

**Tags**: `#Bun`, `#Rust`, `#Zig`, `#JavaScript runtime`, `#software engineering`

---

<a id="item-3"></a>
## [TypeScript 7.0 with Go-based native rewrite released, up to 12x faster](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

Microsoft has released TypeScript 7.0, a complete rewrite in Go that delivers 8-12x faster build times and support for shared-memory multi-threading. Users can install it via npm, and editors support the new language server through LSP. This release represents a dramatic performance improvement for TypeScript developers, reducing compilation times significantly for large codebases. The Go rewrite also enables better scalability with multi-threading, potentially changing how the TypeScript ecosystem approaches tooling. New command-line options --checkers and --builders allow customization of parallelism. A compatibility package enables side-by-side use with TypeScript 6, but tools for embedded languages like Vue and Svelte are not yet supported and must use the older version.

telegram · zaihuapd · Jul 9, 04:01

**Background**: TypeScript is a superset of JavaScript that adds static typing, widely used for large-scale web development. The previous TypeScript compiler was written in TypeScript itself (self-hosted) and compiled to JavaScript, which limited performance. By rewriting in Go—a compiled, natively fast language—Microsoft achieves significant speed gains. The Language Server Protocol (LSP) standardizes communication between editors and language servers, enabling the new TypeScript server to work with most IDEs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Language_Server_Protocol">Language Server Protocol</a></li>
<li><a href="https://microsoft.github.io/language-server-protocol/">Official page for Language Server Protocol</a></li>

</ul>
</details>

**Tags**: `#TypeScript`, `#Go`, `#performance`, `#language release`, `#Microsoft`

---

<a id="item-4"></a>
## [Ant Group LingBot Open-Sources World's First MoE Embodied Video Foundation Model](https://www.qbitai.com/2026/07/446458.html) ⭐️ 9.0/10

Ant Group's LingBot team has open-sourced LingBot-Video, the world's first Mixture-of-Experts (MoE) based embodied video generation foundation model, with 30B total parameters and 3B active parameters. It achieves state-of-the-art performance on the RBench benchmark with a score of 0.620, surpassing models like Wan2.6, Seedance1.5 Pro, and Cosmos3 Super. This open-sourcing lowers the barrier for embodied AI research by providing a high-performance, efficient foundation model under Apache 2.0, enabling applications such as robot action prediction, simulation data generation, and world model studies. The MoE architecture achieves roughly 3x inference efficiency over dense models of similar scale, making it practical for real-world deployment. LingBot-Video uses a DiT+MoE architecture with a DeepSeek-V3-style sparse MoE (128 experts, top-8 routing, 1.4B active out of 13B per layer). It incorporates a six-reward reinforcement learning post-training system, including a physical-plausibility reward evaluated by a VLM, and supports an action-to-video mode that predicts robot rollouts from action and hand-pose conditions.

telegram · zaihuapd · Jul 9, 04:30

**Background**: Mixture-of-Experts (MoE) is a neural network architecture that divides the model into multiple 'experts' and activates only a subset per input, improving efficiency without sacrificing capacity. Diffusion Transformers (DiT) combine diffusion models with transformer backbones, enabling high-quality video generation. Embodied AI focuses on agents that perceive and act in physical environments, with video generation serving as a tool for planning and simulation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/deepseek-v3">DeepSeek-V3: Open Sparse MoE Model</a></li>
<li><a href="https://encord.com/blog/diffusion-models-with-transformers/">Diffusion Transformer (DiT) Models: A Beginner’s Guide</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion raised concerns about the physical-plausibility reward being judged by a VLM (Vision-Language Model), questioning whether it is a defensible measure or prone to reward hacking despite added real-video negatives. Commenters also noted the lack of closed-loop robot results and that the model is only second on general text-to-video evaluation, with reasoning-heavy dimensions still led by closed models.

**Tags**: `#embodied AI`, `#video generation`, `#MoE`, `#open source`, `#robotics`

---

<a id="item-5"></a>
## [Meta's Self-Developed AI Chip 'Iris' to Enter Production in September](https://www.reuters.com/world/asia-pacific/meta-put-ai-chip-into-production-september-it-looks-double-computing-capacity-2026-07-09/) ⭐️ 9.0/10

Meta plans to mass-produce its self-designed AI chip code-named 'Iris' starting in September 2026. The chip is part of the fourth generation of the Meta Training and Inference Accelerator (MTIA) program and aims to double Meta's computing capacity by 2027. This move reduces Meta's reliance on external suppliers like NVIDIA and AMD, giving it more control over its AI infrastructure. It also signals a major trend among tech giants toward vertical integration in AI hardware. The 'Iris' chip was co-designed with Broadcom and will be manufactured by TSMC; testing took only six weeks with no major issues found. Meta plans to deploy 7 gigawatts of computing infrastructure this year and increase it to 14 gigawatts by 2027, investing up to $145 billion in AI infrastructure this year.

telegram · zaihuapd · Jul 9, 12:37

**Background**: Meta's MTIA (Meta Training and Inference Accelerator) program is a family of custom chips designed for Meta's AI workloads, covering ranking and recommendation as well as generative AI. The program has rapidly evolved across four generations, with Iris being the latest addition. By developing its own chips, Meta aims to optimize performance and reduce costs compared to buying from commercial vendors.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/09/meta-to-put-ai-chip-into-production-in-september-report.html">Meta to put AI chip into production in September as it looks to double computing capacity, Reuters reports</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/meta-start-production-iris-ai-122141801.html">Meta to start production of Iris AI chip in September 2026</a></li>

</ul>
</details>

**Tags**: `#AI`, `#hardware`, `#Meta`, `#chip`, `#infrastructure`

---

<a id="item-6"></a>
## [John Deere Settles FTC Right-to-Repair Case](https://apnews.com/article/john-deere-right-to-repair-agriculture-equipment-cb7514ffedb95c130a976af661f2bc02) ⭐️ 8.0/10

The Federal Trade Commission (FTC) reached a settlement with John Deere, requiring the company to allow farmers and independent repair shops to repair Deere equipment. The settlement mandates that Deere provide repair tools, software, and documentation for at least 10 years. This settlement is a significant victory for the right-to-repair movement, which advocates for consumers' ability to fix products they own. It sets a precedent for other manufacturers, especially in agriculture and technology, potentially reducing costs for farmers and increasing equipment longevity. Deere must pay $1 million collectively to five states for antitrust enforcement costs and will be subject to strict compliance oversight for 10 years. The settlement applies only to John Deere and does not create a binding legal precedent for other companies, but it may encourage similar actions.

hackernews · djoldman · Jul 8, 23:37 · [Discussion](https://news.ycombinator.com/item?id=48838876)

**Background**: The right-to-repair movement seeks to give consumers and independent repair shops access to the tools, parts, and software needed to repair products like electronics, vehicles, and farm equipment. Manufacturers often restrict repairs to maintain control and profit from aftermarket services. Louis Rossmann is a prominent advocate who runs Consumer Rights Wiki and supports initiatives like the FULU Foundation bounty for making Ring cameras work without Amazon servers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Right_to_repair_movement">Right to repair movement</a></li>

</ul>
</details>

**Discussion**: Community comments praised Louis Rossmann's advocacy but criticized the small fine as insufficient deterrent. Some expressed disbelief that such a basic right required litigation, while others noted the irony of tech workers supporting right-to-repair while building closed ecosystems. A commenter emphasized that right to repair is a fundamental freedom, not a negotiable business term.

**Tags**: `#right to repair`, `#FTC`, `#John Deere`, `#agriculture`, `#consumer rights`

---

<a id="item-7"></a>
## [EU Parliament passes Chat Control 1.0 allowing warrantless message scanning](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 8.0/10

The EU Parliament passed Chat Control 1.0 on July 9, 2026, allowing US tech companies to scan private messages without a warrant or prior suspicion, after the regulation had been rejected twice in March 2026. This regulation undermines end-to-end encryption and mass surveillance, affecting millions of EU citizens' privacy, and was pushed through via controversial parliamentary procedures, raising concerns about democratic legitimacy. The motion to reject the regulation failed to secure an absolute majority of 361 votes, with 314 against, 276 in favor, 17 abstentions, and 113 absent; the measure will remain in effect until 2028 and applies to direct messages on platforms like Instagram, Discord, Snapchat, Skype, Xbox, Gmail, and iCloud.

hackernews · rapnie · Jul 9, 11:03 · [Discussion](https://news.ycombinator.com/item?id=48843923)

**Background**: Chat Control, officially the Child Sexual Abuse Regulation (CSAR), was proposed by the European Commission in May 2022 to combat online child sexual abuse. Critics argue it mandates mass surveillance of all private communications and cannot be implemented without breaking encryption, leading to false positives and privacy violations. The original proposal was rejected in March 2026 but was revived and fast-tracked for a decisive vote in July 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control_1.0">Chat Control 1.0</a></li>

</ul>
</details>

**Discussion**: Community comments express strong disapproval of the procedural tactics used, such as holding the vote just before the summer break and requiring an absolute majority to reject. Users accuse the EU of using parliamentary tricks to pass unpopular legislation and warn that this could erode trust in the EU project.

**Tags**: `#privacy`, `#EU policy`, `#surveillance`, `#chat control`, `#digital rights`

---

<a id="item-8"></a>
## [OpenAI Exposes Flaws in Coding Benchmarks](https://openai.com/index/separating-signal-from-noise-coding-evaluations/) ⭐️ 8.0/10

OpenAI identified four common failure modes in coding benchmarks—overly strict tests, underspecified prompts, low coverage, and misleading prompts—that distort model evaluation results. This matters because flawed benchmarks can lead to inaccurate comparisons of AI coding abilities, potentially misleading developers and organizations about model performance. The findings are based on OpenAI's manual review of fewer than 800 tasks in their benchmark, highlighting that small benchmark sizes can be thoroughly vetted by engineers.

hackernews · sk4rekr0w · Jul 8, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48837396)

**Background**: Coding benchmarks are standardized tests used to evaluate how well AI models can write or understand code. Common benchmarks like HumanEval often have hidden test cases that may not align with the prompt, leading to false negatives or positives.

**Discussion**: Community members noted that the same issues extend beyond coding benchmarks, with some calling for cost-aware benchmarks that measure efficiency alongside intelligence. Others criticized that the fundamental problem is that tasks assigned to developers are often incomplete or contradictory.

**Tags**: `#benchmarks`, `#coding evaluations`, `#AI evaluation`, `#OpenAI`, `#software testing`

---

<a id="item-9"></a>
## [OpenAI Launches GPT-Live Voice Mode with GPT-5.5 Delegation](https://simonwillison.net/2026/Jul/8/introducing-gptlive/#atom-everything) ⭐️ 8.0/10

OpenAI has introduced GPT-Live, a new voice mode for ChatGPT that uses an upgraded model and can delegate complex tasks to GPT-5.5 in the background while maintaining conversation flow. This upgrade significantly improves the utility of voice interactions with ChatGPT, enabling more natural and capable conversations, and demonstrates OpenAI's multi-model architecture for handling diverse tasks. GPT-Live uses a newer model than the previous GPT-4o era model, with a knowledge cut-off updated to be more recent, and OpenAI plans to continuously update the frontier model used in the background. During preview, a bug caused the model to interrupt with laughter at non-jokes, which OpenAI reportedly fixed.

rss · Simon Willison · Jul 8, 23:20

**Background**: GPT-Live is a new voice model from OpenAI powering ChatGPT Voice. It can delegate harder tasks to GPT-5.5, a frontier model released in April 2026 with strong coding and reasoning capabilities. Previous ChatGPT voice mode was based on an older GPT-4o model with a 2024 knowledge cutoff.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-live/">Introducing GPT-Live | OpenAI</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5-5/">Introducing GPT-5.5 | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#ChatGPT`, `#voice mode`, `#GPT-Live`, `#GPT-5.5`

---

<a id="item-10"></a>
## [Samsung Display Cancels Apple Vision Air Panel; Project Ends](https://finance.sina.com.cn/stock/t/2026-07-09/doc-inihczpn4610103.shtml) ⭐️ 8.0/10

Samsung Display has canceled its development of display panels for Apple's Vision Air headset, effectively ending the project. The panel, codenamed G-VR, was based on improved OLEDoS technology with a PPI of 1600-1700, half that of Vision Pro's 3386 PPI, and was intended to reduce costs. This cancellation highlights Apple's strategic pivot from high-cost VR/AR headsets to AI smart glasses, following the Vision Pro's poor sales and lackluster ecosystem. It impacts the AR/VR supply chain and signals a shift in industry focus toward lighter, more practical wearable devices. The G-VR panel was designed for mass production after 2028, but Samsung Display pulled the plug. Apple had already reduced Vision Pro production, removed advertisements, and disbanded the development team, with Chinese pricing near 30,000 RMB and a 2-hour battery life.

telegram · zaihuapd · Jul 9, 03:16

**Background**: OLEDoS (OLED on Silicon) is a microdisplay technology combining organic LEDs with silicon backplanes to achieve high pixel density, used in VR/AR headsets. Apple's first headset, Vision Pro, featured a 3386 PPI display but suffered from high cost, heavy weight, limited battery life, and poor app ecosystem, leading to weak sales. The canceled Vision Air was meant to be a more affordable version, but Apple has now shifted focus to AI-powered smart glasses.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sciencedirect.com/science/article/pii/S2949829525000014">OLED-on-silicon (OLEDoS) microdisplays: Technology challenges, design considerations, and adaptation in eXtended Reality (XR) ecosystem – Review - ScienceDirect</a></li>
<li><a href="https://www.businessresearchinsights.com/market-reports/oledos-technology-market-112940">OLEDoS Technology Market Size Forecast & Outlook till 2035</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Samsung`, `#VR/AR`, `#Display Technology`, `#AI Smart Glasses`

---

<a id="item-11"></a>
## [National Supercomputing Internet Core Node Launches in Zhengzhou with 100,000+ Domestic AI Cards](https://36kr.com/newsflashes/3887797387344387) ⭐️ 8.0/10

On July 9, the core node of China's National Supercomputing Internet went live in Zhengzhou, providing over 100,000 cards of domestic AI computing power. This milestone significantly boosts China's domestic AI computing infrastructure, enabling large-scale AI model training and inference with locally produced hardware, reducing reliance on foreign chips. The node is the largest single domestic AI computing resource pool connected to the National Supercomputing Internet platform, and it also serves as a national hub for resource scheduling, operation management, and industry incubation.

telegram · zaihuapd · Jul 9, 07:00

**Background**: The National Supercomputing Internet is a nationwide initiative to interconnect supercomputing centers, providing unified resource scheduling. The core node in Zhengzhou acts as the central coordination point. Domestic AI computing cards refer to accelerators developed by Chinese companies, such as those from Huawei, Cambricon, or others.

**Tags**: `#supercomputing`, `#AI`, `#China`, `#computing infrastructure`, `#domestic computing`

---

<a id="item-12"></a>
## [OpenAI Releases National Security Principles](https://openai.com/index/government-national-security-partnerships/) ⭐️ 8.0/10

OpenAI has published a set of national security principles that explicitly ban the use of its technology for autonomous weapons, mass surveillance, and high-risk automated decision-making, while expanding defense collaborations with US allies. This policy marks a significant step in AI governance, setting clear red lines for military applications and signaling OpenAI's commitment to ethical use, which could influence industry standards and government regulations. The principles include hard restrictions on mass domestic surveillance and autonomous weapon systems, and OpenAI has partnered with countries including Australia, Canada, Japan, South Korea, France, Germany, Poland, the Netherlands, and EU institutions through the Daybreak cyber defense program.

telegram · zaihuapd · Jul 9, 13:22

**Background**: As AI systems become more powerful, concerns have grown about their potential misuse in warfare and surveillance. OpenAI, a leading AI research organization, has previously emphasized safety and ethical guidelines but had not specifically addressed national security partnerships until now.

**Tags**: `#AI governance`, `#national security`, `#OpenAI`, `#ethics`, `#policy`

---