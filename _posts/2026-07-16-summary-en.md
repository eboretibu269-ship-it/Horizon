---
layout: default
title: "Horizon Summary: 2026-07-16 (EN)"
date: 2026-07-16
lang: en
---

> From 33 items, 11 important content pieces were selected

---

1. [xAI open-sources Grok Build after privacy backlash](#item-1) ⭐️ 9.0/10
2. [Claude web_fetch Flaw Allows Memory Exfiltration](#item-2) ⭐️ 9.0/10
3. [xAI sues user for generating child abuse deepfakes with Grok](#item-3) ⭐️ 9.0/10
4. [Inkling: Largest Open-Weight Audio Model Released](#item-4) ⭐️ 8.0/10
5. [Running Gemma 4 26B on 13-Year-Old CPU at 5 tok/s](#item-5) ⭐️ 8.0/10
6. [Disentangling Convolutional Neurons via Hadamard Product Clustering](#item-6) ⭐️ 8.0/10
7. [170x slowdown on T4 vs A100 for PyTorch model with 4D correlations](#item-7) ⭐️ 8.0/10
8. [Google to Host Third-Party App Stores on Play from July 22](#item-8) ⭐️ 8.0/10
9. [DeepSeek Completes First Funding Round; Tencent Becomes Top External Shareholder](#item-9) ⭐️ 8.0/10
10. [Telegram Launches Serverless Platform for Bot Backends](#item-10) ⭐️ 8.0/10
11. [CXMT to match Micron DRAM capacity by 2026, China second largest producer](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [xAI open-sources Grok Build after privacy backlash](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 9.0/10

xAI open-sourced the entire Grok Build codebase under Apache 2.0 after a severe privacy bug in its Grok CLI tool was discovered to upload entire directories to Google Cloud storage, triggering community backlash. This incident underscores critical privacy risks in AI-powered developer tools and shows how open-sourcing can be a strategic move to restore user trust, setting a precedent for transparency in the AI coding assistant market. The Grok Build codebase contains 844,530 lines of Rust, with only about 3% vendored, and was released as a single commit, providing no development history. The repository includes a self-contained Mermaid diagram terminal renderer and tool implementations inspired by other coding agents.

rss · Simon Willison · Jul 15, 23:59

**Background**: The Grok CLI is a command-line tool that leverages xAI's Grok 4 model to assist developers with coding tasks directly in the terminal. Prior to open-sourcing, the tool was closed-source and suffered a bug where running it in a directory would upload that entire directory to xAI's Google Cloud buckets, including sensitive files like SSH keys and password manager databases. This raised serious privacy concerns, prompting xAI to delete all retained user data and disable the upload feature.

<details><summary>References</summary>
<ul>
<li><a href="https://lalatenduswain.medium.com/automate-your-terminal-with-grok-cli-a-developers-guide-to-xai-s-ai-powered-tool-eb8e2b0460bf">Automate Your Terminal with Grok CLI: A Developer’s Guide... | Medium</a></li>
<li><a href="https://cloud.google.com/storage">Cloud Storage | Google Cloud</a></li>

</ul>
</details>

**Discussion**: Community members expressed mixed reactions: some praised the code quality and the model's performance (e.g., better than Opus 4.8), while others criticized the data exfiltration as unacceptable. Several forks appeared quickly, such as a privacy-oriented fork that stripped telemetry and blocked auto-updates, indicating a desire for a more trustworthy alternative. Some viewed the open-sourcing as a tactical move rather than a genuine commitment to privacy.

**Tags**: `#security`, `#open source`, `#AI`, `#CLI tool`, `#privacy`

---

<a id="item-2"></a>
## [Claude web_fetch Flaw Allows Memory Exfiltration](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 9.0/10

Security researcher Ayush Paul discovered a bypass in Anthropic's Claude web_fetch tool that allowed an attacker to exfiltrate private user data (memories) by crafting a honeypot website that tricked the AI into navigating a chain of URLs, extracting the user's name, city, and employer. This attack demonstrates a critical security risk in AI assistants that combine access to private user data with web browsing capabilities, undermining user trust and highlighting the need for stronger safeguards against prompt injection and data exfiltration. The vulnerability exploited the web_fetch tool's ability to follow links from fetched pages; Anthropic had already patched the hole by removing that ability before the disclosure, but declined to pay a bug bounty because they claimed to have internally identified it first.

rss · Simon Willison · Jul 15, 14:21

**Background**: Claude's web_fetch tool is designed to only fetch URLs explicitly provided by the user or returned from a companion web_search tool, preventing dynamic URL construction for exfiltration. The 'lethal trifecta' refers to the combination of processing untrusted input, having access to private data, and being able to exfiltrate data externally. In this attack, the attacker hosted a honeypot site that presented instructions to Claude to navigate to personalized URLs that leaked data.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Sep/10/claude-web-fetch-tool/">Claude API: Web fetch tool</a></li>
<li><a href="https://www.osohq.com/learn/lethal-trifecta-ai-agent-security">Understanding the Lethal Trifecta of AI Agents</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion expressed concerns about AI security and the difficulty of preventing such attacks, with some users debating whether Anthropic's bug bounty policy was fair and others suggesting broader mitigations like restricting web tool usage.

**Tags**: `#AI Security`, `#Vulnerability`, `#Data Exfiltration`, `#Claude`, `#Prompt Injection`

---

<a id="item-3"></a>
## [xAI sues user for generating child abuse deepfakes with Grok](https://www.reuters.com/legal/litigation/musks-xai-sues-grok-user-over-sexualized-deepfakes-2026-07-15/) ⭐️ 9.0/10

xAI filed a lawsuit against South Carolina man Terry Harwood, alleging he used its Grok AI chatbot to generate child sexual abuse material and non-consensual adult deepfakes, violating the terms of service. This is one of the first lawsuits by an AI company against a user for generating abusive deepfakes, setting a significant legal precedent for AI accountability and safety. xAI has suspended 52,222 accounts and reported 73,604 cases to the National Center for Missing & Exploited Children, leading to at least 244 arrests; the suit seeks damages and a permanent ban for Harwood.

telegram · zaihuapd · Jul 16, 01:45

**Background**: Grok is an AI chatbot developed by xAI, led by Elon Musk. Deepfakes are AI-generated synthetic media that can depict real people in false scenarios. This lawsuit highlights the misuse of generative AI for illegal content and the legal responsibilities of AI providers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Deepfake">Deepfake - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#deepfakes`, `#legal precedent`, `#child protection`, `#xAI`

---

<a id="item-4"></a>
## [Inkling: Largest Open-Weight Audio Model Released](https://thinkingmachines.ai/news/introducing-inkling/) ⭐️ 8.0/10

Thinking Machines Lab released Inkling, an open-weights multimodal model that supports audio and can be fine-tuned via its Tinker platform, claiming it as the largest open-weight audio model to date. This release advances open-weight AI for audio, enabling enterprises to customize models for specific tasks at lower cost, potentially democratizing access to advanced multimodal AI. Inkling is not the strongest overall model but excels as a base for customization due to its multimodal capabilities, efficient thinking, and availability for fine-tuning on Tinker. It supports audio input, which is rare for open-weight models.

hackernews · vimarsh6739 · Jul 15, 18:12 · [Discussion](https://news.ycombinator.com/item?id=48924912)

**Background**: An open-weight model means its core components are publicly released, allowing anyone to download, run, study, and modify it. Multimodal models integrate and process multiple types of data such as text, audio, and images, enabling a more holistic understanding. Inkling's release combines these aspects, offering an open-weight multimodal model with audio support.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our open-weights model - Thinking Machines Lab</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**Discussion**: Commenters expressed interest in Inkling's audio capabilities, with some sharing links for local execution. The business model of providing a strong base model for fine-tuning received praise, though some noted it lags behind frontier models in overall performance. One commenter expressed hope that open models will win in the long run.

**Tags**: `#open-weights`, `#multimodal`, `#AI`, `#machine learning`, `#audio`

---

<a id="item-5"></a>
## [Running Gemma 4 26B on 13-Year-Old CPU at 5 tok/s](https://www.neomindlabs.com/2026/06/08/running-gemma-4-26b-at-5-tokens-sec-on-a-13-year-old-xeon-with-no-gpu/) ⭐️ 8.0/10

A developer demonstrated inference of Google's Gemma 4 26B MoE model at 5 tokens per second using only a 13-year-old dual Xeon CPU, without any GPU acceleration. This demonstration shows that large language models can run on very old hardware, challenging the assumption that GPUs are necessary for local inference and potentially lowering the barrier for experimentation and privacy-sensitive applications. The Gemma 4 26B (A4B) model activates only 4B parameters per token, making it efficient for CPU inference. Achieving 5 tok/s on such old hardware likely required aggressive quantization (e.g., 4-bit) and optimized software.

hackernews · neomindryan · Jul 15, 15:34 · [Discussion](https://news.ycombinator.com/item?id=48922434)

**Background**: Large language models traditionally require GPUs due to their computational demands. However, techniques like mixture-of-experts (MoE), quantization, and CPU-optimized inference engines have made it possible to run models on CPUs, albeit slower. Gemma 4 is Google's latest open-weight model family, including multimodal capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://ollama.com/library/gemma4">gemma4</a></li>
<li><a href="https://insiderllm.com/guides/cpu-only-llms-what-actually-works/">CPU-Only LLMs: What Actually Works | InsiderLLM</a></li>
<li><a href="https://www.medoid.ai/blog/a-hands-on-walkthrough-on-model-quantization/">A Hands-On Walkthrough on Model Quantization - Medoid AI</a></li>

</ul>
</details>

**Discussion**: Commenters debated cost-efficiency, noting that cloud inference may be cheaper than local electricity costs for low-speed CPUs. Some shared experiences running other models at similar speeds on older hardware, and predictions were made that larger MoE models will soon run on consumer devices.

**Tags**: `#machine learning`, `#model optimization`, `#hardware`, `#inference`, `#cost analysis`

---

<a id="item-6"></a>
## [Disentangling Convolutional Neurons via Hadamard Product Clustering](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 8.0/10

A novel method uses the Hadamard product of a neuron's receptive field and its weights to cluster patterns detected by a single 1x1 convolutional neuron in InceptionV1, revealing clean monosemantic clusters such as cars, cats, and dogs. This work advances mechanistic interpretability by providing a finer-grained decomposition of convolutional neurons, helping researchers understand how vision models encode concepts. It also highlights how gradient descent deliberately silences low-activation patterns, offering insights into model behavior. The method clusters the element-wise product of the input receptive field and the neuron's weight vector, yielding multiple monosemantic clusters per neuron. Low-activation clusters (e.g., letters) show balanced positive and negative weights from dependent neurons, suggesting active suppression by gradient descent.

reddit · r/MachineLearning · /u/narang_27 · Jul 15, 06:59

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks by analyzing their internal structures, similar to understanding conventional software. The Hadamard product, or element-wise multiplication, is used here to compute what a neuron 'sees.' Monosemanticity refers to a neuron detecting a single, interpretable concept. Prior work on monosemanticity has focused on language models; this study extends it to convolutional neural networks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hadamard_product_(matrices)">Hadamard product (matrices) - Wikipedia</a></li>
<li><a href="https://transformer-circuits.pub/2024/scaling-monosemanticity/">Scaling Monosemanticity: Extracting Interpretable Features from Claude 3 Sonnet</a></li>

</ul>
</details>

**Discussion**: The Reddit post expresses disappointment that the community shows little interest in convolutional neuron interpretability, with the author noting they may shift focus to language models. No specific comments are provided, but the overall sentiment is one of limited engagement.

**Tags**: `#mechanistic interpretability`, `#convolutional neural networks`, `#neuron analysis`, `#monosemanticity`, `#interpretability`

---

<a id="item-7"></a>
## [170x slowdown on T4 vs A100 for PyTorch model with 4D correlations](https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/) ⭐️ 8.0/10

A user reports a 170x slowdown running a point-tracking model on an NVIDIA T4 GPU compared to an A100, using pure FP32 with 4D correlation volumes and transformers. This extreme performance gap highlights a critical non-obvious bottleneck that can trap ML practitioners migrating between GPU generations, likely due to memory bandwidth differences and the T4's lack of Tensor Cores for FP32 operations. The model achieves 99% GPU utilization on T4, ruling out underutilization, and the same slowdown appears on two independent T4 machines. The architecture involves building local 4D correlation volumes (dense matching between frames) followed by transformer layers.

reddit · r/MachineLearning · /u/Future-Structure-296 · Jul 15, 13:44

**Background**: 4D correlation volumes store similarity scores between all pairs of grid positions across two feature maps, enabling dense matching for tasks like optical flow and point tracking. The T4 GPU lacks Tensor Cores for FP32 (they only operate on FP16/INT8), while the A100 has dedicated FP32 Tensor Cores, and the A100 also offers much higher memory bandwidth (1.5 TB/s vs 300 GB/s), which is critical for correlation volume computations.

<details><summary>References</summary>
<ul>
<li><a href="https://discuss.pytorch.org/t/could-pytorch-provide-correlation-operator/84030">Could pytorch provide correlation operator? - vision - PyTorch Forums</a></li>
<li><a href="https://arxiv.org/html/2507.06233">AnthroTAP: Learning Point Tracking with Real-World Motion</a></li>

</ul>
</details>

**Tags**: `#PyTorch`, `#GPU performance`, `#A100`, `#T4`, `#hardware bottlenecks`

---

<a id="item-8"></a>
## [Google to Host Third-Party App Stores on Play from July 22](https://www.theverge.com/policy/965792/google-epic-withdraw-injunction-third-party-app-stores-coming-google-play) ⭐️ 8.0/10

Google and Epic Games have withdrawn a motion to modify the antitrust injunction, and Google will begin hosting third-party app stores in Google Play starting July 22, 2026. This marks a major shift in Google's app store policy due to antitrust litigation, potentially reshaping app distribution on Android and giving users more choice. Third-party app stores must pay an annual $5,000 security review fee, are restricted to the US, and must meet requirements including open access for developers and clear trust and safety policies.

telegram · zaihuapd · Jul 15, 11:15

**Background**: The change stems from the Epic Games v. Google antitrust case, where a court ordered Google to allow competing app stores on its platform. Google had initially appealed but later reached a settlement with Epic, leading to the upcoming implementation.

<details><summary>References</summary>
<ul>
<li><a href="https://9to5google.com/2026/07/15/google-play-store-third-party-android-app-store-changes-july/">Google opens the floodgates to third-party app stores on Android</a></li>
<li><a href="https://www.engadget.com/2215452/google-allow-third-party-app-stores-android-july-22/">Google Will Allow Third-Party App Stores On Android Next Week</a></li>
<li><a href="https://www.cnet.com/tech/google-play-third-party-app-stores-android/">Google Play Opens the Door to Third-Party App Stores... - CNET</a></li>

</ul>
</details>

**Tags**: `#Google Play`, `#Epic Games`, `#antitrust`, `#app stores`, `#Android`

---

<a id="item-9"></a>
## [DeepSeek Completes First Funding Round; Tencent Becomes Top External Shareholder](https://www.cls.cn/detail/2427193) ⭐️ 8.0/10

DeepSeek's affiliated company recently completed a business registration change, adding new investors including Tencent as the largest external shareholder. The company also announced that the full DeepSeek-V4 model will be released mid-month. This funding round marks DeepSeek's first external investment and signals strong backing from major Chinese tech firms, which could accelerate its AI development and competition with other large language model providers. The upcoming DeepSeek-V4 release may further disrupt the AI landscape with cost-effective, high-performance models. Tencent holds over 33% of the investment platform, making it the largest external shareholder; other investors include NIO, JD.com, IDG, and the National AI Industry Fund. DeepSeek has also launched large-scale recruitment for roles in agents, code intelligence, and computing infrastructure.

telegram · zaihuapd · Jul 15, 12:56

**Background**: DeepSeek is a Chinese AI company founded in July 2023 by Liang Wenfeng, owned by hedge fund High-Flyer. It gained attention for releasing cost-effective open-weight models like DeepSeek-R1, which rivaled GPT-4 at a fraction of the training cost. The company uses techniques like Mixture of Experts and weaker AI chips due to export restrictions, yet achieves competitive performance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>
<li><a href="https://www.deepseek.com/en/">DeepSeek</a></li>
<li><a href="https://api-docs.deepseek.com/news/news260424/">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>

</ul>
</details>

**Tags**: `#AI`, `#DeepSeek`, `#Funding`, `#Tencent`, `#Large Language Models`

---

<a id="item-10"></a>
## [Telegram Launches Serverless Platform for Bot Backends](https://core.telegram.org/bots/serverless) ⭐️ 8.0/10

Telegram has launched a serverless platform that allows developers to deploy bot and Mini App backend code directly on Telegram's infrastructure without managing their own servers. The platform uses a V8 sandbox for code execution and includes a built-in SQLite database. This simplifies bot development significantly, reducing operational overhead and potentially attracting more developers to the Telegram ecosystem. It also aligns with the industry trend toward serverless computing, making Telegram more competitive with platforms like Discord and Slack. Deployment is done via a single command 'npx tgcloud push' using standard JavaScript modules. The code runs in an isolated V8 sandbox close to the Bot API, and each bot has its own SQLite database built-in.

telegram · zaihuapd · Jul 15, 16:00

**Background**: Serverless computing allows developers to run code without provisioning or managing servers, with the cloud provider handling scaling and maintenance. Telegram's new platform uses V8 sandbox isolation, a technology known for executing untrusted JavaScript securely. This is similar to how Cloudflare Workers and other serverless platforms operate, but integrated directly with Telegram's bot ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://www.generative.inc/ai-agent-sandboxes-the-infrastructure-layer-every-builder-needs-to-understand">AI Agent Sandboxes: Infrastructure Guide 2026 | Generative, Inc.</a></li>
<li><a href="https://www.ftandy.dev/posts/system-design-liteweight-lambda">System Design Look Back - Serverless and Sandbox</a></li>

</ul>
</details>

**Tags**: `#Telegram`, `#Serverless`, `#机器人`, `#云平台`

---

<a id="item-11"></a>
## [CXMT to match Micron DRAM capacity by 2026, China second largest producer](https://www.tomshardware.com/pc-components/dram/cxmt-close-to-matching-microns-memory-capacity-in-2026-research-claims-would-put-china-on-track-to-become-worlds-second-largest-dram-producer) ⭐️ 8.0/10

Citrini Research predicts that CXMT will reach approximately 350,000 wafers per month of DRAM capacity by the end of 2026, close to Micron's 375,000 wafers per month, making China the world's second largest DRAM production base. This shift could reshape global DRAM supply dynamics, reducing reliance on Samsung, SK Hynix, and Micron, and potentially stabilizing prices. However, export controls on immersion DUV lithography equipment pose a significant bottleneck. If all planned expansions materialize (including from Swayzing, Jinhua, and XMC), China's total DRAM capacity could reach 600,000 wafers per month excluding foreign-owned plants. The MATCH Act could block advanced immersion DUV exports, hampering near-term growth.

telegram · zaihuapd · Jul 16, 02:30

**Background**: DRAM (Dynamic Random Access Memory) is a key memory chip used in computers, servers, and mobile devices. Immersion DUV lithography uses a liquid layer between the lens and wafer to achieve finer patterning, critical for advanced DRAM nodes. The MATCH Act is a US bill aimed at closing loopholes in semiconductor export controls to China.

<details><summary>References</summary>
<ul>
<li><a href="https://www.asml.com/en/products/duv-lithography-systems">DUV lithography systems | Products</a></li>
<li><a href="https://cryptobriefing.com/cxmt-us-export-control-challenges/">Changxin Memory Technologies faces US export control challenges...</a></li>
<li><a href="https://nltimes.nl/2026/06/24/dutch-government-irritated-us-plans-new-asml-export-restrictions">Dutch government irritated by U.S. plans for new ASML export...</a></li>

</ul>
</details>

**Tags**: `#DRAM`, `#semiconductor`, `#China`, `#memory manufacturing`, `#geopolitics`

---