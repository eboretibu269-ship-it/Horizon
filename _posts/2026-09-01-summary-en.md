---
layout: default
title: "Horizon Summary: 2026-09-01 (EN)"
date: 2026-09-01
lang: en
---

> From 37 items, 6 important content pieces were selected

---

1. [Tim Cook Steps Down, John Ternus Becomes Apple CEO to Lead AI Push](#item-1) ⭐️ 9.0/10
2. [Google Pulls Manifest V2 Extensions, Including uBlock Origin, from Chrome Web Store](#item-2) ⭐️ 8.0/10
3. [NAT as the Original Sin of Internet Centralization](#item-3) ⭐️ 8.0/10
4. [Sliding-Window Attention Beats Linear on Long-Context Reasoning](#item-4) ⭐️ 8.0/10
5. [SynthFin-AML: New Benchmark Exposes Temporal Leakage in GNNs](#item-5) ⭐️ 8.0/10
6. [DeepSeek releases V4-Flash-Vision-Exp, first multimodal V4 model](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Tim Cook Steps Down, John Ternus Becomes Apple CEO to Lead AI Push](https://www.bloomberg.com/news/articles/2026-08-30/apple-s-new-ceo-john-ternus-takes-reins-from-tim-cook-focusing-on-ai) ⭐️ 9.0/10

Tim Cook officially stepped down as Apple CEO on August 31, 2026, with John Ternus taking over on September 1 and Cook remaining as executive chairman. Ternus's top priority is accelerating Apple's AI efforts, including fixing delayed Siri upgrades, ahead of the September 9 event where the first foldable iPhone is expected to debut. This leadership transition marks a generational shift at one of the world's most influential technology companies, signaling Apple's strategic pivot toward AI. The new CEO's focus and the upcoming foldable iPhone launch will shape Apple's competitive position against rivals such as Samsung and Google. Ternus, a 51-year-old hardware engineering veteran, has led hardware design since 2021 and was instrumental in the development of Apple silicon Macs. The first foldable iPhone is reported to feature 12 GB RAM and deep Siri AI integration, understanding real-world scenes through screen, calendar, and camera context.

telegram · zaihuapd · Aug 31, 10:21

**Background**: Apple Intelligence, introduced in June 2024, is Apple's suite of AI features combining on-device and server processing, available on iOS 18, iPadOS 18, and macOS Sequoia, and supported on devices with Apple silicon or newer iPhones. John Ternus previously served as Apple's senior vice president of Hardware Engineering, overseeing design and development of products such as the Mac, iPad, and iPhone.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/John_Ternus">John Ternus</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#CEO transition`, `#AI`, `#Tim Cook`, `#John Ternus`

---

<a id="item-2"></a>
## [Google Pulls Manifest V2 Extensions, Including uBlock Origin, from Chrome Web Store](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

Google has enforced its Manifest V3 migration by removing all Manifest V2 extensions from the Chrome Web Store, including popular privacy and ad-blocking tools like uBlock Origin. This removal makes it much harder for users to install these extensions on Chrome. This marks the end of an era for Chrome extensions, forcing users of privacy tools to switch to alternatives like Firefox or accept the less capable uBlock Origin Lite. It also raises concerns about a single company controlling how users block ads and protect their privacy. Manifest V3 replaces the older extension APIs that allowed deep, dynamic network interception with a more limited declarativeNetRequest model, which removed capabilities uBlock Origin relied on. The full uBlock Origin still works in Firefox, which continues to support the more permissive WebExtensions API.

hackernews · twapi · Aug 31, 21:10 · [Discussion](https://news.ycombinator.com/item?id=49514878)

**Background**: Chrome extensions are built on a set of capabilities defined by a manifest version. Manifest V2 (MV2) has been the standard for years, but Google introduced Manifest V3 (MV3) in 2020 to improve privacy, security, and performance. By 2025, MV2 was effectively phased out for most Chrome users, and the Chrome Web Store has now removed MV2 extensions entirely. Ad blockers like uBlock Origin are affected because MV3 restricts the ability to block network requests in the flexible ways MV2 allowed.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V3 | Chrome for Developers</a></li>
<li><a href="https://www.pcworld.com/article/3160794/the-last-lifeline-for-ublock-origin-in-chrome-is-almost-gone-for-good.html">The last lifeline for uBlock Origin in Chrome is almost gone for good | PCWorld</a></li>
<li><a href="https://factually.co/fact-checks/technology/manifest-v3-impact-ublock-origin-chromium-blocking-workarounds-4c8757">How Does Manifest V3 Change What uBlock Origin Can Blo...</a></li>

</ul>
</details>

**Discussion**: Commenters on the news item are overwhelmingly critical of Google's decision. Many recommend switching to Firefox, noting that uBlock Origin always worked best there, while others express resentment toward Google's control over the web and say they will keep using Firefox or its forks even if the browser's market share shrinks. Some highlight that ad blocking is now a safety issue, especially for less tech-savvy users who may fall for malicious ads.

**Tags**: `#Chrome`, `#Manifest V3`, `#ad blocking`, `#privacy`, `#web extensions`

---

<a id="item-3"></a>
## [NAT as the Original Sin of Internet Centralization](https://dreamstation.systems/personal/ntppost.html) ⭐️ 8.0/10

An essay argues that NAT, not just later developments, was a foundational cause of internet centralization, eroding self-hosting and normalizing the client-server model. It reframes address scarcity as a key force that shaped how people perceive the internet. This reframes the narrative of internet centralization by shifting responsibility to an early technical artifact that most users do not even know about. It matters to anyone concerned with self-hosting, net neutrality, and the power balance between users and large cloud platforms. The author calls NAT the original sin and notes that it trained people to see client-server as natural, when that was an artifact of IPv4 address scarcity. The essay also suggests that running a server used to be trivial before NAT became ubiquitous.

hackernews · robinpie · Aug 31, 02:23 · [Discussion](https://news.ycombinator.com/item?id=49504905)

**Background**: NAT (Network Address Translation) maps multiple private IP addresses to a single public IP address, allowing many devices to share one public address, and was widely adopted to conserve limited IPv4 addresses. The client-server model is a computing architecture where clients request resources from centralized servers, as opposed to peer-to-peer or self-hosted setups where each node can act as both provider and consumer.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Network_address_translation">Network address translation - Wikipedia</a></li>
<li><a href="https://www.cisco.com/site/us/en/learn/topics/networking/what-is-network-address-translation-nat.html">What Is Network Address Translation (NAT)? - Cisco</a></li>
<li><a href="https://www.geeksforgeeks.org/system-design/client-server-architecture-system-design/">Client-Server Architecture - System Design - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: Commenters are divided. RustyRussell, the Linux NAT implementer, apologizes for the current NAT system, admitting it eroded the ability to have public endpoints. Others argue that NAT is not the original sin, noting that Carrier Grade NAT is the real problem while regular NAT is manageable and protected many insecure devices from exposure.

**Tags**: `#NAT`, `#networking`, `#internet architecture`, `#centralization`, `#history`

---

<a id="item-4"></a>
## [Sliding-Window Attention Beats Linear on Long-Context Reasoning](https://www.reddit.com/r/MachineLearning/comments/1w3j1vw/slidingwindow_attention_beats_linear_on/) ⭐️ 8.0/10

A new arXiv preprint (2608.28444) reports that sliding-window attention with attention sinks achieves 2 to 10 times higher performance than linear attention on Needle-in-a-Haystack and BABILong long-context reasoning benchmarks. The authors argue that the post-training-to-linear pipeline has not been properly compared to simpler baselines and recommend switching to SWA. This challenges the recent industry direction of investing post-training compute to convert LLMs to linear attention for efficiency. If SWA matches or beats these models without any post-training, it could shift focus back to simpler, cheaper baselines and reshape long-context LLM design. The gap is reported as massive: SWA performance is 2 to 10 times higher than linear attention on the selected benchmarks, which include Needle-in-a-Haystack and BABILong. The authors concede that linear attention 'may have shown some promise, but they likely require to be trained from scratch or extensive post-training in order to even match SWA.' The paper's recommendation is to switch to SWA instead of post-training linear models.

reddit · r/MachineLearning · /u/Justgototheeffinmoon · Aug 31, 16:35

**Background**: Standard Transformer attention has quadratic cost with sequence length, making long-context inference memory- and compute-intensive. Linear attention variants attempt to reduce this to linear complexity through kernel approximations or recurrent formulations, but often require post-training to adapt existing LLMs. Sliding-window attention (SWA) restricts each token's attention to a fixed local window, which also achieves linear scaling in a simple way, and adding 'attention sinks' helps stabilize it. BABILong is a long-context reasoning benchmark that probes models' ability to reason over distributed facts in very long documents.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.28444">[2608.28444] Sliding-window beats linear attention - arXiv.org</a></li>
<li><a href="https://arxiv.org/abs/2406.10149">[2406.10149] BABILong: Testing the Limits of LLMs with Long ...BABILong: Testing the Limits of LLMs with Long Context ...BABILong Benchmark - emergentmind.comRMT-team/babilong · Datasets at Hugging FaceBABILong Benchmark Scores & AI Model Leaderboard | BenchmarkListCogniFold/benchmarks/babilong/README.md at main - GitHub</a></li>
<li><a href="https://www.digitalocean.com/community/tutorials/sliding-window-attention-efficient-long-context-models">Sliding Window Attention: Efficient Long-Context Modeling | DigitalOcean</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#attention mechanisms`, `#long-context reasoning`, `#linear attention`, `#LLM efficiency`

---

<a id="item-5"></a>
## [SynthFin-AML: New Benchmark Exposes Temporal Leakage in GNNs](https://www.reddit.com/r/MachineLearning/comments/1w3imxy/your_gnn_is_probably_just_an_overcomplicated_mlp/) ⭐️ 8.0/10

The authors release SynthFin-AML v10.0, a 100k-node, 1.2M-edge synthetic benchmark that enforces strict causal boundaries in dynamic graph evaluation. They show that standard transductive random splits leak future edges into GNN training, and propose a 3-snapshot point-in-time split to fix this issue. This addresses a critical evaluation flaw in dynamic graph research, where models can cheat by seeing future information, inflating reported performance. The benchmark, submitted to PyTorch Geometric, could become a standard for causal evaluation and help the AML community reliably compare GNNs against simpler baselines. The 3-snapshot architecture uses train graph edges up to Day 7, validation up to Day 8, and test up to Day 10, physically bounding the GNN's receptive field. The authors also eliminated the 'amount split cheat' by making fraud and retail transaction amounts follow the same lognormal distribution (μ=8.517, σ=0.8).

reddit · r/MachineLearning · /u/Glabmayt2075 · Aug 31, 16:21

**Background**: Dynamic graphs model evolving relationships, such as financial transaction networks where edges appear over time. GNNs compute node embeddings by aggregating neighbor information; if training uses a static snapshot containing future edges, the model can access information unavailable at prediction time. This temporal leakage inflates performance, and standard random splits are particularly problematic for financial transaction graphs. SynthFin-AML is a synthetic benchmark designed to prevent such leakage; it follows the spirit of earlier synthetic AML datasets like SynthAML, which was built on real bank data.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nature.com/articles/s41597-023-02569-2">A synthetic data set to benchmark anti-money laundering methods | Scientific Data</a></li>
<li><a href="https://arxiv.org/html/2509.23631v2">Leakage-Free Evaluation and Distribution-Robust Spatio-Temporal Graph ...</a></li>
<li><a href="https://deepwiki.com/2024SIG/SIG/7.3-data-leakage-prevention">Data Leakage Prevention | 2024SIG/SIG | DeepWiki</a></li>

</ul>
</details>

**Tags**: `#graph neural networks`, `#temporal leakage`, `#anti-money laundering`, `#benchmark`, `#causality`

---

<a id="item-6"></a>
## [DeepSeek releases V4-Flash-Vision-Exp, first multimodal V4 model](https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-Vision-Exp) ⭐️ 8.0/10

DeepSeek has released DeepSeek-V4-Flash-Vision-Exp, an experimental multimodal variant of its V4-Flash model that adds a vision module through continued training. On the ApexBench multimodal agent benchmark, it improves from 26.2 to 36.5 compared to V4-Flash-0731, while text agent performance remains roughly unchanged. This is DeepSeek's first V4-generation multimodal model, and the large jump on ApexBench signals a significant improvement in multimodal agent capabilities. It strengthens DeepSeek's position in the competitive open-weight LLM landscape and provides a strong baseline for agentic AI development. The model builds on the V4-Flash-0731 architecture with an added vision module and continued training. It shows a 10.3-point gain on ApexBench (from 26.2 to 36.5) for multimodal agent tasks, while text agent performance stays approximately flat, indicating training was well-targeted.

telegram · zaihuapd · Aug 31, 11:41

**Background**: Multimodal models combine text and visual understanding, enabling agents to perceive images, screenshots, or UI layouts while reasoning and acting. Benchmarks like ApexBench evaluate AI agents on long-horizon, real-world-style tasks such as poster editing, code refactoring, and knowledge-work scenarios, making them relevant for agentic AI systems. DeepSeek's V4 series is the latest generation of its open-weight models, and this experimental release adds vision capabilities to the existing V4-Flash line.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/apex-bench">APEX-Bench: High-Fidelity Benchmarking</a></li>
<li><a href="https://www.mercor.com/apex/">APEX Benchmarks: AI Productivity Index Leaderboards | Mercor</a></li>
<li><a href="https://link.springer.com/article/10.1007/s11390-025-4802-8">Multimodal Agent AI: A Survey of Recent Advances and Future ...</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#multimodal`, `#model release`, `#AI`, `#LLM`

---