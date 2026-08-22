---
layout: default
title: "Horizon Summary: 2026-08-22 (ZH)"
date: 2026-08-22
lang: zh
---

> 从 29 条内容中筛选出 4 条重要资讯。

---

1. [SGLang v0.5.18 发布：合并 710 个 PR，新增多类模型支持](#item-1) ⭐️ 8.0/10
2. [新 MCP 路线图优先推进 HTTP、智能体身份与移除 Sampling 功能。](#item-2) ⭐️ 8.0/10
3. [从零训练的 250M 参数 LLM 经亚 2 比特量化后仅 60MB](#item-3) ⭐️ 8.0/10
4. [SemiAnalysis：开源加速追赶，每代追平时间减半](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.18 发布：合并 710 个 PR，新增多类模型支持](https://github.com/sgl-project/sglang/releases/tag/v0.5.18) ⭐️ 8.0/10

SGLang v0.5.18 正式发布，包含来自 212 位贡献者的 710 个合并 PR。该版本新增了对自回归模型（Muse Glimmer、Intern-S2-Mobius）和扩散模型（SANA-Video、LingBot-Video-MoE、LTX-2.5、Cosmos3 Edge & Distilled、LongCat-Image）的支持。 此次发布意义重大，因为 SGLang 是广泛使用的开源大模型推理框架，大量贡献反映了社区的高活跃度。新增模型支持和性能优化将惠及在生产环境中部署自回归与扩散模型的开发者。 性能改进包括重叠检查点暂存，使 Qwen3-32B 在 H100 上启动速度最多提升 2.38 倍；TP LMHead 改用 all-to-all，使 DeepSeek-V4-Pro 的 LMHead 时间从 320 微秒降至 169 微秒；FlashInfer MNNVL 纯 allreduce 在 Blackwell 上使解码性能最多提升 6.9%。该版本还统一了 SGLANG_CACHE_DIR 下的编译内核缓存，并将依赖更新为 torch 2.13.0、triton 3.7.1、flashinfer 0.6.17 和 sgl-kernel 0.4.6.post1。

github · Fridge003 · 8月22日 00:09

**背景**: SGLang 是一个开源推理框架，旨在快速部署大规模语言模型和多模态模型。它支持自回归模型和扩散模型（如视频生成），并利用 CUDA graphs、张量并行和 FlashInfer 内核等技术优化吞吐量和延迟。本次新增的模型，如 Meta 的 Muse Glimmer 和 Intern-S2-Mobius，代表了开放权重多模态与推理优化模型的最新进展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.meta.ai/blog/introducing-muse-glimmer-open-agentic-model">Introducing Muse Glimmer: An Open Agentic Model That Runs on ...</a></li>
<li><a href="https://huggingface.co/internlm/Intern-S2-Mobius">internlm/Intern-S2-Mobius · Hugging Face</a></li>
<li><a href="https://huggingface.co/Efficient-Large-Model/SANA-Video_2B_480p">Efficient-Large-Model/SANA-Video_2B_480p · Hugging Face</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#sglang`, `#open source`, `#release`, `#AI infrastructure`

---

<a id="item-2"></a>
## [新 MCP 路线图优先推进 HTTP、智能体身份与移除 Sampling 功能。](https://blog.modelcontextprotocol.io/posts/mcp-roadmap/) ⭐️ 8.0/10

Anthropic 发布的新 MCP 路线图将远程服务器改为标准 HTTP 工作负载，标准化智能体身份与授权，并移除 sampling 功能，这些变更预计在 2026-07-28 版本中落地。 该路线图决定了 AI 工具互操作性的未来方向，直接影响构建智能体与集成的开发者。这些调整回应了智能体身份和简化 HTTP 部署的实际需求，但移除 sampling 可能限制某些智能体行为模式。 该路线图以 2026-07-28 版本为目标，使远程 MCP 服务器像其他 HTTP 工作负载一样工作。它还提议在现有标准之上标准化智能体身份与授权，同时弃用允许服务器通过客户端请求 LLM 补全的 sampling 功能。

hackernews · pentagrama · 8月22日 13:31 · [社区讨论](https://news.ycombinator.com/item?id=49399591)

**背景**: MCP（模型上下文协议）是 Anthropic 于 2024 年 11 月推出的开放标准，用于将 AI 助手连接到外部工具和数据源。它使 Claude 或 ChatGPT 等应用能够与数据仓库、业务工具和开发环境交互。Sampling 是一项允许服务器通过客户端请求 LLM 补全的功能，用于支持智能体行为。MCP 授权传统上依赖用户在浏览器中批准访问，但智能体工作负载需要标准化的身份与委托机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://modelcontextprotocol.io/docs/2026-07-28/getting-started/intro">What is the Model Context Protocol (MCP)? - Model Context Protocol</a></li>
<li><a href="https://modelcontextprotocol.io/specification/2025-06-18/client/sampling">Sampling - Model Context Protocol</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些开发者欢迎转向标准 HTTP 和智能体身份，另一些人则质疑 MCP 端点是否真的比 REST 加 skills.md 文件更简单。多位评论者对移除 sampling 表示遗憾，一位网络安全开发者表示，频繁的转向和复杂性让他对 MCP 失去信心，如今更倾向于本地工具和 API。

**标签**: `#MCP`, `#AI protocols`, `#developer tools`, `#API design`, `#agent interoperability`

---

<a id="item-3"></a>
## [从零训练的 250M 参数 LLM 经亚 2 比特量化后仅 60MB](https://www.reddit.com/r/MachineLearning/comments/1vv2nkh/i_developed_my_own_quantized_llm_from_scratch/) ⭐️ 8.0/10

一位开发者从零开始用 FineWeb 的 300 亿个 token 训练了一个 2.5 亿参数的 LLM，并将其量化到每个权重低于 2 比特，使整个部署缩小到 60MB。该模型在笔记本电脑 CPU 上能以约 400 token/秒的速度运行，并配有基于磁盘的压缩 KV 缓存，可检索多达 1 亿个 token 的历史内容。 这表明了一条实用的路径：让模型足够小并支持长上下文，在无 GPU 的普通硬件上运行，从而降低端侧和边缘 AI 的部署门槛。将亚 2 比特量化与基于磁盘的记忆结合是新颖的，可能会推动模型压缩和检索增强生成方面的进一步研究。 该模型没有采用可训练的嵌入表，而是为 13.1 万个 token 分别分配固定的 512 位编码；最近的 2048 个 token 仍以 fp16 存放在 KV 缓存中，更早的条目则被压缩到约每 token 320 字节并写入磁盘。基础模型在保留的英文网页文本上困惑度为 23.3，仓库中还提供了包含主权重的微调工具包。

reddit · r/MachineLearning · /u/Final-Data-1410 · 8月22日 04:39

**背景**: KV 缓存会保存前面 token 在注意力计算中产生的键（Key）和值（Value）中间结果，使模型在自回归生成时无需重新计算，从而大幅加速推理。FineWeb 是一个基于 Common Crawl 构建的开放数据集，包含 15 万亿个 token，常被用于预训练并优于其他公开语料。低于约 3 比特的极低比特量化是一个活跃研究方向，例如 VPTQ 等方法就试图在不重训的情况下压缩大模型并保持精度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://magazine.sebastianraschka.com/p/coding-the-kv-cache-in-llms">Understanding and Coding the KV Cache in LLMs from Scratch</a></li>
<li><a href="https://arxiv.org/abs/2406.17557">[2406.17557] The FineWeb Datasets: Decanting the Web for the ...GitHub - huggingface/fineweb-2The FineWeb Datasets: Decanting the Web for the Finest Text ...FineWeb (dataset)The FineWeb Datasets: Decanting the Web for the Finest Text ...</a></li>
<li><a href="https://github.com/microsoft/VPTQ">VPTQ: Extreme Low-bit Vector Post-Training Quantization for ...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#quantization`, `#long-context`, `#edge-deployment`, `#training-from-scratch`

---

<a id="item-4"></a>
## [SemiAnalysis：开源加速追赶，每代追平时间减半](https://newsletter.semianalysis.com/p/are-open-models-catching-up) ⭐️ 8.0/10

SemiAnalysis 报告指出，开源模型正在以加速的速率缩小与闭源领先模型的差距，且每一代追平时间都会减半。在智能体时代，Kimi K2.6 用了 4.8 个月超越 Opus 4.5，而 GLM-5.2 用了 6 个月超过 GPT-5.2。 这种加速追赶威胁到 Anthropic 等闭源实验室的商业护城河，因为开源模型如今已能胜任许多支撑数十亿美元年化收入的编程和智能体任务。这表明模型层正日益商品化，差异化正转向产品化和用户体验。 SemiAnalysis 将大模型历史分为扩展、推理和智能体三个时代，并发现能力差距呈现周期性波动。文章指出，GLM 5.3 和 Kimi K3 已经能胜任许多曾为 Anthropic 带来 650 亿美元以上年化收入的任务，但基准测试并非全部，Anthropic 的产品化能力仍是其优势。

telegram · zaihuapd · 8月22日 08:26

**背景**: SemiAnalysis 是 Dylan Patel 主理的一档 Substack 刊物，聚焦半导体与人工智能产业。「智能体时代」指的是 AI 的第三次浪潮：系统能够调用连接的工具和数据采取行动，而不仅仅是回应提示。GLM、Kimi 等开放权重模型在 SWE-bench 等编程基准上已越来越有竞争力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/about">About - SemiAnalysis</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-the-agentic-era-google-io-2026">What Is the Agentic Era? How Google I/O 2026 Defined the Next Phase of AI | MindStudio</a></li>
<li><a href="https://artificialanalysis.ai/models/comparisons/glm-5-2-vs-kimi-k2-6">GLM-5.2 (max) vs Kimi K2.6: Model Comparison</a></li>

</ul>
</details>

**标签**: `#open-source`, `#closed-source`, `#AI`, `#model commoditization`, `#industry analysis`

---