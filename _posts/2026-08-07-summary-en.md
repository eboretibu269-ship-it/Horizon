---
layout: default
title: "Horizon Summary: 2026-08-07 (EN)"
date: 2026-08-07
lang: en
---

> From 28 items, 13 important content pieces were selected

---

1. [DeepSeek V4 Flash 0731 Impresses on ARC-AGI with Speed and Value](#item-1) ⭐️ 9.0/10
2. [OpenAI says Astra model may reach 'critical' cyberattack capability, could delay release](#item-2) ⭐️ 9.0/10
3. [Oracle Bans AI-Generated Contributions to OpenJDK](#item-3) ⭐️ 8.0/10
4. [Making Postgres 300x Faster for Analytics with Rust Query Engine](#item-4) ⭐️ 8.0/10
5. [2027 Memory Capacity Reportedly Sold Out Amid AI-Driven HBM Demand](#item-5) ⭐️ 8.0/10
6. [One Year of Fighting Scrapers on a 1.5-Million-Page Website](#item-6) ⭐️ 8.0/10
7. [New Mexico court orders Meta to pay $567m over children's mental health harms](#item-7) ⭐️ 8.0/10
8. [Show HN: Wyzer Language Aims to Prevent Distributed Deadlocks and Memory Bugs](#item-8) ⭐️ 8.0/10
9. [Tokenpocalypse: Companies Scramble to Cut AI Token Spending](#item-9) ⭐️ 8.0/10
10. [SpaceX 10GW Space Solar by 2027 Could Yield $300B ARR, Says SemiAnalysis](#item-10) ⭐️ 8.0/10
11. [Gemini's Long-Term Woes Are Google Cloud's Short-Term Gain](#item-11) ⭐️ 8.0/10
12. [US Probes Chinese AI Firms' Offshore Access to Nvidia Chips](#item-12) ⭐️ 8.0/10
13. [SK Hynix Confirms V10 NAND: 375-Layer Stacking with Wafer Bonding](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DeepSeek V4 Flash 0731 Impresses on ARC-AGI with Speed and Value](https://arcprize.org/results/deepseek-v4-flash-0731) ⭐️ 9.0/10

DeepSeek released V4 Flash 0731, an updated version of its V4 Flash model, which demonstrates strong performance and speed on the ARC-AGI benchmark. The release has drawn significant community attention for its cost-effectiveness and local execution capabilities. This release is significant because it shows a major open-model developer delivering competitive reasoning performance at a fraction of the cost of frontier systems, making advanced AI more accessible. It also highlights the growing importance of ARC-AGI-style benchmarks in evaluating real-world agentic intelligence. The 0731 release is a substantial update over the earlier V4 Flash preview, with users reporting a noticeable quality jump. On local dual RTX Pro 6000 Blackwell GPUs, users observe roughly 8k tok/s prefill and about 250 tok/s generation on a single stream, though some report regressions like infinite loops and wasted tokens during tool use.

hackernews · tosh · Aug 7, 17:56 · [Discussion](https://news.ycombinator.com/item?id=49214008)

**Background**: ARC-AGI (Abstraction and Reasoning Corpus for Artificial General Intelligence) is a benchmark that measures progress toward general intelligence by challenging models with novel, human-like reasoning tasks. The ARC Prize foundation, which runs the benchmark, has also introduced ARC-AGI-3, an interactive version that tests agentic intelligence in novel environments. DeepSeek V4 Flash's results on this benchmark indicate that open-weight models are closing the gap with frontier systems on reasoning-heavy tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi">ARC Prize - What is ARC-AGI?</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>

</ul>
</details>

**Discussion**: Community reactions are largely positive, with users praising the model's cost-effectiveness (running multiple sessions for under $5 per day) and its speed on local hardware. However, some users report regressions compared to the previous version, including infinite loops where the model talks to itself without executing tool calls and wastes tokens.

**Tags**: `#AI`, `#DeepSeek`, `#LLM`, `#ARC-AGI`, `#Machine Learning`

---

<a id="item-2"></a>
## [OpenAI says Astra model may reach 'critical' cyberattack capability, could delay release](https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/) ⭐️ 9.0/10

On August 7, 2026, OpenAI disclosed that its upcoming Astra model showed major advances in agentic coding and cybersecurity during internal evaluations, with initial results strong enough that OpenAI cannot rule out it reaching the 'critical' cyber capability threshold. Previous models like GPT-5.6-Sol were only rated 'high' on the same assessment. This marks a frontier AI model potentially able to autonomously discover and exploit zero-day vulnerabilities in hardened real systems without human intervention, a capability that could dramatically lower the barrier to sophisticated cyberattacks. The expanded safety testing and possible release delay set an important precedent for how AI labs handle critical-risk models, affecting the broader AI and cybersecurity landscape. OpenAI has suspended internal Astra activities that do not meet the strengthened safety requirements, and has implemented isolated test environments, enhanced encryption, and universal monitoring. The company will also work with government agencies and AI safety organizations on third-party testing, according to the report.

telegram · zaihuapd · Aug 7, 16:44

**Background**: OpenAI's Preparedness Framework is its structured process for tracking and preparing for catastrophic risks from frontier AI capabilities, with cybersecurity as one of the core tracked categories. Under the framework, reaching the 'critical' threshold means the model can autonomously discover and exploit zero-day vulnerabilities in hardened real systems, or plan and execute end-to-end novel cyberattacks from high-level objectives alone. Agentic coding refers to autonomous AI agents that plan, write, test, and modify code with minimal human intervention, a capability that directly relates to offensive cyber operations. Recent real-world cases, such as Google's disclosure of an AI-developed zero-day exploit for 2FA bypass, illustrate why such thresholds are taken seriously.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/updating-our-preparedness-framework/">Our updated Preparedness Framework | OpenAI</a></li>
<li><a href="https://cdn.openai.com/pdf/18a02b5d-6b67-4cec-ab64-68cdfbddebcd/preparedness-framework-v2.pdf">Preparedness Framework Version 2. Last updated: 15th April, 2025</a></li>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/ai-vulnerability-exploitation-initial-access">Adversaries Leverage AI for Vulnerability Exploitation, Augmented Operations, and Initial Access | Google Cloud Blog</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#cybersecurity`, `#OpenAI`, `#frontier AI`, `#model release`

---

<a id="item-3"></a>
## [Oracle Bans AI-Generated Contributions to OpenJDK](https://app.dealroom.co/news/feed/oracle-bans-ai-generated-code-from-openjdk-despite-ellison-s-claim-oracle-isn-t-writing-its-own-code) ⭐️ 8.0/10

Oracle has issued an interim policy prohibiting contributions generated by generative AI tools to OpenJDK. The policy, published on openjdk.org/legal/ai, will remain in effect until Oracle's legal team drafts a final version. OpenJDK is the reference implementation of Java and underpins a vast enterprise ecosystem, so this policy could influence how other open-source projects handle AI-generated code. It highlights the growing legal and provenance risks that AI-assisted development introduces to software supply chains. The interim policy is published on openjdk.org/legal/ai, and Oracle's lawyers are drafting the final version. The rationale includes avoiding legal liability for code provenance and not overburdening the already limited time of human reviewers.

hackernews · delduca · Aug 7, 17:36 · [Discussion](https://news.ycombinator.com/item?id=49213754)

**Background**: Code provenance refers to the verifiable, auditable history of where code came from, including who wrote it and how it was changed. With generative AI, provenance becomes murkier because AI output may be derived from copyrighted or licensed code, creating legal uncertainty. OpenJDK is a major open-source project, and Oracle's move reflects broader industry concerns about AI-generated code, licensing, and software supply chain transparency.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fortegrp.com/insights/understanding-code-provenance">Understanding Code Provenance in The Age of Generative AI</a></li>
<li><a href="https://www.gitclear.com/help/technical/code_provenance">What is "code provenance" and why does it matter? - GitClear</a></li>
<li><a href="https://jfrog.com/learn/grc/software-provenance/">What Is Software Provenance? | Secure Supply Chain Practices | JFrog</a></li>

</ul>
</details>

**Discussion**: Comments on the news are mixed. Some see the policy as a sensible risk-management decision given Java's history of copyright disputes, while others question whether Oracle, which is heavily invested in AI, will be able to enforce it consistently. Several commenters note the irony of Oracle banning AI code despite its own AI push, and point out that the core issue is provenance and legal liability rather than a rejection of AI tools.

**Tags**: `#OpenJDK`, `#AI-generated code`, `#Oracle`, `#open source`, `#legal policy`

---

<a id="item-4"></a>
## [Making Postgres 300x Faster for Analytics with Rust Query Engine](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/) ⭐️ 8.0/10

The post details how pgrust, a Rust-based query engine, makes Postgres hundreds of times faster (up to 300x) for analytics by using batching, operator fusion, and SIMD. The author also reports formal verification and differential fuzz testing over 1,000 user-facing functions to ensure logic parity with Postgres. This work shows a credible path to dramatically accelerate Postgres for analytical workloads without changing SQL semantics, which could influence the analytics database market. It also demonstrates the viability of adaptive planning and Rust-based reimplementations within the Postgres ecosystem. The optimizations focus on reducing CPU and memory bandwidth usage, using vectorized batching of 1024-plus rows per operation, operator fusion to avoid materializing intermediates, and SIMD instructions. The main article includes correctness proof directories and differential fuzzing, and the engine is designed to be a drop-in replacement for the Postgres query executor.

hackernews · poly2it · Aug 7, 11:00 · [Discussion](https://news.ycombinator.com/item?id=49208535)

**Background**: Traditional Postgres executes queries row-by-row using the volcano model, which is inefficient for analytics. Vectorized execution processes data in column-oriented batches, amortizing interpretation overhead and enabling SIMD. Operator fusion combines multiple query operators to reduce data materialization, a technique also used by modern engines like DuckDB and ClickHouse.

<details><summary>References</summary>
<ul>
<li><a href="https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/">Rebuilding Postgres for 300x faster analytics: batching, operator...</a></li>
<li><a href="https://clickhouse.com/resources/engineering/vectorized-query-execution">What is vectorized query execution? - clickhouse.com</a></li>
<li><a href="https://arxiv.org/pdf/1610.09166">Push vs. Pull-Based Loop Fusion in Query Engines</a></li>

</ul>
</details>

**Discussion**: The author (malisper) emphasized correctness as the top priority, citing formal verification and differential fuzz testing. Commenter sgt countered that trust in the official Postgres team matters more than performance, so adoption may be limited. Others praised the potential for adaptive planning and embedding pgrust as an alternative to SQLite/Turso.

**Tags**: `#postgres`, `#rust`, `#query-engine`, `#performance`, `#simd`

---

<a id="item-5"></a>
## [2027 Memory Capacity Reportedly Sold Out Amid AI-Driven HBM Demand](https://www.ign.com/articles/ramageddon-continues-another-year-as-2027-memory-capacity-is-reportedly-sold-out) ⭐️ 8.0/10

Memory capacity for 2027 has reportedly sold out, as HBM (High Bandwidth Memory) production consumes an increasing share of wafer supply and AI demand intensifies shortages. This signals prolonged memory shortages that will push up prices for DDR5 and other DRAM products, affecting consumers, PC builders, and data centers. It also highlights how AI infrastructure demand is reshaping the broader semiconductor supply chain. The HBM-to-DDR5 wafer capacity tradeoff is roughly 3-to-1: producing the same number of bits with HBM3E consumes about three times the wafer supply as DDR5. As a result, the ramp of HBM production directly constrains supply growth for non-HBM memory products.

hackernews · inigyou · Aug 7, 07:58 · [Discussion](https://news.ycombinator.com/item?id=49207236)

**Background**: HBM is a 3D-stacked DRAM architecture designed for high-bandwidth, low-power operation, widely used in AI accelerators and high-performance computing. As AI demand surges, memory makers prioritize HBM production, which yields higher margins but also consumes far more wafer area, squeezing capacity for commodity DDR5 memory and driving up prices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.micron.com/products/memory/hbm">High-bandwidth memory (HBM) | Micron Technology Inc.</a></li>
<li><a href="https://www.rambus.com/blogs/hbm3-everything-you-need-to-know/">High Bandwidth Memory (HBM): Everything You Need to Know - Rambus</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern over HBM eating into DDR5 wafer supply, citing the 3-to-1 capacity tradeoff, and warned of broader inflationary effects on consumer devices. Some suggested standardized upgradeable RAM interfaces, while others said the memory crunch makes them hesitate to embrace AI.

**Tags**: `#memory`, `#HBM`, `#AI`, `#supply chain`, `#semiconductors`

---

<a id="item-6"></a>
## [One Year of Fighting Scrapers on a 1.5-Million-Page Website](https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/) ⭐️ 8.0/10

A site owner published a detailed account of a year-long battle against scraper bots that made up 99% of traffic and caused a 500% cost spike in one month. He shared lessons learned about bot mitigation, and commenters debated the tradeoffs of using Cloudflare and alternative approaches like proof-of-work. This is a high-relevance practical war story for web operators, highlighting how bot traffic can silently drive up costs and force difficult tradeoffs. The community discussion raises important questions about outsourcing access decisions to Cloudflare and whether aggressive bot-blocking harms the open web. The owner noted his normal $90/month bill jumped about 500% during a bad spike month, and he acknowledged that his own site scrapes public documents, so he is 'a scraper writing a blog post complaining about scrapers.' In the comments, others shared that Claude-searchbot alone fetched roughly 205,000 pages in 72 hours and that the proof-of-work tool Anubis effectively stopped fake user-agent bots.

hackernews · petercooper · Aug 7, 14:51 · [Discussion](https://news.ycombinator.com/item?id=49211386)

**Background**: Scrapers are automated programs that systematically crawl and extract data from websites, and they can overwhelm a site's resources even when they aren't malicious. Many site owners turn to services like Cloudflare to filter bot traffic, but this means the company effectively decides who can access the site. Proof-of-work is an alternative anti-bot technique that requires the client to perform a small computational puzzle to prove it is a real browser, rather than a cheap automated scraper. The current battle is also fueled by AI companies whose crawlers (such as Claude-searchbot) fetch massive numbers of pages for training or retrieval.

**Discussion**: Commenters were broadly sympathetic but split on the solution: some worried that defaulting to Cloudflare outsources who can access your site to a corporation, while others recommended tooling like Anubis's proof-of-work or dropping D1 entirely for a static site. One commenter shared that Claude-searchbot fetched ~205,000 pages in 72 hours with just one referral, feeling 'cheated' by AI scrapers. The owner's self-aware admission that he is also a scraper drew wry acknowledgment.

**Tags**: `#web scraping`, `#bot detection`, `#cloudflare`, `#cost optimization`, `#site reliability`

---

<a id="item-7"></a>
## [New Mexico court orders Meta to pay $567m over children's mental health harms](https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta) ⭐️ 8.0/10

On August 6, 2026, a New Mexico court ordered Meta to pay $567 million (other reports say $942 million) to fund teen mental health programs and to make changes for underage users. The ruling follows a lawsuit alleging Meta's social media platforms contribute to children's mental health harms. This is a landmark legal ruling that holds a major social media company liable for algorithmic harm to minors under public-nuisance law, and it could spur other states to file similar lawsuits. The size of the penalty per New Mexico resident makes it significant even if it is small relative to Meta's global revenue. The court found Meta violated New Mexico's public-nuisance law, NMSA 1978 § 30-8-1, which covers acts injurious to public health, safety, morals, or welfare. Reports differ on the exact award amount—$567 million vs. $942 million—possibly reflecting separate damage calculations or reporting discrepancies. New Mexico has just over 2 million residents, so the per-capita judgment is very high.

hackernews · boplicity · Aug 7, 00:06 · [Discussion](https://news.ycombinator.com/item?id=49204352)

**Background**: Meta is the parent company of Facebook, Instagram, and WhatsApp. Across the United States, many state governments and school districts have sued social media companies, claiming that algorithmic features such as infinite scrolling and personalized recommendations harm adolescents' mental health. Public-nuisance laws give states a legal basis to stop activities that affect the health, safety, or welfare of the public at large. This case is part of broader regulatory and legal pressure on tech firms over youth mental health, addictive design, and platform accountability.

**Discussion**: Commenters debated whether the penalty is a mere 'slap on the wrist' globally but still enormous for a small state like New Mexico, with some noting the award exceeds what proportional revenue calculations might suggest. Others shared personal experiences of Instagram Reels and TikTok feeling like addictive substances and criticized the toxic comment sections, while some discussed the potential impact on Meta's stock price and algorithm design.

**Tags**: `#legal`, `#social-media`, `#mental-health`, `#regulation`, `#Meta`

---

<a id="item-8"></a>
## [Show HN: Wyzer Language Aims to Prevent Distributed Deadlocks and Memory Bugs](https://github.com/Wyzer-Lang/wyzer) ⭐️ 8.0/10

A developer unveiled Wyzer, a new statically typed, compiled, resource-oriented programming language that combines choreographic programming with the Perceus memory model; version 0.1.0 is scheduled for release soon. It extends compile-time safety beyond memory management to distributed coordination, directly addressing distributed deadlocks and cross-service protocol mismatches that Rust does not cover. If successful, it could offer a new direction for ensuring correctness in multi-service systems. Wyzer uses linear/affine types and Perceus reference counting instead of Rust's borrow checker and lifetimes, which the author says is simpler for tooling such as an LSP to analyze. It is still early-stage, with the project starting after about five months of research and a few weeks of development.

hackernews · v0id_isgood · Aug 7, 12:28 · [Discussion](https://news.ycombinator.com/item?id=49209385)

**Background**: Choreographic programming is a paradigm for distributed systems in which programs are written as a single interaction among multiple participants; deadlock freedom is guaranteed because every send has a matching receive. Perceus is an algorithm for garbage-free reference counting with reuse, used in languages like Koka and implemented without a runtime garbage collector. Resource-oriented computing treats computing as programs managing resources through execution contexts, a relevant framing for Wyzer's design. Wyzer draws on academic research to generalize these ideas into a practical high-level language.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Choreographic_programming">Choreographic programming</a></li>
<li><a href="https://www.microsoft.com/en-us/research/publication/perceus-garbage-free-reference-counting-with-reuse/">Perceus: Garbage Free Reference Counting with... - Microsoft Research</a></li>
<li><a href="https://en.wikipedia.org/wiki/Resource-oriented_computing">Resource-oriented computing - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters praised the ambition and the clear structure of the README, but said the genuinely novel ideas are hard to find and more examples are needed. Several also questioned how deadlock freedom is actually guaranteed in a choreography, such as how cycles across participants are rejected.

**Tags**: `#programming-languages`, `#distributed-systems`, `#memory-safety`, `#choreographic-programming`, `#rust`

---

<a id="item-9"></a>
## [Tokenpocalypse: Companies Scramble to Cut AI Token Spending](https://simonwillison.net/2026/Aug/7/pdfs-are-terrible/#atom-everything) ⭐️ 8.0/10

A 404 Media report from June 24, based on leaked Accenture meeting audio, reveals that non-engineers—not engineers—are driving token consumption, and that converting PDFs into images and then markdown is one of the biggest token chewers. Simon Willison highlighted the story, adding that PDFs are a terrible medium for communicating information. This matters because AI token costs are becoming a major operational burden for enterprises, and hidden, non-obvious workflows can silently inflate bills. It shows that cost optimization—not just model capability—is now central to real-world LLM deployment. Token consumption is the sum of input and output tokens across every API call, and PDFs are expensive because content can be tokenized into images, markdown, or other intermediate formats that multiply token counts. Converting files to clean markdown can reduce token usage by 65–90% with no loss of content quality, according to practitioners.

rss · Simon Willison · Aug 7, 16:18

**Background**: LLM APIs are priced per token, where a token is a chunk of text typically smaller than a word, so the more tokens a workflow consumes, the higher the cost. PDFs are notoriously token-hungry because their layout, images, and formatting often require multimodal or verbose text conversion, making plain markdown far more efficient. The story also touches on agentic AI—semi-autonomous systems that perceive, reason, and act—which can multiply token spending as these agents automate more tasks across an organization.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mindstudio.ai/blog/convert-files-markdown-reduce-ai-tokens">How to Convert Files to Markdown to Reduce AI Token Usage by Up to 90% | MindStudio</a></li>
<li><a href="https://iternal.ai/token-usage-guide">Token Usage Guide 2026: How Many Tokens AI Really Uses</a></li>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained | MIT Sloan</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Token Costs`, `#Enterprise AI`, `#LLM`, `#Cost Optimization`

---

<a id="item-10"></a>
## [SpaceX 10GW Space Solar by 2027 Could Yield $300B ARR, Says SemiAnalysis](https://newsletter.semianalysis.com/p/spacex-10gw-in-2027-why-its-real) ⭐️ 8.0/10

SemiAnalysis published a deep-dive arguing that SpaceX's plan to deliver 10GW of space-based solar power to Earth by 2027 is realistic, and could generate $300 billion in annual recurring revenue (ARR). The report also contends Microsoft will become the largest offtaker of this orbital power, enabling triple-digit growth for Azure. If realized, this would fundamentally reshape AI infrastructure, energy supply, and cloud economics by decoupling massive AI compute from terrestrial grid constraints. Microsoft's potential role as the anchor buyer would give SpaceX a credible revenue path while helping Azure escape power limits. The analysis assumes inference workloads can process around 100 billion tokens per gigawatt per year, and references Microsoft's '10GW 2026 Awakening' as a demand catalyst. However, the 2027 timeline is forward-looking and unverified; current space-based solar demonstrations such as Caltech's MAPLE have only beamed microwatts to Earth.

rss · Semianalysis · Aug 7, 20:08

**Background**: Space-based solar power (SBSP) involves collecting solar energy in orbit, where sunlight is not attenuated by the atmosphere, and beaming it to Earth as microwaves or lasers. An offtake agreement is a long-term contract in which a buyer commits to purchasing a project's future output, commonly used to secure financing for large infrastructure. Proposals for orbital AI data centers and SBSP have recently gained attention due to the rapidly growing power demands of AI, but significant technical and economic hurdles remain before gigawatt-scale space power is feasible.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Space-based_solar_power">Space-based solar power</a></li>
<li><a href="https://en.wikipedia.org/wiki/Offtake_agreement">Offtake agreement</a></li>
<li><a href="https://www.cnbc.com/2026/06/21/do-space-based-ai-data-centers-make-economic-sense.html">Do space-based AI data centers make economic sense?</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#AI infrastructure`, `#Microsoft`, `#energy`, `#data centers`

---

<a id="item-11"></a>
## [Gemini's Long-Term Woes Are Google Cloud's Short-Term Gain](https://newsletter.semianalysis.com/p/gemini-is-cooked-but-gcp-is-cooking) ⭐️ 8.0/10

SemiAnalysis published an analysis arguing that DeepMind's long-term struggles with Gemini could paradoxically create short-term opportunities for Google Cloud. The piece reframes Gemini's difficulties as a potential revenue driver for GCP. This analysis offers a nuanced perspective on the strategic dynamics inside Alphabet, affecting AI infrastructure and cloud competition. Cloud customers, investors, and AI developers may need to adjust expectations about Google's AI roadmap. The piece likely argues that DeepMind's enormous compute consumption, regardless of Gemini's long-term success, generates revenue for Google Cloud. In the short term, GCP may benefit from internal resource reallocation or from attracting clients who are dissatisfied with DeepMind's direction.

rss · Semianalysis · Aug 7, 02:32

**Background**: DeepMind is Alphabet's AI research division, responsible for building Gemini, a family of large language models competing with OpenAI's GPT. Google Cloud Platform (GCP) sells cloud infrastructure, including TPUs and GPUs, to external customers. The internal relationship is complex: DeepMind consumes GCP resources, but if its models underperform, GCP may gain by reallocating capacity or serving clients who seek alternatives beyond DeepMind.

**Tags**: `#AI`, `#Google Cloud`, `#DeepMind`, `#Gemini`, `#Cloud Computing`

---

<a id="item-12"></a>
## [US Probes Chinese AI Firms' Offshore Access to Nvidia Chips](https://www.bloomberg.com/news/articles/2026-08-07/us-reviews-china-s-offshore-access-to-nvidia-chips-after-ai-breakthroughs) ⭐️ 8.0/10

The US Commerce Department's Bureau of Industry and Security (BIS) is systematically reviewing how Chinese AI companies obtain and use Nvidia chips overseas, including remote access to cloud computing and shell company arrangements. The review follows the release of Moonshot AI's Kimi K3 model, which a White House official accused of using illegally obtained Nvidia chips accessed remotely via Thailand. This investigation could reshape the global AI landscape by testing whether US export controls can govern remote cloud access to advanced chips. It affects Chinese AI companies like Moonshot AI and Alibaba, as well as Nvidia and other US tech firms that oppose expanding restrictions. BIS is compiling two lists: countries where smuggling of restricted chips into China is suspected, and countries where Chinese firms remotely rent chips. Remote access itself is not illegal under current regulations, so the US House has passed a bipartisan bill to grant BIS explicit authority, though Nvidia and others are expected to oppose it. Alibaba is reported to use a Singapore shell company controlled via a Cayman entity, using Nvidia chips in Malaysia through Megaspeed.

telegram · zaihuapd · Aug 7, 11:18

**Background**: Since 2022, the US has restricted exports of advanced Nvidia chips to China, but Chinese AI firms have found workarounds such as renting computing power abroad through cloud services. Kimi K3 is an open-weight, 2.8-trillion-parameter multimodal model from Moonshot AI with a 1-million-token context window, and its strong performance has heightened US concerns about the effectiveness of export controls. The BIS investigation aims to address potential loopholes in these offshore arrangements, even if they currently may not violate the letter of the law.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(AI)">Kimi (AI) - Wikipedia</a></li>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3">moonshotai/Kimi-K3 · Hugging Face</a></li>
<li><a href="https://www.msn.com/en-us/money/general/bis-targets-legal-cloud-compute-as-china-ai-firms-bypass-export-controls/ar-AA29Cltq">BIS targets legal cloud compute as China AI firms bypass export...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#semiconductors`, `#export controls`, `#US-China tech`, `#Nvidia`

---

<a id="item-13"></a>
## [SK Hynix Confirms V10 NAND: 375-Layer Stacking with Wafer Bonding](https://www.gelonghui.com/live/2599953) ⭐️ 8.0/10

At FMS 2026, SK Hynix confirmed that its next-generation V10 NAND flash features 375-layer stacking and, for the first time, uses wafer bonding technology in its NAND products. The company claims the V10 delivers 2.5 times the performance per watt of the previous V9 generation. This marks a significant milestone in 3D NAND scaling and power efficiency, directly benefiting AI data centers where storage energy efficiency is increasingly critical. It also signals SK Hynix is catching up with competitors like Kioxia and YMTC, which have already deployed wafer bonding in volume NAND production. V10 is the successor to the 321-layer V9 '4D NAND' and is SK Hynix's first NAND product to adopt wafer bonding. The 2.5x performance-per-watt improvement is specifically optimized for AI infrastructure environments that require both high energy efficiency and strong performance.

telegram · zaihuapd · Aug 7, 12:19

**Background**: NAND flash memory is a type of non-volatile storage commonly used in solid-state drives. To increase capacity and reduce cost, manufacturers stack memory cells vertically in 3D NAND, and the number of layers roughly determines density. Wafer bonding is an alternative manufacturing approach in which the CMOS logic wafer and the memory cell array wafer are fabricated separately and then bonded together, improving density and performance. Kioxia's CBA and YMTC's Xtacking are existing examples of wafer-bonded NAND in volume production, and SK Hynix is now adopting a similar technique with V10.

<details><summary>References</summary>
<ul>
<li><a href="https://www.digitimes.com/news/a20250714PD212/kioxia-ymtc-nand-cmos-wafer.html">Kioxia, YMTC jump ahead with wafer-bonded NAND in volume production</a></li>
<li><a href="https://www.eetimes.com/high-density-3d-flash-memory-using-high-precision-wafer-bonding-brings-new-value-to-storage/">KIOXIA: Features of BiCS FLASH 3D Flash Memory - EE Times</a></li>

</ul>
</details>

**Tags**: `#NAND`, `#SK Hynix`, `#semiconductor`, `#wafer bonding`, `#AI storage`

---