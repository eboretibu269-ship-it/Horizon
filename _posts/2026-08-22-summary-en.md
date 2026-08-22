---
layout: default
title: "Horizon Summary: 2026-08-22 (EN)"
date: 2026-08-22
lang: en
---

> From 29 items, 4 important content pieces were selected

---

1. [SGLang v0.5.18 Released with 710 PRs and New Model Support](#item-1) ⭐️ 8.0/10
2. [New MCP Roadmap Prioritizes HTTP, Agent Identity, and Sampling Removal.](#item-2) ⭐️ 8.0/10
3. [Trained from Scratch 250M LLM Fits in 60MB with Sub-2-Bit Quantization](#item-3) ⭐️ 8.0/10
4. [SemiAnalysis: Open Models Narrow Gap Twice as Fast Each Generation](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.18 Released with 710 PRs and New Model Support](https://github.com/sgl-project/sglang/releases/tag/v0.5.18) ⭐️ 8.0/10

SGLang v0.5.18 was released with 710 pull requests from 212 contributors. The release adds support for new autoregressive models (Muse Glimmer, Intern-S2-Mobius) and diffusion models (SANA-Video, LingBot-Video-MoE, LTX-2.5, Cosmos3 Edge & Distilled, LongCat-Image). This release is significant because SGLang is a widely adopted open-source LLM inference framework, and the high volume of contributions reflects strong community momentum. New model support and performance optimizations will benefit developers deploying both autoregressive and diffusion models in production. Performance improvements include overlapped checkpoint staging that speeds Qwen3-32B startup by up to 2.38x on H100, TP LMHead with all-to-all that reduces LMHead time from 320us to 169us on DeepSeek-V4-Pro, and FlashInfer MNNVL pure allreduce that improves decode performance up to 6.9% on Blackwell. The release also unifies compiled-kernel caches under SGLANG_CACHE_DIR and updates dependencies to torch 2.13.0, triton 3.7.1, flashinfer 0.6.17, and sgl-kernel 0.4.6.post1.

github · Fridge003 · Aug 22, 00:09

**Background**: SGLang is an open-source inference framework designed for fast serving of large language and multimodal models. It supports both autoregressive models and diffusion models (e.g., video generation), and uses techniques like CUDA graphs, tensor parallelism, and FlashInfer kernels to optimize throughput and latency. The models added in this release, such as Meta's Muse Glimmer and Intern-S2-Mobius, represent the latest developments in open-weight multimodal and reasoning-optimized models.

<details><summary>References</summary>
<ul>
<li><a href="https://research.meta.ai/blog/introducing-muse-glimmer-open-agentic-model">Introducing Muse Glimmer: An Open Agentic Model That Runs on ...</a></li>
<li><a href="https://huggingface.co/internlm/Intern-S2-Mobius">internlm/Intern-S2-Mobius · Hugging Face</a></li>
<li><a href="https://huggingface.co/Efficient-Large-Model/SANA-Video_2B_480p">Efficient-Large-Model/SANA-Video_2B_480p · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#sglang`, `#open source`, `#release`, `#AI infrastructure`

---

<a id="item-2"></a>
## [New MCP Roadmap Prioritizes HTTP, Agent Identity, and Sampling Removal.](https://blog.modelcontextprotocol.io/posts/mcp-roadmap/) ⭐️ 8.0/10

Anthropic's new MCP roadmap makes remote servers standard HTTP workloads, standardizes agent identity and authorization, and removes the sampling feature, with changes targeting the 2026-07-28 release. This roadmap shapes the future of AI tool interoperability, directly affecting developers building agents and integrations. The shifts address real-world needs for agent identity and simpler HTTP-based deployment, but the removal of sampling may limit certain agentic patterns. The roadmap targets the 2026-07-28 release, making remote MCP servers behave like any other HTTP workload. It also proposes standardized agent identity and authorization built on existing standards, while deprecating the sampling feature that let servers request LLM completions through clients.

hackernews · pentagrama · Aug 22, 13:31 · [Discussion](https://news.ycombinator.com/item?id=49399591)

**Background**: MCP (Model Context Protocol) is an open standard introduced by Anthropic in November 2024 to connect AI assistants to external tools and data sources. It allows applications like Claude or ChatGPT to interact with data repositories, business tools, and development environments. Sampling was a feature that enabled servers to request LLM completions through the client, supporting agentic behaviors. MCP authorization has traditionally relied on a person approving access in a browser, but agent workloads need standardized identity and delegation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://modelcontextprotocol.io/docs/2026-07-28/getting-started/intro">What is the Model Context Protocol (MCP)? - Model Context Protocol</a></li>
<li><a href="https://modelcontextprotocol.io/specification/2025-06-18/client/sampling">Sampling - Model Context Protocol</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some developers welcome the move to standard HTTP and agent identity, while others question whether MCP endpoints are truly easier than REST plus a skills.md file. Several commenters regret the removal of sampling, and one cybersecurity developer says the constant pivots and complexity burned them on MCP, so they now prefer local tools and APIs.

**Tags**: `#MCP`, `#AI protocols`, `#developer tools`, `#API design`, `#agent interoperability`

---

<a id="item-3"></a>
## [Trained from Scratch 250M LLM Fits in 60MB with Sub-2-Bit Quantization](https://www.reddit.com/r/MachineLearning/comments/1vv2nkh/i_developed_my_own_quantized_llm_from_scratch/) ⭐️ 8.0/10

A developer trained a 250M-parameter language model from scratch on 30B tokens of FineWeb, then quantized it below 2 bits per weight, shrinking the full deployment to 60 MB. The model runs at about 400 tokens per second on a laptop CPU and adds a disk-based compressed KV cache that allows retrieval from up to 100M tokens of history. This shows a practical path toward extremely compact, long-context LLMs that run on commodity hardware without a GPU, which could lower barriers for on-device and edge AI. The combination of sub-2-bit quantization and disk-backed memory is novel and may inspire further research in model compression and retrieval-augmented generation. Instead of a trainable embedding table, each of the 131k tokens is a fixed 512-bit code, and the most recent 2048 tokens stay in fp16 while older KV cache entries are compressed to about 320 bytes per token on disk. The base model reaches 23.3 perplexity on held-out English web text, and the repository includes a fine-tuning kit with master weights.

reddit · r/MachineLearning · /u/Final-Data-1410 · Aug 22, 04:39

**Background**: The KV cache stores intermediate key and value computations from earlier tokens so the model does not recompute them during autoregressive generation, which greatly speeds up inference. FineWeb is a 15-trillion-token open dataset derived from Common Crawl that often outperforms other public pretraining corpora. Extremely low-bit quantization — below about 3 bits — is an active research area, with methods like VPTQ aiming to compress large models without retraining while preserving accuracy.

<details><summary>References</summary>
<ul>
<li><a href="https://magazine.sebastianraschka.com/p/coding-the-kv-cache-in-llms">Understanding and Coding the KV Cache in LLMs from Scratch</a></li>
<li><a href="https://arxiv.org/abs/2406.17557">[2406.17557] The FineWeb Datasets: Decanting the Web for the ...GitHub - huggingface/fineweb-2The FineWeb Datasets: Decanting the Web for the Finest Text ...FineWeb (dataset)The FineWeb Datasets: Decanting the Web for the Finest Text ...</a></li>
<li><a href="https://github.com/microsoft/VPTQ">VPTQ: Extreme Low-bit Vector Post-Training Quantization for ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#long-context`, `#edge-deployment`, `#training-from-scratch`

---

<a id="item-4"></a>
## [SemiAnalysis: Open Models Narrow Gap Twice as Fast Each Generation](https://newsletter.semianalysis.com/p/are-open-models-catching-up) ⭐️ 8.0/10

SemiAnalysis reports that open-source models are closing the gap with closed-source leaders at an accelerating rate, with the time-to-parity halving each generation. In the agent era, Kimi K2.6 overtook Opus 4.5 in 4.8 months, while GLM-5.2 surpassed GPT-5.2 in 6 months. This accelerating catch-up threatens the commercial moat of closed-source labs like Anthropic, since open models can now handle many coding and agentic tasks that underpin billions in annualized revenue. It points to growing commoditization of the model layer, pushing differentiation toward productization and user experience. SemiAnalysis divides LLM history into scaling, reasoning, and agent eras, and finds that the capability gap fluctuates cyclically. The article notes that GLM 5.3 and Kimi K3 can already handle tasks that contributed to Anthropic's $65B+ annualized revenue, though benchmarks are not everything and Anthropic's productization remains an advantage.

telegram · zaihuapd · Aug 22, 08:26

**Background**: SemiAnalysis is a Substack publication by Dylan Patel that covers semiconductors and the AI industry. The 'agent era' refers to the third wave of AI, where systems act on connected tools and data rather than just respond to prompts. Open-weight models such as GLM and Kimi have become increasingly competitive on coding benchmarks like SWE-bench.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/about">About - SemiAnalysis</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-the-agentic-era-google-io-2026">What Is the Agentic Era? How Google I/O 2026 Defined the Next Phase of AI | MindStudio</a></li>
<li><a href="https://artificialanalysis.ai/models/comparisons/glm-5-2-vs-kimi-k2-6">GLM-5.2 (max) vs Kimi K2.6: Model Comparison</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#closed-source`, `#AI`, `#model commoditization`, `#industry analysis`

---