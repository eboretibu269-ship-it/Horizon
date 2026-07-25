---
layout: default
title: "Horizon Summary: 2026-07-25 (EN)"
date: 2026-07-25
lang: en
---

> From 26 items, 11 important content pieces were selected

---

1. [vLLM v0.26.0 Released with Inkling Family and Performance Boosts](#item-1) ⭐️ 9.0/10
2. [Anthropic Releases Claude Opus 5 at Half the Cost of Fable 5](#item-2) ⭐️ 9.0/10
3. [SGLang v0.5.16: DSpark Decoding & Inkling Model Support](#item-3) ⭐️ 8.0/10
4. [Open-Weight AI Mirrors Kubernetes as Foundational Platform](#item-4) ⭐️ 8.0/10
5. [Android May Restrict On-Device ADB Usage](#item-5) ⭐️ 8.0/10
6. [Ruff v0.16.0 Enables 413 Default Lint Rules](#item-6) ⭐️ 8.0/10
7. [Can AMD Break CUDA Moat? Agentic Kernels & MI455X](#item-7) ⭐️ 8.0/10
8. [China's new tax rules require annual reporting and 20% tax on offshore trust assets and gains](#item-8) ⭐️ 8.0/10
9. [China Fines Ctrip Record 51.79 Billion Yuan for Antitrust](#item-9) ⭐️ 8.0/10
10. [Qualcomm Announces Price Hike Across All Products Starting Sept 1](#item-10) ⭐️ 8.0/10
11. [Microsoft to use TPM chip to block pirated Windows activation](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 Released with Inkling Family and Performance Boosts](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 has been released with 411 commits from 212 contributors, introducing support for the Inkling model family, performance enhancements for DeepSeek-V4, fp32 lm_head support, and a flexible attention backend that can be selected per KV-cache group. This release is significant because vLLM is a widely-used LLM inference library, and the new features improve flexibility, performance, and model support, benefiting the entire LLM serving ecosystem. Notable technical details include piecewise CUDA graph support for the Inkling model, specialized routing kernels for DeepSeek-V4, and the new 'head_dtype' parameter for fp32 lm_head. The attention backend can now be selected per KV-cache group, and sliding-window support is an explicit capability.

github · khluu · Jul 25, 10:38

**Background**: vLLM is an open-source library for high-throughput LLM inference, supporting various models and hardware. The Inkling model family is a new multimodal MoE model from Thinking Machines Lab with 975B total parameters. Piecewise CUDA graphs improve performance by splitting computation into pieces, and Hopper FA4 refers to FlashAttention-4 optimized for NVIDIA Hopper architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://docs.sglang.io/advanced_features/piecewise_cuda_graph.html">Piecewise CUDA Graph - SGLang Documentation</a></li>
<li><a href="https://arxiv.org/html/2603.05451v1">FlashAttention-4: Algorithm and Kernel Pipelining Co-Design for Asymmetric Hardware Scaling</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#vLLM`, `#deep learning`, `#model serving`, `#GPU optimization`

---

<a id="item-2"></a>
## [Anthropic Releases Claude Opus 5 at Half the Cost of Fable 5](https://simonwillison.net/2026/Jul/24/introducing-claude-opus-5/#atom-everything) ⭐️ 9.0/10

Anthropic has released Claude Opus 5, a new AI model that approaches the frontier intelligence of Claude Fable 5 while being priced at half the cost. It is currently leading the Artificial Analysis leaderboard, surpassing even Fable 5. This release offers near-frontier AI capabilities at a significantly reduced price, potentially democratizing access to advanced AI for more developers and businesses. It also demonstrates continued rapid progress in large language model development, intensifying competition among providers. Claude Opus 5 is priced the same as its predecessor Opus 4.8 and includes a fast mode at twice the base cost. It has improved cybersecurity vulnerability detection capabilities but has not been deliberately trained on exploitation tasks, making it safer.

rss · Simon Willison · Jul 24, 23:48

**Background**: Anthropic is a leading AI company known for its Claude series of large language models. Frontier intelligence refers to the most advanced AI capabilities, with Claude Fable 5 being Anthropic's previous top-tier model. The Artificial Analysis leaderboard ranks models based on performance across various benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/leaderboards/models">LLM Leaderboard - Comparison of AI models from OpenAI, Anthropic...</a></li>
<li><a href="https://huggingface.co/spaces/ArtificialAnalysis/LLM-Performance-Leaderboard">LLM Performance Leaderboard - a Hugging Face Space by...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#language models`, `#machine learning`

---

<a id="item-3"></a>
## [SGLang v0.5.16: DSpark Decoding & Inkling Model Support](https://github.com/sgl-project/sglang/releases/tag/v0.5.16) ⭐️ 8.0/10

SGLang v0.5.16 introduces DSpark, a confidence-scheduled speculative decoding algorithm, and adds support for the Inkling multimodal MoE model with 975B parameters and 1M-token context. The release also includes UnifiedRadixTree as the default cache structure, performance improvements for linear attention on Blackwell GPUs, and several model additions like LongCat 2.0. DSpark achieves 383.7 tok/s on DeepSeek-V4-Pro with acceptance length ~5, significantly boosting per-user generation throughput. Inkling's support enables serving a massive 975B multimodal MoE model with up to 71.7k tok/s input and 171.0 tok/s per-user decode, pushing the boundaries of open-weight model serving. DSpark uses semi-autoregressive block drafting with confidence-based verification window sizing, enabled via --speculative-algorithm DSPARK. Inkling mixes sliding-window, full attention, and Mamba2 linear attention with NVFP4 MoE, and is verified on Blackwell, H200, and AMD MI350X. The release also removes experimental QServe and FBGEMM FP8 quantization paths.

github · Qiaolin-Yu · Jul 25, 00:13

**Background**: Speculative decoding accelerates LLM inference by using a small draft model to generate multiple tokens that are then verified by the target model. DSpark improves on fixed-length draft methods by adaptively sizing the verification window based on the draft model's confidence. Inkling is a 975B-parameter multimodal MoE model developed by Thinking Machines Lab, featuring a 1M-token context and hybrid attention mechanisms including Mamba2 linear attention. Mamba2 is a state-space model that achieves linear-time sequence modeling, making it efficient for long contexts.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.05147">[2607.05147] DSpark: Confidence-Scheduled Speculative ...</a></li>
<li><a href="https://inkling-model.com/">Inkling Model: Architecture, Capabilities, Context & Access</a></li>
<li><a href="https://arxiv.org/abs/2312.00752">[2312.00752] Mamba: Linear-Time Sequence Modeling with Selective State Spaces</a></li>

</ul>
</details>

**Tags**: `#sglang`, `#speculative decoding`, `#LLM serving`, `#multimodal MoE`, `#performance optimization`

---

<a id="item-4"></a>
## [Open-Weight AI Mirrors Kubernetes as Foundational Platform](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

The article argues that open-weight AI models are poised to become a foundational platform akin to Kubernetes, driving widespread adoption and collaborative innovation in the AI industry. This shift could democratize AI development, reduce dependency on closed models, and foster a collaborative ecosystem similar to what Kubernetes did for cloud computing, enabling startups and enterprises to build on shared, open-weight models. Open-weight models provide access to the model's weights but not necessarily full training data or code, differing from fully open-source models. The analogy highlights that like Kubernetes, open-weight AI can standardize and accelerate innovation while still allowing commercial use.

hackernews · tknaup · Jul 25, 14:49 · [Discussion](https://news.ycombinator.com/item?id=49048034)

**Background**: Kubernetes is an open-source container orchestration platform that became the industry standard for deploying and managing applications at scale. Similarly, open-weight AI models release the trained neural network weights, enabling others to fine-tune, host, and build upon them without needing to retrain from scratch. This approach lowers the barrier to entry and promotes collaboration, though it is distinct from fully open-source AI which also includes training code and data.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open-weight AI : what if we finally opened the bonnet ?</a></li>
<li><a href="https://openai.com/index/introducing-gpt-oss/">Introducing gpt-oss | OpenAI</a></li>

</ul>
</details>

**Discussion**: Community commenters debated the feasibility of banning Chinese AI models by origin, noting that weights are just numbers and impossible to trace geographically. Others discussed the volatile pricing of closed models like GPT-4 and suggested open-weight models provide a stable baseline. There was also support for collaborative model development akin to Linux, with calls for more frequent updates from labs like OpenAI.

**Tags**: `#open-weight AI`, `#Kubernetes`, `#AI models`, `#open source`, `#AI industry`

---

<a id="item-5"></a>
## [Android May Restrict On-Device ADB Usage](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

Android may implement restrictions on on-device ADB (Android Debug Bridge) usage, potentially limiting its availability or requiring authentication, based on a feature request discussion. This change could significantly impact developers and power users who rely on ADB for debugging and customization, while improving security for the broader user base. It reignites the debate between security and developer freedom. The proposed restriction appears to target remote ADB over Wi-Fi, requiring users to enable developer options and remote debugging. The community is divided on whether the security benefits outweigh the usability costs.

hackernews · shscs911 · Jul 25, 06:57 · [Discussion](https://news.ycombinator.com/item?id=49045159)

**Background**: ADB is a command-line tool that allows developers to communicate with Android devices for debugging, installation, and shell access. On-device ADB over Wi-Fi enables wireless debugging but can expose devices to network attacks if left enabled. Google has historically tightened security around developer features.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>
<li><a href="https://www.howtogeek.com/125769/how-to-install-and-use-abd-the-android-debug-bridge-utility/">How to Install and Use ADB, the Android Debug Bridge Utility</a></li>
<li><a href="https://xdaforums.com/t/q-adb-over-wifi-security.1452999/">[Q] adb over wifi ... security | XDA Forums</a></li>

</ul>
</details>

**Discussion**: Comments show mixed reactions. Some argue the attack vector is minimal since it requires both developer options and remote ADB enabled. Others see it as a step towards further restricting user control. A few developers propose more nuanced solutions like IP whitelisting.

**Tags**: `#Android`, `#ADB`, `#Security`, `#Developer Tools`

---

<a id="item-6"></a>
## [Ruff v0.16.0 Enables 413 Default Lint Rules](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0, released on July 23, 2026, increased the default number of enabled lint rules from 59 to 413, a 7x expansion that catches many previously undetected issues including syntax errors and runtime bugs. This major default rule expansion causes widespread CI failures for projects without pinned Ruff versions, forcing developers to adapt their codebases. It significantly strengthens Python code quality standards across the ecosystem, especially as Ruff's adoption continues to grow. The update brings 968 total rules (up from 708 in v0.1.0), and the new defaults include rules from categories like B (bugbear), UP (pyupgrade), and RUF (Ruff-specific). The `ruff check . --fix --unsafe-fixes` command can automatically fix many issues, as demonstrated by fixing 1538 out of 1618 errors in sqlite-utils.

rss · Simon Willison · Jul 25, 22:44

**Background**: Ruff is an extremely fast Python linter and code formatter written in Rust, designed to replace tools like Flake8, Black, and isort. It has gained popularity for its speed (10-100x faster than existing linters) and its ability to bundle multiple tools into a single binary. The Astral company behind Ruff was recently acquired by OpenAI.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff">GitHub - astral-sh/ruff: An extremely fast Python linter and code formatter, written in Rust. · GitHub</a></li>
<li><a href="https://pydevtools.com/blog/ruff-0-16-0-default-rules/">Ruff 0.16.0 Enables 7x More Rules by Default | pydevtools</a></li>
<li><a href="https://docs.astral.sh/ruff/rules/">Rules | Ruff</a></li>

</ul>
</details>

**Tags**: `#Python`, `#linting`, `#tooling`, `#version release`

---

<a id="item-7"></a>
## [Can AMD Break CUDA Moat? Agentic Kernels & MI455X](https://newsletter.semianalysis.com/p/can-amd-break-the-cuda-moat-amd-advancing) ⭐️ 8.0/10

A Semianalysis report examines AMD's strategy to break Nvidia's CUDA dominance through agentic kernel generation and the new Instinct MI455X GPU, while detailing severe production challenges and up to 105% financial discounts. If AMD overcomes its software and production hurdles, it could offer a viable alternative to Nvidia's CUDA ecosystem, reducing lock-in for AI developers and potentially lowering costs. The MI455X is a 2nm GPU with 432GB of HBM4 memory, and AMD's 'agentic kernel generation' uses LLMs to automatically optimize CUDA-compatible kernels, but internal development clusters remain unstable and production ramp is described as 'hell'.

rss · Semianalysis · Jul 25, 00:33

**Background**: CUDA is Nvidia's proprietary parallel computing platform that creates a 'moat' by locking developers into their hardware. AMD's open-source ROCm platform aims to compete but has historically lagged in software maturity. Agentic kernel generation, as demonstrated by projects like CUDA Agent, uses reinforcement learning to automatically generate and optimize high-performance kernels, potentially easing the transition from CUDA to AMD hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/can-amd-break-the-cuda-moat-amd-advancing">Can AMD break the CUDA Moat? AMD Advancing AI 2026</a></li>
<li><a href="https://www.phoronix.com/news/AMD-Instinct-MI455X-Helios">AMD Launches Instinct MI455X, Helios AI Rack - Phoronix</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/amd-takes-the-wraps-off-its-instinct-mi455x-ai-accelerator-cdna-5-and-helios-rack-scale-architecture-combine-to-take-the-fight-to-nvidia-in-the-data-center">AMD takes the wraps off its Instinct MI455X AI accelerator — CDNA 5 and Helios rack-scale architecture combine to take the fight to Nvidia in the data center | Tom's Hardware</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#CUDA`, `#GPU computing`, `#AI hardware`, `#machine learning`

---

<a id="item-8"></a>
## [China's new tax rules require annual reporting and 20% tax on offshore trust assets and gains](https://liaoning.chinatax.gov.cn/art/2026/7/24/art_5869_7823.html) ⭐️ 8.0/10

On July 24, 2026, China's Ministry of Finance and State Taxation Administration jointly issued Announcement No. 21, requiring resident individuals to report and pay personal income tax on assets transferred into offshore trusts and on trust gains (whether distributed or not) at a flat 20% rate. This regulation closes long-standing tax avoidance loopholes used by wealthy Chinese individuals to defer or avoid taxes through offshore trusts, significantly impacting cross-border wealth planning and compliance obligations for high-net-worth individuals. The 20% tax applies to the net appreciation (current value minus original value and costs) upon asset transfer into the trust, annual trust gains, and liquidation gains; a 90-day grace period allows taxpayers to voluntarily rectify unreported taxes from 2023–2025 without late payment penalties.

telegram · zaihuapd · Jul 25, 00:31

**Background**: Offshore trusts have been widely used by Chinese residents for asset protection and inheritance planning, but China's tax law has historically lacked clear rules on when and how to tax trust assets and gains. The new rules adopt a look-through approach, treating the trust as transparent for tax purposes, so all economic benefits are attributed to the settlor annually.

<details><summary>References</summary>
<ul>
<li><a href="https://yangxiang.blog.caixin.com/archives/286129">yangxiang.blog.caixin.com/archives/286129</a></li>
<li><a href="https://www.donews.com/news/detail/8/6645794.html">donews.com/news/detail/8/6645794.html</a></li>
<li><a href="https://www.workercn.cn/c/2026-07-25/8855325.shtml">政策解读·问答｜离岸信托需缴纳个人所得税 - 经济 - 中工网</a></li>

</ul>
</details>

**Tags**: `#tax regulation`, `#offshore trusts`, `#China`, `#personal finance`

---

<a id="item-9"></a>
## [China Fines Ctrip Record 51.79 Billion Yuan for Antitrust](https://www.xinhuanet.com/fortune/20260725/693124245aa44d2bbc7520b7a0c244ea/c.html) ⭐️ 8.0/10

On July 25, 2026, China's State Administration for Market Regulation fined Ctrip Group 51.79 billion yuan (16.58 billion yuan disgorgement plus 35.21 billion yuan fine) for abusing market dominance, and ordered corrective actions including refunding 122 million yuan to hotel operators and implementing 19 rectification measures. This is the largest antitrust fine ever imposed on a Chinese tech company, signaling intensified regulatory enforcement under China's updated antitrust regime. It sets a precedent for actions against other platform economy players and reshapes competition in online travel. The fine consists of 16.58 billion yuan in confiscated illegal gains and 35.21 billion yuan in penalties, totaling 51.79 billion yuan. Ctrip must stop exclusive cooperation agreements, remove 'lowest price' requirements, and overhaul its distribution model, including discontinuing the first-level commissioned distribution (special brand) model.

telegram · zaihuapd · Jul 25, 02:24

**Background**: China's Anti-Monopoly Law prohibits abuse of market dominance, such as forcing exclusive dealings or imposing unfair trading conditions. Ctrip, as the dominant online travel agency, was found to have forced hotels into exclusive arrangements and imposed 'lowest price' clauses, harming competition. The State Administration for Market Regulation has intensified antitrust enforcement, particularly targeting large platform companies.

**Tags**: `#antitrust`, `#regulation`, `#China`, `#Ctrip`, `#tech industry`

---

<a id="item-10"></a>
## [Qualcomm Announces Price Hike Across All Products Starting Sept 1](https://tw.news.yahoo.com/%E7%8D%A8%E5%AE%B6-%E9%AB%98%E9%80%9A%E6%BC%B2%E5%83%B9%E4%BF%A1%E6%9B%9D%E5%85%89-%E5%85%A8%E7%B7%9A%E7%94%A2%E5%93%819-1%E8%B5%B7%E8%AA%BF%E6%BC%B2-%E7%9B%B4%E8%A8%80-142730846.html) ⭐️ 8.0/10

On July 24, 2026, Qualcomm sent a price adjustment notice to customers, announcing that all products shipped on or after September 1, 2026, will see price increases. The company cited rising costs in wafer fabrication, packaging, and substrate materials, as well as surging AI and data center demand squeezing supply chain capacity. This price hike affects Qualcomm's wide range of chips used in smartphones, PCs, IoT, and automotive sectors, potentially raising consumer electronics prices or reducing features. It signals a structural shift in semiconductor industry costs driven by AI demand and advanced packaging costs. Qualcomm did not specify a uniform percentage or list specific product models, stating that account managers would contact customers individually with new quotes. Some orders already placed but scheduled for shipment after September 1 may also be repriced.

telegram · zaihuapd · Jul 25, 03:01

**Background**: Advanced packaging techniques like TSMC's CoWoS and Intel's EMIB are increasingly used to integrate multiple dies, improving performance without relying solely on transistor scaling. These processes, along with rising substrate material costs, add to semiconductor manufacturing expenses. Qualcomm's dominance in mobile and automotive chips makes its pricing decisions influential across the industry.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Advanced_packaging_(semiconductors)">Advanced packaging (semiconductors)</a></li>
<li><a href="https://www.trendforce.com/news/2025/12/01/news-gold-and-ccl-price-surge-pressures-substrate-makers-driving-shift-toward-high-value-ai-products/">[News] Gold and CCL Price Surge Squeezes Substrate Makers as ...</a></li>

</ul>
</details>

**Tags**: `#Qualcomm`, `#price increase`, `#chip shortage`, `#AI demand`, `#semiconductor industry`

---

<a id="item-11"></a>
## [Microsoft to use TPM chip to block pirated Windows activation](https://www.techspot.com/news/113232-microsoft-using-tpm-chips-crack-down-pirated-windows.html) ⭐️ 8.0/10

Microsoft announced it will add TPM-based hardware attestation to its Key Management Services (KMS) activation, requiring KMS servers to prove their hardware identity is Microsoft-certified and untampered before processing bulk activation requests. The change will be mandatory starting with the next Windows Server release and will deliver readiness prompts from August 2026 on Windows Server 2025. This anti-piracy measure targets the widely abused KMS-based activation exploits used by pirated Windows copies, potentially rendering common tools like Online KMS ineffective. It represents a significant hardening of enterprise activation workflows and could shift the cat-and-mouse game between Microsoft and activation bypass developers. Microsoft already blocked the KMS38 exploit in 2025, and the new TPM attestation is expected to break the Online KMS method that requires periodic reconnection to a fake server. However, the Massgrave group has already released TSforge, which claims to bypass the entire Microsoft DRM activation architecture, making the outcome of this arms race uncertain.

telegram · zaihuapd · Jul 25, 15:55

**Background**: KMS (Key Management Services) is a volume activation method used by enterprises to activate multiple Windows and Office clients on their network using a local KMS host. TPM (Trusted Platform Module) is a hardware security chip that can provide cryptographic attestation of a system's identity. Pirated Windows activations have long exploited fake KMS servers to bypass licensing, and Microsoft has been gradually hardening activation against these attacks.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/windows-server/get-started/kms-client-activation-keys">Key Management Services (KMS) client activation... | Microsoft Learn</a></li>
<li><a href="https://massgrave.dev/">Microsoft Activation Scripts | MAS</a></li>
<li><a href="https://github.com/massgravel/TSforge">GitHub - massgravel/TSforge: A collection of activation/evaluation...</a></li>

</ul>
</details>

**Tags**: `#Windows`, `#TPM`, `#Anti-piracy`, `#KMS`, `#Software licensing`

---