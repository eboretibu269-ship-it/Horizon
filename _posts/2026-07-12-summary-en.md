---
layout: default
title: "Horizon Summary: 2026-07-12 (EN)"
date: 2026-07-12
lang: en
---

> From 30 items, 9 important content pieces were selected

---

1. [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](#item-1) ⭐️ 9.0/10
2. [GPT-5.6 Proves 50-Year-Old Graph Conjecture in One Hour](#item-2) ⭐️ 9.0/10
3. [Nvidia, CoreWeave, and Nebius: Inside the Circular Financing of the GPU Boom](#item-3) ⭐️ 8.0/10
4. [ClickHouse scales PgBouncer to 4x throughput](#item-4) ⭐️ 8.0/10
5. [SQLite: Prefer Strict Tables for Type Safety](#item-5) ⭐️ 8.0/10
6. [Six U-Boot bugs allow code execution before OS boot](#item-6) ⭐️ 8.0/10
7. [ZhiPu Founder Announces 'Touch High' AGI Plan](#item-7) ⭐️ 8.0/10
8. [xAI Grok CLI Uploads Entire Codebases and Key Files by Default](#item-8) ⭐️ 8.0/10
9. [EU plans fines for tech giants failing to protect consumers](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 makes Model Runner V2 the default execution path for all dense models, removes the legacy PagedAttention implementation, and achieves performance parity between the Transformers modeling backend and native vLLM. This release marks a major architectural milestone for vLLM, simplifying the codebase and improving maintainability while delivering performance that matches native kernels, making it easier for developers to deploy and customize LLM serving. Model Runner V2 now supports EVS, realtime embeddings, prefix caching for Mamba hybrids, and dynamic speculative decoding with full CUDA graphs. The Transformers backend gained FP8 MoE support and CUDA graph fixes, and PagedAttention was entirely deleted.

github · khluu · Jul 11, 20:06

**Background**: vLLM is an open-source library for fast LLM serving that originally introduced PagedAttention to manage KV cache efficiently using virtual memory paging. Over time, the team developed Model Runner V2 to address design issues and technical debt from the V1 architecture. The Transformers backend allows users to run models with minimal code changes by leveraging Hugging Face Transformers.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://en.wikipedia.org/wiki/PagedAttention">PagedAttention</a></li>
<li><a href="https://docs.vllm.ai/en/stable/features/speculative_decoding/dynamic_speculative_decoding/">Dynamic Speculative Decoding - vLLM</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#LLM serving`, `#AI infrastructure`, `#model optimization`, `#open source`

---

<a id="item-2"></a>
## [GPT-5.6 Proves 50-Year-Old Graph Conjecture in One Hour](https://www.qbitai.com/2026/07/447873.html) ⭐️ 9.0/10

OpenAI's GPT-5.6 Sol Ultra model proved the cycle double cover conjecture, a 50-year-old open problem in graph theory, in under one hour by employing 64 sub-agents and a detailed prompt. This achievement demonstrates a breakthrough in AI's ability to tackle long-standing mathematical problems through multi-agent reasoning, potentially accelerating research in mathematics and related fields. The model converted the conjecture into a problem on finite fields and linear equations, assigning two labels per edge so that edges with the same label form cycles. OpenAI also released the full 700-character prompt, which specifies verification criteria and boundary conditions rather than fixed steps.

telegram · zaihuapd · Jul 12, 03:49

**Background**: The cycle double cover conjecture asks whether every bridgeless undirected graph has a collection of cycles such that each edge appears exactly twice. It is a well-known open problem in graph theory posed by Tutte, Itai and Rodeh, Szekeres, and Seymour. Finite fields are algebraic structures with a finite number of elements, used here to formulate the problem algebraically. Sub-agents are smaller AI assistants that can be delegated subtasks to manage complexity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/Finite_field">Finite field</a></li>
<li><a href="https://anthropic.skilljar.com/introduction-to-subagents">Introduction to subagents</a></li>

</ul>
</details>

**Tags**: `#AI`, `#mathematics`, `#graph theory`, `#GPT-5.6`, `#reasoning`

---

<a id="item-3"></a>
## [Nvidia, CoreWeave, and Nebius: Inside the Circular Financing of the GPU Boom](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 8.0/10

An analysis reveals how Nvidia, CoreWeave, and Nebius are interconnected through investments and GPU supply deals, sparking debate on whether this constitutes circular financing. Understanding these financial dynamics is crucial as they underpin the booming AI infrastructure market, potentially affecting GPU pricing, cloud competition, and the stability of the AI ecosystem. Nvidia invested $2 billion in CoreWeave for a 9% stake, while CoreWeave plans $35 billion in CapEx for 2026, with Nvidia's investment covering only a fraction. Meanwhile, Nebius signed a $27 billion AI infrastructure deal with Meta, using Nvidia's GPUs.

hackernews · adletbalzhanov · Jul 11, 17:21 · [Discussion](https://news.ycombinator.com/item?id=48873836)

**Background**: CoreWeave and Nebius are independent GPU cloud providers that offer Nvidia's GPUs for AI workloads. The GPU boom has led to massive capital expenditures, with cloud providers relying on investments from hardware vendors like Nvidia and revenue from large tech companies like Meta.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coreweave.com/products/gpu-compute">GPUs for AI Models and Innovation | CoreWeave</a></li>
<li><a href="https://nebius.com/">Nebius - The Ultimate AI Cloud</a></li>
<li><a href="https://tech-insider.org/meta-nebius-27-billion-ai-infrastructure-deal-2026/">Meta-Nebius 7B AI Infrastructure Deal Breakdown [2026]</a></li>

</ul>
</details>

**Discussion**: Commenters are split: some argue that Nvidia's small stake relative to CoreWeave's CapEx disproves circular financing, while others focus on profitability concerns and metrics like ROI per token. A few discuss Nebius capacity and interview experiences.

**Tags**: `#GPU boom`, `#Nvidia`, `#CoreWeave`, `#cloud infrastructure`, `#AI financing`

---

<a id="item-4"></a>
## [ClickHouse scales PgBouncer to 4x throughput](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse published a blog post describing how they scaled PgBouncer, a PostgreSQL connection pooler, to 4x throughput by using peer-to-peer connection sharing and enabling SO_REUSEPORT on multiple processes. This optimization breaks a common bottleneck in PostgreSQL deployments, allowing pooler-saturated systems to handle significantly more traffic without scaling Postgres itself. It demonstrates a practical, low-cost method to improve database infrastructure performance. The improvement involves running multiple PgBouncer processes on the same host with SO_REUSEPORT to share the same port, and enabling peering so that cancellation requests are forwarded to the correct process. This configuration is now the default in ClickHouse Managed Postgres.

hackernews · saisrirampur · Jul 11, 15:28 · [Discussion](https://news.ycombinator.com/item?id=48872874)

**Background**: PgBouncer is a lightweight connection pooler for PostgreSQL that manages database connections to reduce overhead. Traditionally, a single PgBouncer process can become a bottleneck under high concurrency. Peering allows multiple PgBouncer processes to share connection metadata and forward cancellation requests, preventing dropped queries. SO_REUSEPORT enables multiple processes to listen on the same TCP port, distributing incoming connections.

<details><summary>References</summary>
<ul>
<li><a href="https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres">How we scale PgBouncer in ClickHouse Managed Postgres</a></li>
<li><a href="https://www.pgbouncer.org/">PgBouncer - lightweight connection pooler for PostgreSQL</a></li>
<li><a href="https://www.pgbouncer.org/config.html">PgBouncer config</a></li>

</ul>
</details>

**Discussion**: Comments discuss technical details: some question why PgBouncer needs to handle cancellations at all, and alternatives like Odyssey and pgdog are mentioned. Overall sentiment is positive, with users noting the usefulness of scaling via Kubernetes and interest in peering configuration.

**Tags**: `#PostgreSQL`, `#PgBouncer`, `#performance`, `#connection pooling`, `#scalability`

---

<a id="item-5"></a>
## [SQLite: Prefer Strict Tables for Type Safety](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 8.0/10

Evan Hahn published an article advocating the use of STRICT tables in SQLite to enforce column type constraints, preventing accidental data corruption from type mismatches. This practice improves data integrity for SQLite users, especially in multi-application or production environments, by catching type errors at insert time rather than silently corrupting data. STRICT tables were introduced in SQLite version 3.37.0 (2021-11-27) and are enabled per table. However, there is no direct ALTER TABLE command to convert existing tables; tools like sqlite-utils can perform the transformation by copying data.

hackernews · ingve · Jul 11, 17:33 · [Discussion](https://news.ycombinator.com/item?id=48873940)

**Background**: In ordinary SQLite tables, column data types are hints, not strict rules, allowing any type of value in any column. This flexibility, known as dynamic typing, can lead to silent data corruption when, for example, a string is inserted into an integer column. STRICT tables enforce column types at the database level, rejecting values that do not match.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sqlite.org/stricttables.html">STRICT Tables</a></li>
<li><a href="https://antonz.org/sqlite-strict-tables/">STRICT tables in SQLite</a></li>
<li><a href="https://www.sqlitetutorial.net/sqlite-strict-tables/">SQLite Strict Tables</a></li>

</ul>
</details>

**Discussion**: Comments highlight both support and concerns: simonw added a feature to sqlite-utils for converting tables; dfabulich referenced the official 'flextypegood' document arguing against strict as default; jll29 expressed desire for strict to be default; ezekiel68 noted the trade-off between simplicity and reliability; petilon pointed out missing data types like Date in strict mode.

**Tags**: `#SQLite`, `#databases`, `#data integrity`, `#strict tables`, `#software engineering`

---

<a id="item-6"></a>
## [Six U-Boot bugs allow code execution before OS boot](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

Security firm Binarly disclosed six vulnerabilities in U-Boot's FIT signature verification code, two of which allow arbitrary code execution and four cause denial of service, affecting devices since U-Boot 2013.07. These flaws allow attackers to execute malicious code before the operating system and security software start, potentially disabling firmware security features and installing persistent malware, with remote exploitation possible on systems like BMCs. The vulnerabilities reside in the FIT signature verification code and affect over 50 stable releases and downstream forks; patches have been accepted by U-Boot maintainers but require integration by hardware vendors into firmware updates.

telegram · zaihuapd · Jul 11, 08:32

**Background**: U-Boot is an open-source bootloader widely used in embedded devices like routers, IoT devices, and servers. FIT (Flat Image Tree) is a packaging format for kernel, device tree, and initramfs with signature verification to ensure integrity. BMC (Baseboard Management Controller) is a remote management processor allowing administrators to update firmware over the network, making remote exploitation possible.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.u-boot.org/en/latest/usage/fit/signature.html">U-Boot FIT Signature Verification — Das U-Boot unknown version documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Intelligent_Platform_Management_Interface">Intelligent Platform Management Interface - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#security`, `#U-Boot`, `#firmware`, `#vulnerability`, `#bootloader`

---

<a id="item-7"></a>
## [ZhiPu Founder Announces 'Touch High' AGI Plan](https://mp.weixin.qq.com/s/3CQSkf_kBnXiCDgS4L-Cgg) ⭐️ 8.0/10

Tang Jie, founder of ZhiPu, released an internal letter announcing the 'Touch High' (Mo Gao) plan, outlining a multi-year roadmap to achieve AGI through long-term tasks, autonomous agent systems, complete self-training, and extreme safety governance, with a massive investment in mechanistic interpretability. This plan signals a major strategic commitment from one of China's leading AI companies to pursue AGI over short-term commercial gains, highlighting the importance of interpretability and safety. It could influence the direction of AGI research globally, especially in China's AI ecosystem. The plan identifies four key 'peaks' to conquer: long-horizon tasks, autonomous agents, fully self-training, and extreme safety governance. ZhiPu commits over 10 billion yuan to mechanistic interpretability research, aiming to make black-box models transparent. The company's GLM-5.2 model is reportedly near the frontier of overseas models and is open-source.

telegram · zaihuapd · Jul 11, 13:59

**Background**: AGI (Artificial General Intelligence) refers to AI systems that can perform any intellectual task that a human can. Mechanistic interpretability is a subfield aiming to reverse-engineer neural networks to understand their internal algorithms and circuits. Autonomous agent systems can independently plan and execute complex tasks, which is a key step toward AGI. ZhiPu is a prominent Chinese AI company known for its open-source GLM series models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://en.wikipedia.org/wiki/Autonomous_agent">Autonomous agent - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AGI`, `#AI Safety`, `#Interpretability`, `#ZhiPu`, `#Open Source`

---

<a id="item-8"></a>
## [xAI Grok CLI Uploads Entire Codebases and Key Files by Default](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 8.0/10

Security researchers discovered that xAI's Grok CLI tool (version 0.2.93) automatically uploads entire code repositories and sensitive files like .env keys to xAI servers, even when the 'improve model' setting is disabled. This poses a critical privacy and security risk for developers using the tool, as it could expose proprietary code, credentials, and other sensitive data to xAI without user consent or knowledge. The tool uploads files via two channels: file contents are embedded in model requests and uploaded to Google Cloud Storage, and the entire repository is sent as a git bundle regardless of user prompts. In tests, a file explicitly instructed not to be opened was found intact in the upload.

telegram · zaihuapd · Jul 12, 04:19

**Background**: Grok CLI is a command-line tool developed by xAI that integrates Grok models (like Grok 4.5) into the terminal for coding assistance. A git bundle is a single binary file containing a full Git repository, including all branches and history. The 'improve model' setting is intended to control data sharing for model training, but here it fails to prevent uploads.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://github.com/Norlem/grok-cli">GitHub - Norlem/grok-cli: A terminal UI for xAI's Grok models...</a></li>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git-bundle Documentation</a></li>

</ul>
</details>

**Tags**: `#security`, `#privacy`, `#xAI`, `#CLI`, `#code leakage`

---

<a id="item-9"></a>
## [EU plans fines for tech giants failing to protect consumers](https://www.ft.com/content/25640be5-a5bd-4548-81f9-bd0e16f87f35) ⭐️ 8.0/10

EU Justice Commissioner Michael McGrath announced that the European Commission will propose new legislation by end of 2025 to empower the EU to fine large tech companies for failing to protect consumers, especially children, from addictive design, subscription traps, and dark patterns. This marks a significant expansion of EU consumer protection enforcement, potentially forcing major platforms to redesign interfaces and reduce deceptive practices. The move could set a global precedent for regulating dark patterns and addictive design. The new rules will cover not only large tech companies already subject to digital regulations but also smaller online merchants and game developers. McGrath noted that current member-state enforced rules have never led to fines and lack deterrence.

telegram · zaihuapd · Jul 12, 06:25

**Background**: Dark patterns are deceptive user interface designs that trick users into actions they did not intend, such as buying unnecessary insurance or making unwanted purchases. The EU has previously enacted regulations like the Digital Services Act, but consumer protection enforcement has been weak. The proposed legislation aims to close enforcement gaps and give the EU direct authority to penalize systemic violations.

**Tags**: `#EU regulation`, `#consumer protection`, `#dark patterns`, `#tech policy`, `#online platform regulation`

---