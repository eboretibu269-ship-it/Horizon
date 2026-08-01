---
layout: default
title: "Horizon Summary: 2026-08-01 (EN)"
date: 2026-08-01
lang: en
---

> From 41 items, 9 important content pieces were selected

---

1. [NetBSD 11.0 Released with 10ms MICROVM Boot and NPF Firewall Upgrades](#item-1) ⭐️ 9.0/10
2. [OpenAI's Astra Model Cracks Ten Long-Standing Math Problems](#item-2) ⭐️ 9.0/10
3. [Canada Quietly Signs UN Cybercrime Convention, Raising Privacy Concerns](#item-3) ⭐️ 8.0/10
4. [DeepSeek V4 Flash-0731: 304B Agentic LLM, Low Cost, High Value](#item-4) ⭐️ 8.0/10
5. [Stateless MCP Recaptures Interest, Inspires mcp-explorer and datasette-mcp](#item-5) ⭐️ 8.0/10
6. [VLMs Score Well on Benchmarks While Silently Erasing Clinical Terms](#item-6) ⭐️ 8.0/10
7. [Study Probes Symmetry Inside Superhuman Go Neural Networks](#item-7) ⭐️ 8.0/10
8. [EA to Close $55B Sale to Saudi-Led Consortium Next Week](#item-8) ⭐️ 8.0/10
9. [Microsoft confirms Copilot 'super app' launching this year](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [NetBSD 11.0 Released with 10ms MICROVM Boot and NPF Firewall Upgrades](https://blog.netbsd.org/tnf/entry/netbsd_11_0_released) ⭐️ 9.0/10

NetBSD 11.0 is now officially released. It introduces a new MICROVM kernel for x86 that can boot in about 10 ms, along with major NPF firewall improvements including layer 2 and user/group filtering. This is a major NetBSD release that brings an ultra-fast booting microVM kernel, which could benefit edge computing and lightweight virtualization workloads. The NPF enhancements make NetBSD more attractive as a secure network appliance or router. The MICROVM kernel is designed to build VMs as small as 10 MB that boot in about 10 ms, and it works on Linux, macOS, and NetBSD hosts. The release also includes various hardware and system improvements, though open issues remain as with any major release.

hackernews · jaypatelani · Aug 1, 17:56 · [Discussion](https://news.ycombinator.com/item?id=49136736)

**Background**: NetBSD is a free, open-source Unix-like operating system descended from Berkeley Software Distribution (BSD), known for its portability and clean design. The MICROVM kernel is a specialized kernel configuration used by projects like smolBSD to create ultra-lightweight virtual machines that boot almost instantly. NPF is NetBSD's stateful packet filter firewall, comparable to Linux's iptables or OpenBSD's PF. NetBSD 11.0 is the nineteenth major release of the NetBSD operating system.

<details><summary>References</summary>
<ul>
<li><a href="https://netbsd.org/releases/formal-11/NetBSD-11.0.html">Announcing NetBSD 11.0 RC7 (July 21, 2026)</a></li>
<li><a href="https://ostechnix.com/build-10mb-netbsd-vms-boot-10ms-smolbsd/">Build 10MB NetBSD VMs That Boot in 10ms Using... - OSTechNix</a></li>
<li><a href="https://en.wikipedia.org/wiki/NPF_(firewall)">NPF (firewall) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters are asking about the current status of the BSDs compared to Linux, and whether Wine support has been maintained. Others highlight the valuable NPF filtering features and the surprising 10 ms boot time, while one notes the release announcement's honest tone about open issues is refreshing.

**Tags**: `#netbsd`, `#bsd`, `#operating-systems`, `#release`, `#virtualization`

---

<a id="item-2"></a>
## [OpenAI's Astra Model Cracks Ten Long-Standing Math Problems](https://simonwillison.net/2026/Aug/1/ten-advances-in-mathematics/#atom-everything) ⭐️ 9.0/10

OpenAI announced that an internal version of its next major model, Astra, solved ten open problems in mathematics and theoretical computer science, spending less than $2,000 per problem at GPT-5.6 Sol token prices. The results were released with Lean 4 formalizations, a research paper, and an LLM-generated PDF describing the reasoning traces. This is a major milestone in AI-driven scientific discovery, showing that frontier models can produce auditable research results at remarkably low cost. Following Anthropic's Claude cryptographic weakness discovery, it strengthens the case for what Terence Tao calls 'big mathematics,' where AI handles technical grunt work and humans focus on creative parts. OpenAI did not reveal how many problems were attempted unsuccessfully, which leaves a potential selection-bias caveat. The openai/ten-proofs repository contains Lean 4 formalizations, and a separate paper plus an LLM-generated PDF describe the proofs, but the exact prompts used were not published. The problems span areas such as high-dimensional sphere packing, non-Sofic groups, Connes rigidity conjecture counterexamples, arithmetic circuit lower bounds, quantum parallel repetition, nearest vector problem hardness, and multicolor Ramsey numbers.

rss · Simon Willison · Aug 1, 20:34

**Background**: This announcement follows Anthropic's revelation that its unreleased Claude Mythos Preview discovered cryptographic weaknesses in software after spending $100,000 on tokens with prompts explicitly seeking genuinely hard findings. The mathematical community is reacting with both excitement and existential concern: mathematician Kirwin Hampshire published 'The Dark Night of Mathematics' describing a 'profound spiritual crisis,' while Terence Tao envisions 'big mathematics' as decentralized human-machine collaboration. OpenAI's approach includes Lean 4, a proof assistant that allows computers to formally verify mathematical arguments.

<details><summary>References</summary>
<ul>
<li><a href="https://runtimewire.com/article/openai-astra-ten-open-math-problems">OpenAI says unreleased Astra model solved 10 open... - RuntimeWire</a></li>
<li><a href="https://scalevise.com/resources/openai-public-materials-no-astra-model/">OpenAI Public Materials Do Not List Astra</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Discussion on Hacker News, via Simon Willison's post, focused on wanting to see the exact prompts used and on the lack of information about unsuccessful attempts. Some mathematicians are experiencing a collective 'Deep Blue moment,' with feelings ranging from excitement to a spiritual crisis about the role of humans in mathematics, while others appreciate the transparency provided by Lean 4 formalizations.

**Tags**: `#AI research`, `#Mathematics`, `#OpenAI`, `#LLM capabilities`, `#Scientific discovery`

---

<a id="item-3"></a>
## [Canada Quietly Signs UN Cybercrime Convention, Raising Privacy Concerns](https://www.michaelgeist.ca/2026/07/a-surveillance-treaty-in-disguise-the-trouble-with-canadas-quiet-decision-to-sign-the-un-cybercrime-convention/) ⭐️ 8.0/10

Privacy expert Michael Geist published an analysis in July 2026 revealing that Canada quietly signed the United Nations Cybercrime Convention. He argues that the treaty, despite its name, is effectively a surveillance treaty that could expand government monitoring powers. The signing matters because it may obligate Canada to adopt surveillance-friendly measures, potentially undermining domestic privacy protections and setting a precedent for other democracies. Privacy advocates worry that the treaty's vague language could enable mass data sharing and government surveillance of citizens. Canada is among the 76 signatories listed as of May 2026, but signature alone does not create binding obligations; the treaty will only enter into force after 40 instruments of ratification are deposited. Geist's analysis focuses on provisions concerning expedited preservation of electronic evidence and cross-border cooperation, which he says could be exploited for surveillance purposes.

hackernews · iamnothere · Aug 1, 14:19 · [Discussion](https://news.ycombinator.com/item?id=49134694)

**Background**: The United Nations Convention against Cybercrime, adopted by the UN General Assembly in December 2024, is the first binding international treaty dedicated to combatting cybercrime. It seeks to improve international cooperation on issues like cross-border evidence sharing and law enforcement coordination, but civil liberties groups have raised concerns that its provisions on electronic evidence and data preservation are too broad and could enable government surveillance and censorship.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unodc.org/unodc/en/cybercrime/convention/home.html">United Nations Convention against Cybercrime</a></li>
<li><a href="https://www.linkedin.com/pulse/united-nations-cybercrime-convention-defining-step-toward-a-wali-moyrf">The United Nations Cybercrime Convention: A Defining Step...</a></li>
<li><a href="https://www.napforum.org/policy-briefs/dangers-of-ambiguity-in-the-un-cybercrime-treaty">Dangers of Ambiguity in the UN Cybercrime Treaty - Marshall Green</a></li>

</ul>
</details>

**Discussion**: Commenters gave mixed reactions: some, like panarchy, praised Michael Geist's long track record, while others argued that being a signatory has limited effect unless ratified (alephnerd). Some observed that Canada signing most UN treaties is routine, and yet another commenter speculated about the political signalling behind such agreements.

**Tags**: `#privacy`, `#surveillance`, `#cybercrime`, `#treaty`, `#Canada`

---

<a id="item-4"></a>
## [DeepSeek V4 Flash-0731: 304B Agentic LLM, Low Cost, High Value](https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/#atom-everything) ⭐️ 8.0/10

DeepSeek released V4-Flash-0731, a 304B-parameter model with substantially enhanced agentic capabilities. Priced at $0.14 per million input tokens and $0.27 per million output tokens, it is ranked ahead of the 428B-parameter MiniMax M3 on the Artificial Analysis Intelligence Index. This model may currently offer the best value-per-intelligence in the market, delivering competitive performance against much larger models at a fraction of the cost. It strengthens DeepSeek's position in the intensifying AI model race and gives developers a cheaper option for agentic workloads. The model is 167GB on Hugging Face and was tested by Simon Willison via OpenRouter, showing that output quality depends strongly on the reasoning_effort setting: default yielded a mangled pelican illustration, while 'high' produced a much better result. Artificial Analysis highlights it as sitting alone in the 'most attractive' quadrant on its Intelligence Index vs. Cost per Task chart.

rss · Simon Willison · Jul 31, 23:59

**Background**: Agentic capabilities refer to an LLM's ability to autonomously use tools, learn from execution feedback, and complete multi-step workflows rather than just generating text. The Artificial Analysis Intelligence Index aggregates multiple benchmarks into a single model-level score, allowing comparisons of intelligence, speed, and price across many AI models. DeepSeek is a Chinese AI lab known for releasing strong open-weight models at aggressive prices.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://benchlm.ai/benchmarks/artificialanalysis">Artificial Analysis Intelligence Index Leaderboard... | BenchLM.ai</a></li>
<li><a href="https://www.linkedin.com/pulse/developing-agentic-capabilities-llms-automate-business-workflows-mp1tf">Developing Agentic Capabilities for LLMs to automate business...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#DeepSeek`, `#LLM`, `#machine learning`, `#model release`

---

<a id="item-5"></a>
## [Stateless MCP Recaptures Interest, Inspires mcp-explorer and datasette-mcp](https://simonwillison.net/2026/Jul/31/stateless-mcp/#atom-everything) ⭐️ 8.0/10

The Model Context Protocol (MCP) 2.0 specification (2026-07-28) has been released, introducing a stateless protocol that reduces tool calls to a single HTTP request. Simon Willison built two new tools, mcp-explorer and datasette-mcp, to explore and expose MCP servers. This is the most significant MCP spec change since launch, making client and server implementations much simpler and more scalable. It also helps MCP regain relevance in AI agent tooling, with Claude adopting it and enabling teams to expose internal tools without inbound firewall rules. The new stateless flow uses a single POST request with headers such as MCP-Protocol-Version, Mcp-Method, and Mcp-Name, instead of a two-step initialize-then-call sequence with a session ID. Official SDKs, such as the C# SDK v2.0, implement the 2026-07-28 spec while remaining backward compatible and supporting Multi Round-Trip Requests for interactive tools.

rss · Simon Willison · Jul 31, 23:13

**Background**: MCP is the Model Context Protocol introduced by Anthropic in November 2024, describing a standard way to expose tools to LLM-powered agent frameworks. It saw huge interest in 2025 but was somewhat eclipsed by Anthropic's Skills, since an agent with a terminal and curl could do much of the same work. The stateless redesign addresses complexity by eliminating server-side session state, making the protocol a better fit for scalable web applications and easier for smaller models to drive.

<details><summary>References</summary>
<ul>
<li><a href="https://devblogs.microsoft.com/dotnet/announcing-v20-of-the-official-mcp-csharp-sdk/">Announcing v2.0 of the official MCP C# SDK - .NET Blog</a></li>
<li><a href="https://claude.com/blog/bringing-mcp-2026-07-28-to-claude">MCP 2026-07-28 spec: stateless core, coming to Claude | Claude by Anthropic</a></li>
<li><a href="https://github.com/simonw/mcp-explorer">GitHub - simonw/mcp-explorer: CLI tool for exploring an MCP server</a></li>

</ul>
</details>

**Tags**: `#MCP`, `#AI agents`, `#protocol`, `#software engineering`, `#LLM`

---

<a id="item-6"></a>
## [VLMs Score Well on Benchmarks While Silently Erasing Clinical Terms](https://www.reddit.com/r/MachineLearning/comments/1vcipzz/vlms_can_score_well_on_benchmarks_while_silently/) ⭐️ 8.0/10

Researchers from DTU Compute show that VLMs for chest X-ray report generation can score well on standard benchmark metrics while erasing rare, clinically meaningful terms and producing repetitive 'normal' templates. The paper 'Measuring What VLMs Don't Say' introduces a framework to quantify clinical terminology erasure and biased term introduction. This finding is significant because benchmark metrics that reward safe, templated language may mask models that are clinically useless, which is dangerous in high-stakes medical applications. It underscores the need for evaluation methods that account for clinical terminology coverage and fairness, not just lexical overlap with reference reports. The proposed framework uses reference-based weighting to reveal which clinically important terms (frequent in human reports) are systematically avoided by generated reports. The paper is authored by Aditya Parikh, Aasa Feragen, Sneha Das, and Stella Frank at DTU Compute, Technical University of Denmark.

reddit · r/MachineLearning · /u/ade17_in · Aug 1, 09:27

**Background**: Vision-language models (VLMs) combine image and text understanding; in radiology, they are used for automatic report generation from images such as chest X-rays. Standard captioning metrics like BLEU, ROUGE, or CIDEr score how similar generated text is to a reference, so models can 'game' them by outputting short, generic phrases like 'no acute findings.' Clinical terminology erasure means rare but important findings (e.g., 'pneumothorax' or 'nodule') may be omitted entirely, making the report useless for a physician reading it.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2603.01625">Measuring What VLMs Don't Say: Validation Metrics Hide Clinical...</a></li>
<li><a href="https://arxiv.org/abs/2403.02469">[2403.02469] Vision-Language Models for Medical Report ...Vision-Language Models for Medical Report Generation and ...Vision-Language Model for Multitask Medical Text GenerationVision-Language Models in medical image analysis: From simple ...Vision-language models for medical report generation andMedical Vision-Language Models: Existing Technologies ... - MDPI</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1574013726001413">Medical image captioning: A systematic review of methods ...</a></li>

</ul>
</details>

**Tags**: `#VLM`, `#evaluation`, `#radiology`, `#clinical NLP`, `#benchmarks`

---

<a id="item-7"></a>
## [Study Probes Symmetry Inside Superhuman Go Neural Networks](https://www.reddit.com/r/MachineLearning/comments/1vcrki2/how_symmetric_are_the_insides_of_a_go_network_r/) ⭐️ 8.0/10

KataGo's author published an interpretability study probing how superhuman Go networks handle the game's rotational/reflection symmetry. Using only stochastic 8-fold data augmentation rather than enforced symmetry, the study finds a mix of orientation-invariant representations and per-orientation memorization, with one unexpected result. This offers rare, concrete insight into how superhuman models internalize symmetry in board games, a question relevant to interpretability, equivariant architectures, and data augmentation. The findings could inform future training and architectural choices for game AI and other settings with known symmetries. The study centers on KataGo, an open-source Go engine, and relies on stochastic 8-fold augmentation that randomizes board orientation during training without enforcing symmetry. The writeup was largely produced with AI assistance under detailed human direction, and code is linked from the study page.

reddit · r/MachineLearning · /u/icosaplex · Aug 1, 16:18

**Background**: Go is fully symmetric under rotation and reflection, but neural networks are not architecturally constrained to respect that symmetry. Data augmentation like random flipping or rotating is a common way to encourage models to generalize across orientations. Researchers distinguish between invariance (output unaffected by orientation) and equivariance (internal features transform predictably with orientation), and interpretability studies often probe which of these behaviors emerges naturally in trained networks.

<details><summary>References</summary>
<ul>
<li><a href="https://katagotraining.org/">KataGo Distributed Training</a></li>
<li><a href="https://distill.pub/2020/circuits/equivariance/">Naturally Occurring Equivariance in Neural Networks</a></li>
<li><a href="https://machinelearningmastery.com/how-to-configure-image-data-augmentation-when-training-deep-learning-neural-networks/">How to Configure Image Data Augmentation in Keras</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#interpretability`, `#neural-networks`, `#go`, `#symmetry`

---

<a id="item-8"></a>
## [EA to Close $55B Sale to Saudi-Led Consortium Next Week](https://www.gamersky.com/news/202607/2180618.shtml) ⭐️ 8.0/10

Electronic Arts announced that its $55 billion sale to a consortium led by Saudi Arabia's Public Investment Fund has received all regulatory approvals, with the transaction expected to close on August 4, 2026. Once completed, EA will become a privately held company and will no longer disclose its financial results publicly. This deal is the second-largest acquisition in gaming history, trailing only Microsoft's $75.4 billion purchase of Activision Blizzard in 2023. It significantly expands Saudi Arabia's influence over the global gaming industry, while EA's privatization removes a major independent publisher from public markets. The buyer group includes Saudi Arabia's Public Investment Fund (PIF), Silver Lake, and Affinity Partners. PIF has been steadily increasing its stakes in gaming companies and previously acquired developers such as Scopely and Niantic outright.

telegram · zaihuapd · Aug 1, 09:10

**Background**: PIF is Saudi Arabia's sovereign wealth fund, established in 1971 to finance strategically important commercial projects for the kingdom's economic development. Silver Lake is a private equity firm founded in 1999 that focuses on mature technology companies, managing over $102 billion in assets. Affinity Partners, founded by Jared Kushner in 2021, is a private equity firm whose funds largely come from Middle Eastern government-backed sources. The consortium's acquisition of EA is a landmark in the ongoing consolidation of the gaming industry.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tmtpost.com/6830849.html">沙特主权基金PIF是何来头？ -钛媒体官方网站</a></li>
<li><a href="https://zh.wikipedia.org/wiki/银湖资本">银湖资本 - 维基百科，自由的百科全书</a></li>
<li><a href="https://baike.baidu.com/item/Affinity+Partners/67958593">Affinity Partners_百度百科</a></li>

</ul>
</details>

**Tags**: `#EA`, `#游戏行业`, `#收购`, `#沙特公共投资基金`, `#游戏产业`

---

<a id="item-9"></a>
## [Microsoft confirms Copilot 'super app' launching this year](https://www.theverge.com/tech/972927/microsoft-copilot-super-app-confirmed) ⭐️ 8.0/10

During a Wednesday earnings call, Microsoft CEO Satya Nadella confirmed the company will launch an AI 'super app' this year. The app will combine Copilot's chat, coding, and agentic capabilities into a single experience for consumers and businesses. This move signals Microsoft's ambition to consolidate its AI products into a unified hub, intensifying competition with OpenAI's ChatGPT Work and other AI assistants. It could reshape how developers, enterprises, and everyday users access AI-powered tools across Microsoft's ecosystem. The super app will merge Copilot chat, GitHub Copilot, Copilot Cowork, and Autopilot systems, with the integration happening this quarter. Nadella also noted that Microsoft's latest quarterly revenue reached $90 billion, driven largely by AI and cloud business.

telegram · zaihuapd · Aug 1, 13:18

**Background**: Copilot is Microsoft's AI assistant embedded across its products, while Copilot Cowork is an agentic system that plans, executes, and delivers work by coordinating tasks across apps, files, and data. Autopilot represents a more autonomous AI that can execute workflows on behalf of users. Agentic AI refers to AI systems that can pursue goals, use tools, and take actions with varying degrees of autonomy, operating within human-defined objectives and constraints.

<details><summary>References</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/microsoft-365/blog/2026/03/09/copilot-cowork-a-new-way-of-getting-work-done/">Copilot Cowork: A new way of getting work done | Microsoft ...</a></li>
<li><a href="https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/">Copilot Cowork overview | Microsoft Learn</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#Copilot`, `#AI`, `#Super App`, `#GitHub Copilot`

---