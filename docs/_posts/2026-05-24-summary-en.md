---
layout: default
title: "Horizon Summary: 2026-05-24 (EN)"
date: 2026-05-24
lang: en
---

> From 74 items, 19 important content pieces were selected

---

1. [C# moves toward union types](#item-1) ⭐️ 8.0/10
2. [Starship v3 test shows progress and setbacks](#item-2) ⭐️ 8.0/10
3. [80386 Microcode Reverse-Engineered](#item-3) ⭐️ 8.0/10
4. [Deep Learning Performance, Explained from First Principles](#item-4) ⭐️ 8.0/10
5. [npm Adds Staged Publishing and Install Source Controls](#item-5) ⭐️ 8.0/10
6. [Apple outlines formal verification for corecrypto](#item-6) ⭐️ 8.0/10
7. [US limits in-country green card applications](#item-7) ⭐️ 7.0/10
8. [AI Memory Demand Is Raising Device Prices](#item-8) ⭐️ 7.0/10
9. [FTC Fines Firms Over Fake “Active Listening” Ads](#item-9) ⭐️ 7.0/10
10. [Datasette Agent brings chat to data exploration](#item-10) ⭐️ 7.0/10
11. [GitHub Open-Sources Copilot for Eclipse](#item-11) ⭐️ 7.0/10
12. [Jira workflows get a formal Turing-completeness proof](#item-12) ⭐️ 7.0/10
13. [Modern C++ Lock-Free Queue Walkthrough](#item-13) ⭐️ 7.0/10
14. [16-byte x86 demo explained](#item-14) ⭐️ 7.0/10
15. [CodeGraph brings local code graphs to AI coding tools](#item-15) ⭐️ 7.0/10
16. [Understand-Anything maps codebases into knowledge graphs](#item-16) ⭐️ 7.0/10
17. [Graphify builds codebase knowledge graphs for AI tools](#item-17) ⭐️ 7.0/10
18. [Chrome DevTools arrives for AI coding agents](#item-18) ⭐️ 7.0/10
19. [Rust CLI proxy targets LLM token waste](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [C# moves toward union types](https://andrewlock.net/exploring-the-dotnet-11-preview-2-dotnet-gets-union-types/) ⭐️ 8.0/10

A widely shared post highlights that upcoming .NET/C# work is finally bringing union types to the language, a feature C# developers have requested for years. The change is being explored in the context of newer .NET previews and would let developers model values that can be one of several allowed types more directly. Union types can make APIs more expressive and type-safe by replacing many ad hoc patterns based on inheritance, enums, nulls, or loosely structured result objects. For the large .NET ecosystem, this could improve library design and bring C# closer to capabilities that developers already use in languages such as F#, Rust, and TypeScript. According to Microsoft's C# feature specification, the proposal is for type unions rather than full built-in discriminated or tagged unions. The spec notes that discriminated unions can be expressed on top of type unions by introducing fresh case types, which is an important design distinction for developers expecting F#-style unions.

hackernews · ingve · May 22, 12:28 · [Discussion](https://news.ycombinator.com/item?id=48234954)

**Background**: In programming languages, union or sum-like types represent values that may be one of several alternatives, often described as an “OR” type. They are useful for modeling results, states, and protocol messages without falling back to weakly typed conventions. C# has long lacked a native version of this feature, so .NET developers have often used libraries or class hierarchies instead. The renewed attention reflects a broader trend of mainstream languages adding stronger type-system features to improve correctness and API clarity.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/proposals/unions">Unions - C# feature specifications (preview) | Microsoft Learn</a></li>
<li><a href="https://github.com/dotnet/csharplang/blob/main/meetings/working-groups/discriminated-unions/TypeUnions.md">csharplang/meetings/working-groups/discriminated-unions ... - GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Algebraic_data_type">Algebraic data type - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The discussion is broadly positive, with many commenters saying union types are long overdue and praising the C# team for finally pushing the feature forward. A recurring theme is that F# has offered similar capabilities for years, while others compare the potential impact to Rust and TypeScript and wonder whether library authors will actually adopt unions in public APIs.

**Tags**: `#C#`, `#.NET`, `#programming-languages`, `#type-systems`, `#language-features`

---

<a id="item-2"></a>
## [Starship v3 test shows progress and setbacks](https://www.space.com/space-exploration/launches-spacecraft/spacex-starship-v3-megarocket-first-test-flight) ⭐️ 8.0/10

SpaceX carried out a major Starship v3 test flight that achieved launch, stage separation, reentry, and a targeted ship splashdown, but also exposed problems with booster recovery and engine reliability. According to the provided summary and discussion, the booster lost an engine during ascent, failed its boost-back relight after separation, and landed hard and off target, while the ship also lost an engine yet still completed reentry. This test is significant because Starship is central to SpaceX's reusable heavy-lift strategy, so every improvement or failure directly affects the timeline for cheaper and more frequent large-scale launches. The flight also highlights the tradeoff in rapid hardware iteration: meaningful system-level progress can happen even when critical subsystems such as engine relight and booster recovery still fall short. Community observations emphasized that the ship's reentry appeared cleaner than on previous flights, with no obvious hot spots or burn-through, suggesting improved heat shield performance. The booster's failed post-separation relight and the ship's visible engine-bay anomalies indicate that Raptor propulsion and recovery operations remain important technical risk areas.

hackernews · busymom0 · May 22, 23:41 · [Discussion](https://news.ycombinator.com/item?id=48242959)

**Background**: Starship is SpaceX's fully reusable launch system, made up of the Super Heavy booster as the first stage and the Starship spacecraft as the upper stage. Super Heavy is intended to provide the initial lift, then return for recovery so the overall system can lower launch costs through reuse and scale. Starship development has also relied on hot staging, where the upper stage ignites during separation, and on Raptor engines that burn liquid methane and liquid oxygen in a full-flow staged combustion cycle. Those choices promise high performance, but they also increase engine and operations complexity during staging, relight, and landing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/List_of_Super_Heavy_boosters">List of Super Heavy boosters - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Raptor">SpaceX Raptor - Wikipedia</a></li>
<li><a href="https://interestingengineering.com/innovation/spacex-shares-stunning-images-of-starship-liftoff-and-separation">SpaceX shares stunning images of Starship liftoff and separation</a></li>

</ul>
</details>

**Discussion**: The discussion was broadly positive about SpaceX's rapid build-test-learn approach, with many commenters arguing that partial failures are acceptable if they produce useful flight data. Technically minded commenters focused on the booster's unsuccessful return sequence, the ship's engine issues, and what looked like notably improved heat shield performance during reentry.

**Tags**: `#spaceflight`, `#aerospace-engineering`, `#systems-engineering`, `#spacex`, `#rocket-reusability`

---

<a id="item-3"></a>
## [80386 Microcode Reverse-Engineered](https://www.reenigne.org/blog/80386-microcode-disassembled/) ⭐️ 8.0/10

A new reverse-engineering writeup reports that the Intel 80386's microcode ROM has been disassembled, using a high-resolution image of the chip's microcode ROM and prior understanding from earlier x86 microcode work. The result reconstructs how this landmark 32-bit x86 CPU internally sequences micro-operations for instruction execution. This matters because the 80386 was the first 32-bit processor in the x86 line, so understanding its microcode gives rare visibility into the internal control logic of a historically important architecture. It is especially valuable for hardware reverse engineers, emulator authors, and CPU historians interested in how complex CISC processors actually implement instructions beneath the ISA surface. The project builds on die-level imaging of the 80386 microcode ROM rather than relying only on black-box behavioral testing, and it follows earlier public reverse-engineering work on x86 microcode such as the 8086. The available context also suggests the 80386 uses a structured microcode word format, which is useful for mapping ROM bits to internal data paths and control operations, though the work is still specialized and not equivalent to recovering a complete transistor-level HDL design.

hackernews · nand2mario · May 23, 12:11 · [Discussion](https://news.ycombinator.com/item?id=48247004)

**Background**: Microcode is a low-level control layer inside many CPUs that translates architecturally visible instructions into smaller internal operations. In x86 processors, this helps implement complex instructions while hiding the hardware details from software. The Intel 80386, introduced as the first 32-bit x86 CPU, was a major step in the evolution of the architecture and used multiple internal functional units operating in parallel. Recent reverse-engineering work on older Intel chips, including the 8086, has shown that die photos and ROM analysis can reveal how these internal control sequences work.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reenigne.org/blog/80386-microcode-disassembled/">80386 microcode disassembled « Reenigne blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/I386">i386 - Wikipedia</a></li>
<li><a href="http://www.righto.com/2023/04/reverse-engineering-8086-divide-microcode.html">Reverse-engineering the division microcode in the Intel 8086 processor</a></li>

</ul>
</details>

**Discussion**: The discussion was strongly positive, with commenters calling the black-box decoding effort both extremely difficult and deeply impressive. A major theme was curiosity about methodology: readers asked how high-resolution die images can be turned into reconstructed microcode and whether that process yields something like Verilog or requires transistor-by-transistor circuit understanding. Commenters also linked the work to related open-source efforts such as z386 and to educational material on microprogramming.

**Tags**: `#reverse-engineering`, `#cpu-architecture`, `#microcode`, `#hardware`, `#systems`

---

<a id="item-4"></a>
## [Deep Learning Performance, Explained from First Principles](https://horace.io/brrr_intro.html) ⭐️ 8.0/10

A widely praised 2022 explainer by Horace He is being resurfaced as a high-value primer on why modern deep learning workloads run fast and where they bottleneck. The article breaks performance down from hardware and systems fundamentals, covering ideas like compute throughput, memory bandwidth, and optimization tradeoffs that shape real ML training and inference speed. This matters because ML performance is increasingly determined not just by model architecture, but by how effectively software maps computation onto GPUs, memory systems, and runtimes. For practitioners, the piece offers durable mental models for understanding why some optimizations help dramatically while others fail to deliver portable speedups across frameworks and hardware. The discussion aligns with concepts such as the Roofline model, which relates achievable performance to arithmetic intensity and memory traffic, helping explain whether a workload is compute-bound or bandwidth-bound. Community comments also highlight practical complications: exported ONNX graphs, ONNX Runtime CUDA execution providers, and TensorRT backends can all behave differently, so optimization advice often depends on the exact runtime, hardware target, and memory available during tuning.

hackernews · tosh · May 23, 11:50 · [Discussion](https://news.ycombinator.com/item?id=48246889)

**Background**: Deep learning workloads are dominated by large tensor operations, especially matrix multiplications and convolutions, which run efficiently on GPUs because GPUs provide massive parallel compute throughput and high memory bandwidth. A common way to reason about performance is the Roofline model, which compares a kernel’s arithmetic intensity with the machine’s compute and bandwidth limits. Another important optimization is kernel fusion, where multiple operations are combined to reduce memory traffic and launch overhead. These ideas help explain why implementation details and runtime choices can have outsized effects on observed ML speed.

<details><summary>References</summary>
<ul>
<li><a href="https://community.intel.com/t5/Blogs/Tech-Innovation/Artificial-Intelligence-AI/Applying-the-Roofline-Model-for-Deep-Learning-Performance/post/1335698">Applying the Roofline Model for Deep Learning Performance ...</a></li>
<li><a href="https://github.com/dmlc/nnvm-fusion">GitHub - dmlc/nnvm-fusion: Kernel Fusion and Runtime Compilation Based on NNVM · GitHub</a></li>
<li><a href="https://www.abhik.ai/articles/kernel-fusion">Kernel Fusion: Boosting Neural Network Performance | Abhik Sarkar</a></li>

</ul>
</details>

**Discussion**: The comments are strongly positive, with readers calling the post a classic and useful for building intuition about ML systems. Several commenters emphasize NVIDIA’s remarkable ability to maintain its lead through sustained gains in FLOPs, bandwidth, and interconnects, while others argue that performance advice is frustratingly non-portable across PyTorch, ONNX, ONNX Runtime, TensorRT, hardware targets, and tuning conditions. There is also curiosity about implementation-level tricks such as why chained expressions like x.cos().cos() may run faster than separate calls, pointing to graph-level optimization and fusion behavior beneath Python code.

**Tags**: `#deep-learning`, `#ml-systems`, `#gpu-performance`, `#hardware-acceleration`, `#optimization`

---

<a id="item-5"></a>
## [npm Adds Staged Publishing and Install Source Controls](https://github.blog/changelog/2026-05-22-staged-publishing-and-new-install-time-controls-for-npm) ⭐️ 8.0/10

GitHub announced that staged publishing for npm is now generally available, and it also added new install-time allow-list flags: --allow-file, --allow-remote, and --allow-directory. These new flags complement the existing --allow-git option and are aimed at improving supply-chain security for both package publishers and consumers. npm is a foundational package distribution channel for the JavaScript ecosystem, so changes to how packages are published and installed can affect a very large number of developers and CI systems. The update adds more deliberate checks before a package becomes installable and gives users finer control over which dependency sources are permitted during installation. According to npm documentation, staged publishing uploads a prebuilt tarball into a stage queue instead of making the version immediately available, and a maintainer must explicitly approve it before consumers can install it. npm docs also note that npm stage publish does not require 2FA, while staged packages can be reviewed in the CLI or on npmjs.com before approval.

rss · GitHub Blog Changelog · May 22, 18:27

**Background**: npm is the default package manager and registry workflow for much of the JavaScript ecosystem, so it is a common target in software supply-chain security discussions. Staged publishing changes the release flow by separating artifact upload from public availability, which creates a review step before distribution. Install-time source controls matter because dependencies can come from different origins such as git, local files, directories, or remote locations, and restricting those origins can reduce accidental or risky package resolution paths.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.npmjs.com/staged-publishing/">Staged publishing for npm packages | npm Docs</a></li>
<li><a href="https://github.blog/changelog/2026-05-22-staged-publishing-and-new-install-time-controls-for-npm/">Staged publishing and new install-time controls for npm</a></li>

</ul>
</details>

**Tags**: `#npm`, `#supply-chain-security`, `#javascript`, `#package-management`, `#github`

---

<a id="item-6"></a>
## [Apple outlines formal verification for corecrypto](https://security.apple.com/blog/formal-verification-corecrypto/) ⭐️ 8.0/10

Apple published a technical blueprint for formally verifying parts of corecrypto, its foundational cryptographic library used by Security framework, CryptoKit, and CommonCrypto. The post says Apple has also added post-quantum encryption to corecrypto in 2024 and is now applying formal methods to strengthen assurance for production cryptographic code. Formal verification is one of the strongest ways to prove correctness properties in security-critical code, and applying it to a widely deployed cryptographic library raises the bar for software assurance. If successful, this approach could influence how major vendors build and validate cryptography for operating systems and applications. Apple frames this as a blueprint rather than a claim that all of corecrypto has already been fully verified. The focus is on parts of the library that underpin low-level cryptographic primitives, where formal evidence can complement traditional testing and code review.

reddit · r/programming · mttd · May 22, 22:03 · [Discussion](https://www.reddit.com/r/programming/comments/1tkxgmb/a_blueprint_for_formal_verification_of_apple/)

**Background**: corecrypto is Apple’s foundational cryptographic library, and higher-level frameworks such as Security framework, CryptoKit, and CommonCrypto rely on it for low-level primitives. Formal verification uses mathematical specifications and proofs to show that an implementation matches intended security and correctness properties. In cryptography, this is especially valuable because small bugs can have outsized security consequences.

<details><summary>References</summary>
<ul>
<li><a href="https://security.apple.com/blog/formal-verification-corecrypto/">A blueprint for formal verification of Apple corecrypto</a></li>
<li><a href="https://github.com/apple/corecrypto">GitHub - apple/corecrypto: Apple corecrypto</a></li>
<li><a href="https://www.amazon.science/publications/formal-verification-of-cryptographic-software-at-aws-current-practices-and-future-trends">Formal verification of cryptographic software at AWS ...</a></li>

</ul>
</details>

**Tags**: `#formal-verification`, `#cryptography`, `#security-engineering`, `#apple`, `#software-verification`

---

<a id="item-7"></a>
## [US limits in-country green card applications](https://www.nytimes.com/2026/05/22/us/politics/green-card-changes-trump.html) ⭐️ 7.0/10

USCIS announced that most people seeking a green card while temporarily in the United States must now leave the country and apply through consular processing abroad. Under the new policy, adjustment of status inside the U.S. will be granted only in "extraordinary circumstances," reversing the common path many legal immigrants used while on visas such as H-1B. This change could disrupt employment-based immigration for skilled workers, especially in tech, where many employees transition from temporary work visas to permanent residency without leaving the U.S. It also increases practical risks for families and employers because overseas consular appointments, travel constraints, and long waits can interrupt jobs, schooling, and legal status planning. USCIS framed adjustment of status as a discretionary benefit that should be used only as an extraordinary alternative to the standard immigrant visa process at a U.S. consulate. That is a major operational shift because employment-based green card cases commonly rely on in-country Form I-485 filing after an approved immigrant petition, and consular processing can involve additional delays and travel burdens.

hackernews · tlhunter · May 22, 21:27 · [Discussion](https://news.ycombinator.com/item?id=48241890)

**Background**: There are two main paths to a green card for many applicants mentioned here: adjustment of status inside the United States, and consular processing at a U.S. consulate abroad. For many employment-based immigrants already working in the U.S., adjustment of status has been the practical route because it lets them continue living and often working in the country while the case proceeds. H-1B is especially relevant because it is commonly used by skilled workers and is treated as a dual-intent visa, meaning holders may pursue permanent residency. The new USCIS policy narrows that long-standing practice by saying in-country adjustment should generally be reserved for extraordinary circumstances.

<details><summary>References</summary>
<ul>
<li><a href="https://www.uscis.gov/newsroom/news-releases/us-citizenship-and-immigration-services-will-grant-adjustment-of-status-only-in-extraordinary">U.S. Citizenship and Immigration Services Will Grant ‘Adjustment of Status’ Only in Extraordinary Circumstances | USCIS</a></li>
<li><a href="https://en.wikipedia.org/wiki/H-1B_visa">H-1B visa - Wikipedia</a></li>
<li><a href="https://www.uscis.gov/green-card/green-card-eligibility/green-card-for-employment-based-immigrants">Green Card for Employment-Based Immigrants | USCIS</a></li>

</ul>
</details>

**Discussion**: The discussion was overwhelmingly alarmed, with many commenters arguing that applying from inside the U.S. is not a loophole but the only workable path for legal immigrants on H, J, or O visas. People highlighted family disruption, years-long consular backlogs, and the risk that skilled workers may decide the U.S. is no longer worth the uncertainty. A few comments broadened the debate to long-term quality-of-life and tax considerations, but the dominant sentiment was that the policy is reckless and highly destabilizing.

**Tags**: `#immigration-policy`, `#tech-workforce`, `#us-politics`, `#hacker-news`, `#legal-process`

---

<a id="item-8"></a>
## [AI Memory Demand Is Raising Device Prices](https://simonwillison.net/2026/May/22/memory-shortage/#atom-everything) ⭐️ 7.0/10

The post argues that surging AI demand for HBM is taking a much larger share of limited DRAM wafer capacity, rising from about 2% historically to an expected 20% by the end of 2026. As manufacturers prioritize higher-margin HBM for GPUs, supply for DDR and LPDDR used in PCs and phones tightens, pushing up consumer electronics prices. This matters because AI infrastructure spending is no longer affecting only data centers; it is now reshaping the cost structure of mainstream electronics. The impact is especially important for low-cost devices such as sub-$100 smartphones, which are highly price-sensitive in markets including Africa and South Asia. HBM uses advanced 3D-stacked DRAM packaging and, as cited in the post, a single gigabyte of HBM can consume more than three times the wafer capacity of a gigabyte of DDR or LPDDR. With only a few major memory manufacturers left and a history of avoiding overexpansion, the industry has limited incentive to add enough new capacity to quickly relieve shortages.

rss · Simon Willison · May 22, 22:01

**Background**: HBM, or High Bandwidth Memory, is a type of DRAM that stacks memory dies vertically to deliver much higher bandwidth for AI and high-performance GPUs. DDR is the mainstream memory used in desktops and servers, while LPDDR is a low-power variant designed for mobile devices such as smartphones and tablets. In semiconductor manufacturing, wafer capacity is finite, so shifting more production toward one memory type can reduce output available for others. Recent industry tracking has also described an ongoing global memory shortage tied to AI-driven demand and constrained supply.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/DDR_SDRAM">DDR SDRAM - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#semiconductors`, `#memory`, `#consumer electronics`, `#hardware economics`

---

<a id="item-9"></a>
## [FTC Fines Firms Over Fake “Active Listening” Ads](https://simonwillison.net/2026/May/22/ftc-active-listening/#atom-everything) ⭐️ 7.0/10

The FTC said Cox Media Group, MindSift, and 1010 Digital Works will pay nearly $1 million to settle charges that they misled customers about an AI-powered “Active Listening” marketing service. According to the FTC, the companies claimed smart devices listened to conversations in real time for ad targeting, but the service actually did not use voice data and instead resold email lists from data brokers. This is a notable enforcement action at the intersection of AI marketing, privacy, and consumer protection, because it challenges sensational claims about surveillance-based ad tech. It also signals that burying supposed consent in app terms of service is not enough for invasive data practices, which could affect how adtech and AI products are marketed going forward. The FTC complaints said the firms not only falsely described the product as using real-time listening, but also misrepresented consumer opt-in and the service’s ability to place ads in the customer’s desired locations. The regulator further argued that if the product had actually collected voice data from inside homes as advertised, doing so without adequate consent could itself violate Section 5 of the FTC Act.

rss · Simon Willison · May 22, 04:48

**Background**: The controversy began after a 2024 Cox Media Group pitch deck promoted “Active Listening” as a way to capture “real-time intent data” from smart devices and combine it with behavioral data for advertising. That claim resonated because many consumers already suspect phones and smart speakers are secretly listening to them, even though such fears are often amplified by confusing or misleading adtech marketing. In practice, behavioral targeting usually relies on existing signals such as app activity, identifiers, and brokered data rather than literal live microphone surveillance. The FTC’s action therefore serves both as a consumer protection case and as a correction to a persistent public myth about how targeted advertising works.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emarketer.com/content/cox-media-active-listening-pitch-deck-ad-targeting-privacy">‘ Active Listening ’ pitch deck prompts questions about ad targeting...</a></li>
<li><a href="https://captaincompliance.com/education/ftc-cox-media-group-active-listening-ai-fine/">The FTC's $930,000 Active Listening ... - Captain Compliance</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#privacy`, `#adtech`, `#FTC`, `#consumer protection`

---

<a id="item-10"></a>
## [Datasette Agent brings chat to data exploration](https://simonwillison.net/2026/May/21/datasette-agent/#atom-everything) ⭐️ 7.0/10

Simon Willison announced the first release of Datasette Agent on May 21, 2026, as an extensible AI assistant for Datasette. It adds conversational querying over Datasette-hosted data, and with the datasette-agent-charts plugin it can also generate charts from query results. This release connects Datasette's data publishing and exploration workflow with Willison's LLM tooling, making natural-language analysis more accessible to developers and analysts working with SQLite-backed datasets. It also extends the Datasette plugin model into AI-assisted data exploration, which could encourage a broader ecosystem of specialized tools. The live demo at agent.datasette.io uses Gemini 3.1 Flash-Lite, which Willison describes as cheap, fast, and capable of writing SQLite queries. The initial plugin set includes chart generation powered by Observable Plot, and the demo shows the assistant translating a natural-language question into a concrete SQL query before answering.

rss · Simon Willison · May 21, 19:52

**Background**: Datasette is an open-source tool for exploring, analyzing, and publishing data as an interactive website and API, with a strong focus on SQLite and plugin-based extensibility. Willison's LLM project is a Python library and CLI for working with many different large language models through both remote APIs and locally run models. Datasette Agent combines those two projects so a model can interact with structured data inside the Datasette environment.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette : An open source multi-tool for exploring and publishing data</a></li>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/ llm : Access large language models from the...</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-agent/">Datasette Agent , an extensible AI assistant for... - Datasette Blog</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#Datasette`, `#developer tools`, `#data analysis`, `#Python`

---

<a id="item-11"></a>
## [GitHub Open-Sources Copilot for Eclipse](https://github.blog/changelog/2026-05-21-github-copilot-for-eclipse-is-open-source) ⭐️ 7.0/10

GitHub announced that its Copilot plugin for Eclipse is now open source. The code has been published on GitHub under the MIT license, making the Eclipse integration publicly accessible. This matters because open-sourcing the Eclipse plugin gives developers and organizations more transparency into how the integration works and allows them to inspect, modify, or contribute to it. It is also a notable step for the Eclipse ecosystem, which remains important in many enterprise Java workflows and can benefit from broader access to AI coding assistance tooling. The announcement specifically says the plugin is available under the MIT license, which is a permissive open-source license. However, the post is brief and does not provide deeper technical details about architecture, supported features, or whether the underlying Copilot service itself has changed.

rss · GitHub Blog Changelog · May 21, 23:50

**Background**: GitHub Copilot is an AI coding assistant that integrates into development environments to provide code suggestions and related assistance while a developer works. Eclipse is a long-standing integrated development environment, especially common in Java and enterprise settings. Open-sourcing a plugin typically means the client-side integration code is publicly available, but it does not necessarily mean the hosted AI models or backend services behind the product are open source.

**Tags**: `#GitHub Copilot`, `#Open Source`, `#Eclipse`, `#Developer Tools`, `#AI Coding Assistants`

---

<a id="item-12"></a>
## [Jira workflows get a formal Turing-completeness proof](https://seriot.ch/computation/jira.html) ⭐️ 7.0/10

An article on seriot.ch gives a formal proof for a long-running folklore claim that Jira workflows are Turing-complete. Instead of just joking that Jira can do anything, it shows how Jira workflow behavior can simulate a Turing-complete computational model. This is a technically interesting result because Turing-completeness claims are common in programming folklore, but formal proofs are much rarer. It also highlights how workflow and automation systems can become unexpectedly expressive, which is amusing in Jira’s case but relevant more broadly for understanding the power and complexity of business-process tools. By the standard definition, a system is Turing-complete if it can simulate a universal Turing machine or an equivalent model of computation. The article’s contribution is specifically the missing proof step behind the folklore claim, not a new Jira product feature, and the result is mostly a computation-theory curiosity rather than practical guidance for Jira users.

reddit · r/programming · Dull_Replacement8890 · May 23, 14:31 · [Discussion](https://www.reddit.com/r/programming/comments/1tli2gg/jira_is_turingcomplete/)

**Background**: Turing-completeness means a system can compute anything that a Turing machine can compute, assuming enough time and memory. In practice, people often use the term loosely for languages, games, query systems, or automation tools that can encode arbitrary logic. Jira is best known as an issue-tracking and workflow platform, and its workflow and automation features let users define state transitions and rule-based behavior, which is why people have long joked that it is effectively a programming environment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Turing_completeness">Turing completeness - Wikipedia</a></li>
<li><a href="https://www.atlassian.com/software/jira/guides/automation/overview">Jira Automation: Basics & Common Use Cases | Atlassian</a></li>

</ul>
</details>

**Discussion**: The comment thread is mostly amused and exasperated, leaning into the joke that Jira is computationally powerful yet still painful for ordinary workflow tasks. Several commenters riff on familiar Jira frustrations, while others celebrate the proof as the kind of absurd but delightful result that might inspire even more stunts, like trying to run Doom in Jira.

**Tags**: `#computation-theory`, `#turing-completeness`, `#jira`, `#programming-languages`, `#reddit-discussion`

---

<a id="item-13"></a>
## [Modern C++ Lock-Free Queue Walkthrough](https://jaysmito.dev/blog/blog/04-fast-lockfree-queues/) ⭐️ 7.0/10

A new technical blog post explains how to build a fast lock-free queue from scratch in modern C++, focusing on concurrency design and performance-sensitive implementation details. The post also sparked discussion about alternative queue designs, memory ordering choices, and hazard pointer usage. Lock-free queues are a core building block in low-latency and highly concurrent systems, so clear implementation walk-throughs are useful for systems programmers who need both speed and correctness. The discussion is especially valuable because lock-free code often fails in subtle ways when memory ordering or memory reclamation is handled incorrectly. The community comments highlight a major design tradeoff between linked-node queues and fixed-size ring buffers, with the latter often being simpler and faster in single-producer or single-consumer scenarios. A technically important note from the discussion is that some atomic operations may not need the strongest seq_cst ordering, and that acquire semantics can be sufficient in parts of hazard pointer protection.

reddit · r/programming · Beginning-Safe4282 · May 22, 21:51 · [Discussion](https://www.reddit.com/r/programming/comments/1tkx5r7/building_a_fast_lockfree_queue_in_modern_c_from/)

**Background**: Lock-free data structures aim to make progress without using traditional mutex locks, typically by relying on atomic operations such as compare-and-swap. In C++, correctness depends heavily on memory ordering rules, because relaxed, acquire, release, and seq_cst semantics control what other threads are allowed to observe. Queue implementations also need to handle memory reclamation safely, since removing nodes can otherwise introduce hazards such as use-after-free or ABA-related issues.

<details><summary>References</summary>
<ul>
<li><a href="https://stackoverflow.com/questions/70512371/are-memory-orders-for-each-atomic-correct-in-this-lock-free-spsc-ring-buffer-que">c++ - Are memory orders for each atomic correct in this</a></li>
<li><a href="https://en.wikipedia.org/wiki/ABA_problem">ABA problem - Wikipedia</a></li>
<li><a href="https://stackoverflow.com/questions/40818465/explain-michael-scott-lock-free-queue-algorithm">data structures - Explain Michael & Scott lock - free queue algorithm</a></li>

</ul>
</details>

**Discussion**: The overall reaction was positive, with readers appreciating the depth of the write-up even while noting minor spelling and grammar issues. More technical comments focused on whether a fixed-size array would be faster and simpler than a linked queue, and whether some memory-ordering choices in the hazard pointer logic were stronger than necessary.

**Tags**: `#C++`, `#Lock-Free Programming`, `#Concurrency`, `#Data Structures`, `#Systems Programming`

---

<a id="item-14"></a>
## [16-byte x86 demo explained](https://hellmood.111mb.de//wake_up_16b_writeup.html) ⭐️ 7.0/10

HellMood published an in-depth write-up explaining how 16 bytes of x86 code generate both a Matrix-like textmode visual effect and music using mathematical patterns related to Sierpiński waves. According to the post, the program also ran on a real 286-era machine with MDA/Hercules-compatible hardware. This is a striking example of demoscene sizecoding, where extreme byte limits force unusually elegant combinations of math, hardware knowledge, and low-level programming. It matters to assembly programmers, retrocomputing enthusiasts, and code golfers because it shows how much behavior can emerge from tiny real-mode x86 programs, even on very old text-only display hardware. The write-up focuses on the underlying math, including the self-similar patterns associated with Sierpiński-style structures, to explain how one compact routine can drive both rhythm/melody and textmode animation. A practical caveat is that this is a niche technical deep-dive rather than a general-purpose technique, and at least one commenter questioned whether parts of the mathematical explanation were fully convincing.

reddit · r/programming · Hell__Mood · May 22, 12:06 · [Discussion](https://www.reddit.com/r/programming/comments/1tkh0w0/16_bytes_of_code_that_turn_sierpinski_waves_into/)

**Background**: The demoscene is a programming art subculture centered on producing impressive audiovisual effects under strict technical constraints, often with fixed size limits such as a few bytes or kilobytes. In that context, sizecoding refers to writing programs that achieve the most output with the fewest possible bytes. The Sierpiński triangle is a classic self-similar mathematical pattern, and related bitwise or recursive structures often appear in compact generative graphics and sound experiments. IBM's Monochrome Display Adapter offered only a monochrome 80x25 text mode rather than pixel-addressable graphics, which makes this kind of textmode effect on 286-era hardware especially notable.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sierpiński_triangle">Sierpiński triangle - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/IBM_Monochrome_Display_Adapter">IBM Monochrome Display Adapter - Wikipedia</a></li>
<li><a href="http://www.sizecoding.org/wiki/Main_Page">SizeCoding</a></li>

</ul>
</details>

**Discussion**: The overall reaction was highly enthusiastic, with several commenters praising the result as amazing, wild, and technically beautiful. The main dissent was limited: one commenter felt the mathematical section did not fully make sense, while others were especially impressed that both rhythmic and melodic structure could emerge from Sierpiński-related patterns.

**Tags**: `#x86-assembly`, `#demoscene`, `#code-golf`, `#mathematics`, `#retrocomputing`

---

<a id="item-15"></a>
## [CodeGraph brings local code graphs to AI coding tools](https://github.com/colbymchenry/codegraph) ⭐️ 7.0/10

The GitHub project colbymchenry/codegraph is trending after gaining 334 stars in 24 hours. It presents a TypeScript-based, fully local, pre-indexed code knowledge graph aimed at Claude Code and other coding agents such as Codex, Cursor, OpenCode, and Hermes Agent to reduce token use and tool-call overhead. AI coding agents often spend many tool calls exploring repositories with file reads and search operations, which increases latency and consumes context budget. A local pre-indexed graph can give those agents faster access to code structure and relationships, which is especially useful for larger codebases and privacy-sensitive workflows. The repository description explicitly emphasizes three properties: pre-indexed knowledge, fewer tool calls, and 100% local execution. Search results indicate the graph is intended to expose information such as symbol relationships and call graphs, but the provided material does not include benchmarks, architecture details, or measured token savings yet.

ossinsight · colbymchenry · May 24, 02:06

**Background**: Code intelligence tools build structured representations of a repository so software or models can answer questions beyond simple keyword search. A code knowledge graph typically links symbols, files, references, and call relationships into a queryable structure. Claude's own tool-calling documentation notes that reducing unnecessary tool interactions can lower latency and token consumption, which helps explain the appeal of pre-indexing code locally before an AI agent starts working.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/colbymchenry/codegraph">GitHub - colbymchenry/codegraph: Pre-indexed code knowledge ...</a></li>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/programmatic-tool-calling">Programmatic tool calling - Claude API Docs</a></li>
<li><a href="https://knightli.com/en/2026/05/23/codegraph-local-code-knowledge-graph-ai-coding-agent/">What is CodeGraph? A local code map for Claude Code, Codex ...</a></li>

</ul>
</details>

**Discussion**: No community discussion was provided with the news item, so there is not enough evidence to summarize user sentiment or debate.

**Tags**: `#AI coding tools`, `#code intelligence`, `#knowledge graph`, `#TypeScript`, `#developer tools`

---

<a id="item-16"></a>
## [Understand-Anything maps codebases into knowledge graphs](https://github.com/Lum1104/Understand-Anything) ⭐️ 7.0/10

The GitHub project Understand-Anything, written in TypeScript, is trending after gaining 271 stars in the past 24 hours. It presents itself as a tool that analyzes a codebase, builds an interactive knowledge graph of files, functions, classes, and dependencies, and lets users explore or question that graph through tools such as Claude Code, Codex, Cursor, Copilot, and Gemini CLI. Developers increasingly rely on AI coding assistants, but those tools often struggle to maintain a coherent mental model of a large codebase. A persistent, explorable knowledge graph could make code search, onboarding, architecture understanding, and AI-assisted Q&A more reliable across multiple assistants instead of being tied to a single IDE workflow. According to the project description and website, the tool uses a multi-agent analysis pipeline and stores a local .understand-anything/knowledge-graph.json file as a persistent map of the system. Its main differentiator is not just visualizing structure, but exposing a clickable dashboard and search/Q&A layer on top of that graph; however, the available materials do not provide benchmark data or independent validation of accuracy on large real-world repositories.

ossinsight · Lum1104 · May 24, 02:06

**Background**: Code knowledge graphs represent software artifacts such as files, functions, classes, and dependencies as nodes and relationships, giving developers a structured map of how a codebase fits together. This is useful because modern repositories are often too large for either humans or LLM-based assistants to understand from raw source files alone. The project's website emphasizes that many existing code graphs show structure but not enough explanatory context, so its goal is to make the graph teachable and queryable rather than merely visual.

<details><summary>References</summary>
<ul>
<li><a href="https://understand-anything.com/">Understand Anything — Graphs that teach the codebase</a></li>
<li><a href="https://github.com/Lum1104/Understand-Anything">GitHub - Lum1104/ Understand -Anything: Graphs that teach > graphs ...</a></li>
<li><a href="https://www.aitoolnet.com/understand-anything">Understand Anything - AI-Powered Code Understanding - Aitoolnet</a></li>

</ul>
</details>

**Tags**: `#developer-tools`, `#code-understanding`, `#knowledge-graphs`, `#ai-coding`, `#typescript`

---

<a id="item-17"></a>
## [Graphify builds codebase knowledge graphs for AI tools](https://github.com/safishamsi/graphify) ⭐️ 7.0/10

Graphify, a Python-based GitHub project from safishamsi, started trending after gaining 102 stars in 24 hours. The tool claims to turn a folder containing code, SQL schemas, scripts, documents, papers, images, and videos into a unified queryable knowledge graph for AI coding assistants such as Claude Code, Codex, Cursor, OpenCode, and Gemini CLI. AI coding assistants often struggle to answer repository-wide questions because relevant context is scattered across source files, schemas, docs, and infrastructure definitions. A unified knowledge graph could give these tools a persistent structural view of a project, improving code intelligence and reducing reliance on repeatedly stuffing raw files into model context windows. Graphify's positioning is broader than traditional code-only graph representations because it explicitly includes application code, database schema, and infrastructure-related artifacts in one graph. Based on the available information, this appears to be an early-stage developer tool with growing interest, but there is no evidence here yet of large-scale adoption, benchmark results, or a published graph schema.

ossinsight · safishamsi · May 24, 02:06

**Background**: Knowledge graphs represent entities and relationships as connected nodes and edges, which makes them useful for querying how files, symbols, schemas, and other artifacts relate to each other. In software analysis, a related concept is the code property graph, a graph representation that combines structures such as syntax and data-flow information for code querying and analysis. Other recent projects, including Noumenon and CodeGraph, reflect a broader trend toward giving AI coding agents pre-indexed, queryable views of repositories instead of relying only on raw source retrieval.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/leifericf/noumenon">leifericf/noumenon: Queryable knowledge graph for codebases ...</a></li>
<li><a href="https://pyshine.com/CodeGraph-Pre-Indexed-Code-Knowledge-Graph-AI-Coding-Agents/">CodeGraph: Pre-Indexed Code Knowledge Graph for AI ... | PyShine</a></li>
<li><a href="https://en.wikipedia.org/wiki/Code_property_graph">Code property graph - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI coding assistants`, `#knowledge graphs`, `#developer tools`, `#Python`, `#code intelligence`

---

<a id="item-18"></a>
## [Chrome DevTools arrives for AI coding agents](https://github.com/ChromeDevTools/chrome-devtools-mcp) ⭐️ 7.0/10

ChromeDevTools/chrome-devtools-mcp is a new TypeScript project from the Chrome DevTools team that exposes Chrome DevTools capabilities to coding agents. According to the project description, it acts as an MCP server and also provides a CLI so agents or users can control, inspect, debug, and analyze a live Chrome browser. This matters because AI coding assistants are increasingly expected to do more than edit code; they also need access to runtime debugging, browser inspection, and performance tooling. Backing from the official Chrome DevTools team gives the project credibility and could make browser-aware agent workflows more practical for developers using tools such as Claude, Cursor, Gemini, or Copilot. The repository is written in TypeScript and is described as “Chrome DevTools for agents.” The available project and npm descriptions emphasize reliable automation, in-depth debugging, performance analysis, and live Chrome control through MCP, but the provided news item does not include deeper implementation details or documented limitations.

ossinsight · ChromeDevTools · May 24, 02:06

**Background**: Model Context Protocol, or MCP, is a standard way for AI applications to connect to external tools and data sources. In software development, MCP has been adopted to let coding assistants access richer project context and capabilities beyond plain text prompts. Chrome DevTools is Google’s browser debugging and performance toolkit, so exposing it through an MCP server lets an agent interact with a live browser session instead of only reasoning about source code statically.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ChromeDevTools/chrome-devtools-mcp/">GitHub - ChromeDevTools/chrome-devtools-mcp: Chrome DevTools ...</a></li>
<li><a href="https://www.npmjs.com/package/chrome-devtools-mcp">chrome-devtools-mcp - npm</a></li>
<li><a href="https://openai.github.io/openai-agents-python/mcp/">Model context protocol (MCP) - OpenAI Agents SDK</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#Chrome DevTools`, `#Developer Tools`, `#TypeScript`, `#MCP`

---

<a id="item-19"></a>
## [Rust CLI proxy targets LLM token waste](https://github.com/rtk-ai/rtk) ⭐️ 7.0/10

The GitHub repository rtk-ai/rtk is trending as a Rust-based CLI proxy that claims to reduce LLM token consumption by 60-90% for common development commands. The project is presented as a single-binary, zero-dependency tool aimed at lowering the cost of LLM-powered developer workflows. LLM-assisted coding agents often spend many tokens on verbose shell output from tools like git, test runners, and package managers, so reducing that context can directly cut API cost and sometimes improve responsiveness. If rtk works as described, it could become a practical optimization layer for developers and teams building AI-assisted engineering workflows. Search results describe RTK as a thin proxy that compresses or rewrites the output of 100+ common developer commands before that output reaches the LLM, rather than changing the model itself. The current signal is still early: the repo gained 36 stars in 24 hours, with modest overall activity and no included benchmark discussion here to independently verify the 60-90% savings claim.

ossinsight · rtk-ai · May 24, 02:06

**Background**: In LLM-powered tooling, every token sent to or produced by a model can affect both cost and latency, so trimming unnecessary context is a common optimization strategy. One approach is prompt caching, which can reduce repeated input costs when prompts stay stable, while another is context reduction, which removes or compresses low-value text before it ever reaches the model. RTK appears to follow the second approach by sitting between the shell and the AI agent and transforming verbose command output into a more token-efficient form.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/arshtechpro/how-rtk-reduces-llm-token-usage-for-ai-coding-agents-2kfd">RTK: Cut Your AI Coding Bill by 80% With One CLI ... - DEV Community</a></li>
<li><a href="https://github.com/Rookie-Adventures/rtk-token">GitHub - Rookie-Adventures/rtk- token : CLI proxy that reduces LLM ...</a></li>
<li><a href="https://redis.io/blog/what-is-prompt-caching/">What Is Prompt Caching? LLM Speed & Cost Guide</a></li>

</ul>
</details>

**Tags**: `#LLM tooling`, `#Rust`, `#CLI`, `#developer tools`, `#token optimization`

---