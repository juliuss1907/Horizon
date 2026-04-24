# Horizon Daily - 2026-04-24

> From 48 items, 24 important content pieces were selected

---

1. [DeepSeek V4 Released: Open-Source 1.6T MoE with 1M Context](#item-1) ⭐️ 9.0/10
2. [OpenAI Releases GPT-5.5: First Fully Retrained Base Model Since GPT-4.5](#item-2) ⭐️ 9.0/10
3. [Claude Expands App Connectors to Personal Life Apps](#item-3) ⭐️ 7.0/10
4. [US accuses China of “industrial-scale” AI theft. China says it’s “slander.”](#item-4) ⭐️ 7.0/10
5. [Researchers Decipher 2005 Malware Predating Stuxnet, Linked to Iran Nuclear Attacks](#item-5) ⭐️ 7.0/10
6. [U.S. Soldier Charged With Using Classified Intel for Prediction Market Profit](#item-6) ⭐️ 7.0/10
7. [Orwell's 1946 Essay Why I Write Resurfaces on Hacker News](#item-7) ⭐️ 6.0/10
8. [Tolaria: Open-Source macOS App for Markdown Knowledge Management](#item-8) ⭐️ 6.0/10
9. [Keygate: Lightweight Pre-Commit Hook Blocks Secret Leaks](#item-9) ⭐️ 6.0/10
10. [OpenAI Launches Workspace Agents, Replacing Custom GPTs](#item-10) ⭐️ 6.0/10
11. [Clarity Act Explained: US Crypto Token Classification Bill](#item-11) ⭐️ 6.0/10
12. [Mantle Proposes 30K ETH Credit Facility for Aave rsETH Rescue](#item-12) ⭐️ 6.0/10
13. [Countries Move to Ban Social Media for Children](#item-13) ⭐️ 5.0/10
14. [CNT Wiring Nears Copper Conductivity Through Chemical Doping](#item-14) ⭐️ 5.0/10
15. [Complete Guide to SaaS Security and Privacy Compliance Released](#item-15) ⭐️ 5.0/10
16. [Stop Handing Over Your Entire Wallet: DTOs in .NET Explained](#item-16) ⭐️ 5.0/10
17. [Magento 2 llms.txt Tutorial: Generate AI-Ready Site Summary](#item-17) ⭐️ 5.0/10
18. [xAI Releases Grok Voice Think Fast 1.0, Claims Top Voice Benchmark](#item-18) ⭐️ 5.0/10
19. [Leak reveals new Xbox Game Pass ‘Starter Edition’ that’s part of Discord Nitro](#item-19) ⭐️ 4.0/10
20. [VAST Tests Flight Suits, Timepiece for Haven-1 Visitors](#item-20) ⭐️ 4.0/10
21. [What IEEE and ACM Codes Actually Require for AI-Assisted Work](#item-21) ⭐️ 4.0/10
22. [Gogram: Modern Go Library for Telegram MTProto Protocol](#item-22) ⭐️ 4.0/10
23. [19-Year-Old Thiel Fellow Raises $7.3M for African Super App Swoop](#item-23) ⭐️ 4.0/10
24. [KelpDAO Bridge Exploit Drains $292M in April 2026](#item-24) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [DeepSeek V4 Released: Open-Source 1.6T MoE with 1M Context](https://dev.to/owen_fox/deepseek-v4-released-open-source-16t-moe-1m-context-apache-20-and-its-already-on-the-api-14d6) ⭐️ 9.0/10

DeepSeek released V4 on April 24, 2026, featuring two MoE variants: deepseek-v4-pro (1.6T total parameters, 49B activated) and deepseek-v4-flash (284B total, 13B activated). Both models support 1M-token context with 384K max output, are fully open-source under Apache 2.0 license, and are immediately available via API at $1.74/$3.48 per million tokens for Pro. This release directly competes with GPT-5.5 on the same launch day while offering open-source weights and significantly lower pricing than competitors like Opus 4.7, GLM-5.1, or Kimi K2.6. The breakthrough in long-context efficiency—reducing KV cache to just 10% of V3.2 levels—makes 1M-token context economically viable for mainstream deployment. V4 introduces Compressed Sparse Attention (CSA), Heavily Compressed Attention (HCA), and Manifold-Constrained Hyper-Connections (mHC), enabling inference FLOPs at just 27% of V3.2 levels. The model was pre-trained on 32T+ tokens using FP4 + FP8 mixed precision. On Arena Code leaderboard, V4-Pro Thinking achieved #3 among open models with 1,456 Elo, an 88-point jump over V3.2.

rss · Dev.to · Apr 24, 04:51

**Background**: Mixture of Experts (MoE) is a neural network architecture that activates only a subset of model parameters for each input, allowing massive parameter counts without proportional computational cost. DeepSeek has pioneered cost-efficient open-source AI releases since 2025, using techniques like FP4/FP8 mixed precision training to reduce memory requirements. The 'Thinking Mode' refers to models that output chain-of-thought reasoning before final answers, similar to OpenAI's o1/o3 reasoning models.

<details><summary>References</summary>
<ul>
<li><a href="https://intuitionlabs.ai/articles/mixture-of-experts-moe-models">Understanding Mixture of Experts (MoE) Neural Networks</a></li>
<li><a href="https://qubittool.com/blog/moe-architecture-explained">Mixture of Experts (MoE) Architecture Explained [2026]: GPT-4 ...</a></li>
<li><a href="https://chat-deep.ai/docs/deepseek-thinking-mode/">DeepSeek Thinking Mode - DeepSeek AI</a></li>

</ul>
</details>

**Discussion**: The community response is overwhelmingly positive, with users praising the 'insane value deal' of frontier-level performance at a fraction of the cost. Some的好奇 about local running capabilities on consumer hardware despite the 1.6T parameter count, given that only 49B parameters are activated per token. Developers are noting immediate availability on OpenRouter with competitive Flash pricing at $0.14/$0.28 per million tokens. One user compared pelican image outputs from Flash versus Pro, finding Flash's output preferable despite its lower parameter count.

**Tags**: `#deepseek`, `#open-source`, `#mixture-of-experts`, `#large-language-models`, `#AI-agents`

---

<a id="item-2"></a>
## [OpenAI Releases GPT-5.5: First Fully Retrained Base Model Since GPT-4.5](https://dev.to/owen_fox/gpt-55-released-first-fully-retrained-base-model-since-gpt-45-1m-context-530-pricing-4nj0) ⭐️ 9.0/10

OpenAI released GPT-5.5 on April 23, 2026, as the first fully retrained base model since GPT-4.5, featuring a groundbreaking 1M-token context window and agent-oriented training objectives. The release includes two variants: GPT-5.5 Thinking at $5/$30 per million tokens and GPT-5.5 Pro at $30/$180 per million tokens. GPT-5.5 对 OpenAI 来说是一个重大的架构转变，代表了首次从零开始的重训练，而非对同一基座进行后训练迭代。100 万 token 的上下文窗口使得处理超长文档和多步骤智能体工作流程成为可能，而以智能体为导向的训练目标则使模型能够在无需人工在每个步骤重新提示的情况下完成自主任务。 The model achieves 82.7% on Terminal-Bench 2.0 (a 13-point lead over Opus 4.7), 84.9% on GDPval for knowledge work, and scores 60 on the Artificial Analysis Intelligence Index—ending a three-way tie with competitors. However, Opus 4.7 still wins on SWE-Bench Pro at 64.3% vs GPT-5.5's 58.6%, which most closely maps to fixing real GitHub issues in real codebases.

rss · Dev.to · Apr 24, 04:49

**Background**: Terminal-Bench 2.0 is a benchmark that evaluates AI agents on high-skill, long-horizon command-line tasks using realistic simulated environments. A "fully retrained base model" means the foundational neural network was trained from scratch on a new dataset, rather than taking an existing base model and applying post-training refinements—which is what previous GPT-5.x releases (5.1 through 5.4) did. Agent-oriented training objectives specifically optimize the model for multi-step task completion, tool use, and self-correction capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/terminal-bench-2-0">Terminal - Bench 2 . 0 : AI Agent Benchmark</a></li>
<li><a href="https://codingscape.com/blog/llms-with-largest-context-windows">LLMs with largest context windows</a></li>

</ul>
</details>

**Tags**: `#GPT-5.5`, `#OpenAI`, `#Large Language Models`, `#AI Agents`, `#Model Releases`

---

<a id="item-3"></a>
## [Claude Expands App Connectors to Personal Life Apps](https://www.theverge.com/ai-artificial-intelligence/917871/anthropic-claude-personal-app-connectors) ⭐️ 7.0/10

Anthropic has expanded Claude's app connectors to include popular personal apps like Spotify, Uber, Uber Eats, Audible, AllTrails, TripAdvisor, Instacart, and TurboTax, moving beyond previous work-focused integrations such as Microsoft apps. This expansion represents a significant shift in AI assistant strategy, moving from enterprise and work productivity toward everyday personal activities. It positions Claude as more deeply embedded in users' daily lives, potentially competing with other AI assistants for personal use cases. The new connectors dynamically surface relevant apps during conversations based on user queries. In addition to the personal apps mentioned, existing work-related connectors continue to be supported, creating a comprehensive ecosystem spanning both professional and personal domains.

rss · The Verge · Apr 23, 22:27

**Background**: App connectors allow AI assistants like Claude to access and interact with external applications, enabling users to complete tasks across different platforms through natural language. Anthropic initially focused on enterprise integrations with Microsoft apps, but this expansion to personal apps marks a strategic pivot toward consumer markets. Dynamic app surfacing means the AI intelligently determines which app to suggest based on conversation context rather than requiring manual selection.

**Discussion**: Tech observers note this represents a natural evolution for AI assistants moving from workplace to personal contexts. Some express enthusiasm about the convenience of managing everyday tasks through a single AI interface, while others raise privacy concerns about granting AI access to personal apps like financial (TurboTax) and location-based (Uber, AllTrails) services.

**Tags**: `#anthropic`, `#claude`, `#ai-assistants`, `#product-launch`, `#app-integration`

---

<a id="item-4"></a>
## [US accuses China of “industrial-scale” AI theft. China says it’s “slander.”](https://arstechnica.com/tech-policy/2026/04/us-accuses-china-of-industrial-scale-ai-theft-china-says-its-slander/) ⭐️ 7.0/10

The US has accused China of conducting 'industrial-scale' AI theft, prompting China to label the accusations as slander, with potential sanctions threatening the planned Trump-Xi summit.

rss · Ars Technica · Apr 23, 21:45

**Tags**: `#AI Policy`, `#US-China Relations`, `#Tech Geopolitics`, `#Export Controls`, `#AI Competition`

---

<a id="item-5"></a>
## [Researchers Decipher 2005 Malware Predating Stuxnet, Linked to Iran Nuclear Attacks](https://www.wired.com/story/fast16-malware-stuxnet-precursor-iran-nuclear-attack/) ⭐️ 7.0/10

Cybersecurity researchers have finally deciphered Fast16, a mysterious malware created in 2005 that is capable of silently tampering with calculation and simulation software, and appears to be a precursor to Stuxnet likely deployed by the US or an ally against Iran's nuclear program. This discovery reveals that state-sponsored cyber sabotage capabilities existed earlier than previously known, providing crucial insight into the evolution of cyber weapons used against critical infrastructure. It demonstrates a sophisticated early capability to quietly manipulate scientific calculations before the more infamous Stuxnet attack. Researchers Kamluk and Guerrero-Saade identified three potential types of physical simulation software that Fast16 was designed to tamper with, including Modelo Hidrodinâmico (hydrodynamic model). The malware could subtly alter computational results to cause undetected errors in simulations without leaving obvious traces.

rss · Wired · Apr 23, 22:00

**Background**: Stuxnet was discovered in 2010 and was widely attributed to the US and Israel as the first publicly known cyberweapon designed to physically destroy critical infrastructure, specifically Iran's uranium enrichment centrifuges. However, Fast16 demonstrates that sophisticated cybersabotage capabilities existed at least five years earlier. The malware represents a shift from simple data-destroying wiper attacks to targeted computational manipulation of scientific software.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wired.com/story/fast16-malware-stuxnet-precursor-iran-nuclear-attack/">Newly Deciphered Sabotage Malware May Have Targeted Iran’s ...</a></li>
<li><a href="https://conzit.com/post/unveiling-fast16-a-precursor-to-cyber-sabotage-in-iran">Unveiling Fast16: A Precursor to Cyber Sabotage in Iran</a></li>
<li><a href="https://en.wikipedia.org/wiki/Stuxnet">Stuxnet - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The cybersecurity community has reacted with fascination to this revelation, praising the researchers for finally uncovering a piece of cyber warfare history that had remained mysterious for over 15 years. Many see this as evidence that state actors were conducting sophisticated digital attacks long before such operations became public knowledge.

**Tags**: `#cybersecurity`, `#nation-state malware`, `#cyber warfare`, `#Stuxnet`, `#Iran nuclear program`

---

<a id="item-6"></a>
## [U.S. Soldier Charged With Using Classified Intel for Prediction Market Profit](https://www.justice.gov/opa/pr/us-soldier-charged-using-classified-information-profit-prediction-market-bets) ⭐️ 7.0/10

U.S. Army Master Sergeant Gannon Ken Van Dyke has been charged with using classified military intelligence about the operation that captured Venezuelan President Nicolás Maduro to bet approximately $33,000 on Polymarket, generating roughly $409,000 in profit. He allegedly attempted to conceal his identity by deleting accounts and routing funds through a foreign cryptocurrency vault, and now faces multiple criminal charges including violations of the Commodity Exchange Act. This case marks the first U.S. arrest for insider trading on a prediction market, establishing a legal precedent that could reshape how prediction markets are regulated and how insider trading laws apply to decentralized platforms. The charges have prompted the Trump administration to review federal employees' participation in prediction markets, potentially leading to new policy restrictions across the government. Van Dyke faces five counts: unlawful use of confidential government information, theft of nonpublic government information, commodities fraud, wire fraud, and monetary transactions in property derived from unlawful activity. The CFTC has filed a parallel civil complaint against him, and the U.S. Attorney for the Southern District of New York announced the charges on April 23, 2026.

telegram · ahboyashreads · Apr 24, 04:10

**Background**: Polymarket is a decentralized prediction market platform built on Ethereum and Polygon blockchains, where users speculate on real-world event outcomes by buying yes/no shares. The CFTC regulates derivatives and commodities markets under the Commodity Exchange Act, and has been increasingly scrutinizing prediction markets as they can function similarly to financial instruments. This case highlights the legal ambiguity around prediction markets and how existing securities and commodity laws may apply to them.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coingecko.com/learn/what-is-polymarket-decentralized-prediction-markets-guide">What Is Polymarket? A Guide to Decentralized Prediction ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Commodity_Futures_Trading_Commission">United States Commodity Futures Trading Commission - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters raised questions about the distinction between insider trading on prediction markets versus leaking classified information, with one user noting the cynicism around whether this prosecution protects Peter Thiel's Polymarket investment. Several commenters drew parallels to congressional stock trading, with one stating it would be 'demoralizing' that soldiers face prosecution for betting while those giving orders profit from insider knowledge. Some noted the irony that prediction markets are 'working as intended' by detecting market manipulation.

**Tags**: `#prediction-markets`, `#polymarket`, `#crypto-regulation`, `#insider-trading`, `#national-security`

---

<a id="item-7"></a>
## [Orwell's 1946 Essay Why I Write Resurfaces on Hacker News](https://www.orwellfoundation.com/the-orwell-foundation/orwell/essays-and-other-works/why-i-write/) ⭐️ 6.0/10

George Orwell's 1946 essay 'Why I Write' was shared on Hacker News, where it garnered 87 points and 18 substantive comments from readers relating the essay's themes to their own creative experiences. This essay's continued relevance demonstrates the timeless nature of questions about creative motivation. The lively discussion among tech community members shows that the tension between artistic vision and political purpose remains a vital concern for writers across disciplines. Orwell identifies four motivations for writing: political purpose, historical impulse, aesthetic gratification, and sheer ego. The essay's famous description of writing as a 'horrible, exhausting struggle' driven by an irresistible 'demon' particularly resonated with commenters sharing their own experiences.

hackernews · RyanShook · Apr 24, 02:26

**Background**: George Orwell (1903-1950) was the pen name of English novelist and journalist Eric Arthur Blair. 'Why I Write,' written in 1946 during his recovery from tuberculosis, serves as both a personal reflection and a literary manifesto. The essay was written shortly before he began work on Nineteen Eighty-Four, the dystopian novel for which he is most famous.

**Discussion**: Commenters overwhelmingly related to Orwell's 'demon' metaphor, describing their own compulsive relationship with creative work. One reader noted the struggle to fuse political purpose with artistic craft, while another observed how Orwell's awareness of letting political propaganda weaken storytelling applied to Nineteen Eighty-Four. The overall sentiment expressed gratitude for rediscovering such resonant writing.

**Tags**: `#literature`, `#writing`, `#george-orwell`, `#creativity`, `#classic-essay`

---

<a id="item-8"></a>
## [Tolaria: Open-Source macOS App for Markdown Knowledge Management](https://github.com/refactoringhq/tolaria) ⭐️ 6.0/10

Tolaria is a newly released open-source macOS app for managing large Markdown knowledge bases, created by Luca who writes the refactoring.fm newsletter and manages over 10,000 notes across 6 years of content creation. The app is offline-first, file-based, with first-class git versioning support, AI integration capabilities, and opinionated note organization features including types and relationships. In a crowded knowledge management space with established players like Obsidian, Tolaria differentiates itself through its combination of offline-first architecture, git-versioned plain Markdown files, and AI-context optimization—addressing a growing need for tools that work well with modern AI agents while keeping data ownership in user hands. The app uses a consistent frontmatter schema for all notes and includes an "inbox" concept for capturing thoughts. User wkcheng reported a sorting bug where notes cannot be properly sorted by last modified date after performing a git commit, likely caused by preserving file modification times during vault import. A similar project called Sig shares architectural overlap with Tolaria.

hackernews · lucaronin · Apr 23, 22:01

**Background**: Offline-first architecture treats local functionality as the default experience, ensuring users can access and modify their data even without internet connectivity. Git provides distributed version control with complete history tracking, including author, date, and change notes. Markdown is a lightweight markup language commonly used for notes and documentation, and its plain text nature makes it ideal for git-based versioning and AI processing.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@jusuftopic/offline-first-architecture-designing-for-reality-not-just-the-cloud-e5fd18e50a79">Offline - First Architecture : Designing for Reality, Not Just... | Medium</a></li>
<li><a href="https://www.atlassian.com/git/tutorials/what-is-version-control">What is version control | Atlassian Git Tutorial</a></li>

</ul>
</details>

**Discussion**: Community response shows measured interest with constructive feedback. Users appreciate the "inbox" concept and see potential for using Tolaria on project docs folders. Smadam9 highlights architectural overlap with their own project Sig, noting different workflow focuses. Dewey's question about mobile sync reflects a common concern in the file-based knowledge management space, while wkcheng's sorting bug report provides actionable technical feedback that could impact real-world usage.

**Tags**: `#macos`, `#knowledge-management`, `#markdown`, `#git`, `#open-source`, `#productivity`

---

<a id="item-9"></a>
## [Keygate: Lightweight Pre-Commit Hook Blocks Secret Leaks](https://dev.to/yuichi/keygate-a-fast-pre-commit-guardrail-against-secret-leaks-1i7o) ⭐️ 6.0/10

Keygate is a new Git pre-commit hook that scans only staged added lines to detect secrets before they enter repository history, combining rule-based detection, entropy analysis, and context scoring with a block/warn/ignore scoring system. As AI coding agents generate larger diffs at higher speed, the risk of accidentally committing secrets increases significantly. Keygate provides a fast, offline local guardrail optimized for the developer workflow, targeting the critical moment right before `git commit` succeeds. Keygate detects secrets using format-specific rules for AWS keys, OpenAI keys, GitHub tokens, Slack tokens, PEM keys, JWTs, Stripe keys, and URLs with embedded credentials. It scores findings as block (70+), warn (40-69), or ignore (<40), and includes structured JSON output for AI agent integration and inline ignore comments as escape hatches for false positives.

rss · Dev.to · Apr 24, 05:06

**Background**: Git pre-commit hooks are scripts that run automatically before a commit is finalized, allowing developers to catch issues like missing semicolons or (in this case) committed secrets before they enter history. Once a secret is committed, it remains in Git history even if deleted later, making pre-commit detection critical for security. Keygate is designed to be fast enough for hook execution while remaining offline and focused on staged changes rather than full repository scans.

<details><summary>References</summary>
<ul>
<li><a href="https://pre-commit.com/">pre-commit</a></li>
<li><a href="https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks">Git - Git Hooks</a></li>

</ul>
</details>

**Tags**: `#security`, `#git-hooks`, `#secret-detection`, `#devops`, `#developer-tools`

---

<a id="item-10"></a>
## [OpenAI Launches Workspace Agents, Replacing Custom GPTs](https://dev.to/harsh_m04/openai-quietly-killed-custom-gpts-this-week-2eek) ⭐️ 6.0/10

OpenAI has launched Workspace Agents, a successor to Custom GPTs that integrates directly into enterprise tools like Slack. Powered by Codex, these shared team agents can run on schedules or be human-triggered, operate within organizational permission scopes, and are now available for Business, Enterprise, and Edu plans with free access until May 6 before switching to credit-based pricing. This shift addresses the fundamental failure mode of custom AI tools: not capability, but distribution. By embedding agents where work actually happens—Slack, ticketing systems, CRM—rather than requiring users to remember to open a separate chat interface, OpenAI is betting that workspace integration will drive the adoption that the GPT Store never achieved. This represents a significant pivot from personal customization to team automation as the default use case. Workspace Agents differ from Custom GPTs in being shared rather than personal, scheduled or permissioned rather than purely on-demand, and fundamentally scoped as "headcount" rather than novelty tools. Early evidence from implementations at companies like Upswing suggests usage can increase by 20x when agents live in existing messaging channels rather than behind separate portals. The agents can be configured using plain language through the agent builder chat interface.

rss · Dev.to · Apr 24, 04:50

**Background**: Custom GPTs were launched as part of OpenAI's vision for personal AI customization, allowing anyone to build tailored assistants and share them through the GPT Store. However, the GPT Store failed to gain traction because users don't navigate to a separate interface to get work done—they work in Slack, their ticketing system, or their CRM. This distribution problem is well-known in software: tools that require behavior change rarely get adopted at scale. Codex is OpenAI's coding agent, launched as a research preview in May 2025, designed to handle software engineering tasks like writing features, fixing bugs, and reviewing code.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI | OpenAI</a></li>
<li><a href="https://openai.com/academy/workspace-agents/">Workspace agents | OpenAI</a></li>
<li><a href="https://maverickstudios.net/2026/04/23/openai-unveils-workspace-agents-a-successor-to-custom-gpts-for-enterprises-that-can-plug-directly-into-slack-salesforce-and-more/">OpenAI unveils Workspace Agents , a successor to custom GPTs for...</a></li>

</ul>
</details>

**Discussion**: The author argues that within six months, "workspace agent" will become the default unit of internal automation, and the GPT Store will become a footnote. The core insight—that distribution is the real product problem, not capability—resonates with industry experience showing that AI tools succeed when they integrate into existing workflows rather than demanding new ones. However, some might note this pattern is well-established in software distribution rather than a novel breakthrough.

**Tags**: `#OpenAI`, `#AI Agents`, `#Product Strategy`, `#Workspace Tools`, `#AI Integration`

---

<a id="item-11"></a>
## [Clarity Act Explained: US Crypto Token Classification Bill](https://x.com/0xLouisT/status/2047345868324384951?s=20) ⭐️ 6.0/10

The Clarity Act (H.R.3633) introduces a comprehensive regulatory framework that categorizes every crypto token into either security, digital commodity, or permitted payment stablecoin, determining whether the SEC or CFTC exercises oversight. The bill also establishes a 20% decentralization threshold—requiring no single party to control more than 20% of a token—to reclassify tokens from securities to digital commodities. This legislation represents the most significant attempt to date to resolve the regulatory ambiguity that has plagued the US crypto industry, where projects have faced inconsistent enforcement actions from both the SEC and CFTC. If passed, it would provide legal clarity for tokens like BTC, ETH, SOL, and XRP, potentially unlocking CFTC-regulated trading, bank custody services, and clearer DeFi developer protections. Under the Act, digital commodities would fall under lighter CFTC regulation with reduced disclosure obligations and simpler custody requirements compared to SEC-regulated securities. The bill also bans retail central bank digital currencies (CBDCs) and passive stablecoin yield while protecting self-custody rights. To become law, it must clear bipartisan Senate committee votes, reconciliation, and obtain 60 Senate votes before year-end 2025.

telegram · ahboyashreads · Apr 24, 04:10

**Background**: The US regulatory approach to cryptocurrencies has been fragmented for years, with the SEC under Gary Gensler asserting that most tokens are securities subject to its jurisdiction, while the CFTC argued that commodities like Bitcoin and Ether fall under its purview. In March 2026, both agencies issued a joint interpretive release naming 16 specific tokens—including Bitcoin, Ether, Solana, and XRP—as digital commodities. The Digital Asset Market Clarity Act of 2025 aims to codify this distinction into law, providing the industry with regulatory certainty that has been requested by both traditional financial institutions and crypto-native companies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.congress.gov/bill/119th-congress/house-bill/3633">H.R.3633 - Digital Asset Market Clarity Act of 2025</a></li>
<li><a href="https://www.jenner.com/en/news-insights/client-alerts/sec-and-cftc-issue-landmark-joint-interpretation-on-crypto-asset-classification">SEC and CFTC Issue Landmark Joint Interpretation on Crypto Asset Classification | Jenner & Block LLP | Law Firm</a></li>
<li><a href="https://www.banking.senate.gov/newsroom/majority/the-facts-the-clarity-act">The Facts: The CLARITY Act | United States Committee on ...</a></li>

</ul>
</details>

**Tags**: `#crypto-regulation`, `#clarity-act`, `#sec-cftc-oversight`, `#token-classification`, `#stablecoins`, `#defi`

---

<a id="item-12"></a>
## [Mantle Proposes 30K ETH Credit Facility for Aave rsETH Rescue](https://forum.mantle.xyz/t/discussion-mip-34-strategic-credit-facility-for-aave-dao-rseth-exploit/9417) ⭐️ 6.0/10

Mantle Treasury has proposed lending up to 30,000 ETH to Aave DAO at approximately Lido rate + 1% APR for up to 36 months. The loan aims to address the $292 million bad debt created by the KelpDAO exploit, which drained 116,500 rsETH through a LayerZero bridge vulnerability on April 18, 2026. This proposal represents an unprecedented cross-protocol liquidity rescue mechanism in DeFi, transforming treasury management into strategic crisis response. If approved, it would establish Mantle as a "first-response liquidity partner" while accelerating Aave's native deployment on Mantle Network. The facility is collateralized through a 5-of-5 multisig controlling 5% of Aave protocol revenue plus $11M+ in Aave tokens. Mantle will earn the Lido + 1% yield on its treasury capital, effectively turning idle assets into productive income while supporting protocol-level crisis resolution.

telegram · ahboyashreads · Apr 24, 04:10

**Background**: rsETH is a Liquid Restaking Token (LST) issued by KelpDAO, a decentralized restaking protocol built on EigenLayer. EigenLayer enables ETH stakers to restake their assets across multiple validation tasks, creating a shared security model for blockchain networks. On April 18, 2026, attackers exploited a vulnerability in KelpDAO's LayerZero bridge to mint 116,500 unbacked rsETH worth approximately $292 million, representing roughly 18% of the token's circulating supply. Mantle Network is an Ethereum Layer 2 solution using ZK validity proofs and was the first L2 to adopt EigenDA technology.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coindesk.com/tech/2026/04/19/2026-s-biggest-crypto-exploit-kelp-dao-hit-for-usd292-million-with-wrapped-ether-stranded-across-20-chains">Kelp DAO exploited for $292 million with wrapped ether ...</a></li>
<li><a href="https://www.mantle.xyz/">Mantle Network | Building the Liquidity Chain of the Future</a></li>
<li><a href="https://consensys.io/blog/eigenlayer-decentralized-ethereum-restaking-protocol-explained">EigenLayer: Decentralized Ethereum Restaking Protocol Explained | Consensys</a></li>
<li><a href="https://defiprime.com/kelpdao-rseth-exploit">The KelpDAO rsETH Exploit: $292M Minted From a 1-of-1 Bridge</a></li>

</ul>
</details>

**Tags**: `#DeFi`, `#Treasury Management`, `#Aave`, `#Liquidity Provision`, `#Governance`

---

<a id="item-13"></a>
## [Countries Move to Ban Social Media for Children](https://techcrunch.com/2026/04/23/social-media-ban-children-countries-list/) ⭐️ 5.0/10

Australia became the first country to implement a ban on social media for children under 16 in late 2025, effective December 10. The ban mandates that social media platforms take reasonable steps to prevent Australian minors from accessing their services, with enforcement under amendments to the Online Safety Act 2021. This policy marks a significant shift in global tech regulation, as Australia leads a worldwide movement that could reshape how major social media platforms operate. The success or failure of age verification enforcement in Australia may influence similar legislation in the UK, EU, and other countries currently developing comparable frameworks. Platforms face fines up to AUD 50 million for non-compliance, and the legislation requires "reasonable" age assurance measures rather than mandating specific technologies. The UK is also implementing age verification requirements under its Online Safety Act, with a survey showing 22% of children aged 8-17 lie about their age to access platforms.

rss · TechCrunch · Apr 23, 21:33

**Background**: The legislative movement stems from growing concerns about mental health impacts, cyberbullying, and exposure to harmful content among young users. Australia amended its Online Safety Act 2021 in late 2024 to introduce a Social Media Minimum Age framework, and conducted an Age Assurance Technology Trial to evaluate verification methods. The UK similarly passed its Online Safety Act requiring platforms to implement stronger age verification measures coming into force in 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://www.infrastructure.gov.au/sites/default/files/documents/social-media-minimum-age-and-age-assurance-trial-fact-sheet-july-2025.pdf">Social Media Minimum Age – Fact sheet</a></li>
<li><a href="https://www.bbc.com/news/articles/cn4v52ezx17o">Do 'much, much more' on age verification , social media apps told</a></li>
<li><a href="https://www.aph.gov.au/About_Parliament/Parliamentary_departments/Parliamentary_Library/Research/Research_Papers/2024-25/Children_online_safety">Children, online safety, and age verification – Parliament of ...</a></li>

</ul>
</details>

**Tags**: `#social-media-regulation`, `#child-safety`, `#policy`, `#australia`, `#tech-law`

---

<a id="item-14"></a>
## [CNT Wiring Nears Copper Conductivity Through Chemical Doping](https://arstechnica.com/science/2026/04/researchers-get-carbon-nanotube-wiring-to-conduct-more-like-copper/) ⭐️ 5.0/10

Researchers have enhanced carbon nanotube (CNT) wiring conductivity by chemically doping CNT bundles, boosting current-carrying capacity by up to tenfold, with some samples achieving over 15 times improvement over baseline. However, the material degrades over time, tempering enthusiasm for near-term applications. This progress brings carbon nanotube wiring closer to practical use in electronics manufacturing as a potential alternative to copper interconnects. If the degradation issue can be solved, it could help address the physical limitations that copper wiring faces as chip feature sizes continue shrinking. The conductivity enhancement comes from chemical doping of CNT bundles, with single-walled carbon nanotubes theoretically capable of achieving ~100 MS/m compared to copper's 59.6 MS/m. The primary obstacle remains the material's tendency to degrade over time, which limits its viability for long-term electronic applications.

rss · Ars Technica · Apr 23, 21:22

**Background**: Carbon nanotube interconnects refer to the proposed use of carbon nanotubes as wiring between elements in integrated circuits. CNTs are essentially single atomic layer graphite sheets rolled up into seamless cylinders, offering superior electrical conductivity properties and mechanical strength compared to copper. As traditional silicon chip manufacturing approaches physical scaling limits, researchers have been exploring carbon-based materials as next-generation interconnect solutions.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/science/2026/04/researchers-get-carbon-nanotube-wiring-to-conduct-more-like-copper/">Carbon nanotube wiring gets closer to competing with copper</a></li>
<li><a href="https://www.mdpi.com/1996-1073/16/9/3665">Carbon Nanotubes as an Alternative to Copper Wires in ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Carbon_nanotubes_in_interconnects">Carbon nanotubes in interconnects - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#materials science`, `#nanotechnology`, `#carbon nanotubes`, `#electronics`, `#research`

---

<a id="item-15"></a>
## [Complete Guide to SaaS Security and Privacy Compliance Released](https://dev.to/jayata_pal_b5961a26521741/security-and-privacy-compliance-for-saas-startups-a-complete-guide-to-tools-costs-and-3f8b) ⭐️ 5.0/10

A comprehensive guide has been published on dev.to covering security and privacy compliance frameworks for SaaS startups, detailing SOC 2, ISO 27001, and GDPR requirements along with tool selection strategies, cost breakdowns, and step-by-step implementation roadmaps. For SaaS startups targeting enterprise customers, compliance certifications like SOC 2 Type II are no longer optional—they're deal prerequisites. This guide provides a practical roadmap for lean teams to build compliance postures that support growth rather than stall it, potentially saving months of trial-and-error navigation. The guide specifies typical SOC 2 Type II timelines of 9–18 months with costs of $15,000–$40,000, while ISO 27001 ranges from 6–18 months at $20,000–$60,000+. GDPR penalties can reach €20 million or 4% of global annual turnover. Key insight: SOC 2 Type II compliance naturally addresses most GDPR Article 32 technical requirements.

rss · Dev.to · Apr 24, 05:10

**Background**: Security and privacy compliance for SaaS companies operates across three interconnected layers: legal/regulatory requirements (GDPR, CCPA, HIPAA), security frameworks (SOC 2, ISO 27001, NIST), and contractual obligations from enterprise customers (DPAs, BAAs). SOC 2, developed by the AICPA, evaluates controls across five Trust Service Criteria: Security, Availability, Processing Integrity, Confidentiality, and Privacy. Unlike SOC 2's audit report, ISO 27001 results in a certificate valid for three years with annual surveillance audits.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cookieyes.com/blog/gdpr-software-requirements/">GDPR Software Requirements: A Complete Guide</a></li>
<li><a href="https://fastercapital.com/content/Compliance-requirements--Navigating-Compliance-Requirements-in-SaaS.html">Compliance requirements : Navigating Compliance ... - FasterCapital</a></li>

</ul>
</details>

**Tags**: `#security`, `#compliance`, `#saas`, `#privacy`, `#startups`

---

<a id="item-16"></a>
## [Stop Handing Over Your Entire Wallet: DTOs in .NET Explained](https://dev.to/m_orkhan/stop-handing-over-your-entire-wallet-dtos-in-net-explained-1eg8) ⭐️ 5.0/10

A beginner-friendly explanation of Data Transfer Objects in .NET using a relatable analogy about not handing over your wallet to illustrate why APIs should only return necessary data.

rss · Dev.to · Apr 24, 05:03

**Tags**: `#dotnet`, `#dto`, `#api-design`, `#software-architecture`, `#backend-development`

---

<a id="item-17"></a>
## [Magento 2 llms.txt Tutorial: Generate AI-Ready Site Summary](https://dev.to/angeo/llmstxt-for-magento-2-what-it-is-why-it-matters-and-how-to-generate-it-in-5-minutes-58fi) ⭐️ 5.0/10

A tutorial demonstrates how to generate an llms.txt file for Magento 2 stores, explaining how this plain-text file hosted at yourstore.com/llms.txt provides AI assistants with structured summaries of your catalog, categories, products, and CMS pages. As AI assistants like ChatGPT and Claude increasingly influence shopping decisions, having an llms.txt file ensures your store can be discovered and cited correctly in AI-generated responses, giving e-commerce operators a competitive advantage in the emerging AI-driven search landscape. The specification defined at llmstxt.org defines llms.txt as a markdown file providing background information and links to detailed content. Some AI systems like Perplexity actively read llms.txt while others like GPTBot primarily rely on page content and Product schema JSON-LD instead.

rss · Dev.to · Apr 24, 04:48

**Background**: Traditional search engines like Google crawl websites over time and build indexes, but AI assistants operate differently — they parse pre-existing knowledge or structured data in milliseconds rather than crawling in real time. The llms.txt format serves as a README.md for e-commerce sites, allowing AI systems to understand site structure and content without live crawling.

<details><summary>References</summary>
<ul>
<li><a href="https://llmstxt.org/">The /llms.txt file – llms-txt</a></li>
<li><a href="https://www.semrush.com/blog/llms-txt/">What Is LLMs.txt & Should You Use It? - Semrush</a></li>

</ul>
</details>

**Tags**: `#llms.txt`, `#Magento 2`, `#AI integration`, `#SEO`, `#e-commerce`

---

<a id="item-18"></a>
## [xAI Releases Grok Voice Think Fast 1.0, Claims Top Voice Benchmark](https://x.ai/news/grok-voice-think-fast-1) ⭐️ 5.0/10

xAI released grok-voice-think-fast-1.0, a new flagship voice agent model developed in partnership with Starlink. The model claims the #1 position on the τ-voice Bench leaderboard, which tests voice agents under real-world conditions including noise, accents, interruptions, and live turn-taking. The Think Fast 1.0 release marks a significant shift in the competitive voice AI landscape, positioning xAI as a formidable challenger to established players like OpenAI and Google. By ranking first in comprehensive real-world benchmarks and emphasizing cost-effectiveness, xAI is targeting enterprise customers seeking high-performance yet affordable voice solutions for customer support and sales applications. The model prioritizes low response latency and organic conversational ability while maintaining accuracy and tool orchestration capabilities. xAI describes it as a "step change" designed specifically for complex, ambiguous, multi-step workflows across enterprise applications.

telegram · ahboyashreads · Apr 24, 04:10

**Background**: Voice agents are AI systems capable of processing speech input, generating responses, and producing voice output in real-time. The τ-voice Bench is a benchmark that evaluates voice agents under challenging real-world conditions, testing their ability to handle noise, diverse accents, interruptions, and dynamic conversation flow. xAI, founded by Elon Musk, has been rapidly expanding its AI product portfolio, and the Think Fast release represents its most significant entry into the voice AI market to date.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/news/grok-voice-think-fast-1">Grok Voice Think Fast 1.0 - x.ai</a></li>
<li><a href="https://aitoolsrecap.com/Blog/grok-voice-mode-xai-2026-features-how-to-use">Grok Voice Mode 2026 — Features, Access & How It Works</a></li>
<li><a href="https://kingy.ai/uncategorized/grok-voice-think-fast-1-0-xais-new-flagship-voice-agent-takes-the-crown/">Grok Voice Think Fast 1.0: xAI’s New Flagship ... - kingy.ai</a></li>

</ul>
</details>

**Discussion**: The announcement has generated excitement among AI enthusiasts and developers, with one prominent post calling it a "complete game-changer" and emphasizing that it represents an incremental update rather than a fundamentally new approach. Community members are particularly interested in how Think Fast 1.0 performs against existing voice AI solutions like GPT-4o and Gemini.

**Tags**: `#ai`, `#grok`, `#xai`, `#voice`, `#product-announcement`

---

<a id="item-19"></a>
## [Leak reveals new Xbox Game Pass ‘Starter Edition’ that’s part of Discord Nitro](https://www.theverge.com/news/917880/xbox-game-pass-starter-edition-discord-nitro-bundle) ⭐️ 4.0/10

A leaked listing reveals that Microsoft is bundling a new Xbox Game Pass 'Starter Edition' with Discord Nitro, offering access to over 50 games from the Game Pass library.

rss · The Verge · Apr 23, 22:36

**Tags**: `#gaming`, `#xbox`, `#discord`, `#subscription-services`, `#microsoft`

---

<a id="item-20"></a>
## [VAST Tests Flight Suits, Timepiece for Haven-1 Visitors](https://arstechnica.com/space/2026/04/vast-reveals-flight-suit-tests-timepiece-for-commercial-space-station/) ⭐️ 4.0/10

VAST announced testing of flight suits and a specially designed timepiece for visitors to Haven-1, the world's first commercial space station scheduled to launch in May 2026. The announcement was made in April 2026 as a teaser for the upcoming station's crew accommodations and visitor provisions. This announcement marks another step toward normalizing commercial space travel and space tourism. As private companies develop dedicated infrastructure for civilian visitors, the space industry is gradually transitioning from a government-dominated domain to a commercial ecosystem with accessible facilities. Haven-1 is designed to host crews of four for two-week missions aboard a single-module outpost. The station will launch aboard a SpaceX Falcon 9 rocket and will serve as a proof-of-concept before scaling up to the larger, multi-module Haven-2. The flight suits and timepiece are part of VAST's effort to provide comfortable and functional attire for visitors in microgravity environments.

rss · Ars Technica · Apr 23, 22:14

**Background**: VAST is a California-based aerospace company founded in 2021 by Jed McCaleb. The company is developing Haven-1 as the world's first commercial space station, with the goal of accelerating access to space for research and commercial purposes. This initiative comes as NASA plans to decommission the ISS, creating an opening for private alternatives to provide ongoing human spaceflight capabilities in low Earth orbit.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nasaspaceflight.com/2026/04/vast-astronaut-flight-suit-docking-adapter/">Vast unveils Astronaut Flight Suit and... - NASASpaceFlight.com</a></li>
<li><a href="https://en.wikipedia.org/wiki/Space_station">Space station - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/realogic-analytics-inc-_commercialrealestate-nasa-space-activity-7404215905733365760-Xd4B">#commercialrealestate #nasa # space #outerspace #iss...</a></li>

</ul>
</details>

**Tags**: `#commercial space station`, `#spaceflight fashion`, `#VAST`, `#Haven-1`, `#private space industry`

---

<a id="item-21"></a>
## [What IEEE and ACM Codes Actually Require for AI-Assisted Work](https://dev.to/alexrebula/the-ethics-of-ai-assisted-work-what-the-professional-codes-actually-say-35dd) ⭐️ 4.0/10

Developer Alex Rebula explores what professional codes from IEEE and ACM actually require regarding AI use in work, finding that both require disclosure and accountability but do not prohibit AI use entirely. The article outlines three core obligations: understanding your output, disclosing AI use in published work, and ensuring humans remain fully responsible while AI cannot be listed as an author. This analysis matters because it cuts through the noise of the AI ethics debate to show what professional bodies actually mandate, offering concrete guidance rather than vague opinions. Developers and professionals can understand their actual obligations rather than guessing based on social media discourse. The IEEE Software Engineering Code of Ethics and ACM Code of Ethics require disclosure when AI is used, but neither code prohibits AI use in professional work. The author also notes a practical example: an LLM defaulted to American English for Australian clients because most training data is American, demonstrating why professional oversight remains necessary.

rss · Dev.to · Apr 24, 04:53

**Background**: The IEEE (Institute of Electrical and Electronics Engineers) and ACM (Association for Computing Machinery) are the two largest professional organizations in computing and software engineering. Both have published codes of ethics that establish standards for professional conduct. IEEE's Software Engineering Code of Ethics specifically addresses obligations software engineers have regarding their work products and professional responsibilities. As AI tools become increasingly prevalent in professional settings, these existing codes provide a framework for determining appropriate use and disclosure requirements.

**Discussion**: No community discussion is available for this article as the content appears truncated before reader comments can be displayed.

**Tags**: `#AI ethics`, `#professional conduct`, `#software development`, `#career advice`, `#AI tools`

---

<a id="item-22"></a>
## [Gogram: Modern Go Library for Telegram MTProto Protocol](https://dev.to/classccai/gogram-27eo) ⭐️ 4.0/10

Gogram, a newly released Go library for Telegram's MTProto protocol, was announced on dev.to, providing a modern framework for interacting with the Telegram API through user accounts or bot identities. For Go developers building Telegram integrations, Gogram offers an alternative to existing libraries like tdlib or python-telegram-bot, with concurrent support and generics-powered design potentially offering better performance and cleaner API patterns. Gogram requires Go 1.18 or later to utilize Go generics, and is currently in stable release stage with acknowledged potential bugs. The library is installed via `go get -u github.com/amarnathcjd/gogram/telegram`.

rss · Dev.to · Apr 24, 04:48

**Background**: MTProto is Telegram's proprietary protocol designed for secure, fast communication between clients and servers. As of version 4.6, major Telegram clients use MTProto 2.0. Building native MTProto implementations in different programming languages allows developers to create custom Telegram clients without relying on official libraries.

<details><summary>References</summary>
<ul>
<li><a href="https://core.telegram.org/mtproto">MTProto Mobile Protocol</a></li>

</ul>
</details>

**Tags**: `#golang`, `#mtproto`, `#telegram`, `#go-libraries`, `#open-source`

---

<a id="item-23"></a>
## [19-Year-Old Thiel Fellow Raises $7.3M for African Super App Swoop](https://fortune.com/2026/04/23/19-year-old-thiel-fellow-7-3-million-african-super-app-swoop/) ⭐️ 4.0/10

19-year-old Thiel Fellow Kofi Gen A has secured $7.3 million in seed funding for his African super app startup Swoop. The funding round signals strong investor confidence in youth-led ventures targeting underserved African markets. The large funding amount for a teenager leading an African super app underscores growing venture capital interest in emerging markets and youth entrepreneurship. It also highlights how the Thiel Fellowship continues to identify and support unconventional founders who bypass traditional education. Swoop aims to be a super app combining financial services and commerce on a single platform, though the Fortune article provides limited technical detail about the app's architecture or engineering approach. The article focuses primarily on the founder's age and funding milestone rather than technical implementation or innovation.

telegram · ahboyashreads · Apr 24, 04:10

**Background**: The Thiel Fellowship, founded by billionaire Peter Thiel in 2011, provides $200,000 to young people who leave college to build ventures. Super apps are platforms that integrate multiple services—such as payments, messaging, and e-commerce—into a single ecosystem, a model popularized by apps like WeChat in China. Africa's tech ecosystem has seen rapid growth as startups address gaps in digital payments and financial access across the continent.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Thiel_Fellowship">Thiel Fellowship - Wikipedia</a></li>
<li><a href="https://thielfellowship.org/">Thiel Fellowship</a></li>
<li><a href="https://www.elluminatiinc.com/super-apps-examples/">Top 6 Successful Super Apps Examples in Market – 2026</a></li>

</ul>
</details>

**Tags**: `#startup-funding`, `#africa-tech`, `#thiel-fellowship`, `#entrepreneurship`, `#venture-capital`

---

<a id="item-24"></a>
## [KelpDAO Bridge Exploit Drains $292M in April 2026](https://www.chainalysis.com/blog/kelpdao-bridge-exploit-april-2026/) ⭐️ 4.0/10

KelpDAO suffered a major security exploit in April 2026, with approximately $292 million drained from its bridge protocol, making it the largest cryptocurrency exploit recorded in 2026 to date. Chainalysis published an analysis examining the on-chain evidence and the specific monitoring challenges this type of exploit presents. This incident underscores the persistent vulnerability of cross-chain bridges in DeFi, a category that has now lost over $2.8 billion to exploits historically. The scale of this attack and its technical complexity will likely drive renewed scrutiny of bridge security models and monitoring capabilities across the industry. The exploit resulted in wrapped ether (presumably a wrapped version of ETH used for cross-chain transfers) being stranded across approximately 20 different blockchain networks, significantly complicating asset recovery efforts. Chainalysis noted that this class of exploit requires a fundamentally different approach to on-chain monitoring compared to standard DeFi attacks.

telegram · ahboyashreads · Apr 24, 04:10

**Background**: KelpDAO is a liquid restaking protocol operating within the EigenLayer ecosystem, providing users with rsETH (restaked Ether) that enables access to staking rewards and DeFi opportunities. Bridge protocols facilitate asset transfers between different blockchain networks, and their complex multi-chain architecture has historically made them attractive targets for attackers. The founders of KelpDAO previously established Stader Labs, a multi-chain liquid staking platform.

<details><summary>References</summary>
<ul>
<li><a href="https://www.chainalysis.com/blog/kelpdao-bridge-exploit-april-2026/">Inside the KelpDAO Bridge Exploit</a></li>
<li><a href="https://www.coindesk.com/tech/2026/04/19/2026-s-biggest-crypto-exploit-kelp-dao-hit-for-usd292-million-with-wrapped-ether-stranded-across-20-chains">Kelp DAO exploited for $292 million with wrapped ether stranded...</a></li>
<li><a href="https://cleansky.io/blog/bridges-weakest-link-defi/">Bridges : The Weakest Link in DeFi — $2.8B Lost... | CleanSky Blog</a></li>

</ul>
</details>

**Tags**: `#crypto-exploit`, `#defi-security`, `#blockchain`, `#bridge-hack`, `#security-incident`

---

