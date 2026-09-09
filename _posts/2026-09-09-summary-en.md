---
layout: default
title: "Horizon Summary: 2026-09-09 (EN)"
date: 2026-09-09
lang: en
---

> From 37 items, 10 important content pieces were selected

---

1. [OpenAI Claims Breakthrough on Navier-Stokes Millennium Problem](#item-1) ⭐️ 10.0/10
2. [AlphaGenome Atlas: A High-Resolution Predictive Map of Human DNA](#item-2) ⭐️ 9.0/10
3. [Benchmarking Qwen3.8 27B quantizations: 4-bit holds up, 1-bit collapses](#item-3) ⭐️ 8.0/10
4. [Copperhead Brings Cursor-Style AI Assistance to Circuit Board Design](#item-4) ⭐️ 8.0/10
5. [NeurIPS Desk-Rejects 178 Papers Using Flawed AI Detector That Flagged Chairs' Own Work](#item-5) ⭐️ 8.0/10
6. [Malaysia Eyes Huawei Ascend 910C Chips for Sovereign AI Project](#item-6) ⭐️ 8.0/10
7. [Tim Cook Steps Aside, New CEO John Ternus to Present Apple's Foldable iPhone Sept. 9](#item-7) ⭐️ 8.0/10
8. [ASML and TSMC Team Up to Shift High NA EUV to 12-Inch Photomasks](#item-8) ⭐️ 8.0/10
9. [China Targets 9,800 EFLOPS AI Compute by 2030, Quadrupling Capacity](#item-9) ⭐️ 8.0/10
10. [OpenAI Releases ChatGPT Images 2.5 with Faster and More Precise Generation](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Claims Breakthrough on Navier-Stokes Millennium Problem](https://www.reddit.com/r/MachineLearning/comments/1wavdi7/openal_says_it_has_cracked_one_of_maths/) ⭐️ 10.0/10

In September 2026, OpenAI announced that an unreleased internal model produced a proposed resolution to the Navier–Stokes existence and smoothness problem, one of the Clay Mathematics Institute's Millennium Prize Problems. The claimed result shows that a smooth, finite-energy 3D incompressible flow subject to a smooth external force can develop a singularity in finite time, providing a negative answer to the problem. If verified, this would be the first AI- produced solution to a Millennium Prize Problem, potentially transforming how fundamental mathematics is conducted. The surrounding priority dispute and allegations that OpenAI may have used human researchers' private sessions in its training also raise urgent questions about AI ethics and research credit. OpenAI said the solution was reached after roughly 88 hours of agent execution, using about 130 billion output tokens, with an additional 17 hours of Lean formalization via GPT-6 Astra. NYU mathematician Tristan Buckmaster accused OpenAI of using his and Levent Alpöge's private Codex sessions; OpenAI said it could not rule out that de-identified user data helped improve its models.

reddit · r/MachineLearning · /u/Shizuka_Kuze · Sep 8, 17:42

**Background**: The Navier–Stokes equations describe the motion of viscous fluids, and it remains unproven whether smooth, global solutions always exist in three dimensions. In 2000, the Clay Mathematics Institute designated this as one of its seven Millennium Prize Problems, each carrying a $1 million reward; only the Poincaré conjecture has been officially solved so far. OpenAI's claim, which has not yet been verified by the Clay Institute or the wider mathematical community, reportedly builds on a 2023 blowup technique developed by Diego Córdoba and Luis Martínez Zoroa.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier-Stokes_existence_and_smoothness_problem">Navier-Stokes existence and smoothness problem</a></li>
<li><a href="https://en.wikipedia.org/wiki/Millennium_Prize_Problems">Millennium Prize Problems</a></li>

</ul>
</details>

**Discussion**: Community comments express deep suspicion and anger over the alleged intellectual theft. One top comment lays out the accusation timeline, noting Buckmaster and Alpöge had breakthroughs on a related problem in August, while OpenAI's effort began only after learning of it. Another quotes Buckmaster's account that OpenAI warned him, "Why would you ruin your career?" when he objected, and commenters argue that OpenAI's inability to rule out training on user data fatally undermines its defense.

**Tags**: `#OpenAI`, `#Mathematics`, `#Navier-Stokes`, `#Millennium Problems`, `#AI Research`

---

<a id="item-2"></a>
## [AlphaGenome Atlas: A High-Resolution Predictive Map of Human DNA](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/) ⭐️ 9.0/10

Google DeepMind has introduced AlphaGenome Atlas, a predictive catalogue that estimates the molecular effects and AVI scores for all 9 billion possible single-nucleotide variants across the human genome. It is presented as a high-resolution map of how single-letter DNA changes may affect genome function. The Atlas brings genome-wide variant interpretation closer to the kind of impact AlphaFold has had on protein science by offering effect predictions for every single-letter change, not just variants already observed in patients. This could accelerate rare-disease diagnosis, personalized medicine, and functional genomics research by helping clinicians and scientists tell harmless variants from disease-causing mutations. Rather than restricting scoring to protein-coding genes, the Atlas provides effect predictions for single-nucleotide variants in both coding and non-coding DNA. It is part of Google DeepMind's AlphaGenome platform, is queryable through a public web interface, and users report that no affiliation is required to access the atlas.

hackernews · utiiiD · Sep 8, 14:55 · [Discussion](https://news.ycombinator.com/item?id=49611251)

**Background**: A single-nucleotide variant (SNV) is a change of one DNA letter at one position in the genome; such changes can be benign, risk-conferring, or pathogenic. Predicting their effects is difficult because many occur in non-coding DNA, and experimental saturation mutagenesis can only cover localized regions in the laboratory. Variant effect predictors (VEPs) are computational tools that estimate the likely functional impact of genetic mutations, and AlphaGenome Atlas is a genome-wide, deep-learning-driven catalogue of such effect predictions.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/blog/alphagenome-atlas-a-predictive-map-of-every-possible-dna-letter-change-in-the-human-genome/">AlphaGenome Atlas: Molecular predictions for 9 Billion human DNA ...</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/">Introducing AlphaGenome Atlas - The Keyword</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11098935/">Variant effect predictors: a systematic review and practical guide</a></li>

</ul>
</details>

**Discussion**: In the Hacker News discussion, commenters were engaged but technically cautious. Some questioned whether the Atlas only repackages precomputed AlphaGenome API values rather than offering new information, and others asked whether promoter sequences are genuinely covered despite the stated inclusion of non-coding DNA. Several practical questions also came up, such as whether consumer genomics files from 23andMe can be used to find pathogenic mutations, while one commenter confirmed that the web portal can be accessed without an institutional affiliation.

**Tags**: `#genomics`, `#deepmind`, `#ai`, `#health`, `#bioinformatics`

---

<a id="item-3"></a>
## [Benchmarking Qwen3.8 27B quantizations: 4-bit holds up, 1-bit collapses](https://quesma.com/blog/qwen38-27b-quantizations-benchmarked/) ⭐️ 8.0/10

Benchmarking Qwen3.8 27B's quantized variants shows that 4-bit quantization preserves model performance, while 1-bit quantization degrades it sharply. The results also show a graded performance curve down to the 2-bit level. This gives practitioners a practical reference for running Qwen3.8 27B on limited GPU hardware by selecting the quantization level that best balances memory, speed, and output quality. It also signals that extreme 1-bit compression remains impractical for this class of model. According to the benchmark, 4-bit variants show little difference from the full-precision model, while the 2-bit version scores slightly lower and the 1-bit version collapses. Community commenters note that KV cache quantization, sub-16 GB VRAM scenarios, and longer-context performance remain untested.

hackernews · stared · Sep 8, 14:49 · [Discussion](https://news.ycombinator.com/item?id=49611128)

**Background**: Quantization compresses large language models by converting weights from high-precision values to lower-precision ones, reducing VRAM requirements and speeding up inference. Qwen3.8-27B is an Apache-2-licensed compact vision-language model released by Alibaba's Qwen team, designed for deployment-friendly multi-step reasoning tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/quantization-for-large-language-models">Quantization for Large Language Models (LLMs): Reduce AI Model Sizes Efficiently | DataCamp</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen</a></li>

</ul>
</details>

**Discussion**: Commenters raise several follow-up questions: one notes that Wilson confidence intervals do not capture run-to-run variation, and another suggests Qwen's extended thinking can partially offset quality loss at lower quant levels. Several users ask for benchmarks of KV cache quantization, the sub-16 GB VRAM range, and end-to-end quality measurement rather than token-level metrics.

**Tags**: `#LLM`, `#quantization`, `#Qwen`, `#benchmark`, `#AI`

---

<a id="item-4"></a>
## [Copperhead Brings Cursor-Style AI Assistance to Circuit Board Design](https://copperhead.sh/) ⭐️ 8.0/10

Copperhead is an AI-powered printed circuit board (PCB) design tool that gives hardware engineers a Cursor-like experience with generation, layout, and export features. It was shared as a Show HN and quickly drew 198 points and 77 comments on Hacker News. This reflects the growing movement to apply AI coding-agent techniques to hardware design, potentially lowering the skill barrier for PCB layout. It will matter for electronics hobbyists, professional hardware engineers, and established EDA tool vendors watching for disruption. Marketed capabilities include one-click Gerber, DXF/STEP, render and BOM export, with cloud plans that add Altium support beyond KiCad. Community testing on desktop Chrome/macOS found an input bug in the board-creation flow, and some users questioned why anyone would use a hosted version when local export exists.

hackernews · animeshchouhan · Sep 8, 13:26 · [Discussion](https://news.ycombinator.com/item?id=49610059)

**Background**: Cursor is an AI coding agent and development environment launched in 2022 that lets developers write and edit code through natural-language instructions; it grew rapidly to a US$29.3 billion valuation and over $3 billion in annual recurring revenue. Copperhead takes this model and applies it to printed circuit board design, where traditional workflows depend on EDA tools such as KiCad or Altium and manual component placement and routing. By turning board layout into a conversational task, tools like Copperhead aim to make hardware iteration as fast and approachable as code editing has become with Cursor.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>

</ul>
</details>

**Discussion**: Commenters see the space heating up, citing Flux.ai, Silixon, Quilter, DeepPCB, and Astra as competitors, with some comparing Copperhead to KiCad workflows. Several practical concerns appeared as well: a user on macOS Chrome reported being unable to type text in the board-creation modal, another asked whether the tool can deliver fully assembled boards, and one questioned the value of a hosted version when local export exists.

**Tags**: `#PCB design`, `#AI tools`, `#hardware engineering`, `#EDA`, `#KiCad`

---

<a id="item-5"></a>
## [NeurIPS Desk-Rejects 178 Papers Using Flawed AI Detector That Flagged Chairs' Own Work](https://www.reddit.com/r/MachineLearning/comments/1wakf62/neurips_deskrejected_178_papers_for_being/) ⭐️ 8.0/10

NeurIPS desk-rejected 178 papers, or 18.4% of submissions to its Position Paper Track, using the proprietary AI detector Pangram without human review or appeal. Independent tests showed the same detector flagged the track chairs' own recent papers as 24% to 69% AI-generated, which would have put them at risk under their own rules. This controversy raises serious concerns about the fairness and reliability of using black-box AI detectors in academic review, especially without an appeal process. It disproportionately risks harming ESL researchers, could damage trust in top conferences like NeurIPS, and sets a troubling precedent for automated integrity enforcement. According to the report, Pangram's default setting initially flagged about 42.7% of the entire track, and nearly half of all submissions scored 90-100% as AI; organizers only reduced the flag rate to 12.7% by shrinking the text windows. Twenty-two papers were rejected for scoring above 0.5 despite authors denying AI use, and a Stanford study cited in the post found 61.22% of human-written TOEFL essays are falsely flagged because formal non-native English is structurally rigid.

reddit · r/MachineLearning · /u/tughanbulut · Sep 8, 10:19

**Background**: NeurIPS is one of the world's top machine learning conferences, and desk rejection means a paper is rejected by organizers before peer review. AI detectors such as Pangram do not verify whether a document matches known AI output; instead, they statistically estimate authorship by looking for patterns that differ between AI-generated and human-written text. These tools are known to produce false positives, particularly on formal, structured, or non-native English writing, which has led to criticism that they encourage 'witch hunts' rather than reliable detection.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pangram_(AI_detector)">Pangram (AI detector)</a></li>
<li><a href="https://timrequarth.substack.com/p/why-you-shouldnt-trust-ai-detector">The Problem with AI Detector Companies - by Tim Requarth</a></li>

</ul>
</details>

**Tags**: `#AI detection`, `#NeurIPS`, `#academic publishing`, `#ethics`, `#machine learning`

---

<a id="item-6"></a>
## [Malaysia Eyes Huawei Ascend 910C Chips for Sovereign AI Project](https://www.businesstimes.com.sg/international/malaysia-eyes-huawei-chips-ai-project-despite-us-warning) ⭐️ 8.0/10

Malaysia is evaluating Huawei's Ascend 910C AI chips as the core of a 2 billion ringgit (about US$494 million) sovereign AI project. If the plan proceeds, it would become the first case of a foreign government officially choosing Chinese AI accelerators over US alternatives. This could be a landmark moment in AI geopolitics, signaling that US export controls may not deter governments from adopting Chinese AI hardware. It may also encourage other US-aligned countries to consider Chinese chips for their sovereign AI initiatives. No details have been released on the number of chips Malaysia would purchase. The Trump administration reportedly warned that using Huawei's AI accelerator could violate US export rules, while Malaysia views the decision as purely commercial. Reported specs put the Ascend 910C at about 800 TFLOPS FP16 and 3.2 TB/s memory bandwidth, making it roughly comparable to Nvidia's H100.

telegram · zaihuapd · Sep 8, 03:35

**Background**: Sovereign AI refers to the products, technology stack, and tools that allow a nation to deploy AI systems on its own terms rather than relying on outside providers. Huawei's Ascend 910C is a Chinese-designed AI accelerator developed amid US sanctions, with media-reported performance near Nvidia's H100 in certain metrics. This context matters because the US has sought to limit China's advanced chip capabilities, making export controls a central tool in that competition.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huaweicentral.com/huawei-ascend-910c-alleged-specs-suggest-it-a-tough-rival-to-nvidia-h100/">Huawei Ascend 910C alleged specs suggest it a tough rival to ...</a></li>
<li><a href="https://www.redhat.com/en/topics/ai/sovereign-ai">What is sovereign AI?</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#Huawei`, `#geopolitics`, `#export controls`, `#sovereign AI`

---

<a id="item-7"></a>
## [Tim Cook Steps Aside, New CEO John Ternus to Present Apple's Foldable iPhone Sept. 9](https://www.macrumors.com/2026/09/07/tim-cook-wont-appear-apple-sept-9-event-video/) ⭐️ 8.0/10

Apple's September 9 'Surprise and Shine' event video will not feature Tim Cook, who stepped down as CEO on September 1 and became executive chairman. New CEO John Ternus will instead lead the presentation of the foldable iPhone. This marks a carefully staged leadership transition at Apple, giving Ternus the spotlight at one of the company's most anticipated product launches in years. The decision signals that Apple wants consumers and investors to associate its next chapter—and its foldable device push—with the new CEO. According to Bloomberg's Mark Gurman, Cook will attend a screening of the event on Wednesday but will not appear in the event video itself. Apple reportedly designed the handoff so Ternus becomes the public face for the foldable iPhone and future products, because a Cook cameo would dilute that effect.

telegram · zaihuapd · Sep 8, 05:03

**Background**: The event video is Apple's polished product presentation, so choosing who appears in it is a messaging decision as much as a practical one. Tim Cook's move from CEO to executive chairman is a common succession structure that allows a veteran leader to remain involved in governance while a new CEO takes charge of day-to-day operations. A foldable iPhone would be a major new product category for Apple, using a bendable display to offer a phone that can unfold into a larger screen.

**Tags**: `#Apple`, `#CEO transition`, `#foldable iPhone`, `#tech news`

---

<a id="item-8"></a>
## [ASML and TSMC Team Up to Shift High NA EUV to 12-Inch Photomasks](https://www.nrc.nl/nieuws/2026/09/08/asml-gaat-samenwerken-met-taiwanese-chipgigant-tsmc-om-zijn-nieuwste-chipmachines-te-upgraden-a4936073) ⭐️ 8.0/10

On September 7, 2026, ASML and TSMC announced a collaboration to move High NA EUV lithography from 6-inch photomasks to a 12-inch format. They plan to establish a 12-inch photomask pilot line by 2031 and deploy the related systems for advanced-process high-volume manufacturing in 2033, with TSMC aiming to use High NA EUV for large-scale advanced-node production starting in 2030. This collaboration gives High NA EUV a clear industrial roadmap, which matters because 12-inch masks can increase fab productivity, lower chipmaking costs, and remove stitching constraints that currently limit pattern sizes. The move will shape the next generation of advanced chip manufacturing and affect the broader semiconductor ecosystem, including TSMC's rivals and ASML's other customers. High NA EUV will still first be adopted in production using the existing 6-inch masks, with the transition to 12-inch masks planned as a subsequent step. The 12-inch format requires the industry to develop new mask infrastructure, including blanks, patterning tools, and metrology, to support the planned 2031 pilot line and early-2030s production timeline.

telegram · zaihuapd · Sep 8, 06:55

**Background**: High NA EUV is the next generation of extreme ultraviolet lithography, a technique that uses 13.5nm wavelength light to print the smallest features on advanced microchips. A higher numerical aperture enables chipmakers to print finer patterns, but the lithographic exposure field is physically limited, so larger patterns on a chip currently have to be 'stitched' together from multiple exposures. Moving from 6-inch to 12-inch photomasks enlarges the usable field and reduces this stitching overhead, boosting productivity and lowering cost.

<details><summary>References</summary>
<ul>
<li><a href="https://www.asml.com/en/news/press-releases/2026/tsmc-and-asml-announce-industry-transition-to-large-format-photomasks-for-high-na-euv">TSMC and ASML Announce Initiative to Pioneer Industry Transition to Large-Format Photomasks for High NA EUV</a></li>
<li><a href="https://www.asml.com/en/company/stories/2024/5-things-high-na-euv">5 things you should know about High NA EUV lithography - ASML</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#EUV lithography`, `#ASML`, `#TSMC`, `#chip manufacturing`

---

<a id="item-9"></a>
## [China Targets 9,800 EFLOPS AI Compute by 2030, Quadrupling Capacity](https://www.scmp.com/tech/policy/article/3366733/china-targets-fourfold-boost-ai-computing-capacity-2030-major-tech-push) ⭐️ 8.0/10

China's Ministry of Industry and Information Technology published a five-year industrial plan targeting 9,800 EFLOPS of intelligent computing capacity by 2030, with 3.8 trillion yuan in information infrastructure investment from 2026 to 2030. The plan also calls for deploying AI computing clusters at the 10,000-card and 100,000-card scale, while improving adaptation with domestic AI chips. This policy marks a major state-driven push to expand China's AI computing infrastructure, potentially reshaping global hardware supply chains and intensifying competition with the United States. The scale of investment and growth targets indicates that AI compute will be a strategic national priority, with knock-on effects for chipmakers, cloud providers, and AI developers. As of late June this year, China's intelligent computing capacity stood at 2,185 EFLOPS, up 177% year-over-year, meaning the 2030 goal would require more than a fourfold increase from that base. The plan also includes deploying clusters with 10,000 and 100,000-plus accelerators and strengthening compatibility between infrastructure and domestic AI chips.

telegram · zaihuapd · Sep 8, 11:23

**Background**: EFLOPS (exa floating-point operations per second) is a unit of computing performance equal to one quintillion (10^18) floating-point operations per second. Leading supercomputers like the US Frontier and El Capitan achieve around 1 EFLOPS in benchmark tests, which helps illustrate how enormous China's 9,800-EFLOPS target is. National intelligent-computing efforts typically combine dedicated AI chips, large data-center clusters, and software ecosystems to train and run large-scale AI models.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/每秒浮點運算次數">每秒浮点运算次数 - 维基百科，自由的百科全书</a></li>
<li><a href="https://blog.csdn.net/qq_16498553/article/details/123491738">什么是EFLOPS？-CSDN博客</a></li>

</ul>
</details>

**Tags**: `#China`, `#AI infrastructure`, `#EFLOPS`, `#policy`, `#computing`

---

<a id="item-10"></a>
## [OpenAI Releases ChatGPT Images 2.5 with Faster and More Precise Generation](https://openai.com/index/introducing-chatgpt-images-2-5/) ⭐️ 8.0/10

On September 8, OpenAI launched ChatGPT Images 2.5, delivering sharper detail, more precise editing, and up to 50% lower latency than GPT-Image-2. The model is now rolling out to all users across ChatGPT, ChatGPT Work, and Codex, while the API adds two new models: GPT-Image-2.5 Flare and GPT-Image-2.5 Sunburst. This release significantly improves the quality, speed, and editing reliability of AI image generation for millions of ChatGPT users, benefiting both creative professionals and casual users. The introduction of Flare and Sunburst API models also gives developers flexible options for high-quality generation versus precision-driven editing, reinforcing OpenAI's leadership in multimodal AI. ChatGPT adds new capabilities including Sketch-guided creation, templates, image comments, and prompt sharing. GPT-Image-2.5 Flare delivers the same quality, editing, and speed improvements as the flagship model with 50% lower latency, while GPT-Image-2.5 Sunburst offers extra precision for detailed creative tasks.

telegram · zaihuapd · Sep 8, 18:45

**Background**: ChatGPT Images is OpenAI's text-to-image generation system integrated into ChatGPT, allowing users to create and edit images through natural language prompts. The previous version, GPT-Image-2, established the baseline for quality and speed. Version 2.5 builds on that foundation by reducing latency and improving editing fidelity. API access enables developers to embed these image-generation capabilities into third-party applications.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-chatgpt-images-2-5/">Introducing ChatGPT Images 2.5 - OpenAI</a></li>
<li><a href="https://x.com/OpenAIDevs/status/2097399255975813387">OpenAI Developers on X: "Meet GPT-Image-2.5 Flare and ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Image Generation`, `#ChatGPT`, `#AI Model Release`, `#API`

---