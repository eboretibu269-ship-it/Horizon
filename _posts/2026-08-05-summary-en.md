---
layout: default
title: "Horizon Summary: 2026-08-05 (EN)"
date: 2026-08-05
lang: en
---

> From 32 items, 13 important content pieces were selected

---

1. [Jeff Dean's Discovery Loop Aims to Automate Scientific Experimentation](#item-1) ⭐️ 9.0/10
2. [Hassabis to Chair DeepMind, Jeff Dean Departs Google](#item-2) ⭐️ 9.0/10
3. [ChainDrop Worm Compromises 1,300+ npm Packages](#item-3) ⭐️ 9.0/10
4. [Neon's Castform Beats GPT-5.6 Sol on Retrieval at 100x Lower Cost](#item-4) ⭐️ 8.0/10
5. [Meta Ran Ads Containing AI-Generated Child Sexual Abuse Imagery](#item-5) ⭐️ 8.0/10
6. [Cloudflare OS: Open Platform for Agents, Apps, and Work](#item-6) ⭐️ 8.0/10
7. [Position Paper Argues LLMs Cannot Jump to Scientific Discovery](#item-7) ⭐️ 8.0/10
8. [Elon Musk: SpaceX to Exclusively Use Nvidia AI Architecture](#item-8) ⭐️ 8.0/10
9. [DeepSeek Restarts Second Funding Round at 500B Yuan Pre-Money Valuation](#item-9) ⭐️ 8.0/10
10. [Samsung, SK Hynix Testing Chinese Chip Tools to Hedge US Export Controls](#item-10) ⭐️ 8.0/10
11. [ByteDance's SeedRealtime: Native Audio-Video Full-Duplex Model](#item-11) ⭐️ 8.0/10
12. [FFmpeg 9.0 brings animated WebP, Vulkan filters, Playdate encoding](#item-12) ⭐️ 8.0/10
13. [China Exchanges Shut In-House LAN Lines, Nearby Data Center Rents Jump](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Jeff Dean's Discovery Loop Aims to Automate Scientific Experimentation](https://www.discoveryloop.com/) ⭐️ 9.0/10

Discovery Loop launched with the mission to automate the experimental loop for scientific discovery, starting with machine learning research and engineering. The initiative uses frontier AI models and large-scale compute to propose, run, and learn from evaluations. This initiative could transform how scientific research is conducted, accelerating progress across numerous disciplines. It also represents a new paradigm where the scientific method itself is partially automated, potentially reshaping the roles of human researchers. The approach reportedly has three stages, with the initial focus on improving ML research before expanding to other scientific domains. The founders hope to discover better algorithms and possibly new model architectures through automated experimentation loops.

hackernews · xtreak29 · Aug 5, 16:19 · [Discussion](https://news.ycombinator.com/item?id=49184960)

**Background**: Discovery Loop was founded by Jeff Dean, a renowned computer scientist and former senior fellow at Google. Automating the experimental loop means using AI systems to autonomously generate hypotheses, design experiments, run them, and interpret results. This concept builds on earlier ideas like Karpathy's AutoResearch, but at a much larger institutional scale. Traditional scientific discovery relies heavily on human-driven iteration, which is time-consuming and resource-intensive.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unite.ai/jeff-dean-leaves-google-to-automate-the-scientific-method-with-discovery-loop/">Jeff Dean Leaves Google to Automate the Scientific Method With...</a></li>
<li><a href="https://superintelligencenews.com/ai-fields/large-language-models/google-ai-startup-discovery-loop/">Google AI Startup Discovery Loop Launches</a></li>
<li><a href="https://mljar.com/blog/autoresearch-karpathy-autonomous-ai-research/">AutoResearch by Karpathy and the Future of Autonomous AI Research</a></li>

</ul>
</details>

**Discussion**: Commenters noted similarities to Karpathy's AutoResearch and questioned how physical experimentation could be automated, with one describing the initiative as a 'retirement home' for senior Google engineers. Others debated the philosophical implications of AI-driven research. Overall sentiment was a mix of excitement and skepticism.

**Tags**: `#automation`, `#machine-learning`, `#scientific-discovery`, `#research`, `#AI`

---

<a id="item-2"></a>
## [Hassabis to Chair DeepMind, Jeff Dean Departs Google](https://blog.google/company-news/inside-google/message-ceo/next-chapter-ai-momentum/) ⭐️ 9.0/10

Google DeepMind announced that Demis Hassabis will move from CEO to Chair, while longtime Google engineers Jeff Dean and Sanjay Ghemawat are departing to launch an independent public benefit corporation focused on machine learning, science, and engineering. This marks a major shift in leadership at one of the world's most prominent AI research organizations, raising concerns that Google is losing its top AI talent to rivals and startups. The shake-up could affect Google's competitive position in the global AI race, especially as it competes with OpenAI, Anthropic, and others. Jeff Dean is leaving after a 27-year career at Google; he and fellow Senior Fellow Sanjay Ghemawat are launching an independent public benefit corporation to accelerate discoveries in machine learning, science, and engineering. Demis Hassabis will move from CEO to Chair of Google DeepMind.

hackernews · colesantiago · Aug 5, 16:05 · [Discussion](https://news.ycombinator.com/item?id=49184755)

**Background**: Google DeepMind is Alphabet's AI research division, formed in 2023 by merging DeepMind and Google Brain. Demis Hassabis is a co-founder of DeepMind, which became famous for developing AlphaGo. Jeff Dean is a legendary Google engineer and a key figure behind many of the company's foundational systems and AI infrastructure. The leadership transition comes at a time of intense competition in the AI industry, with top researchers often leaving big companies to start or join startups and labs.

**Discussion**: Commenters expressed a strong sense of loss, calling it the 'end of a golden era' and compiling the many prominent AI researchers who have left Google recently. One user joked that when Jeff Dean leaves, Google's stock drops 20 points, while others emphasized that the real news is the departure of Dean and Ghemawat rather than Hassabis's new role. Overall sentiment is pessimistic about Google's ability to retain its top talent.

**Tags**: `#Google DeepMind`, `#AI leadership`, `#Jeff Dean`, `#Demis Hassabis`, `#talent exodus`

---

<a id="item-3"></a>
## [ChainDrop Worm Compromises 1,300+ npm Packages](https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/) ⭐️ 9.0/10

The self-propagating ChainDrop worm has compromised over 1,300 npm packages, including popular caching libraries Keyv and Cacheable, with a combined 2 billion monthly downloads. The attack started by compromising a maintainer's GitHub account and is still spreading. This is one of the largest npm supply-chain attacks to date, affecting packages with billions of downloads and targeting developer credentials across GitHub, npm, AWS, and Kubernetes. The worm's self-propagating nature means the number of infected packages is expected to grow, posing a significant risk to the entire open-source ecosystem. Malicious packages install a setup.mjs dropper that executes a 727 KB credential stealer called Math_Symbol.js on `npm install`, harvesting tokens and planting persistence. Security researchers advise treating any system that installed an affected version as compromised and rotating all credentials immediately; the npm-cache[.]com domain can serve as an indicator of compromise.

telegram · zaihuapd · Aug 5, 03:04

**Background**: npm is the default package manager for Node.js and one of the largest software registries in the world, with millions of packages used across the JavaScript ecosystem. Supply-chain attacks work by compromising a maintainer account or build process so that malicious code is delivered automatically to everyone who installs a trusted package. ChainDrop is a worm that uses compromised npm credentials to infect other maintainers' packages, amplifying the attack in a chain reaction.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stepsecurity.io/blog/chaindrop-npm-worm">ChainDrop npm Worm: Bun-loaded CI/CD credential... - StepSecurity</a></li>
<li><a href="https://www.securityweek.com/over-400-npm-packages-infected-in-chaindrop-supply-chain-attack/">Over 400 NPM Packages Infected in ChainDrop... - SecurityWeek</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/08/04/chaindrop-supply-chain-compromise-anatomy-self-propagating-worm/">ChainDrop supply chain compromise... | Microsoft Security Blog</a></li>

</ul>
</details>

**Tags**: `#npm`, `#供应链攻击`, `#安全`, `#恶意软件`, `#开源生态`

---

<a id="item-4"></a>
## [Neon's Castform Beats GPT-5.6 Sol on Retrieval at 100x Lower Cost](https://neon.com/blog/how-castform-neon-beats-frontier-models-on-price-and-efficiency) ⭐️ 8.0/10

Neon's blog post introduces Castform, a purpose-built open model that reportedly beats GPT-5.6 Sol on retrieval tasks while costing 100x less to run. The result challenges the prevailing assumption that the largest general-purpose models should be used for every task. It suggests that specialized, inexpensive open models can make retrieval and RAG pipelines far more cost-efficient, especially as routing between models becomes easier. The comparison focuses on retrieval performance rather than general reasoning, and Castform's weights are openly available. As some commenters note, the post would be stronger if it included a concrete worked example, and retrieval effectiveness in very large document collections remains an open question.

hackernews · moonikakiss · Aug 5, 18:18 · [Discussion](https://news.ycombinator.com/item?id=49186762)

**Background**: Retrieval-augmented generation (RAG) is a technique that lets LLMs pull relevant information from external documents or databases before answering, which helps reduce hallucinations and the need to retrain models. Open-weights models make their parameters publicly accessible, so teams can fine-tune and deploy them at relatively low cost. This makes purpose-built retrieval models an attractive alternative to expensive frontier models for tasks that focus on finding facts in existing data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval-augmented generation</a></li>
<li><a href="https://aws.amazon.com/what-is/retrieval-augmented-generation/">What is RAG? - Retrieval-Augmented Generation AI Explained - AWS</a></li>
<li><a href="https://promptmetheus.com/resources/llm-knowledge-base/open-weights-model">Open-weights Model | LLM Knowledge Base</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly positive about purpose-built models, comparing the shift to 'using the right data structure,' but some asked for a concrete example to prove the point. Others raised open questions about finding needles in larger haystacks, and one commenter said their own tests showed smaller models beating larger ones on fact retrieval while requesting a comparison with GPT-5.6 Luna.

**Tags**: `#LLM`, `#retrieval`, `#specialized models`, `#cost efficiency`, `#open models`

---

<a id="item-5"></a>
## [Meta Ran Ads Containing AI-Generated Child Sexual Abuse Imagery](https://www.wired.com/story/meta-ran-ads-that-contained-ai-generated-child-sexual-abuse-imagery/) ⭐️ 8.0/10

Meta ran ads on its platforms that contained AI-generated child sexual abuse imagery, according to a Wired report. This incident reveals significant gaps in Meta's content moderation systems, allowing illegal synthetic content to slip through. This news matters because it demonstrates how generative AI can be weaponized to produce illegal content at scale, bypassing existing moderation safeguards. It raises urgent questions about platform accountability, regulatory enforcement, and the safety of AI-generated media for online users. The report highlights that Meta's moderation tools, which rely heavily on perceptual hashing like PhotoDNA, may fail to detect novel AI-generated imagery that has no known hash match. Community comments also suggest that reporting such content to Meta is slow and often ineffective, pointing to systemic moderation failures.

hackernews · malshe · Aug 5, 19:47 · [Discussion](https://news.ycombinator.com/item?id=49187977)

**Background**: AI-generated child sexual abuse imagery refers to synthetic depictions of child abuse created using generative models like GANs or diffusion models. Content moderation platforms commonly use perceptual hashing, such as Microsoft's PhotoDNA, to match known illegal images, but these tools struggle with novel AI-generated content that has not been previously fingerprinted. This incident underscores the broader challenge of moderating generative AI outputs at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PhotoDNA">PhotoDNA</a></li>
<li><a href="https://en.wikipedia.org/wiki/Perceptual_hashing">Perceptual hashing</a></li>
<li><a href="https://en.wikipedia.org/wiki/Generative_adversarial_network">Generative adversarial network</a></li>

</ul>
</details>

**Discussion**: Community comments express widespread frustration and distrust in Meta's moderation, with one user noting that ads with sexual content slip through on YouTube too, suggesting no one is truly moderating. Another user remarks that fines are merely a cost of doing business, while others question whether human-edited local newspapers were actually better at oversight. Long reporting delays and Meta's inconsistent enforcement on violent content were also called out.

**Tags**: `#AI-generated content`, `#content moderation`, `#Meta`, `#online safety`, `#ethics`

---

<a id="item-6"></a>
## [Cloudflare OS: Open Platform for Agents, Apps, and Work](https://blog.cloudflare.com/cloudflare-os/) ⭐️ 8.0/10

Cloudflare announced Cloudflare OS on August 5, 2026, an open-source agent workspace built on Cloudflare Workers and AI. It lets employees create documents, build apps, and run agents using their company's own context and systems. This is significant because it moves AI workspaces beyond generic chatbots toward organization-specific operations with governance built in by default. It could shape how enterprises adopt agentic workflows and intensify competition in the AI platform space. Cloudflare OS is open source and hosted on GitHub, described as the first AI workspace built around how companies actually work. Kenton Varda noted it is essentially a remake of his earlier project Sandstorm.io on Cloudflare Workers, deeply leveraging AI.

hackernews · speckx · Aug 5, 13:58 · [Discussion](https://news.ycombinator.com/item?id=49182996)

**Background**: Cloudflare Workers is a serverless functions platform that runs code at the edge, scaling from zero to millions of requests and supporting AI models through Workers AI. Cloudflare OS builds on this infrastructure to let organizations create private, governed agent workspaces. The announcement follows the broader industry trend of AI agents and workspaces, while the 'OS' branding has naturally invited skepticism about whether it is truly an operating system.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/cloudflare-os/">Cloudflare OS: an open platform for agents, apps, and work</a></li>
<li><a href="https://github.com/cloudflare/cloudflare-os">GitHub - cloudflare/cloudflare-os: Agent workspace built on Cloudflare ...</a></li>
<li><a href="https://www.cloudflare.com/press/press-releases/2026/cloudflare-os-is-the-first-ai-workspace-built-around-how-companies-actually-work/">Cloudflare OS Is the First AI Workspace Built Around How Companies ...</a></li>

</ul>
</details>

**Discussion**: Commenters are generally intrigued but skeptical, raising concerns about vendor lock-in, the overuse of the 'OS' label, and how shared data and updates would work when everyone can customize apps and data models. One commenter appreciated Kenton Varda's framing of Cloudflare OS as a modern remake of Sandstorm.

**Tags**: `#cloudflare`, `#platform`, `#agents`, `#ai`, `#workers`

---

<a id="item-7"></a>
## [Position Paper Argues LLMs Cannot Jump to Scientific Discovery](https://openreview.net/challenge?redirect=%2Fforum%3Fid%3DklU4737opt) ⭐️ 8.0/10

A position paper titled "LLMs Can't Jump" arguing that large language models have fundamental limitations in scientific discovery has been published on OpenReview, receiving a high engagement score of 8.0/10 with 228 points and 155 comments. The author, Tom Zahavy, later clarified on social media that the paper does not claim LLMs can never make scientific discoveries. This paper challenges the dominant optimistic narrative about AI-driven scientific discovery, potentially shaping how researchers approach the use of LLMs in science. The active debate it has sparked could influence future research directions and funding priorities in AI for science. The paper specifically argues that science requires "leaps of intuition" that go beyond language-based reasoning, which LLMs cannot perform. Community comments highlight issues such as language being a lossy encoding of human experience and question the reductive historical retellings often used to support LLM capabilities.

hackernews · theanonymousone · Aug 5, 11:01 · [Discussion](https://news.ycombinator.com/item?id=49181083)

**Background**: Position papers are common in AI research venues, where authors advocate a specific viewpoint rather than presenting new experimental results. LLMs are increasingly applied to scientific problems, but this paper argues that the non-linguistic nature of scientific insight poses a fundamental barrier. The debate reflects broader questions about whether reasoning can be fully captured by language models trained on text.

**Discussion**: Community comments show a mix of agreement and clarification: one user argues language is a lossy encoding of human experience, another criticizes the reductive Einstein/Michelson-Morley historical narrative, and a third shares the author's own clarifications on X. Overall sentiment is engaged and nuanced, with some defending the paper and others pushing back on its claims.

**Tags**: `#LLMs`, `#AI for Science`, `#Position Paper`, `#Scientific Discovery`

---

<a id="item-8"></a>
## [Elon Musk: SpaceX to Exclusively Use Nvidia AI Architecture](https://wccftech.com/elon-musk-commits-spacex-exclusively-to-nvidia-gpus-citing-theyre-the-best/) ⭐️ 8.0/10

On August 4, Elon Musk announced during SpaceX's first earnings call that its AI services will run exclusively on Nvidia systems, citing the Vera Rubin architecture as the best AI compute architecture. SpaceX plans to deploy Nvidia Vera Rubin NVL72 racks in ground data centers and in space, targeting over 2 GW of AI compute by the end of this year and nearly 10 GW by the end of 2027. This exclusive commitment makes SpaceX a major anchor customer for Nvidia's next-generation AI infrastructure and extends AI computing into orbit. It could accelerate the development of space-based AI data centers and strengthen Nvidia's dominance in the AI hardware market. The Vera Rubin NVL72 is a rack-scale system that combines 72 Rubin GPUs and 36 Vera CPUs in a liquid-cooled rack using NVLink 6 interconnect. Nvidia has also introduced the space-grade Space-1 Vera Rubin module for satellite and in-orbit AI inference, which will support SpaceX's Starmind satellite project starting next year.

telegram · zaihuapd · Aug 5, 02:04

**Background**: Nvidia's Vera Rubin, unveiled at CES, is the successor to the Blackwell architecture and is reported to offer roughly three times the speed of Blackwell while being up to 10x more efficient. SpaceX's existing Starlink network already operates over 10,000 satellites for internet connectivity, while Starmind represents a pivot toward orbital AI data centers using Nvidia's computing platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aol.com/finance/nvidia-rubin-architecture-game-changer-172211628.html">Nvidia’s Rubin Architecture Is a Game-Changer. Here’s Why. - AOL</a></li>
<li><a href="https://cryptobriefing.com/spacex-starmind-ai-satellite-network/">SpaceX plans Starmind, an AI network powered by satellites in orbit</a></li>

</ul>
</details>

**Tags**: `#AI`, `#NVIDIA`, `#SpaceX`, `#Satellite Infrastructure`

---

<a id="item-9"></a>
## [DeepSeek Restarts Second Funding Round at 500B Yuan Pre-Money Valuation](https://finance.sina.com.cn/wm/2026-08-05/doc-inimfmyv1554159.shtml) ⭐️ 8.0/10

DeepSeek has restarted its second funding round, aiming to raise 50 billion yuan at a pre-money valuation of about 500 billion yuan, with contracts expected to be signed in late August. The round was paused in late July after founder Liang Wenfeng was dissatisfied with a leaked investor meeting transcript. This is a major business milestone for DeepSeek, with its valuation rising about 43% from the first funding round. If completed, the two rounds together will raise over 100 billion yuan, signaling strong investor appetite for Chinese artificial intelligence companies. The funding round initially started in mid-July but was suddenly halted at the end of July. Some institutions that had been actively engaged earlier say they have not yet received news of the restart, suggesting the financing channel may still be in a holding pattern.

telegram · zaihuapd · Aug 5, 02:46

**Background**: DeepSeek is an artificial intelligence company that completed its first funding round in June, raising 50 billion yuan at a valuation exceeding 350 billion yuan. Pre-money valuation refers to the company's value before new investment is added, so the incoming funds will increase the post-money valuation accordingly.

**Tags**: `#DeepSeek`, `#funding`, `#AI`, `#valuation`, `#finance`

---

<a id="item-10"></a>
## [Samsung, SK Hynix Testing Chinese Chip Tools to Hedge US Export Controls](https://www.reuters.com/world/china/samsung-sk-hynix-test-chinese-chip-tools-hedge-against-us-risks-2026-08-05/) ⭐️ 8.0/10

Reuters reported that Samsung Electronics and SK Hynix are evaluating etching tools from Chinese semiconductor equipment maker AMEC for use in their China factories, part of a hedge against tightening US export controls. The companies began testing roughly two years ago but have not yet decided on large-scale deployment; Samsung denied the testing, while SK Hynix declined to comment. This matters because two of the world's top memory chipmakers considering Chinese etching equipment would be a strong endorsement for domestic Chinese semiconductor tools, potentially reshaping competition in China's estimated $28 billion wafer fab equipment market. It also shows how US export controls are pushing US allies to explore Chinese alternatives for business continuity. The US revoked the 'validated end user' (VEU) status for Samsung and SK Hynix's China plants in 2025, replacing it with annual licenses for equipment imports. Chinese equipment typically costs 20% to 30% less than Western counterparts, and Deutsche Bank estimates domestic Chinese makers could take 25% to 30% of China's ~$28 billion wafer fab equipment market this year.

telegram · zaihuapd · Aug 5, 04:32

**Background**: Etching is a critical semiconductor manufacturing process that removes material to form circuit patterns; plasma etching tools are among the most complex and expensive pieces of fab equipment. AMEC (中微公司) is a leading Chinese supplier of plasma etching and MOCVD systems, having shipped over 1,500 CCP etching reaction chambers to fabs around the world. The VEU program previously gave Samsung and SK Hynix a broad exemption to ship US-controlled equipment to China without case-by-case licenses; its withdrawal creates uncertainty about future maintenance and upgrades of Western tools, prompting Korean firms to qualify Chinese suppliers as backups.

<details><summary>References</summary>
<ul>
<li><a href="https://sputniknews.cn/20260805/1072640842.html">媒体：三星、SK海力士在测试中国芯片制造设备，以规避美国风险</a></li>
<li><a href="https://www.ab-sm.com/a/52205">中微公司CCP刻蚀设备反应腔全球出货超3000台 - 艾邦半导体网</a></li>
<li><a href="https://m.elecfans.com/article/7382354.html">半导体“刻蚀（Etch）”工艺技术的详解；-电子发烧友网</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#export-controls`, `#China`, `#Samsung`, `#SK Hynix`

---

<a id="item-11"></a>
## [ByteDance's SeedRealtime: Native Audio-Video Full-Duplex Model](https://seed.bytedance.com/zh/blog/seedrealtime-%E9%9F%B3%E8%A7%86%E9%A2%91%E5%85%A8%E5%8F%8C%E5%B7%A5%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%8F%91%E5%B8%83-%E8%B5%B0%E5%90%91%E5%85%A8%E6%A8%A1%E6%80%81%E8%87%AA%E7%84%B6%E4%BA%A4%E4%BA%92) ⭐️ 8.0/10

On August 5, ByteDance's Seed team released SeedRealtime, a native audio-video full-duplex large model that unifies audio, video, and text in a single end-to-end architecture. The model is already fully deployed in the Doubao app. Unlike cascaded systems that chain ASR, VLM, and TTS modules, SeedRealtime runs perception, understanding, decision-making, and expression in parallel, cutting latency and reducing conversation interruptions. This marks a significant step toward natural, real-time full-duplex human-AI interaction and could improve assistants, live translation, and interactive agents. End-to-end human evaluation found that conversation rhythm problems were reduced by half compared with cascade models, and issues like being interrupted before finishing a sentence decreased significantly. The model requires no external voice activity detection (VAD) to manage turn-taking, enabling 'watch, listen, and speak' simultaneously.

telegram · zaihuapd · Aug 5, 04:42

**Background**: Traditional real-time multimodal systems use a cascade of modules: automatic speech recognition (ASR) converts speech to text, a vision-language model (VLM) handles images and video, and text-to-speech (TTS) produces responses, causing latency and information loss at each step. Full-duplex communication means both parties can send and receive simultaneously, like natural human conversation. SeedRealtime instead integrates these capabilities into one end-to-end model, allowing continuous interaction over live multimodal streams without external voice activity detection.

<details><summary>References</summary>
<ul>
<li><a href="https://technode.com/2026/08/05/bytedance-launches-seedrealtime-full-duplex-audio-video-model/">ByteDance launches SeedRealtime full-duplex audio-video model</a></li>
<li><a href="https://aireiter.com/blog/seedrealtime">SeedRealtime: ByteDance's Audio-Visual Full-Duplex LLM</a></li>
<li><a href="https://www.testingcatalog.com/bytedance-launches-seedrealtime-full-duplex-ai-model/">ByteDance launches SeedRealtime full-duplex AI model</a></li>

</ul>
</details>

**Tags**: `#AI`, `#real-time`, `#multimodal`, `#speech recognition`, `#ByteDance`

---

<a id="item-12"></a>
## [FFmpeg 9.0 brings animated WebP, Vulkan filters, Playdate encoding](https://news.ycombinator.com/item?id=49166202) ⭐️ 8.0/10

FFmpeg 9.0 was officially released, adding an animated WebP decoder and demuxer, a v360_vulkan filter, a Playdate video encoder and muxer, HE-AAC 960 decoding for DAB+, a transpose_cuda filter, an AMF framerate converter filter, and an ONNX Runtime DNN backend. The development team also received six months of free Claude Max access through Anthropic's Claude for Open Source Program, primarily to help find missing backports. FFmpeg is a cornerstone tool for multimedia processing, and this release brings GPU-accelerated filters and broader format support that improve performance and workflow coverage. It also highlights the growing role of AI-assisted development in open source, while raising important questions about how AI-generated changes are reviewed for security. The new v360_vulkan filter converts 360-degree video between spherical projection formats using Vulkan compute shaders on the GPU, making it faster than the CPU-only v360 filter. Animated WebP support in this release covers decoding and demuxing, while Playdate encoding, HE-AAC 960 for DAB+, and the ONNX Runtime DNN backend add further niche but notable capabilities.

telegram · zaihuapd · Aug 5, 10:32

**Background**: FFmpeg is a free, open-source multimedia framework used to process video, audio, and other media streams, with each major release typically adding new codecs, filters, and muxing formats. Vulkan is a cross-platform GPU API, and FFmpeg's Vulkan-based filters offload computation to the GPU via compute shaders. WebP is an image format that supports animation, and DAB+ digital radio commonly uses the HE-AAC v2 audio codec. Claude is Anthropic's AI assistant, and its open-source program provides free access to maintainers, though AI-generated patches still require human review.

<details><summary>References</summary>
<ul>
<li><a href="https://ubuntuhandbook.org/index.php/2026/08/ffmpeg-9-0-new-decoders-ubuntu-ppa/">FFmpeg 9.0 Released with New GPU Accelerated... | UbuntuHandbook</a></li>
<li><a href="https://www.fosslinux.com/159892/install-ffmpeg-vulkan-hardware-acceleration-linux.htm">How to Install FFmpeg with Vulkan Hardware Acceleration on Linux</a></li>

</ul>
</details>

**Discussion**: Community reaction to the release was broadly positive, but some members voiced concerns about the security-review process for AI-assisted development. The debate centered on whether AI-generated code receives sufficient human scrutiny before being merged, especially in a project as widely depended on as FFmpeg.

**Tags**: `#FFmpeg`, `#multimedia`, `#release`, `#AI-assisted development`, `#Open Source`

---

<a id="item-13"></a>
## [China Exchanges Shut In-House LAN Lines, Nearby Data Center Rents Jump](https://mp.weixin.qq.com/s/lH2IAcm1uX33Hw1H_EfPDg) ⭐️ 8.0/10

Starting on July 31, the Shanghai, Shenzhen, and Beijing stock exchanges replaced their in-house LAN trading and quote lines with wide-area network connections that enforce a minimum two-way latency of 2 milliseconds. Trading firms must move servers out of exchange facilities, and rents for nearby data center cabinets have surged. This change reshapes the economics of high-frequency trading, where physical proximity to the exchange matching engine directly affects order execution speed. It raises costs for latency-sensitive players, tightens third-party data center supply, and may make speed advantages less decisive for ultra-fast strategies. In Shanghai's Jinqiao, Waigaoqiao, and Zhangjiang areas, a standard 4,000-watt financial cabinet now rents for about 10,000 yuan per month, up from roughly 7,000 yuan at the start of the year; some prime locations have doubled. Only a few thousand financial-grade third-party cabinets exist near Jinqiao, so supply is tight.

telegram · zaihuapd · Aug 5, 14:44

**Background**: In electronic markets, co-location places a trader's servers physically next to the exchange's systems to cut latency to the minimum, and even microsecond differences can translate into profits for high-frequency strategies. A latency floor, such as the 2ms minimum introduced here, is a regulatory tool that prevents participants from gaining an edge purely through faster physical access, often by randomizing or adding a fixed delay. This move echoes global regulatory debates, including India's NSE co-location case, where fairness of proximity-based advantages was scrutinized.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Low_latency_(capital_markets)">Low latency (capital markets) - Wikipedia</a></li>
<li><a href="https://www.freepatentsonline.com/y2022/0301053.html">EFFICIENT RESOURCE ALLOCATION IN LATENCY FLOOR IMPLEMENTATION - Chicago Mercantile Exchange Inc.</a></li>
<li><a href="https://scroll.in/article/922911/nse-co-location-scam-sebis-fines-bans-are-only-beginning-of-regulation-in-this-area">NSE co-location case: Sebi’s bans, fines are only the beginning of...</a></li>

</ul>
</details>

**Tags**: `#trading-infrastructure`, `#high-frequency-trading`, `#regulation`, `#data-centers`, `#finance`

---