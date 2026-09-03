---
layout: default
title: "Horizon Summary: 2026-09-03 (EN)"
date: 2026-09-03
lang: en
---

> From 33 items, 7 important content pieces were selected

---

1. [OpenAI Unveils GPT-6 Astra with Near-Perfect ARC-AGI-3 Score](#item-1) ⭐️ 10.0/10
2. [Plan to Terminate Third-Level .name Domains Raises Stability Concerns](#item-2) ⭐️ 8.0/10
3. [Ported My 1993 Amiga Assembly Game to Godot in an Evening Using an LLM](#item-3) ⭐️ 8.0/10
4. [Audacity 4.0 Released with Qt6-Based UI Overhaul and Community Debate](#item-4) ⭐️ 8.0/10
5. [Google Antigravity ToS sparks concern over third-party use and full account suspension](#item-5) ⭐️ 8.0/10
6. [Moonshot AI (Kimi) Confidentially Files for Hong Kong IPO at $50B Pre-Money Valuation](#item-6) ⭐️ 8.0/10
7. [US Government Backs OpenAI in NYT Copyright Suit, Calling AI Training Fair Use](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Unveils GPT-6 Astra with Near-Perfect ARC-AGI-3 Score](https://openai.com/index/gpt-6-astra/) ⭐️ 10.0/10

OpenAI announced GPT-6 Astra, a new flagship model release, together with a deployment-safety system card. The model reportedly reaches 99.9% on the ARC-AGI-3 benchmark and shows major gains on coding and reasoning evaluations such as the Artificial Analysis Coding Agent Index. This is a full-version jump in OpenAI's flagship line rather than a point release, so it resets expectations for frontier model capability. A near-perfect ARC-AGI-3 result intensifies debates about whether these systems are approaching general or agentic intelligence, and it affects developers, researchers, and AI-safety conversations. Commenters note that the public ARC-AGI-3 scorecard may be misleading: it lists GPT-5.6 Sol at 7.8%, but with the same responses-API harness used for GPT-6 Astra, Sol would be estimated to score around 30%. OpenAI also published a deployment-safety system card at deploymentsafety.openai.com/gpt-6-astra.

hackernews · kibae · Sep 3, 18:41 · [Discussion](https://news.ycombinator.com/item?id=49554643)

**Background**: ARC-AGI-3 is an interactive reasoning benchmark that asks AI agents to explore novel, abstract, turn-based environments, infer goals on the fly, and build adaptable world models; it is designed to measure agentic intelligence rather than static skill recall. The Artificial Analysis Coding Agent Index is a composite coding score built from benchmarks including DeepSWE, Terminal-Bench v2.1, and SWE-Atlas-QnA. AI system cards are documentation artifacts that describe the architecture, data, and safety context of an AI system as a whole.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/blog/astra">OpenAI's GPT-6 Astra on ARC-AGI-3</a></li>
<li><a href="https://artificialanalysis.ai/agents/coding-agents">AI Coding Agent Benchmarks & Leaderboard - Artificial Analysis</a></li>
<li><a href="https://www.redhat.com/en/blog/security-beyond-model-introducing-ai-system-cards">Security beyond the model: Introducing AI system cards</a></li>

</ul>
</details>

**Discussion**: A common sentiment on Hacker News was respect for the ARC-AGI-3 result combined with caution about how it is reported: intenex argued the scorecard is misleading because it shows GPT-5.6 Sol at 7.8% even though the same responses-API harness would put Sol at roughly 30%. abixb said gains outside ARC-AGI-3 look comparable to ordinary point releases and questioned whether this truly represents an AGI step; astrobiased connected the trend to François Chollet's argument that frontier-model progress still resembles skill acquisition. Meanwhile, some commenters dismissed the autonomous-purchase demos as unconvincing.

**Tags**: `#OpenAI`, `#GPT-6`, `#AI`, `#benchmarks`, `#AGI`

---

<a id="item-2"></a>
## [Plan to Terminate Third-Level .name Domains Raises Stability Concerns](https://neil.fraser.name/news/2026/09/03/) ⭐️ 8.0/10

ICANN is considering a proposal to terminate all existing third-level registrations under the .name top-level domain and release the corresponding second-level domains. If enacted, names of the form first.last.name would no longer function for their current registrants. The proposal threatens the stability and security of existing registrations, contradicts ICANN's mission of ensuring stable and secure operation of the Internet's identifier systems, and could enable squatting when second-level domains are released. Thousands of individuals who registered personal names under the .name scheme could lose long-held addresses. The proposal affects third-level domain names such as first.last.name, which .name originally allowed; owners of already-registered second-level domains like last.name would not be affected. Commenters also note that the proposal does not explain how released second-level domains will be handled, and they doubt registry operator Verisign will reserve them to prevent squatting.

hackernews · pavel_lishin · Sep 3, 14:54 · [Discussion](https://news.ycombinator.com/item?id=49550772)

**Background**: Domain names are organized hierarchically: a top-level domain (TLD) such as .com or .name is the part after the final dot, a second-level domain is the label immediately before it (e.g., google in google.com), and a third-level domain is an additional label further left, such as blog in blog.website.com. Third-level domains often act as subdomains for organizing website content. .name is a TLD originally intended for individuals, and its registration model allowed third-level personal names before second-level registrations were later added.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Domain_name">Domain name - Wikipedia</a></li>
<li><a href="https://www.dynadot.com/help/question/what-is-third-level-domain">What is a third-level domain? | Dynadot</a></li>
<li><a href="https://www.cloudflare.com/learning/dns/top-level-domain/">What is a top-level domain (TLD)? - CloudflareList of Internet top-level domains - WikipediaWhat is a top-level domain? TLD definition and examplesWhat Is a Top-Level Domain (TLD)?What is TLD? Understanding top-level domains and their roleTop-Level Domain Extensions 2026: Complete TLD Guide - Bluehost</a></li>

</ul>
</details>

**Discussion**: Commenters generally sympathize with affected third-level registrants and argue that cancellation should not be abrupt. Some insist the scheme contradicts ICANN's core mission, while others clarify that only third-level names are affected and second-level owners are safe; one commenter also notes that domain names are leased assets and can ultimately disappear.

**Tags**: `#domain names`, `#ICANN`, `#internet governance`, `#DNS`, `#policy`

---

<a id="item-3"></a>
## [Ported My 1993 Amiga Assembly Game to Godot in an Evening Using an LLM](https://babyloniantwins.com/blog/porting-a-1993-amiga-game-to-godot/) ⭐️ 8.0/10

A developer ported his 1993 Amiga game, originally written in MC68000 assembly in Baghdad, to Godot in a single evening using a large language model. He also released the original game for free and published detailed notes about the process. This is a concrete demonstration that LLMs can make decades-old 68000 assembly code legible and portable to a modern engine, potentially lowering the barrier for preserving and reviving retro games. It also sparked thoughtful community discussion about AI-assisted reverse engineering and retrocomputing archaeology. The author had the model first reassemble the code with vasm on a Mac, iterating until the binary was byte-identical to the original game files. A residual 108-byte discrepancy was explained by AsmOne's in-memory assembly workflow, since the shipped files were memory snapshots after the game had run, though the author notes he never verified this explanation himself.

hackernews · rabahs · Sep 3, 14:28 · [Discussion](https://news.ycombinator.com/item?id=49550375)

**Background**: The Commodore Amiga was powered by the Motorola 68000, a 16/32-bit CISC microprocessor that game developers often programmed directly in assembly for speed and direct hardware access. vasm is a portable, retargetable assembler that can generate binary output from assembly source, which the author used to verify the LLM's reconstructed code. AsmOne was an integrated macro assembler for the Amiga that assembled code in memory; because the original game saved memory after it had already run, the shipped binaries were not clean assembler output, explaining the 108-byte discrepancy the author found.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Motorola_68000">Motorola 68000 - Wikipedia</a></li>
<li><a href="http://sun.hasenbraten.de/vasm/">vasm portable and retargetable assembler</a></li>
<li><a href="https://aminet.net/package/dev/asm/ASM-One">Aminet - dev/asm/ASM-One.lhaAsm One 1.02 Manual : Rune Gram-Madsen : Free Download ...Commodore Software - ASM-One v1.02 ManualASM-One Macro Assembler - HandWikiAmiga Assembler Tutorial - Carl HenrikAsm One 1.02 Manual : Free Download, Borrow, and Streaming ...Asm-One v1.20 by The Flame Arrows :: pouët.net</a></li>

</ul>
</details>

**Discussion**: Commenters praised the experiment as a "crazy" demonstration of AI-assisted archaeology: one recalled using Claude to convert a ZX81 memory dump to Go, while another plans to port a forgotten game that is not his own. Others expressed admiration for the original 1993 assembly work and suggested follow-ups such as an exportable engineering guide for similar LLM-based ports.

**Tags**: `#LLM`, `#Godot`, `#retrocomputing`, `#game development`, `#reverse engineering`

---

<a id="item-4"></a>
## [Audacity 4.0 Released with Qt6-Based UI Overhaul and Community Debate](https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0) ⭐️ 8.0/10

Audacity 4.0 has been officially released, featuring a major graphical user interface overhaul built on Qt6 and a collection of bug fixes. The release marks a significant technical transition for the popular open-source audio editor. This release matters because Audacity is one of the most widely used open-source audio editors, and the Qt6 migration brings a modernized interface that could improve usability across Linux, Windows, and macOS. It also intensifies the community debate about the project's technical direction and privacy concerns, which may influence future contributions and user trust. The new UI is based on Qt6, a cross-platform application framework offering native look-and-feel and support for high-DPI displays. Despite the overhaul, community members note that long-standing issues such as non-persistent JACK client handling and unwanted clicking noise between clips remain unaddressed, and some express concerns about integrated audio.com features.

hackernews · ClydeN · Sep 3, 10:53 · [Discussion](https://news.ycombinator.com/item?id=49548395)

**Background**: Audacity is a free, open-source digital audio editor used for recording, editing, and mixing audio, available on Linux, Windows, and macOS. Qt6 is the latest major version of the Qt framework, which developers use to create graphical user interfaces for desktop and embedded platforms; its release introduced improved graphics capabilities and better support for modern display technologies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qt_(software)">Qt (software) - Wikipedia</a></li>
<li><a href="https://doc.qt.io/qt-6/qt-intro.html">Introduction to Qt | Qt 6.11Qt (software) - WikipediaQt 6.11Qt5 vs Qt6: Understanding the Key Differences & Upgrade BenefitsFrom QtWidgets to Qt6 and Beyond: What Is Qt Capable Of?Difference between QT6 and LT20 QT6? : r/qBittorrent - Reddit</a></li>

</ul>
</details>

**Discussion**: Comments show a mix of enthusiasm and skepticism. Some users recommend developer videos praising the new UI, while others express disappointment that technical deficiencies they experienced in earlier versions, such as JACK integration quirks and clip-clicking artifacts, persist in 4.0. Additionally, several commenters reference privacy-related forks like Tenacity and Sneedacity, indicating lingering distrust over telemetry and audio.com integration.

**Tags**: `#Audacity`, `#Open Source`, `#Audio Software`, `#Qt6`, `#Release`

---

<a id="item-5"></a>
## [Google Antigravity ToS sparks concern over third-party use and full account suspension](https://twitter.com/GergelyOrosz/status/2095453567955968398) ⭐️ 8.0/10

Google Antigravity's terms of service initially stated that third-party API usage could lead to suspension of the user's entire Google account. Varun Mohan, head of Antigravity, clarified on X that only the Antigravity account is affected and said the ToS wording will be changed. This matters because a Google account often holds years of emails, calendars, and other critical data, so a policy that could suspend the whole account over an AI-service violation is seen as deeply user-hostile. The controversy could make developers and enterprises more reluctant to adopt Google's AI products, highlighting how essential transparent terms are for trust in AI platforms. The disputed wording is on the official terms page at antigravity.google/terms. Varun Mohan, from the Antigravity team, clarified that the account referred to in the terms is the Antigravity account, not the broader Google account. Some users with direct experience reported that enforcement has affected only Antigravity access, while the un-suspension process can be extremely cumbersome.

hackernews · tosh · Sep 3, 11:01 · [Discussion](https://news.ycombinator.com/item?id=49548452)

**Background**: Google Antigravity is Google's agentic development platform, consisting of a chat-oriented development environment, an IDE, a CLI, and an SDK for orchestrating autonomous AI agents in code generation, execution, and testing. The terms govern how users download, install, access, and use this AI service. Because AI agents often interact with third-party APIs, users were particularly alarmed to see language that appeared to permit suspension of an entire Google account over such usage, especially given how much personal data is stored there.

<details><summary>References</summary>
<ul>
<li><a href="https://antigravity.google/terms">Google Antigravity - Terms of Service</a></li>
<li><a href="https://x.com/GergelyOrosz/status/2095453567955968398">Gergely Orosz on X: "Antigravity's terms of services make it crystal ...</a></li>
<li><a href="https://discuss.ai.google.dev/t/antigravity-account-disabled-violation-of-terms-of-service-requesting-support/123014">Antigravity account disabled - "violation of Terms of Service ...</a></li>

</ul>
</details>

**Discussion**: Commenters called the original wording wildly user-hostile, saying they would rather avoid Google AI products than risk losing their entire account. Some raised the broader stakes of government identity systems that force reliance on Google or Apple accounts, where a ban could lock people out of public services. Others who had experienced suspensions noted that enforcement often only blocks Antigravity access, but that the appeal process can be byzantine, and they welcomed the official clarification.

**Tags**: `#Google`, `#Terms of Service`, `#AI policy`, `#Account suspension`, `#Cloud computing`

---

<a id="item-6"></a>
## [Moonshot AI (Kimi) Confidentially Files for Hong Kong IPO at $50B Pre-Money Valuation](https://www.21jingji.com/article/20260903/herald/4a31937e4c968dcce1d233b83a4759f8.html) ⭐️ 8.0/10

Moonshot AI, the developer of the Kimi chatbot, has confidentially submitted its A1 filing to the Hong Kong Stock Exchange, formally starting its Hong Kong IPO process. It is also advancing a new funding round at a US$50 billion pre-money valuation, likely its final financing before listing. The move signals that one of China's leading AI foundation-model companies is entering the public capital markets amid surging AI valuations. It could reshape the competitive landscape for Chinese AI startups and be followed by DeepSeek, which is widely expected to list in the first half of next year. The A1 filing is confidential, and the company responded that it has no further information to disclose. Its valuation jumped from about US$4.3 billion at the end of 2025 to US$35 billion post-money in July this year—roughly an 8-fold increase in half a year—while Kimi launched K2.5, K2.6, and K3 in January through July on roughly a three-month iteration cycle.

telegram · zaihuapd · Sep 3, 03:15

**Background**: An A1 filing is the document a sponsor submits to the Hong Kong Stock Exchange to formally begin the city's IPO review process; it discloses financials, business model, and risks to investors. Pre-money valuation is a company's value before new investment is added, while post-money valuation equals pre-money plus the newly injected capital. For example, if a company valued at US$10 billion pre-money raises US$1 billion, its post-money valuation becomes US$11 billion. Understanding these terms clarifies why the reported US$50 billion pre-money valuation would rise once the new round closes.

<details><summary>References</summary>
<ul>
<li><a href="https://qifu.zcqtz.com/article/22267.html">香港ipo的a1是指什么 (香港IPO中A1文件含义)-中国香港百科-丝路企服</a></li>
<li><a href="https://www.zhihu.com/question/48450676">大神能不能用例子说明下投前估值和投后估值的区别？ - 知乎</a></li>

</ul>
</details>

**Tags**: `#AI`, `#IPO`, `#融资`, `#月之暗面`, `#大模型`

---

<a id="item-7"></a>
## [US Government Backs OpenAI in NYT Copyright Suit, Calling AI Training Fair Use](https://www.reuters.com/legal/litigation/us-government-backs-openai-new-york-times-copyright-case-2026-09-02/) ⭐️ 8.0/10

The U.S. government filed an amicus brief in Manhattan federal court backing OpenAI in its copyright dispute with The New York Times, arguing that training large language models on copyrighted material generally constitutes fair use. This is the first U.S. government statement on the issue in a major AI copyright case. Although non-binding, the brief could influence how courts and policymakers view AI training and give tech companies more confidence in similar litigation. It also places the U.S. government on one side of a high-stakes debate over the future of generative AI and creator compensation. The brief reportedly argues that using copyrighted works to train AI models generally qualifies as fair use, a position opposed by The New York Times. The Times accused the government of siding with 'a few trillion-dollar AI companies' at the expense of creators, and its 2023 lawsuit against OpenAI and Microsoft alleged unauthorized use of millions of its articles to train ChatGPT.

telegram · zaihuapd · Sep 3, 05:45

**Background**: Fair use is a U.S. legal doctrine that permits limited use of copyrighted material without permission under certain circumstances, such as for commentary, criticism, or transformative purposes. An amicus brief is a document filed by a non-party with an interest in the case, providing information or perspectives to assist the court. The outcome of this lawsuit could have broad consequences for how AI companies obtain training data and whether they must license or pay content owners.

**Tags**: `#AI`, `#copyright`, `#OpenAI`, `#fair-use`, `#legal`

---