---
layout: default
title: "Horizon Summary: 2026-07-10 (EN)"
date: 2026-07-10
lang: en
---

> From 38 items, 13 important content pieces were selected

---

1. [OpenAI Releases GPT-5.6 with SOTA on ARC-AGI-3](#item-1) ⭐️ 9.0/10
2. [EU Parliament Approves Chat Control 1.0, Allows Warrantless Message Scanning](#item-2) ⭐️ 8.0/10
3. [Mitchell Hashimoto on Ghostty, Zig, and Rust Culture](#item-3) ⭐️ 8.0/10
4. [Lisp's Enduring Appeal and Community Debate](#item-4) ⭐️ 8.0/10
5. [Meta Announces Muse Spark 1.1 Agentic Model](#item-5) ⭐️ 8.0/10
6. [Internal TLS certificates best practices debated](#item-6) ⭐️ 8.0/10
7. [Meta's Superintelligence Progress Update](#item-7) ⭐️ 8.0/10
8. [Meta to Mass Produce Custom AI Chip 'Iris' in September](#item-8) ⭐️ 8.0/10
9. [OpenAI publishes national security principles, bans autonomous weapons and mass surveillance](#item-9) ⭐️ 8.0/10
10. [Chinese Courts Rule Game Accounts Inheritable, Invalidating Platform Bans](#item-10) ⭐️ 8.0/10
11. [Anthropic Web Crawler-to-Referral Ratio Hits 2800:1](#item-11) ⭐️ 8.0/10
12. [Long March 10B achieves world's first net-based rocket stage recovery at sea](#item-12) ⭐️ 8.0/10
13. [OpenAI, Google Allegedly Served Blacklisted Chinese Firms via Singapore](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Releases GPT-5.6 with SOTA on ARC-AGI-3](https://openai.com/index/gpt-5-6/) ⭐️ 9.0/10

OpenAI has released GPT-5.6, a new family of models including Sol (flagship), Terra (balanced), and Luna (cost-efficient), achieving a state-of-the-art score of 7.8% on the ARC-AGI-3 benchmark. The model also introduces enhanced intent understanding and original image detail preservation. This release marks a significant step in AI agentic intelligence, as GPT-5.6 Sol is the first verified frontier model to solve an ARC-AGI-3 game. The improved intent understanding and image handling could enhance developer productivity and enable more natural human-AI interaction. The developer guide highlights that GPT-5.6 can infer user intent without explicit step-by-step instructions, though important constraints must still be stated. The model preserves original image dimensions sent to it, and the Sol variant uses max/ultra reasoning and multi-agent collaboration.

hackernews · logickkk1 · Jul 9, 17:04 · [Discussion](https://news.ycombinator.com/item?id=48849066)

**Background**: ARC-AGI-3 is an interactive reasoning benchmark that tests an AI agent's ability to explore, infer goals, and plan in novel turn-based environments. It builds on the static grid tasks of ARC-AGI-1 and 2 by introducing partial observability and multi-turn dynamics. The 7.8% score represents a notable advance, though human performance remains near 100%.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">ARC-AGI-3: A New Challenge for Frontier Agentic IntelligenceARC-AGI-3: A New Challenge for Frontier Agentic IntelligenceARC-AGI-3 Quickstart - ARC-AGI-3 DocsARC-AGI-3: The New Interactive Reasoning Benchmark - DataCampGPT 5.6 Sol Tops ARC-AGI 3 With 7.8%, Becomes First Model To ...ARC-AGI-3: Interactive AGI Benchmark - emergentmind.com</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some praise the ARC-AGI-3 SOTA result and the detailed developer guide, while others note that GPT-5.6's coding performance is similar to GPT-5.5 and behind Sonnet 5. There is also discussion about the exclusion of Fable 5 from certain benchmarks due to refusal behavior, and comparisons between Codex and Claude Code.

**Tags**: `#AI`, `#GPT-5.6`, `#OpenAI`, `#language models`, `#benchmark`

---

<a id="item-2"></a>
## [EU Parliament Approves Chat Control 1.0, Allows Warrantless Message Scanning](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 8.0/10

The European Parliament approved Chat Control 1.0, a temporary regulation that permits major tech platforms like Instagram, Discord, and Gmail to scan private messages without a warrant or prior suspicion to detect child sexual abuse material. This decision effectively reauthorizes mass surveillance of private communications, undermining digital privacy and encryption protections across the EU, and sets a concerning precedent for future surveillance legislation. The regulation passed despite a majority of voting MEPs opposing it (314 against, 276 in favor) because a motion to reject failed to reach the required absolute majority of 361 votes; it will remain in effect until April 3, 2028.

hackernews · rapnie · Jul 9, 11:03 · [Discussion](https://news.ycombinator.com/item?id=48843923)

**Background**: Chat Control 1.0 is an interim measure that grants legal cover for tech companies to voluntarily scan user chats for known and unknown child sexual abuse material. It was initially rejected twice by the Parliament in March 2026, but the European Commission refused to withdraw the proposal, forcing a second reading. Critics argue that the technology for detecting unknown CSAM is unreliable and poses risks to privacy and encryption.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://www.euronews.com/next/2026/07/10/chat-control-10-passed-the-european-parliament-through-the-back-door">Why Chat Control 1.0 is the EU's most Orwellian law yet</a></li>
<li><a href="https://www.theregister.com/security/2026/07/09/meps-fail-to-prevent-chat-control-snoopfest-revival/5269379">EU 'Chat Control' snoopfest returns after vote to kill it falls short</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage over the parliamentary maneuver that allowed the regulation to pass despite majority opposition, calling it undemocratic. Some highlighted that the vote was held just before summer break, reducing attendance, and that the default was acceptance. Others noted that the regulation still allows voluntary scanning, but criticizes the erosion of privacy rights.

**Tags**: `#privacy`, `#surveillance`, `#EU regulation`, `#chat control`, `#encryption`

---

<a id="item-3"></a>
## [Mitchell Hashimoto on Ghostty, Zig, and Rust Culture](https://alexalejandre.com/programming/interview-with-mitchell-hashimoto/) ⭐️ 8.0/10

Mitchell Hashimoto, creator of Ghostty, gave an interview explaining his choice to build the terminal emulator in Zig and discussing his critiques of Rust's community culture. This interview sheds light on the ongoing debate between Zig and Rust in systems programming, highlighting how community culture and engineering pragmatism influence language adoption. Hashimoto emphasized Ghostty’s use of platform-native UI and GPU acceleration for speed, and noted that forking a project requires taking on the burden of synchronization with upstream changes.

hackernews · veqq · Jul 9, 17:17 · [Discussion](https://news.ycombinator.com/item?id=48849292)

**Background**: Ghostty is a fast, cross-platform terminal emulator that uses GPU acceleration and native UI. Zig is a system programming language designed as an alternative to C, focusing on simplicity and performance. The interview contrasts Zig's culture with Rust's, where Hashimoto expressed discomfort with Rust's community attitude.

<details><summary>References</summary>
<ul>
<li><a href="https://ghostty.org/">Ghostty</a></li>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: 👻 Ghostty is a fast, feature-rich, and cross-platform terminal emulator that uses platform-native UI and GPU acceleration.</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Discussion**: Comments debated Hashimoto's criticism of Rust culture, with some users noting negative experiences with both Rust and Zig communities. Another user praised the pragmatic engineering mindset and was motivated by the interview. A commenter also discussed the challenges of forking open-source projects, agreeing that synchronization work is a significant burden.

**Tags**: `#Zig`, `#Rust`, `#terminal emulator`, `#software engineering culture`, `#open source`

---

<a id="item-4"></a>
## [Lisp's Enduring Appeal and Community Debate](https://scotto.me/blog/2026-07-09-why-lisp/) ⭐️ 8.0/10

A reflective essay titled 'A road to Lisp: Why Lisp' explores Lisp's unique features, such as macros, and the tension between programmer freedom and safety, accompanied by a high-engagement Hacker News discussion on its learning curve and future in the age of AI. This discussion highlights the enduring appeal of Lisp as a language prioritizing expressiveness and metaprogramming, contrasting with modern trends toward safety and tooling, and raises questions about the impact of AI on programming language evolution. The post itself is a reflective essay, not a technical tutorial, but the community comments point to recent tooling improvements like Mine (a complete Lisp environment) and Olive (a VSCode plugin), as well as a website bug affecting syntax highlighting.

hackernews · silcoon · Jul 9, 13:06 · [Discussion](https://news.ycombinator.com/item?id=48845209)

**Background**: Lisp is one of the oldest programming languages, known for its macro system that allows code to be manipulated as data (homoiconicity), enabling developers to extend the language syntax. This macro facility offers great flexibility but also contributes to a steep learning curve, as highlighted in the discussion. The commenter davidpapermill expresses a long-held dream that Lisp would become mainstream, but wonders if AI will render that dream obsolete.

<details><summary>References</summary>
<ul>
<li><a href="https://lisp-journey.gitlab.io/blog/common-lisp-macros-by-example-tutorial/">Common Lisp Macros By Example Tutorial</a></li>

</ul>
</details>

**Discussion**: The community comments generally reflect admiration for Lisp's philosophy, such as the 'Light Side vs. Dark Side' tension between safety and power. Some users note the steep learning curve and ecosystem challenges, while others like vindarel highlight recent improvements in Lisp tooling (e.g., Mine, Olive). Overall, the discussion sees a passionate but niche community grappling with Lisp's future relevance.

**Tags**: `#Lisp`, `#programming languages`, `#macros`, `#software engineering`, `#AI`

---

<a id="item-5"></a>
## [Meta Announces Muse Spark 1.1 Agentic Model](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta released Muse Spark 1.1, its first paid agentic AI model, on July 9, 2026, via the Meta Model API in public preview for US developers, also available in the Meta AI app's Thinking mode. This launch marks Meta's strategic pivot to charging for its frontier AI models, directly competing with Anthropic and OpenAI, but the model faces community criticism over benchmark evaluation methodology. Pricing is $1.25/$4.5 per million tokens for input/output, with $0.15 for cached input, and the evaluation report for Terminal-Bench 2.1 used a bash-tool-only harness with 6 CPU cores and 8GB RAM, which some community members argue disqualifies the results due to resource overrides.

hackernews · ot · Jul 9, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48846184)

**Background**: Agentic AI refers to systems that can plan, use tools, and act autonomously to accomplish tasks, unlike traditional chatbots. Muse Spark is Meta's proprietary large language model developed by Meta Superintelligence Labs, first released in April 2026, and version 1.1 introduces agentic capabilities and a paid API.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacamp.com/blog/muse-spark-1-1">Muse Spark 1.1: Meta's Agentic Model and API | DataCamp</a></li>
<li><a href="https://www.digitalapplied.com/blog/meta-muse-spark-1-1-agentic-model-api-2026">Meta Muse Spark 1.1: Meta's First Paid Agent Model</a></li>
<li><a href="https://grokipedia.com/page/Muse_Spark_AI_model">Muse Spark (AI model)</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some criticize the benchmark methodology as invalid due to resource caps, while others praise the competitive pricing and accessibility. Simon Willison created an LLM plugin, and some suggest Meta should focus on commoditizing models rather than competing head-to-head.

**Tags**: `#meta`, `#ai`, `#muse-spark`, `#agentic-model`, `#benchmarking`

---

<a id="item-6"></a>
## [Internal TLS certificates best practices debated](https://tuxnet.dev/posts/tls-for-internal-services/) ⭐️ 8.0/10

A blog post on TLS certificates for internal services sparked a debate criticizing split-horizon DNS and advocating DNS-01 validation with ACME for certificate issuance. This debate highlights the complexity and trade-offs in securing internal services with TLS, affecting how organizations manage certificates and DNS infrastructure. Community members criticized split-horizon DNS for introducing complexity and silent deviations, and recommended using DNS-01 challenges with Let's Encrypt and keeping internal IPs in public zones but restricted by VPN access.

hackernews · mrl5 · Jul 9, 14:57 · [Discussion](https://news.ycombinator.com/item?id=48846995)

**Background**: Split-horizon DNS provides different DNS responses based on the requester's source address, often used to keep internal service names private. ACME (Automatic Certificate Management Environment) is a protocol for automating certificate issuance and validation, commonly used with Let's Encrypt.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Split-horizon_DNS">Split-horizon DNS</a></li>
<li><a href="https://en.wikipedia.org/wiki/ACME_protocol">ACME protocol</a></li>
<li><a href="https://tailscale.com/learn/why-split-dns">What is Split DNS & Why Should You Use It?</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong opposition to split-horizon DNS, calling it 'split-brain' and advocating for ACME-based DNS validation. Others noted the difficulty of configuring trust stores across different programming languages and suggested using public DNS zones with internal IPs restricted by VPN.

**Tags**: `#TLS`, `#certificates`, `#DNS`, `#internal services`, `#security`

---

<a id="item-7"></a>
## [Meta's Superintelligence Progress Update](https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence) ⭐️ 8.0/10

A new RL environment startup has emerged, and Meta is executing the most aggressive compute ramp we have ever seen, spanning over 2000km with scale-across networking. The update also offers strategic advice for Google DeepMind. This signifies a major acceleration in AI infrastructure investment, potentially enabling superintelligence-level models. The advice to DeepMind highlights competitive dynamics among leading AI labs. The compute ramp involves scale-across networking connecting clusters over 2000km, a technique typically used for high-bandwidth inter-datacenter connectivity. The RL environment startup is reportedly AMI Labs, founded by Yann LeCun, focusing on world models.

rss · Semianalysis · Jul 9, 19:16

**Background**: Scale-across networking refers to a network architecture that connects multiple scale-up clusters within a data center or across data centers for high-performance AI training. RL environments are simulations where reinforcement learning agents learn by interacting; world models aim to understand physics and real-world dynamics rather than just language. Meta's superintelligence efforts include both internal labs and external investments.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence">The Future of Meta Superintelligence: A 1 Year Progress Update</a></li>
<li><a href="https://builtin.com/artificial-intelligence/meta-superintelligence-labs">Meta Superintelligence Labs: What We Know So Far | Built In</a></li>
<li><a href="https://www.broadcom.com/topics/what-is-scale-across-networking-for-ai-clusters">Scale-across Networking | AI Clusters | AI Infrastructure</a></li>

</ul>
</details>

**Tags**: `#AI`, `#superintelligence`, `#Meta`, `#compute`, `#reinforcement learning`

---

<a id="item-8"></a>
## [Meta to Mass Produce Custom AI Chip 'Iris' in September](https://www.reuters.com/world/asia-pacific/meta-put-ai-chip-into-production-september-it-looks-double-computing-capacity-2026-07-09/) ⭐️ 8.0/10

Meta plans to mass produce its self-designed AI chip 'Iris' starting September, aiming to double its computing capacity by 2027. The chip, part of the MTIA fourth-generation project, is designed with Broadcom and manufactured by TSMC. This move reduces Meta's reliance on external GPU suppliers like Nvidia and AMD, signaling a strategic shift in the AI compute market. It also reflects the growing trend of tech giants building custom hardware for AI workloads. Meta expects to deploy 7 gigawatts of computing infrastructure this year, doubling to 14 gigawatts by 2027. The company has signed long-term supply agreements with Samsung, SanDisk, and Sumitomo Electric for memory, flash storage, and optical equipment.

telegram · zaihuapd · Jul 9, 12:37

**Background**: Meta's MTIA (Meta Training and Inference Accelerator) is a family of custom AI accelerators designed to handle recommendation systems and generative AI tasks. The 'Iris' chip is the latest iteration, following a rapid development cycle with only six weeks of testing and no major issues found. Meta plans to invest up to $145 billion in AI infrastructure this year.

<details><summary>References</summary>
<ul>
<li><a href="https://aichipfront.com/market-analysis/meta-self-developed-ai-chip-mtia">Meta自研AI芯片MTIA路线图深度解析：摆脱英伟达依赖的算力之战</a></li>
<li><a href="https://news.qq.com/rain/a/20240902A00ROW00">2024 Hot Chips ｜Meta 下一代MTIA：专用于推荐推理的AI处理器</a></li>
<li><a href="https://storagereview.com/zh-CN/news/meta-unveils-next-gen-meta-training-and-inference-accelerator-mtia">Meta 推出下一代元训练和推理加速器 (MTIA) - StorageReview.comTop StoriesMeta 自研 AI 推理芯片：四代路线图深度解读_腾讯新闻Meta自研AI芯片“Iris”即将投产，2027年算力目标翻倍至14GWMeta推出4款MTIA芯片，专注于高性能推理_部署_torch_带宽Meta自研AI芯片将于9月开始量产，剑指降低GPU成本</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#Meta`, `#computing infrastructure`, `#hardware`, `#semiconductor`

---

<a id="item-9"></a>
## [OpenAI publishes national security principles, bans autonomous weapons and mass surveillance](https://openai.com/index/government-national-security-partnerships/) ⭐️ 8.0/10

OpenAI has published its national security principles, explicitly banning the use of its technology for mass domestic surveillance, autonomous weapon systems, and high-risk automated decision-making. The company also expanded its Daybreak cyber defense program partnerships with several US allies. This marks a significant policy shift in AI governance, setting clear boundaries on military and surveillance applications while strengthening defensive collaborations with allies. It could influence global AI ethics standards and shape how other AI companies approach national security partnerships. The principles prohibit using OpenAI's technology for 'mass domestic surveillance,' 'autonomous weapon systems,' and 'high-risk automated decision-making.' The Daybreak program now includes partnerships with Australia, Canada, Japan, South Korea, France, Germany, Poland, the Netherlands, and EU institutions.

telegram · zaihuapd · Jul 9, 13:22

**Background**: Autonomous weapons, also known as lethal autonomous weapon systems (LAWS), can independently search for and engage targets without human intervention, raising ethical concerns. OpenAI's Daybreak program is a cyber defense initiative that integrates AI into security platforms to prioritize threats and generate defenses. These developments reflect ongoing debates about balancing AI innovation with security and ethical constraints.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Autonomous_weapons">Autonomous weapons</a></li>
<li><a href="https://www.cybersecuritydive.com/news/OpenAI-Daybreak-cyber-threats/820122/">OpenAI launches Daybreak to combat cyber threats | Cybersecurity Dive</a></li>
<li><a href="https://www.prnewswire.com/news-releases/cato-advances-enterprise-defense-joining-the-openai-daybreak-cyber-partner-program-302805920.html">Cato Advances Enterprise Defense, Joining the OpenAI Daybreak Cyber Partner Program</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI ethics`, `#national security`, `#AI policy`, `#international relations`

---

<a id="item-10"></a>
## [Chinese Courts Rule Game Accounts Inheritable, Invalidating Platform Bans](https://www.tomshardware.com/tech-industry/big-tech/chinese-courts-allow-heirs-to-inherent-accounts-of-deceased-gamers-multiple-cases-spanning-years-establish-precedent-for-digital-ownership-of-games-in-game-items-and-microtransactions) ⭐️ 8.0/10

Chinese courts in multiple cases over several years have ruled that virtual assets such as game accounts, equipment, and cryptocurrencies are inheritable, and that platform clauses prohibiting inheritance are invalid. This landmark legal precedent affirms digital inheritance rights for users and could force platforms to revise their terms of service globally. The courts specified that purely private content like chat logs is not inheritable and will be archived by the platform; platforms may charge reasonable fees for transferring accounts.

telegram · zaihuapd · Jul 10, 02:56

**Background**: Digital inheritance refers to the transfer of digital assets after a person's death. Traditionally, many service agreements forbid granting access to accounts to heirs, citing privacy and security concerns. These Chinese rulings challenge such clauses by recognizing virtual assets as property with economic value.

**Tags**: `#digital inheritance`, `#virtual assets`, `#Chinese courts`, `#property rights`, `#gaming`

---

<a id="item-11"></a>
## [Anthropic Web Crawler-to-Referral Ratio Hits 2800:1](https://www.businessinsider.com/anthropic-web-bots-crawling-referrals-cloudflare-distillation-2026-7) ⭐️ 8.0/10

Cloudflare data shows that for the week of July 1-7, Anthropic's web crawlers crawled about 2,800 webpages for every one referral sent back to the source websites, the highest ratio among major AI companies. This imbalance highlights ethical concerns about AI companies extracting web content for training while providing minimal referral traffic, potentially undermining the incentives for content creators. The ratio has improved from about 8,800:1 in early April and peaked at 24,700:1 in the first week of May. Anthropic has questioned Cloudflare's methodology, stating it cannot verify the calculations and that its new search feature is increasing site visits.

telegram · zaihuapd · Jul 10, 04:25

**Background**: Cloudflare uses machine learning and behavioral analysis to track AI crawler activity across 20% of global internet traffic. The 'crawl-to-refer' ratio measures how many times a company's bots crawl websites for every referral they send back, serving as a metric for ethical data usage in the AI era.

<details><summary>References</summary>
<ul>
<li><a href="https://www.businessinsider.com/anthropic-web-bots-crawling-referrals-cloudflare-distillation-2026-7">Anthropic Treats the Web Like an All-You-Can-Eat Buffet - Business Insider</a></li>
<li><a href="https://www.businessinsider.com/anthropic-bot-crawlers-feast-on-web-give-little-back-ranking-2025-9">Anthropic Bot Crawlers Feast on the Web and Give Little Back: Ranking - Business Insider</a></li>
<li><a href="https://developers.cloudflare.com/ai-crawl-control/features/analyze-ai-traffic/">Analyze AI traffic · Cloudflare AI Crawl Control docs</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#web scraping`, `#Anthropic`, `#Cloudflare`, `#content attribution`

---

<a id="item-12"></a>
## [Long March 10B achieves world's first net-based rocket stage recovery at sea](https://weibo.com/7340734455/R814of1Ki) ⭐️ 8.0/10

On July 10, 2026, China's Long March 10B rocket launched from Hainan Commercial Space Launch Site and successfully completed the world's first net-based recovery of its first stage at sea, after stage separation about 6 minutes into flight. This milestone demonstrates China's capability in reusable rocket technology, potentially reducing launch costs and increasing launch frequency, which is crucial for future space missions and commercial launches. The net-based recovery method is similar to the arresting gear used on aircraft carriers, where the descending first stage is caught by a net system on a sea platform. This approach differs from the landing leg method used by SpaceX's Falcon 9.

telegram · zaihuapd · Jul 10, 04:36

**Background**: Rocket stage recovery aims to reuse costly components, dramatically lowering the per-launch cost. Traditional recovery methods involve powered vertical landing with legs, but net capture offers an alternative that may reduce complexity. The Long March 10B is being developed as a partially reusable launch vehicle by China's aerospace industry.

<details><summary>References</summary>
<ul>
<li><a href="https://www.news.cn/20260710/ba0ac14f31dd492aaf918e7a86ac844a/c.html">长征十号乙首飞成功 我国运载火箭首次实现可控回收-新华网</a></li>
<li><a href="https://h5.ifeng.com/c/vivoArticle/v0026U0p1yEaP670syi0cuThLxSHZRUClOnfql0NufHtc7Y__?isNews=1&showComments=0">长征十号乙月底发射，再次验证海上网系回收</a></li>

</ul>
</details>

**Tags**: `#aerospace`, `#rocket recovery`, `#space technology`, `#China`

---

<a id="item-13"></a>
## [OpenAI, Google Allegedly Served Blacklisted Chinese Firms via Singapore](https://www.ft.com/content/5d6aafa1-5d47-4585-aa95-6ec06a6cd20f) ⭐️ 8.0/10

OpenAI and Google have allegedly provided advanced AI services to Singapore subsidiaries of Alibaba, Baidu, and Tencent, despite their parent companies being on the U.S. Department of Defense's 1260H list, which flags entities with alleged ties to the Chinese military. This raises renewed calls for stricter U.S. export controls on AI software, as current regulations do not broadly restrict Chinese companies from accessing advanced AI models overseas. The issue highlights gaps in national security oversight of AI technology. OpenAI suspended API access for an Alibaba-affiliated user last month after detecting suspected model distillation, and reported it to the U.S. government. Anthropic, in contrast, enforces a stricter policy that fully bans Chinese companies and their overseas entities from accessing its frontier AI models.

telegram · zaihuapd · Jul 10, 09:59

**Background**: The 1260H list is a U.S. Department of Defense list of entities allegedly linked to China's military. Model distillation is a technique to transfer knowledge from a large AI model to a smaller one, which can be used to replicate capabilities. Current U.S. export controls on AI software are primarily focused on physical exports from the U.S., not on services provided by foreign subsidiaries.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1260H_list">1260H list</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_distillation">Model distillation</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#export controls`, `#OpenAI`, `#Google`, `#China`

---