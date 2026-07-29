---
layout: default
title: "Horizon Summary: 2026-07-29 (EN)"
date: 2026-07-29
lang: en
---

> From 42 items, 11 important content pieces were selected

---

1. [MitchellH Launches Superlogical, a New Company on libghostty](#item-1) ⭐️ 9.0/10
2. [AI worms self-replicate via Copilot in Word documents](#item-2) ⭐️ 9.0/10
3. [Moonshot AI raises $3.5B at $35B valuation after Kimi K3 launch](#item-3) ⭐️ 9.0/10
4. [Open-source engine runs Gemma 4 26B in 2GB RAM on M-series Mac](#item-4) ⭐️ 8.0/10
5. [Moonshot AI Launches Cheaper 256k Context Kimi K3-256k](#item-5) ⭐️ 8.0/10
6. [KOReader: Open-Source E-Reader Enhances Kindle and Kobo](#item-6) ⭐️ 8.0/10
7. [Handbook.md: Long Policy Documents Fail to Govern AI Agents](#item-7) ⭐️ 8.0/10
8. [Green: AI's perfect timing for post-quantum cryptanalysis](#item-8) ⭐️ 8.0/10
9. [Vendor-agnostic ML inference on edge devices using ncnn Vulkan](#item-9) ⭐️ 8.0/10
10. [Report: Hugging Face Models Used to Generate Deepfake Nudes](#item-10) ⭐️ 8.0/10
11. [China drafts anti-cyber violence law, targets AI-generated abuse](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [MitchellH Launches Superlogical, a New Company on libghostty](https://www.superlogical.com/) ⭐️ 9.0/10

MitchellH, creator of HashiCorp, announced Superlogical, a new company that will build terminal applications on the open-source libghostty library, which was previously developed for the Ghostty terminal emulator. He also transferred ownership of Ghostty to a non-profit organization. This announcement signals a new business model for sustainable open-source development, where a company builds proprietary products on top of a community-owned open-source core. It could reshape how terminal applications and developer tools are built and funded. Superlogical will use the MIT-licensed libghostty as a public building block, consuming the same components available to everyone else, and will upstream shared improvements. The company's exact product focus has not been disclosed yet.

hackernews · yan · Jul 29, 15:41 · [Discussion](https://news.ycombinator.com/item?id=49098965)

**Background**: libghostty is a terminal core library written in Zig that parses VT sequences, manages cursor state, and handles text reflow. It was originally developed for Ghostty, a high-performance terminal emulator. By separating the library from the emulator, MitchellH enables other developers to build custom terminal tools without reinventing low-level terminal handling.

<details><summary>References</summary>
<ul>
<li><a href="https://repo-explainer.com/ghostty-org/ghostling">Ghostling: Stripping the Terminal to its... — Repo Explainer</a></li>
<li><a href="https://webteractive.co/blog/ghostty-and-libghostty-the-terminal-core-quietly-reshaping-the-ecosystem">Ghostty and libghostty: The Terminal Core Quietly... — Webteractive</a></li>

</ul>
</details>

**Discussion**: Community members reacted positively, with simonw praising the open-source governance model where the library is owned by a non-profit. Some, like rixed, criticized the vague title as clickbait. Others drew parallels to older technologies like OLE/COM or noted similarities with other modern terminal multiplexers.

**Tags**: `#terminal`, `#open-source`, `#startup`, `#ghostty`, `#libghostty`

---

<a id="item-2"></a>
## [AI worms self-replicate via Copilot in Word documents](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 9.0/10

Researcher Håkon Måløy demonstrated a novel prompt injection attack that turns Microsoft Copilot for Word into a self-replicating AI worm, where malicious instructions hidden in documents cause Copilot to propagate the attack to new documents. This research reveals a critical vulnerability in AI agents that cannot distinguish between instructions and data, posing a serious security threat as such attacks could automatically spread through email, code repositories, and other agent-enabled platforms. The attack uses direct and indirect prompt injection techniques, embedding malicious instructions in document text that Copilot interprets as commands, enabling the worm to alter documents and propagate itself without requiring explicit user action.

hackernews · Canopy9560 · Jul 29, 11:44 · [Discussion](https://news.ycombinator.com/item?id=49096188)

**Background**: Prompt injection is a cybersecurity exploit where attackers embed malicious instructions in inputs that are processed by large language models (LLMs). Because LLMs cannot reliably distinguish between developer-provided instructions and user data, they may execute unintended commands. AI worms are self-propagating malware that leverage such vulnerabilities to spread autonomously through connected AI agents.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://www.sentinelone.com/cybersecurity-101/cybersecurity/ai-worms/">AI Worms Explained: Adaptive Malware Threats - SentinelOne</a></li>

</ul>
</details>

**Discussion**: Commenters expressed alarm, with rwmj noting that fundamentally mixing instructions with data cannot be fixed. boothby warned that increasing agent access will lead to worse attacks, while simonw and averagjoe voiced similar concerns about the inherent insecurity of AI-enabled applications. piker added that techniques like white text still work to hide prompts.

**Tags**: `#AI security`, `#LLM`, `#adversarial attacks`, `#Copilot`, `#prompt injection`

---

<a id="item-3"></a>
## [Moonshot AI raises $3.5B at $35B valuation after Kimi K3 launch](https://www.bloomberg.com/news/articles/2026-07-29/china-s-moonshot-ai-passes-funding-goal-to-hit-35-billion-value) ⭐️ 9.0/10

Moonshot AI completed a $3.5 billion funding round at a $35 billion post-money valuation, far exceeding its initial $1-2 billion target, driven by its breakthrough Kimi K3 model that approaches frontier AI performance. This funding round signals China's accelerated AI race and the disruptive potential of open-weight models like Kimi K3, which triggered a 'DeepSeek moment' by causing tech stock sell-offs and challenging proprietary leaders. Kimi K3 is a 2.8-trillion-parameter Mixture-of-Experts model with native vision and a 1M-token context window, priced at $3 per million input tokens and $15 per million output tokens; Moonshot AI has started a new funding round at a $50B pre-money valuation and plans a Hong Kong IPO this year.

telegram · zaihuapd · Jul 29, 10:12

**Background**: Moonshot AI is a Chinese AI startup known for its large language models. The term 'DeepSeek moment' refers to when DeepSeek-R1, an open-source model, matched proprietary models' performance, signaling a shift in AI competition. Kimi K3 continues this trend with open weights and leaderboard-topping benchmarks, intensifying the race between open-source and proprietary AI.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/cy9w4q8pgp0o">China's Moonshot AI claims Kimi K3 can rival OpenAI and Anthropic</a></li>
<li><a href="https://modal.com/library/moonshot/kimi-k3">Kimi K3 by Moonshot AI | Model Library | Modal</a></li>
<li><a href="https://openrouter.ai/moonshotai/kimi-k3">Kimi K3 - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#AI`, `#funding`, `#Moonshot AI`, `#large language models`, `#China`

---

<a id="item-4"></a>
## [Open-source engine runs Gemma 4 26B in 2GB RAM on M-series Mac](https://github.com/drumih/turbo-fieldfare) ⭐️ 8.0/10

TurboFieldfare, a new open-source inference engine written in Swift and Metal, runs a 4-bit quantized Gemma 4 26B model on any M-series Mac using only about 2GB of RAM by streaming routed experts from SSD. This enables running large language models on memory-constrained consumer hardware like 8GB MacBooks, making powerful on-device AI more accessible without requiring expensive high-RAM machines. The model's 4-bit quantized weights are approximately 14GB, but the engine keeps the shared part and KV cache in RAM while streaming only the needed routed experts from SSD, achieving 5-6 tok/s on an M2 MacBook Air and 31-35 tok/s on an M5 MacBook Pro.

hackernews · gitpusher42 · Jul 29, 15:05 · [Discussion](https://news.ycombinator.com/item?id=49098510)

**Background**: Mixture-of-Experts (MoE) models like Gemma 4 use a gating network to activate only a subset of expert subnetworks per token, reducing computation. 4-bit quantization compresses model weights to 4 bits per weight, shrinking memory footprint. The KV cache stores previously computed key-value pairs to avoid redundant computation during autoregressive generation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://medium.com/@joaolages/kv-caching-explained-276520203249">Transformers KV Caching Explained | by João Lages | Medium</a></li>
<li><a href="https://www.emergentmind.com/topics/4-bit-model-quantization">4-Bit Model Quantization</a></li>

</ul>
</details>

**Discussion**: Comments praise the innovation, with some noting previous similar approaches and discussing comparisons to llama.cpp's mmap. One user provided a workaround for compilation on older macOS, and another mentioned potential collaboration on a related DiffusionGemma project.

**Tags**: `#inference-engine`, `#on-device-AI`, `#gemma-4`, `#mac`, `#machine-learning`

---

<a id="item-5"></a>
## [Moonshot AI Launches Cheaper 256k Context Kimi K3-256k](https://www.kimi.com/code/docs/en/kimi-code/models) ⭐️ 8.0/10

Moonshot AI has released the Kimi K3-256k, a variant of the Kimi K3 model that offers a 256k-token context window at half the quota cost of the full 1M-context version. This pricing reduction makes long-context AI more accessible for developers and enterprises, potentially accelerating adoption of large context windows for tasks like code analysis and document processing. The Kimi K3-256k model consumes about half the API quota of the 1M version while delivering the same quality within the 256k context limit, and is available immediately via the Kimi API.

hackernews · monneyboi · Jul 29, 19:25 · [Discussion](https://news.ycombinator.com/item?id=49101852)

**Background**: The context window of a large language model (LLM) is the maximum amount of text it can consider at once, measured in tokens. A 256k-token context window can hold roughly 200,000 words, enabling analysis of long documents or codebases in a single pass. Models with 1M tokens, like the original Kimi K3, are more expensive and often overkill for many practical use cases.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Context_window">Context window - Wikipedia</a></li>
<li><a href="https://openrouter.ai/moonshotai/kimi-k3">Kimi K3 - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://hosn.om/blog/256k-context-window-practical-uses.html">Practical Use-Cases for 256K Token Context Windows</a></li>

</ul>
</details>

**Discussion**: Commenters generally welcomed the move, noting that 256k context is sufficient for most tasks and that the price cut is substantial. Some see this as evidence of LLM commoditization, with hyperscalers and data center owners who can offer cheap tokens poised to win over high-cost labs.

**Tags**: `#AI`, `#LLMs`, `#model pricing`, `#context windows`, `#Moonshot AI`

---

<a id="item-6"></a>
## [KOReader: Open-Source E-Reader Enhances Kindle and Kobo](https://koreader.rocks/) ⭐️ 8.0/10

KOReader continues to be actively developed as a free, open-source document viewer for E Ink devices, supporting a wide range of file formats including EPUB, PDF, DjVu, and MOBI. This software significantly enhances the reading experience on popular e-readers like Kindle and Kobo, offering features that proprietary firmware often lacks, such as native EPUB support and advanced customization. KOReader requires jailbreaking or custom firmware installation on devices like Kindle, which may be a barrier for some users; the UI/UX has been criticized as non-intuitive and laggy by some community members.

hackernews · Cider9986 · Jul 29, 11:05 · [Discussion](https://news.ycombinator.com/item?id=49095865)

**Background**: E Ink devices like Kindle and Kobo typically run proprietary firmware that limits file format support and customization. KOReader is an alternative open-source application that runs on such devices, providing broader format support and additional reading features.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/KOReader">KOReader</a></li>
<li><a href="https://koreader.rocks/">KOReader</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some users are extremely satisfied, calling KOReader superior to proprietary software and driving purchasing decisions, while others find the UI non-intuitive, laggy, and prefer the default viewer. There is also praise for its native format support and library integration.

**Tags**: `#e-reader`, `#open-source`, `#kindle`, `#kobo`, `#software`

---

<a id="item-7"></a>
## [Handbook.md: Long Policy Documents Fail to Govern AI Agents](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

Researchers at Surge AI released the HANDBOOK.md benchmark, which shows that AI agents fail to reliably follow long policy documents even with large context windows. This highlights a critical limitation of current long-context models, challenging the assumption that simply increasing context length ensures policy compliance in agentic systems. The benchmark spans five enterprise domains, placing agents in live environments with email, Slack, Jira, and calendars, and testing adherence to expert-written standard operating procedures.

hackernews · spIrr · Jul 29, 13:01 · [Discussion](https://news.ycombinator.com/item?id=49096969)

**Background**: AI agents are systems that autonomously perform tasks using an underlying language model. Long-context models, like those claiming 1M token support, are often expected to process entire policy documents, but this research shows they struggle due to attention decay, quantization, and limited reasoning depth.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2607.25398">HANDBOOK.md: A Benchmark for Long-Context Agentic Instruction...</a></li>
<li><a href="https://surgehq.ai/blog/handbook-md">HANDBOOK.md: Can AI Agents Follow a 100-Page Company Policy?</a></li>
<li><a href="https://artdirectiondaily.com/issues/2026-07-29-agents-flunk-the-handbook.html">HANDBOOK.md Agent Benchmark, Vercel eve... | Art Direction Daily</a></li>

</ul>
</details>

**Discussion**: Comments note that human-like limitations such as working memory constraints and instruction forgetting at long contexts mirror model failures. Users report that explicit in-task prompts work better than static CLAUDE.md files, and some argue that extensive reinforcement learning on synthetic data is required for agents to follow custom policies.

**Tags**: `#AI agents`, `#long context`, `#policy compliance`, `#AI safety`, `#LLM limitations`

---

<a id="item-8"></a>
## [Green: AI's perfect timing for post-quantum cryptanalysis](https://simonwillison.net/2026/Jul/29/matthew-green/#atom-everything) ⭐️ 8.0/10

Cryptography expert Matthew Green stated that the historic transition to post-quantum algorithms creates an ideal opportunity for AI-driven cryptanalysis to strengthen confidence in new standards, referencing Impagliazzo's five worlds and HAWK. This commentary underscores the critical juncture where AI cryptanalysis can validate post-quantum cryptography, potentially preventing weaknesses from becoming global standards. It highlights the synergy between AI and cryptography at a pivotal moment. Green's remarks follow Anthropic's Claude Mythos discovering a hidden flaw in HAWK-256, a NIST post-quantum signature candidate, in just 60 hours at $100,000 cost. The HAWK team subsequently withdrew the scheme. He also references Impagliazzo's Minicrypt world where public-key cryptography might not exist.

rss · Simon Willison · Jul 29, 18:18

**Background**: Post-quantum cryptography refers to cryptographic algorithms resistant to attacks from quantum computers. The world is transitioning from traditional public-key systems like RSA and elliptic-curve cryptography to new post-quantum algorithms, with NIST standardizing several schemes. Impagliazzo's five worlds classify computational complexity scenarios; 'Cryptomania' assumes public-key cryptography is possible, while 'Minicrypt' only allows symmetric-key primitives. HAWK is a lattice-based post-quantum signature scheme under NIST evaluation.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/claude-ai-just-cracked-post-quantum.html">Claude AI Just Cracked a Post-Quantum Test Scheme and Found a ...</a></li>
<li><a href="https://startupfortune.com/anthropics-claude-mythos-found-a-hidden-flaw-in-hawk-before-it-could-become-a-global-encryption-standard/">Anthropic's Claude Mythos found a hidden flaw in HAWK before ...</a></li>
<li><a href="https://blog.computationalcomplexity.org/2004/06/impagliazzos-five-worlds.html">Computational Complexity: Impagliazzo's Five Worlds</a></li>

</ul>
</details>

**Tags**: `#cryptography`, `#post-quantum`, `#AI`, `#cryptanalysis`, `#public-key algorithms`

---

<a id="item-9"></a>
## [Vendor-agnostic ML inference on edge devices using ncnn Vulkan](https://www.reddit.com/r/MachineLearning/comments/1v9s4mz/vendoragnostic_ml_inference_on_production_edge/) ⭐️ 8.0/10

PostSlate achieved fast, cross-platform ML inference on edge devices by using ncnn's Vulkan backend, reducing inference times for ArcFace R50 from 30ms to 3ms and SCRFD from 25ms to 2.5ms on an NVIDIA 4070 GPU. This demonstrates a practical, vendor-agnostic solution for on-device ML without requiring CUDA or vendor-specific runtimes, enabling broader deployment across diverse GPU hardware. The speedup comes from GPU offloading via Vulkan, which has drivers pre-installed on most machines. The model size also reduced from 174MB (ONNX fp32) to 87MB (ncnn fp16 weight storage).

reddit · r/MachineLearning · /u/ppchaos · Jul 29, 10:22

**Background**: Vulkan is a cross-platform graphics and compute API that runs on many GPUs (NVIDIA, AMD, Intel, Apple). ncnn is a high-performance neural network inference framework optimized for mobile and edge devices, with a Vulkan backend for GPU acceleration. SCRFD is an efficient face detection model, and ArcFace is a face embedding model used for recognition.

<details><summary>References</summary>
<ul>
<li><a href="https://pypi.org/project/ncnn-vulkan/">ncnn-vulkan · PyPI</a></li>
<li><a href="https://www.insightface.ai/research/scrfd">InsightFace SCRFD Paper Explained: Efficient Face Detection</a></li>
<li><a href="https://github.com/chenggongliang/arcface">GitHub - chenggongliang/arcface</a></li>

</ul>
</details>

**Tags**: `#ML inference`, `#Vulkan`, `#edge devices`, `#ncnn`, `#cross-platform`

---

<a id="item-10"></a>
## [Report: Hugging Face Models Used to Generate Deepfake Nudes](https://www.theverge.com/ai-artificial-intelligence/971723/hugging-face-nudify-deepfake-undress-women-children) ⭐️ 8.0/10

A report from AI Forensics on July 28 reveals that Hugging Face's top nine image editing models, seven of which can easily strip clothes from women with simple prompts, are being widely exploited to create non-consensual deepfake pornography. A honeypot set by the researchers received over 1,000 requests in seven days, with 73% involving sexual content and nearly 7% targeting children. This finding underscores a critical failure in content moderation on a major AI platform, enabling widespread abuse including the creation of child sexual abuse material. It highlights the urgent need for stronger safeguards in open-source model hosting to prevent harm, especially as deepfake technology becomes more accessible. The researchers deployed a honeypot on Hugging Face to monitor activity, and found that the platform implements almost no guardrails despite its policy prohibiting non-consensual intimate content and child nudity. AI Forensics recommends adding prompt filtering and output scanning to prevent harmful image generation.

telegram · zaihuapd · Jul 29, 08:20

**Background**: Hugging Face is a popular platform for hosting and sharing machine learning models, including many open-source image generation models. Deepfakes are synthetic media created using AI techniques like GANs and diffusion models to realistically alter or generate images. A honeypot is a cybersecurity decoy used to attract and monitor malicious activity. The abuse of these models for non-consensual deepfakes has raised serious ethical and legal concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Deepfake">Deepfake - Wikipedia</a></li>
<li><a href="https://www.crowdstrike.com/en-us/cybersecurity-101/exposure-management/honeypots/">What is a Honeypot in Cybersecurity? | CrowdStrike</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#deepfake`, `#content moderation`, `#Hugging Face`, `#ethics`

---

<a id="item-11"></a>
## [China drafts anti-cyber violence law, targets AI-generated abuse](https://mp.weixin.qq.com/s/PrzKFhbwjgFEGBPADvFD6Q) ⭐️ 8.0/10

On July 29, 2026, China's Cyberspace Administration released a draft anti-cyber violence law for public comment, explicitly regulating AI-generated content used to commit cyber violence. This draft law is significant because it marks one of the first national-level attempts to explicitly address AI-powered cyber violence, potentially setting a global precedent for platform responsibility and AI governance. The draft consists of seven chapters and 60 articles, requiring platforms to establish monitoring mechanisms and introduce injunctions for personality rights violations; victims can claim mental distress damages.

telegram · zaihuapd · Jul 29, 10:59

**Background**: Cyber violence in China includes online harassment, defamation, and privacy breaches. AI tools like deepfakes and automated bot armies have amplified such abuse. The draft law builds on earlier regulations such as the AI Content Identification Regulation (effective September 2023) and aims to create a coordinated government governance system.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aibase.com/news/20943">New AI Content Regulations Take Effect on September 1st!</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#cyber violence`, `#internet governance`, `#China law`, `#draft law`

---