---
layout: default
title: "Horizon Summary: 2026-07-30 (EN)"
date: 2026-07-30
lang: en
---

> From 37 items, 14 important content pieces were selected

---

1. [GitHub Launches Stacked Pull Requests in Public Preview](#item-1) ⭐️ 9.0/10
2. [Anthropic's AI Breaks NIST Post-Quantum Candidate HAWK in 60 Hours](#item-2) ⭐️ 9.0/10
3. [Cheap streaming sticks preloaded with malware for ad fraud](#item-3) ⭐️ 8.0/10
4. [Gemini Robotics 2 Enables Whole-Body Robot Control](#item-4) ⭐️ 8.0/10
5. [OpenAI launches GPT-5.6 Luna with 80% price cut](#item-5) ⭐️ 8.0/10
6. [Google expands Android age checks globally via Age Signals API](#item-6) ⭐️ 8.0/10
7. [Economic Benefits of Refactoring Measured](#item-7) ⭐️ 8.0/10
8. [GCC steering committee adopts policy rejecting AI-generated contributions](#item-8) ⭐️ 8.0/10
9. [Professor Loses PhD Candidates Over Flawed Conference Reviews](#item-9) ⭐️ 8.0/10
10. [MLVC: Multi-Platform Learned Video Codec for Real-World Deployment](#item-10) ⭐️ 8.0/10
11. [Kimi K3 Achieves Frontier Open-Weight Performance with Novel Techniques](#item-11) ⭐️ 8.0/10
12. [ByteDance’s Biggest To B Restructure: Feishu Merged with Doubao and Volcano Engine](#item-12) ⭐️ 8.0/10
13. [Google DeepMind Disbands AlphaFold Team, Core Members Move to Anthropic](#item-13) ⭐️ 8.0/10
14. [EU Launches AI Gigafactory Tender to Mobilize €300 Billion](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GitHub Launches Stacked Pull Requests in Public Preview](https://github.blog/changelog/2026-07-30-stacked-pull-requests-are-now-in-public-preview/) ⭐️ 9.0/10

GitHub has made stacked pull requests available in public preview for all repositories, allowing developers to manage dependent PRs as ordered stacks. This feature significantly improves code review workflows by enabling incremental, independent review of stacked changes, which can lead to higher quality code and faster iterations. Stacked PRs require a specific CLI tool (gh-stack) and support merge queue integration rolling out in weeks. Known issues include broken bulk merging when using squash and merge requiring re-approvals.

hackernews · tomzorz · Jul 30, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49112232)

**Background**: Stacked pull requests are a development workflow where a large feature is split into multiple smaller, dependent changes that build on each other. Each change is reviewed independently but merged together in order. This differs from traditional single large PRs and can reduce merge conflicts and speed up review cycles.

<details><summary>References</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-07-30-stacked-pull-requests-are-now-in-public-preview/">Stacked pull requests are now in public preview - GitHub ...</a></li>

</ul>
</details>

**Discussion**: The community is generally positive, with Steve Klabnik calling it one of the biggest changes to GitHub in years. However, some users report bugs in merge and squash merge workflows, and questions about advantages over commit-by-commit review persist.

**Tags**: `#github`, `#pull requests`, `#developer tools`, `#workflow`

---

<a id="item-2"></a>
## [Anthropic's AI Breaks NIST Post-Quantum Candidate HAWK in 60 Hours](https://startupfortune.com/claude-mythos-broke-hawk-and-the-nist-post-quantum-timeline-may-not-survive-it/) ⭐️ 9.0/10

Anthropic announced that its Claude Mythos Preview AI discovered a critical weakness in the NIST post-quantum candidate HAWK, reducing its security margin in just 60 hours at a cost of $100,000 in API fees. This finding had eluded human experts for two years. This demonstrates AI's rapidly growing capability to identify cryptographic vulnerabilities faster than human cryptanalysts, potentially accelerating the post-quantum standardization timeline. It also underscores the urgent need for cryptographic agility and reliance on established standards rather than awaiting perfect algorithms. The attack reduced the effective key strength of HAWK-256 from 2^64 to 2^38, but does not run in polynomial time, so larger keys remain secure. Additionally, the research included an improved attack on a seven-round version of AES-128, but full 10-round AES-128 remains unaffected.

telegram · zaihuapd · Jul 30, 05:47

**Background**: HAWK is a lattice-based digital signature scheme currently in Round 3 of NIST's post-quantum cryptography standardization process. Claude Mythos Preview is a powerful AI model from Anthropic, designed for complex cybersecurity tasks. The discovery highlights the dual-use nature of advanced AI in both defense and attack scenarios.

<details><summary>References</summary>
<ul>
<li><a href="https://www.csoonline.com/article/4202920/mythos-takes-its-first-shot-at-post-quantum-cryptography.html">Anthropic finds weakness in Hawk post-quantum digital signature algorithm | CSO Online</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos</a></li>
<li><a href="https://www.techtimes.com/articles/322174/20260730/south-korea-certifies-hybrid-post-quantum-encryption-module-ai-breaks-hawk-algorithm-60-hours.htm">South Korea Certifies Hybrid Post-Quantum Encryption Module as AI Breaks HAWK Algorithm in 60 Hours</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cryptography`, `#post-quantum`, `#NIST`, `#security`

---

<a id="item-3"></a>
## [Cheap streaming sticks preloaded with malware for ad fraud](https://krebsonsecurity.com/2026/07/read-this-before-you-buy-that-tv-streaming-stick/) ⭐️ 8.0/10

KrebsOnSecurity reports that many inexpensive TV streaming sticks sold by major retailers are preloaded with malware that turns them into residential proxies and commits ad fraud, posing serious security and privacy risks. This exposes a widespread vulnerability in consumer IoT devices, potentially compromising the privacy of millions of users and defrauding online advertisers. It highlights the lack of accountability among major e-commerce platforms for the products they sell. The malware is reportedly used for residential proxy schemes, which route internet traffic through the device's IP address to appear as genuine user connections, and ad fraud, which generates fake clicks and impressions to steal revenue. The devices often run outdated Android versions with no security updates.

hackernews · speckx · Jul 30, 17:04 · [Discussion](https://news.ycombinator.com/item?id=49112744)

**Background**: Residential proxies are intermediary servers that use real ISP-assigned IP addresses to hide the source of internet traffic, making them hard to detect. Ad fraud involves creating fraudulent online advertisement interactions to generate revenue. Cheap streaming sticks often run modified Android operating systems with poor security practices, making them easy targets for malware injection.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Residential_proxy">Residential proxy</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ad_fraud">Ad fraud</a></li>
<li><a href="https://www.cloudflare.com/learning/bots/what-is-ad-fraud/">What Is Ad Fraud? | Ad Click Fraud</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern about retailer responsibility, with many feeling that Amazon, Best Buy, and others should be held accountable for selling these harmful devices. Users shared personal experiences with similar products, and some noted a lack of technical maintenance makes these devices vulnerable even without deliberate malware.

**Tags**: `#security`, `#privacy`, `#IoT`, `#consumer electronics`, `#streaming devices`

---

<a id="item-4"></a>
## [Gemini Robotics 2 Enables Whole-Body Robot Control](https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/) ⭐️ 8.0/10

Google DeepMind has launched Gemini Robotics 2, a new AI model that can control entire humanoid robots, enabling whole-body motions and complex tasks. This marks a shift from previous models that only controlled upper-body movements. This advancement brings humanoid robots closer to practical applications in industries like manufacturing, logistics, and home assistance. It demonstrates DeepMind's progress in embodied intelligence and could accelerate the adoption of versatile robots. Gemini Robotics 2 uses spatial reasoning and long-horizon planning to map multi-step tasks and collaborate between robots. Access is currently limited to trusted testers including Boston Dynamics and Agility Robotics.

hackernews · ai2027 · Jul 30, 15:15 · [Discussion](https://news.ycombinator.com/item?id=49111237)

**Background**: Earlier Gemini Robotics models focused on table-top manipulation using only upper-body control. Whole-body control requires balancing, leg movement, and coordination across more degrees of freedom, making it significantly harder. This model builds on Gemini 2.0, a large language model adapted for robotics.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/">Gemini Robotics 2 brings whole body intelligence to robots — Google DeepMind</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_Robotics">Gemini Robotics</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/gemini-robotics-er-2/">Introducing Gemini Robotics ER 2</a></li>

</ul>
</details>

**Discussion**: A DeepMind researcher shared insider praise for the lab's breadth across AI fields. Commenters noted the robots' current slowness but drew comparisons to early LLMs, predicting rapid improvement. Some expressed skepticism about humanoid hardware limitations like actuators.

**Tags**: `#robotics`, `#AI`, `#DeepMind`, `#Gemini`, `#embodied intelligence`

---

<a id="item-5"></a>
## [OpenAI launches GPT-5.6 Luna with 80% price cut](https://openai.com/index/advancing-the-price-performance-frontier-with-gpt-5-6/) ⭐️ 8.0/10

OpenAI released GPT-5.6 Luna, its fastest and most affordable model, with an 80% price reduction, now costing $0.10 per million input tokens and $0.60 per million output tokens. This dramatic price drop makes advanced AI inference significantly more accessible for developers and businesses, potentially accelerating adoption and enabling new high-volume applications like multi-agent systems. GPT-5.6 Luna supports a 1,050,000-token context window and a maximum output of 128,000 tokens, while OpenAI also reduced serving costs through kernel optimizations and efficiency improvements.

hackernews · tedsanders · Jul 30, 17:15 · [Discussion](https://news.ycombinator.com/item?id=49112867)

**Background**: GPT-5.6 Luna is part of OpenAI's GPT-5.6 model family, which includes the flagship Sol and the balanced Terra. It is designed for cost-sensitive, high-volume workloads. The price cut follows a trend of falling AI model prices after a period of increases, with competitors like Kimi K3 and GLM 5.2 also lowering costs.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://openrouter.ai/openai/gpt-5.6-luna">GPT-5.6 Luna - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://developers.openai.com/api/docs/models/gpt-5.6-luna">GPT-5.6 Luna Model | OpenAI API</a></li>

</ul>
</details>

**Discussion**: The community reacted with excitement and surprise, comparing the price drop to the dial-up to broadband transition. Users noted the potential for running more parallel agents and the challenge of deciding when to use a weaker model. Some questioned whether OpenAI's cost savings from optimizations amount to billions per month.

**Tags**: `#AI`, `#GPT-5.6`, `#OpenAI`, `#cost-efficiency`, `#model-pricing`

---

<a id="item-6"></a>
## [Google expands Android age checks globally via Age Signals API](https://android-developers.googleblog.com/2026/07/google-play-age-signals-api-safer-experiences.html) ⭐️ 8.0/10

Google announced it will expand age verification checks on Android worldwide by the end of 2026, requiring apps to integrate its Play Age Signals API to determine user age ranges. The API, currently in beta, allows apps to retrieve age signals from Google Family Link to enforce age-appropriate content. This move signals a major step toward regulatory compliance across global markets, but raises privacy concerns about mandatory account creation and centralization of age data. It will affect millions of Android app developers and users, potentially reshaping how apps handle age-sensitive content. The Play Age Signals API returns age ranges like 0-12, 13-15, 16-17, and 18+, and supports Android 6.0+ devices. Apps that fail to integrate may risk enforcement actions, though Google has not disclosed specific penalties. The rollout begins with Brazil as a testing ground.

hackernews · dmantis · Jul 30, 10:13 · [Discussion](https://news.ycombinator.com/item?id=49107950)

**Background**: Age verification on mobile platforms has been contentious, with regulators pushing for stronger protections for minors. Google's Family Link already provides parental controls; the Age Signals API extends this to third-party apps. Developers must opt into the API and cannot rely on self-reported ages.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.android.com/google/play/age-signals/use-age-signals-api">Use Play Age Signals API (beta) - Android Developers</a></li>
<li><a href="https://developer.android.com/google/play/age-signals/overview">Play Age Signals overview | Android Developers</a></li>
<li><a href="https://cybernews.com/tech/android-developers-age-verification-tool-google/">What is Google’s Android Age Signals API tool? | Cybernews</a></li>

</ul>
</details>

**Discussion**: Comments reflect divided opinions: some oppose mandatory accounts and fear monopolistic lock-in, while others argue that parental responsibility alone is insufficient and regulation is necessary. A notable concern is that the API is opt-in, leaving gaps where non-compliant apps may still expose children to inappropriate content.

**Tags**: `#privacy`, `#age-verification`, `#android`, `#google-play`, `#regulation`

---

<a id="item-7"></a>
## [Economic Benefits of Refactoring Measured](https://martinfowler.com/articles/exploring-gen-ai/refactoring-economic-benefit.html) ⭐️ 8.0/10

This article presents a quantitative analysis of the economic benefits of refactoring, specifically critiquing vague AI commentary by providing concrete measurements of AI's performance in refactoring tasks. This matters because it moves the conversation about AI in software engineering from abstract speculation to data-driven evidence, helping developers and managers make informed decisions about investing in refactoring and AI tools. The article likely includes specific metrics such as token consumption reductions and argues that refactoring reduces token usage and improves AI reasoning, as noted in community comments.

hackernews · javaeeeee · Jul 30, 15:10 · [Discussion](https://news.ycombinator.com/item?id=49111176)

**Background**: Refactoring is the process of restructuring existing computer code without changing its external behavior, aiming to improve readability, maintainability, and performance. With the rise of AI coding assistants, there has been much discussion about AI's ability to assist with refactoring, but often without concrete evidence. This article provides a data-driven perspective.

**Discussion**: The community highly praises the article for its specific, quantitative approach, contrasting it with vague AI commentary. Some comments highlight that the benefits of refactoring extend beyond token consumption to better reasoning and generalization. Others note that a human-in-the-loop is still essential for understanding the project context during refactoring.

**Tags**: `#refactoring`, `#AI`, `#software engineering`, `#economics`, `#code quality`

---

<a id="item-8"></a>
## [GCC steering committee adopts policy rejecting AI-generated contributions](https://lwn.net/Articles/1086041/) ⭐️ 8.0/10

The GCC steering committee has accepted a policy from the GCC AI policy working group that declines any legally significant code contributions generated by AI or LLM agents, effective immediately. This policy sets a clear precedent for open-source projects grappling with a surge of low-quality AI-generated pull requests, helping maintain code quality and legal clarity while sparking debate on the role of AI in open-source development. The policy targets 'legally significant' contributions such as new features or complex patches, while minor fixes like typo corrections may still be accepted; contributors are expected to certify that the work is their own original creation.

hackernews · arto · Jul 30, 11:45 · [Discussion](https://news.ycombinator.com/item?id=49108685)

**Background**: GCC (GNU Compiler Collection) is a cornerstone open-source compiler project supporting multiple programming languages. The rise of AI coding assistants has led to an influx of automated pull requests that often lack quality and legal provenance, prompting many open-source projects to establish formal AI contribution policies. Similar moves have been made by projects like curl, which shut down its bug bounty program partly due to AI-generated false reports.

<details><summary>References</summary>
<ul>
<li><a href="https://www.phoronix.com/news/GCC-Declining-AI-Contributions">GCC To Decline Any Significant Contributions Made Via AI/LLMs...</a></li>
<li><a href="https://itsfoss.com/news/gcc-bans-ai-code/">GCC Compiler Bans AI Code Contribution But Sensibly</a></li>

</ul>
</details>

**Discussion**: Community comments reveal a spectrum of opinions: some applaud the policy as a necessary safeguard against low-effort AI contributions, while others criticize it as overly restrictive and reminiscent of past misguided bans (e.g., Zig's similar policy). A notable comment argues that 'the true purpose of AI is to allow wealth to access skill without allowing skill to access wealth,' reflecting deeper concerns about equity.

**Tags**: `#GCC`, `#AI policy`, `#open source`, `#community guidelines`

---

<a id="item-9"></a>
## [Professor Loses PhD Candidates Over Flawed Conference Reviews](https://www.reddit.com/r/MachineLearning/comments/1vawwb8/i_have_lost_three_and_a_half_potential_phd/) ⭐️ 8.0/10

An early-career assistant professor reports losing three and a half potential PhD students because the students were disillusioned by the arbitrary and exhausting conference review process in machine learning. This highlights a systemic issue in ML academia where the review process discourages talented young researchers from pursuing PhDs, potentially damaging the future of the field. The professor had papers with strong reviews (e.g., four unanimous weak accepts) still get rejected, leading to endless resubmission cycles where each round introduces new random criticisms.

reddit · r/MachineLearning · /u/AffectionateLife5693 · Jul 30, 15:30

**Background**: Top machine learning conferences (e.g., NeurIPS, ICML, ICLR) use a peer review process with multiple reviewers per paper. In recent years, submission volumes have skyrocketed, making reviews more stressful and inconsistent. The "big three" in ML are often considered NeurIPS, ICML, and ICLR; some also include CVPR for vision.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.roboflow.com/ai-computer-vision-conferences/">Top AI & Computer Vision Conferences in 2026</a></li>
<li><a href="https://www.academia.edu/85652368/Design_and_Analysis_of_the_NIPS_2016_Review_Process">(PDF) Design and Analysis of the NIPS 2016 Review Process</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#conference review`, `#academia`, `#PhD students`, `#research culture`

---

<a id="item-10"></a>
## [MLVC: Multi-Platform Learned Video Codec for Real-World Deployment](https://www.reddit.com/r/MachineLearning/comments/1vb3xwd/mlvc_multiplatform_learned_video_codec_for/) ⭐️ 8.0/10

MLVC is a hardware-robust neural video codec that bypasses cross-platform numerical accuracy issues by transmitting entropy-model scale parameters through the hyperprior, achieving ~100 FPS encoding/decoding on consumer NPUs for 360p/540p video. This work addresses a critical deployment barrier for learned video codecs—cross-platform incompatibility—which has prevented them from replacing traditional codecs like H.264 and AV1 in practice, despite superior coding efficiency. MLVC avoids the need for bit-exact neural network inference across different NPUs by explicitly sending entropy-model parameters via the hyperprior, ensuring correct decoding even when hardware math differs. The codec runs at about 100 FPS on consumer NPUs for lower resolutions.

reddit · r/MachineLearning · /u/tanelai · Jul 30, 19:40

**Background**: Learned video codecs use neural networks to compress video, often achieving better rate-distortion performance than traditional codecs like H.265 and AV1. However, they rely on entropy models that require bit-exact arithmetic between encoder and decoder; small floating-point differences across hardware platforms can cause catastrophic decoding failures. Traditional codecs dominate because they have ubiquitous hardware acceleration and well-specified math, while neural codecs lack cross-platform determinism and efficient deployment paths.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2309.11276">Towards Real-Time Neural Video Codec for Cross-Platform ...[2606.28027v1] MLVC: Multi-platform Learned Video Codec for ...Towards Real-Time Neural Video Codec for Cross-Platform ...Towards Real-Time Neural Video Codec for Cross-Platform ...Towards Real-Time Neural Video Codec for Cross-Platform ...Towards Real-Time Neural Video Codec for Cross-Platform ...Cross-Platform Neural Video Coding: A Case Study - IEEE Xplore</a></li>

</ul>
</details>

**Tags**: `#learned video codecs`, `#neural compression`, `#cross-platform`, `#video encoding`, `#AI deployment`

---

<a id="item-11"></a>
## [Kimi K3 Achieves Frontier Open-Weight Performance with Novel Techniques](https://www.reddit.com/r/MachineLearning/comments/1vaysjf/how_kimi_k3_engineered_its_way_to_the_frontier_r/) ⭐️ 8.0/10

Moonshot AI released Kimi K3, an open-weight model that ranks fourth among 580 models on Artificial Analysis, behind only Claude Opus 5, Fable 5, and GPT-5.6 Sol. The 47-page technical report and code reveal three key innovations: Kimi Delta Attention, Quantile Balancing for 896 experts, and AgentENV for RL training. This model demonstrates that open-weight models can compete with proprietary frontier models, lowering the barrier for researchers and developers to access state-of-the-art capabilities. The novel attention mechanism and expert balancing techniques could influence future architecture designs across the industry. Kimi Delta Attention replaces the KV cache in 69 of 93 layers with a single 128x128 matrix per head, reducing 1M-token context memory from 104.6 GiB to 27.2 GiB. Quantile Balancing computes the selection bias directly from router score quantiles to evenly load 896 experts per layer, overcoming limitations of DeepSeek-V3's fixed-step bias nudging.

reddit · r/MachineLearning · /u/noninertialframe96 · Jul 30, 16:37

**Background**: Large language models often use attention mechanisms that require significant memory for key-value caches, especially at long contexts. Mixture-of-Experts (MoE) models use multiple expert sub-networks and a router to select a subset for each token, requiring load balancing to prevent overloading some experts. Reinforcement learning (RL) training for agent tasks needs isolated sandboxes to execute actions safely and efficiently.

<details><summary>References</summary>
<ul>
<li><a href="https://jianyuh.github.io/attention/2025/12/13/KDA.html">Linear Attention: Kimi Delta Attention | Jianyu Huang’s Blog</a></li>
<li><a href="https://lilting.ch/en/articles/kimi-k3-moe-experts-router-dynamic-transformer">Kimi K3's router picks 16 of 896 experts: an allocator... | lilting channel</a></li>
<li><a href="https://www.marktechpost.com/2026/07/27/kimi-ai-and-kvcache-ai-open-sources-agentenv/">Kimi AI and kvcache-ai Open Sources 'AgentENV... - MarkTechPost</a></li>

</ul>
</details>

**Tags**: `#large language models`, `#attention mechanisms`, `#open-weight models`, `#model optimization`, `#Moonshot AI`

---

<a id="item-12"></a>
## [ByteDance’s Biggest To B Restructure: Feishu Merged with Doubao and Volcano Engine](https://news.qq.com/rain/a/20260730A03CAP00) ⭐️ 8.0/10

ByteDance has announced its largest To B restructuring since founding, integrating the Feishu product team with the Doubao AI assistant team to form a new 'Doubao Product Team', and merging Feishu’s market, sales, and customer service teams with Volcano Engine to create a 'Creativity Service Platform'. This move signals ByteDance’s strategic push to tightly integrate its leading AI assistant Doubao with enterprise productivity tools, potentially reshaping the competitive landscape of China’s enterprise software market. Feishu’s existing product offerings will remain unchanged, and the teams will deepen cooperation on productivity scenarios; the Doubao enterprise edition, co-developed by both teams, is already being internally tested with select Feishu customers.

telegram · zaihuapd · Jul 30, 02:55

**Background**: Feishu (Lark) is ByteDance’s enterprise collaboration suite. Doubao is ByteDance’s AI conversational assistant based on its large language model, with over 50 million active users. Volcano Engine is ByteDance’s enterprise cloud and AI platform. This restructuring aims to unify AI capabilities with enterprise services.

<details><summary>References</summary>
<ul>
<li><a href="https://www.toolcentral.ai/ai-tools/doubao/">Doubao: ByteDance's AI Assistant for Chat & Content - ToolCentral</a></li>
<li><a href="https://aiwiki.ai/wiki/volcano_engine">Volcano Engine | AI Wiki</a></li>

</ul>
</details>

**Tags**: `#ByteDance`, `#AI`, `#Feishu`, `#enterprise software`, `#restructuring`

---

<a id="item-13"></a>
## [Google DeepMind Disbands AlphaFold Team, Core Members Move to Anthropic](https://www.ft.com/content/61b2953d-ee0d-45de-af6e-a9c1cf524b33?syn-25a6b1a6=1) ⭐️ 8.0/10

Google DeepMind has dissolved the AlphaFold team, reassigning most researchers to other projects including Gemini and Isomorphic Labs, while three core members—John Jumper, Jonas Adler, and Alexander Pritzel—have left to join competitor Anthropic. This reorganization shifts resources away from a Nobel Prize-winning breakthrough to focus on large language models and other priorities, signaling a strategic pivot at DeepMind. The departure of key talent to Anthropic underscores intense competition for AI researchers in the industry. Over the past year, most original authors of AlphaFold papers have been reassigned internally to projects like Gemini, enzyme design, nuclear fusion, and genomics, with some moving to Alphabet’s drug discovery subsidiary Isomorphic Labs. Nearly a quarter of the paper authors have left the company entirely.

telegram · zaihuapd · Jul 30, 07:45

**Background**: AlphaFold is an AI system developed by DeepMind that predicts protein structures with high accuracy, winning the Nobel Prize in Chemistry in 2024. It has been widely adopted in biological research. Isomorphic Labs, founded by DeepMind CEO Demis Hassabis, is a separate Alphabet company focused on applying AI to drug discovery, building on AlphaFold technology.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AlphaFold">AlphaFold - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Isomorphic_Labs">Isomorphic Labs</a></li>
<li><a href="https://deepmind.google/science/alphafold/">AlphaFold — Google DeepMind</a></li>

</ul>
</details>

**Tags**: `#AI`, `#DeepMind`, `#AlphaFold`, `#Anthropic`, `#talent migration`

---

<a id="item-14"></a>
## [EU Launches AI Gigafactory Tender to Mobilize €300 Billion](https://www.wsj.com/world/europe/eu-opens-call-for-creation-of-local-ai-gigafactories-c286213d) ⭐️ 8.0/10

The European Commission has officially opened a tender for the creation of up to seven AI gigafactories, aiming to mobilize around €300 billion in total investment. Of this, €10 billion will come from EU-level funds and participating member states. This initiative is a strategic move to bolster the EU's own AI capabilities and compete with the US and other global leaders. The investment could significantly accelerate AI infrastructure development in Europe, affecting startups, researchers, and industries. The tender covers two phases: site selection and expansion. Bids are due by November 12, with results expected by July 2027, and projects must become operational within 18 months of contract signing.

telegram · zaihuapd · Jul 30, 11:50

**Background**: AI gigafactories are large-scale facilities designed to handle the entire lifecycle of very large AI models, from training to deployment. They differ from traditional data centers by integrating powerful computing resources in a unified structure. The EU's High Performance Computing Joint Undertaking (EuroHPC JU) is overseeing the initiative. This move comes as global competition in AI intensifies, with the US and China making significant investments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eurohpc-ju.europa.eu/ai-gigafactories_en">AI Gigafactories - The European High Performance Computing Joint...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#EU`, `#infrastructure`, `#investment`, `#policy`

---