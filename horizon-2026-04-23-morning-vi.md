# Horizon Daily - 2026-04-23

> From 93 items, 40 important content pieces were selected

---

1. [We found a stable Firefox identifier linking all your private Tor identities](#item-1) ⭐️ 8.0/10
2. [Alberta startup sells no-tech tractors for half price](#item-2) ⭐️ 7.0/10
3. [Apple fixes bug that cops used to extract deleted chat messages from iPhones](#item-3) ⭐️ 7.0/10
4. [Over-editing refers to a model modifying code beyond what is necessary](#item-4) ⭐️ 7.0/10
5. [Technical, cognitive, and intent debt](#item-5) ⭐️ 7.0/10
6. [Parallel agents in Zed](#item-6) ⭐️ 7.0/10
7. [Surveillance Pricing: Exploiting Information Asymmetries](#item-7) ⭐️ 7.0/10
8. [RFK Jr. won't back CDC director on vaccines as agency scraps positive data](#item-8) ⭐️ 7.0/10
9. [5 AI Models Tried to Scam Me. Some of Them Were Scary Good](#item-9) ⭐️ 7.0/10
10. [Workspace Agents in ChatGPT](#item-10) ⭐️ 6.0/10
11. [Google turns Chrome into an AI co-worker for the workplace](#item-11) ⭐️ 6.0/10
12. [Our newsroom AI policy](#item-12) ⭐️ 6.0/10
13. [Anthropic tested removing Claude Code from the Pro plan](#item-13) ⭐️ 6.0/10
14. [Google unveils two new TPUs designed for the "agentic era"](#item-14) ⭐️ 6.0/10
15. [Website streamed live directly from a model](#item-15) ⭐️ 5.0/10
16. [US Treasury Secretary Bessent says Gulf, Asian allies request swap lines](#item-16) ⭐️ 5.0/10
17. [Prediction market Kalshi docks three US candidates for betting on own races](#item-17) ⭐️ 5.0/10
18. [Tesla just increased its capex to $25B. Here’s where the money is going.](#item-18) ⭐️ 5.0/10
19. [Hands on with X’s new AI-powered custom feeds](#item-19) ⭐️ 5.0/10
20. [Google Cloud launches two new AI chips to compete with Nvidia](#item-20) ⭐️ 5.0/10
21. [Crypto scam lures ships into Strait of Hormuz, falsely promising safe passage](#item-21) ⭐️ 5.0/10
22. [Lawsuit: Nintendo is getting tariff refunds—its customers should get them instead](#item-22) ⭐️ 5.0/10
23. [You want your Moon landings in HD? So does NASA—here's how it's happening.](#item-23) ⭐️ 5.0/10
24. [Sam Altman’s Orb Company Promoted a Bruno Mars Partnership That Doesn't Exist](#item-24) ⭐️ 5.0/10
25. [🚨 GSR LAUNCHES MULTI-ASSET CRYPTO ETF WITH STAKING](#item-25) ⭐️ 5.0/10
26. [📊 ETHENA USDe SUPPLY DROPS $800M IN 3 DAYS](#item-26) ⭐️ 5.0/10
27. [🚨AAVE STABLECOIN BORROW RATES SPIKE AFTER KELP DAO EXPLOIT](#item-27) ⭐️ 5.0/10
28. [Billionaire backer sues Trump family's crypto firm over alleged extortion](#item-28) ⭐️ 4.0/10
29. [Warner Bros and Paramount merger could reshape US media landscape](#item-29) ⭐️ 4.0/10
30. [Did UK universities pay to ‘spy’ on pro‑Palestine students?](#item-30) ⭐️ 4.0/10
31. [Ukraine restarts Russian oil to Europe, unblocking 90-billion-euro EU loan](#item-31) ⭐️ 4.0/10
32. [How Iran and the United States Are Planning Their Next Moves](#item-32) ⭐️ 4.0/10
33. [Europe Might Sit Out In An Indo-Pacific War — But It Can’t Escape the Fallout](#item-33) ⭐️ 4.0/10
34. [New Low-Cost Cruise Missile Features Tomahawk-Like Range](#item-34) ⭐️ 4.0/10
35. [F-15EX Buy Was Just Doubled By The USAF, Which Makes Perfect Sense](#item-35) ⭐️ 4.0/10
36. [Ford Class Review Puts Navy’s Future Carrier Plans Into Question](#item-36) ⭐️ 4.0/10
37. [Google updates Workspace to make AI your new office intern](#item-37) ⭐️ 4.0/10
38. [AI Overviews are coming to your Gmail at work](#item-38) ⭐️ 4.0/10
39. [Scientists Gave Cocaine to Salmon and You Will Absolutely Believe What Happened Next](#item-39) ⭐️ 4.0/10
40. [🇮🇷🇺🇸🇮🇱Hãng thông tấn IRIB: Iran đang xem xét nhiều khía cạnh khác nhau của việc ](#item-40) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [We found a stable Firefox identifier linking all your private Tor identities](https://fingerprint.com/blog/firefox-tor-indexeddb-privacy-vulnerability/) ⭐️ 8.0/10

Researchers at Fingerprint.com discovered a Firefox vulnerability that exploits IndexedDB to create a persistent identifier, allowing websites to track and link Tor Browser users' private identities across different sessions even when using fresh circuits. This vulnerability specifically targets Tor Browser users who rely on the browser's isolation features for anonymity. By successfully linking private identities, this flaw undermines the core privacy promise of Tor and could expose journalists, activists, or whistleblowers to serious risks. The tracking mechanism is process-scoped rather than origin-scoped, meaning the identifier persists as long as the Firefox process remains running. The vulnerability affects how IndexedDB behaves across Tor circuits, allowing websites to detect when the same Firefox process is reused even with different identity assumptions.

hackernews · danpinto · Apr 22, 17:35

**Background**: IndexedDB is a browser storage API that allows web applications to persistently store data locally. Unlike cookies, IndexedDB data can survive clearing browser history. Tor Browser is designed to provide anonymity by isolating sessions and routing traffic through multiple relays. Browser fingerprinting exploits unique characteristics of a user's browser and device to track them without traditional cookies. This discovery represents a new attack vector that circumvents Tor's session isolation.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/IndexedDB_API/Using_IndexedDB">Using IndexedDB - Web APIs | MDN - MDN Web Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Evercookie">Evercookie - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters raised interesting questions about the business ethics of vulnerability disclosure—one pointed out the apparent conflict for a fingerprinting company to report vulnerabilities rather than monetize them. Others discussed Firefox's multi-process architecture and whether the 2021 redesign adequately addresses this issue. Practical advice emerged: users should exit Tor Browser completely between sessions and avoid mixing different uses within a single session.

**Tags**: `#browser-security`, `#tor-browser`, `#privacy`, `#fingerprinting`, `#vulnerability-research`

---

<a id="item-2"></a>
## [Alberta startup sells no-tech tractors for half price](https://wheelfront.com/this-alberta-startup-sells-no-tech-tractors-for-half-price/) ⭐️ 7.0/10

An Alberta startup is selling simplified tractors without GPS, sensors, or locked software at roughly half the price of conventional farm equipment, sparking debate about corporate lock-in in agriculture. This directly challenges the increasingly proprietary approach of major agricultural equipment manufacturers like John Deere, tapping into growing frustration over locked ecosystems and contributing to the broader right-to-repair movement that affects multiple industries. The tractors prioritize repairability and user control over smart features. Commenters note the business model sustainability concerns since durable machines could saturate the market quickly—farmers have kept tractors running for 60-80 years. Some predict regulatory pushback from established manufacturers.

hackernews · Kaibeezy · Apr 22, 16:29

**Background**: Modern agricultural equipment from major manufacturers increasingly uses proprietary software that restricts repairs to authorized dealers, preventing farmers from self-maintenance. John Deere has been particularly controversial for digital restrictions that prevent independent repair. The right-to-repair movement has gained significant traction, with farmers, legislators, and consumer advocates pushing for laws that require manufacturers to provide repair documentation and parts access to equipment owners. Open-source alternatives represent a growing philosophical response to corporate lock-in across industries.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/business-64206913">US farmers win right to repair John Deere equipment</a></li>
<li><a href="https://thecounter.org/right-to-repair-elizabeth-warren-john-deere/">As farmers fight for the right to repair their tractors, an antitrust...</a></li>
<li><a href="https://www.goodnewsnetwork.org/flood-of-right-to-repair-bills-signals-diy-watershed-moment/">Flood of ‘ Right to Repair ’ Bills For Autos, Phones, and Tractors Equals...</a></li>

</ul>
</details>

**Discussion**: Community commenters express strong appreciation for vintage machinery and shared experiences with classic tractors, with one describing a 1970s Massey Ferguson as 'wonderful' to drive. There's consensus that the tech itself isn't bad, but lock-in and lack of choice are the real problems. Some predict political interference from established manufacturers, while others see opportunity for OEMs who build open, vibrant ecosystems. The desire for low-tech simplicity extends beyond tractors to cars and other consumer goods.

**Tags**: `#agriculture`, `#right-to-repair`, `#corporate-lock-in`, `#no-tech`, `#openness`

---

<a id="item-3"></a>
## [Apple fixes bug that cops used to extract deleted chat messages from iPhones](https://techcrunch.com/2026/04/22/apple-fixes-bug-that-cops-used-to-extract-deleted-chat-messages-from-iphones/) ⭐️ 7.0/10

Apple has patched a vulnerability that allowed law enforcement agencies to recover "deleted" chat messages from iPhone notification caches stored in a local SQLite database managed by iOS itself. This fix addresses a critical privacy flaw where end-to-end encrypted messaging apps could be bypassed through iOS notification handling, undermining user expectations of message deletion. It highlights the broader tension between convenience features and privacy protection in mobile operating systems. The bug specifically failed to remove cached notifications from iOS's internal SQLite database when an app was deleted, meaning notification text persisted independently of the app's own deletion protocols. Users concerned about this vector must manually change notification settings to prevent text storage, as the underlying issue of notifications being stored outside encrypted apps remains architectural.

hackernews · cdrnsf · Apr 22, 20:27

**Background**: iOS stores notification data in SQLite databases that persist independently of app storage. When apps like Signal send end-to-end encrypted messages, the notification content is decrypted locally for display on lock screens and notification centers, then cached by iOS in a database the app has no control over. Apple's Push Notification service (APNs) also handles notification routing, meaning content may pass through Apple's servers before reaching devices. Mobile forensics tools commonly extract evidence from SQLite databases, including deleted or marked records, making notification caches a valuable data source for investigations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.spacedaily.com/sd-n-the-push-notification-backdoor-how-ios-architecture-undermines-end-to-end-encryption-by-design/">The Push Notification Backdoor: How iOS Architecture ...</a></li>
<li><a href="https://blog.clix.so/how-push-notification-delivery-works-internally/">How Push Notification Delivery Works Internally: APNs and FCM ...</a></li>
<li><a href="https://www.systoolsgroup.com/forensics/sqlite/ios.html">Forensics Acquisition of Data from iOS Devices – iPhone, iPad & iPod</a></li>

</ul>
</details>

**Discussion**: Commenters emphasize that this bug represents only part of a deeper privacy issue: notification text storage outside encrypted apps is architectural, not incidental. The discussion highlights that Apple and Google's central role in notification handling creates server-side surveillance risks. Several commenters argue that end-to-end encryption fundamentally cannot protect data once it reaches the OS layer for rendering, as readable text must exist somewhere in the system—this may be an inherent trade-off rather than a solvable problem.

**Tags**: `#privacy`, `#ios-security`, `#mobile-forensics`, `#apple`, `#encryption`

---

<a id="item-4"></a>
## [Over-editing refers to a model modifying code beyond what is necessary](https://nrehiew.github.io/blog/minimal_editing/) ⭐️ 7.0/10

Discussion of 'over-editing' behavior in AI coding agents, where models make unnecessary code changes, with community members sharing workflows for managing this through project-specific training and debate over when aggressive vs. conservative editing is appropriate.

hackernews · pella · Apr 22, 17:51

**Tags**: `#ai-coding-agents`, `#software-development`, `#claude-code`, `#code-quality`, `#ai-workflow`

---

<a id="item-5"></a>
## [Technical, cognitive, and intent debt](https://martinfowler.com/fragments/2026-04-02.html) ⭐️ 7.0/10

Martin Fowler extends the concept of technical debt to include cognitive debt and intent debt, proposing that cognitive bottlenecks between software artifacts represent a significant but often overlooked challenge in modern development. As AI agents increasingly assist with software development, cognitive and intent debt may pose greater risks to long-term software health than traditional technical debt. This framework helps teams identify where shared understanding breaks down across the development pipeline. The framework maps transitions between artifacts: outcome → requirements → spec → acceptance criteria → executable proof → review. A referenced Wharton research paper on 'cognitive surrender' has faced community criticism for appearing AI-generated and lacking peer review, raising questions about the evidentiary foundation of some claims.

hackernews · theorchid · Apr 22, 16:11

**Background**: Technical debt, originally coined by Ward Cunningham in 1992, refers to the implied cost of additional rework caused by choosing expedient solutions over better approaches. Cognitive debt describes knowledge that exists only in developers' minds rather than being properly externalized in documentation or code. Intent debt refers to the erosion or absence of explicit rationale that guides how both humans and AI agents evolve a system.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.22106">[2603.22106] From Technical Debt to Cognitive and Intent Debt: Rethinking Software Health in the Age of AI</a></li>
<li><a href="https://margaretstorey.com/blog/2026/02/09/cognitive-debt/">How Generative and Agentic AI Shift Concern from Technical Debt to Cognitive Debt</a></li>
<li><a href="https://newsletter.getdx.com/p/cognitive-debt-the-hidden-risk-in">Cognitive debt: The hidden risk in AI-driven software development</a></li>

</ul>
</details>

**Discussion**: Community members expressed concern that the cited Wharton research paper appears entirely AI-generated and lacks peer review, undermining its credibility. Others shared practical LLM prompting strategies to address cognitive debt by guiding agents toward minimal code changes and senior-dev instincts. One commenter created an Excalidraw visualization mapping cognitive bottlenecks across artifacts, while another challenged whether abstraction layers inherently create intent debt.

**Tags**: `#software-engineering`, `#technical-debt`, `#cognitive-load`, `#llm-agents`, `#developer-productivity`

---

<a id="item-6"></a>
## [Parallel agents in Zed](https://zed.dev/blog/parallel-agents) ⭐️ 7.0/10

Zed announced a parallel agents feature that allows multiple AI agents to work simultaneously within Git worktrees, enabling agent-agnostic workflows across multiple repositories with lifecycle hooks for automated environment setup and teardown. This feature positions Zed as a serious contender in the AI-assisted coding space, offering a unique approach that is editor-agnostic and supports multi-repository workflows, potentially attracting developers who want flexibility in their AI tooling choices. The implementation leverages Git worktrees to create isolated working environments, and includes lifecycle hooks that can automatically set up local configurations, duplicate databases like Postgres for testing, and clean up resources when worktrees are closed. This approach differs from first-party AI integrations like Claude/Codex by remaining agent-agnostic.

hackernews · ajeetdsouza · Apr 22, 17:38

**Background**: Zed is an open-source, high-performance code editor written in Rust by Nathan Sobo, one of the creators of Atom. Git worktrees are a Git feature that enables multiple working directories for the same repository, allowing developers to work on different branches simultaneously without stashing changes or switching contexts. The concept of AI agents in coding environments refers to autonomous or semi-autonomous AI systems that can execute tasks like writing code, running commands, or managing files with varying levels of human oversight.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zed_(text_editor)">Zed (text editor) - Wikipedia</a></li>
<li><a href="https://git-scm.com/docs/git-worktree">Git - git-worktree Documentation</a></li>
<li><a href="https://zed.dev/">Zed — Love your editor again</a></li>

</ul>
</details>

**Discussion**: Community reaction is largely positive, with users praising the workflow potential especially when combined with lifecycle hooks for environment management. Some users express excitement about the agent-agnostic approach, though others note they still prefer manual oversight of AI-generated code due to quality concerns. One user mentioned Warp launched a similar feature a week earlier but found Zed's implementation more logical. Performance concerns were raised regarding TypeScript language server integration.

**Tags**: `#zed-editor`, `#ai-agents`, `#developer-tools`, `#parallel-processing`, `#ai-assisted-coding`

---

<a id="item-7"></a>
## [Surveillance Pricing: Exploiting Information Asymmetries](https://lpeproject.org/blog/surveillance-pricing-exploiting-information-asymmetries/) ⭐️ 7.0/10

The Roosevelt Institute's Economic Justice Clinic published an analysis examining how surveillance pricing uses personal data to determine individual customers' maximum willingness to pay, enabling companies to extract the highest possible profit from each consumer while raising concerns about algorithmic discrimination and digital redlining. This practice affects virtually every online shopper, as the information asymmetry between corporations and consumers undermines fair market competition. It represents a fundamental shift in how prices are determined, moving from transparent market forces to opaque algorithmic decision-making based on personal characteristics. Surveillance pricing operates by inferring emotional and financial states from location, demographics, browsing patterns, and shopping history. Historical examples date back to the late 1990s, when companies like Orbitz (2012) and earlier tech firms displayed higher-priced options based on device type, assuming Mac users were less price-sensitive than Windows users.

hackernews · cainxinth · Apr 22, 17:13

**Background**: Surveillance pricing is a form of dynamic pricing that has been compared to personalized price gouging. While proponents suggest it could function like a progressive tax enabling price equity, critics raise concerns about consumer privacy, digital redlining, and undermining fundamental price discovery mechanisms. The practice has evolved from early experiments in the 1990s to sophisticated AI-driven systems that can infer willingness to pay in near real-time based on behavioral signals.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Surveillance_pricing">Surveillance pricing</a></li>
<li><a href="https://epic.org/issues/consumer-privacy/surveillance-pricing/">Surveillance Pricing – EPIC – Electronic Privacy Information ...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion revealed sharp ethical critiques and valuable historical context. Commenter teeray argued that computer-enabled discrimination is morally equivalent to human discrimination based on protected characteristics, calling it "abhorrent." Commenter bigiain provided firsthand technical experience from the late 1990s, confirming such practices existed before modern AI. However, commenter 2009mobile constructively disagreed with classifying Uber's surge pricing as surveillance pricing, arguing it primarily aims to increase supply in a two-sided network rather than maximize profit through personal data exploitation.

**Tags**: `#surveillance-capitalism`, `#price-discrimination`, `#algorithmic-ethics`, `#information-asymmetry`, `#tech-society`

---

<a id="item-8"></a>
## [RFK Jr. won't back CDC director on vaccines as agency scraps positive data](https://arstechnica.com/health/2026/04/rfk-jr-doubles-down-on-vaccine-meddling-as-cdc-junks-scientific-study/) ⭐️ 7.0/10

Robert F. Kennedy Jr. has refused to publicly support CDC Director Dr. Makary amid ongoing controversy. The CDC also discarded a study showing positive vaccine data, which has raised concerns about scientific integrity and political interference in public health decisions. This development threatens to undermine public trust in immunization programs and scientific institutions. The clash between Kennedy's vaccine-skeptical stance and the CDC's scientific recommendations could reshape national vaccine policy and affect healthcare outcomes for millions. The discarded study reportedly contained positive findings about vaccine safety or efficacy. Kennedy's refusal to back Dr. Makary signals ongoing tension within the administration over how to approach immunization policy.

rss · Ars Technica · Apr 22, 20:06

**Background**: The CDC (Centers for Disease Control and Prevention) is the leading US federal agency responsible for disease prevention and public health protection. Robert F. Kennedy Jr. has historically advocated for vaccine skepticism and was recently involved with HHS in reviewing vaccine policies. Dr. Makary, the current CDC Director, is a medical researcher known for his evidence-based approach to public health. Their disagreement highlights the ongoing tension between scientific integrity and political considerations in US public health governance.

**Tags**: `#public health policy`, `#vaccines`, `#CDC`, `#healthcare politics`, `#government overreach`

---

<a id="item-9"></a>
## [5 AI Models Tried to Scam Me. Some of Them Were Scary Good](https://www.wired.com/story/ai-model-phishing-attack-cybersecurity/) ⭐️ 7.0/10

A WIRED investigation testing five AI models for phishing capabilities reveals concerning results, with some models demonstrating sophisticated social engineering skills that have experts worried about AI-enabled cyberattacks.

rss · Wired · Apr 22, 18:00

**Tags**: `#AI safety`, `#cybersecurity`, `#phishing`, `#AI ethics`, `#machine learning risks`

---

<a id="item-10"></a>
## [Workspace Agents in ChatGPT](https://openai.com/index/introducing-workspace-agents-in-chatgpt/) ⭐️ 6.0/10

OpenAI has launched Workspace Agents in ChatGPT, enabling business teams to create customized AI agents that can autonomously perform tasks like preparing reports, writing code, and responding to messages. This represents a shift from ChatGPT as a chatbot to a team automation platform, potentially affecting how businesses deploy AI for workflow automation and competing with tools like Notion's custom agents. Workspace Agents are powered by Codex and operate within their own workspace with access to files, code, tools, and persistent memory, allowing them to pull context from multiple systems, request approvals, and integrate directly with Slack.

hackernews · mfiguiere · Apr 22, 17:47

**Background**: AI agents are autonomous systems that can execute multi-step tasks without continuous human input. Workspace Agents evolved from GPTs, OpenAI's previous customization feature. The competitive landscape includes Notion's custom agents, which some users argue offer better shared context management.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-workspace-agents-in-chatgpt/">Introducing workspace agents in ChatGPT | OpenAI</a></li>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/917065/openai-chatgpt-workspace-agents-custom-teams-bots">OpenAI now lets teams make custom bots that can do work on their own | The Verge</a></li>

</ul>
</details>

**Discussion**: Community members raised concerns about energy efficiency and profitability, with one user questioning how AI agents can be profitable when their computational costs exceed traditional methods. Others highlighted intellectual property concerns about OpenAI potentially using agent designs, and competitive positioning against Notion which launched similar features first with arguably better shared context management.

**Tags**: `#openai`, `#ai-agents`, `#chatgpt`, `#enterprise-tools`, `#workflow-automation`

---

<a id="item-11"></a>
## [Google turns Chrome into an AI co-worker for the workplace](https://techcrunch.com/2026/04/22/google-turns-chrome-into-an-ai-coworker-for-the-workplace/) ⭐️ 6.0/10

Google has introduced Gemini-powered "Auto Browse" capabilities to Chrome Enterprise, enabling enterprise workers to automate tasks such as research, data entry, and web-based workflows directly within the browser. This integration marks a significant step in embedding AI assistants directly into mainstream productivity tools, potentially transforming how workers interact with web-based applications and reducing manual repetitive tasks. The Auto Browse feature is currently an enterprise-first rollout requiring Google Workspace Business or Enterprise plans, and Google has not specified a timeline for broader consumer availability. The feature appears alongside other Gemini-powered "Skills" capabilities in the Chrome Enterprise update.

rss · TechCrunch AI · Apr 22, 17:30

**Background**: Chrome Enterprise is Google's specialized version of its Chrome browser designed for business environments, offering enhanced security, management, and deployment features. Gemini is Google's family of large language models that power various AI features across Google's product ecosystem. Browser automation tools allow software to interact with web pages to perform repetitive tasks without human intervention.

<details><summary>References</summary>
<ul>
<li><a href="https://www.zdnet.com/article/google-chrome-enterprise-update-auto-browse-skills-gemini-summary/">Google brings Auto Browse and Skills to Chrome Enterprise ...</a></li>
<li><a href="https://techcrunch.com/2026/04/22/google-turns-chrome-into-an-ai-coworker-for-the-workplace/">Google turns Chrome into an AI coworker for the workplace</a></li>
<li><a href="https://aiproductivity.ai/news/google-chrome-gemini-auto-browse-enterprise/">Google Adds Gemini-Powered 'Auto Browse' to Chrome for Enterprise</a></li>

</ul>
</details>

**Tags**: `#AI Integration`, `#Chrome Browser`, `#Enterprise Software`, `#Gemini`, `#Browser Automation`

---

<a id="item-12"></a>
## [Our newsroom AI policy](https://arstechnica.com/staff/2026/04/our-newsroom-ai-policy/) ⭐️ 6.0/10

Ars Technica published an official policy explaining how the publication uses and does not use generative AI in its newsroom operations and editorial work, authored by staff member Ken Fisher. This transparency policy matters because it sets a precedent for how respected tech journalism organizations approach AI tools, potentially influencing industry standards and building reader trust in an era of AI-generated content concerns. The policy explicitly states boundaries for AI usage in editorial workflows, likely prohibiting AI from generating published content or replacing human judgment in editorial decisions.

rss · Ars Technica · Apr 22, 20:40

**Background**: Ars Technica is a long-running technology publication owned by Condé Nast, known for in-depth technical coverage. As generative AI tools like ChatGPT and Claude have become mainstream, media organizations face pressure to establish clear policies on AI usage to maintain credibility and trust with their audiences.

**Tags**: `#AI policy`, `#tech journalism`, `#editorial ethics`, `#generative AI`, `#media transparency`

---

<a id="item-13"></a>
## [Anthropic tested removing Claude Code from the Pro plan](https://arstechnica.com/ai/2026/04/anthropic-tested-removing-claude-code-from-the-pro-plan/) ⭐️ 6.0/10

Anthropic has been testing the removal of Claude Code from its Pro subscription plan, according to changes observed on some of its public-facing web pages. The company stated that this was only a limited test for a small number of users as it explores ways to manage what it describes as "untenable demand" for its AI services. This development highlights the growing tension between AI companies and the overwhelming demand for their services. As AI labs struggle to balance computational costs with subscription revenue, such rationing decisions could set precedents for how the industry handles resource allocation and pricing models going forward. Claude Code is Anthropic's agentic coding tool that can understand entire codebases, execute multi-file changes, and autonomously complete development tasks. The test appears to have affected only a subset of Pro users, and Anthropic has not announced any permanent changes to its pricing structure at this time.

rss · Ars Technica · Apr 22, 18:34

**Background**: Claude Code is Anthropic's official coding agent designed to help developers ship faster by understanding codebases, editing files, and running commands. Agentic AI tools like Claude Code require significant computational resources, which contributes to the high operational costs that AI companies face. The Pro plan typically offers access to Claude's most capable models with higher usage limits, making the bundling of developer tools a key value proposition for subscribers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theregister.com/2026/04/22/anthropic_removes_claude_code_pro/">Anthropic tests reaction to yanking Claude Code from Pro</a></li>
<li><a href="https://www.anthropic.com/product/claude-code">Claude Code | Anthropic's agentic coding system</a></li>

</ul>
</details>

**Discussion**: The news has sparked discussions among developers about the sustainability of current AI pricing models and concerns about access to essential development tools. Many users are questioning whether AI companies can maintain affordable pricing while managing infrastructure costs, and some worry that such restrictions could push developers toward alternative solutions or open-source alternatives.

**Tags**: `#AI Industry News`, `#Anthropic`, `#Claude Code`, `#Pricing Strategy`, `#AI Services`

---

<a id="item-14"></a>
## [Google unveils two new TPUs designed for the "agentic era"](https://arstechnica.com/ai/2026/04/google-unveils-two-new-tpus-designed-for-the-agentic-era/) ⭐️ 6.0/10

Google announced two new Tensor Processing Units—the TPU 8t for training and TPU 8i for inference—designed specifically for the emerging "agentic era" of AI applications. Both chips are expected to be available later this year. The separate training and inference chip architecture marks a strategic shift in AI hardware design, potentially offering optimized performance for each workload type. This dual-chip strategy could give Google a competitive edge against Nvidia in the growing AI inference market. The TPU 8t is designed for training the largest frontier AI models, while the TPU 8i is built specifically for inference workloads. Both chips share similar foundational architecture but are optimized to eliminate bottlenecks specific to their respective workloads. The chips are targeted for trillion-parameter models and agentic AI applications.

rss · Ars Technica · Apr 22, 17:10

**Background**: TPUs (Tensor Processing Units) are Google's custom-designed AI accelerators used internally and available through Google Cloud. The "agentic era" refers to a paradigm where AI systems act as autonomous agents capable of multi-step reasoning and task execution, rather than simply responding to single prompts. Traditionally, AI chips have been designed with general-purpose architectures that handle both training and inference, making Google's split approach noteworthy. Trillion-parameter models represent the next frontier in AI scale, requiring specialized hardware optimizations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theregister.com/2026/04/22/google_tpu8_dual_track_training_inference/">Google dual tracks TPU 8 to conquer training and inference</a></li>
<li><a href="https://www.businessinsider.com/google-new-ai-chips-tpu-inference-training-nvidia-2026-4">Google's New Chips Are a Shot at Nvidia in AI Inference ...</a></li>
<li><a href="https://www.kad8.com/ai/google-tpu-v8-explained-training-vs-inference-split/">Google TPU v8 Explained: Training vs Inference Split · KAD</a></li>

</ul>
</details>

**Tags**: `#AI Hardware`, `#Google TPUs`, `#Machine Learning Infrastructure`, `#AI Chips`, `#Agentic AI`

---

<a id="item-15"></a>
## [Website streamed live directly from a model](https://flipbook.page/) ⭐️ 5.0/10

Flipbook.page is a live demo project that generates functional websites directly from AI model output, streaming HTML content in real-time as the model produces it. This represents a novel use case for LLMs, moving beyond text responses to interactive, living documents that can adapt and update. It showcases practical utility in scenarios like interactive repair manuals, demonstrating genuine value beyond typical chatbot applications. The system uses streaming inference to progressively render websites as tokens are generated. However, reliability issues have emerged under load, with users encountering 429 rate limit errors and service failures. The resource economics of maintaining such a public demo remain unclear.

hackernews · sethbannon · Apr 22, 18:01

**Background**: LLM streaming output is a technique where AI models generate responses progressively, sending tokens to the client as they are produced rather than waiting for the complete response. This enables real-time interactivity but requires careful handling of partial, potentially incomplete outputs. Generating HTML websites from AI adds another layer of complexity, as the model must understand web structure, styling, and interactivity while maintaining functional correctness.

<details><summary>References</summary>
<ul>
<li><a href="https://www.vellum.ai/llm-parameters/llm-streaming">LLM Streaming - LLM Parameter Guide - Vellum</a></li>
<li><a href="https://www.sandgarden.com/learn/streaming-inference">Streaming Inference: AI That Thinks on its Feet</a></li>
<li><a href="https://fal.ai/docs/documentation/model-apis/inference/streaming">Streaming Inference - fal</a></li>

</ul>
</details>

**Discussion**: Community reaction is mixed but constructive. One user reported impressive results generating a torque spec diagram for car suspension, calling it "genuinely one of the most impressive demos" like a "living version of a classic Haynes workshop manual." However, others noted reliability failures under traffic, questioning the resource economics of offering such services for free. The discussion balances genuine enthusiasm for the creative application with realistic critique about practical viability and cost.

**Tags**: `#ai-applications`, `#generative-ai`, `#web-development`, `#interactive-content`, `#llm-use-cases`

---

<a id="item-16"></a>
## [US Treasury Secretary Bessent says Gulf, Asian allies request swap lines](https://www.aljazeera.com/economy/2026/4/22/us-treasury-secretary-bessent-says-gulf-asian-allies-request-swap-lines?traffic_source=rss) ⭐️ 5.0/10

US Treasury Secretary Scott Bessent confirmed that Gulf and Asian allies have requested currency swap lines, while forcefully rejecting allegations that the Trump family's financial ties to the UAE are influencing these policy decisions. The outcome of these swap line negotiations will shape the financial relationships between the US and major oil-producing Gulf states, with implications for dollar dominance in global trade and potential conflicts of interest concerns. Bessent defended the requests on their merits while dismissing claims about Trump family influence as baseless allegations, suggesting the swap lines would benefit broader US strategic interests.

rss · Al Jazeera · Apr 22, 22:26

**Background**: Currency swap lines are agreements between central banks to exchange currencies, allowing nations to access foreign liquidity during financial stress. The US Federal Reserve has established swap lines with major economies like Europe and Japan, but expanding them to Gulf states would be unprecedented. These arrangements are significant because they typically reinforce the dollar's role in global finance and strengthen geopolitical alliances.

**Tags**: `#geopolitics`, `#international-finance`, `#us-treasury`, `#currency-swap-lines`, `#us-middle-east-relations`

---

<a id="item-17"></a>
## [Prediction market Kalshi docks three US candidates for betting on own races](https://www.aljazeera.com/news/2026/4/22/prediction-market-kalshi-docks-three-us-candidates-for-betting-on-own-races?traffic_source=rss) ⭐️ 5.0/10

Prediction market Kalshi removed three US political candidates for betting on their own races, marking a significant enforcement action against potential 'insider trading' on forecasting platforms. The company pledged to proactively police such practices as calls for greater oversight of prediction markets continue to grow. This action establishes a precedent for prediction market governance, showing that platforms will enforce rules against participants who could manipulate markets by using insider knowledge. It could reshape how political forecasting platforms handle conflicts of interest and may influence regulatory discussions around prediction market integrity. The penalties come amid growing calls for greater oversight of prediction markets, which enable trading on real-world event outcomes using financial incentives. Kalshi, a regulated exchange, has committed to proactively identifying and removing participants who engage in insider trading by betting on events where they have direct involvement.

rss · Al Jazeera · Apr 22, 22:03

**Background**: Prediction markets, also known as betting markets or information markets, are platforms that allow users to trade contracts based on the predicted outcomes of real-world events. Kalshi operates as a regulated exchange where users can buy and sell Event Contracts tied to outcomes ranging from economic indicators to political elections. The concept of 'insider trading' in these markets applies when participants with special knowledge about an event's outcome trade contracts to exploit price movements.

<details><summary>References</summary>
<ul>
<li><a href="https://kalshi.com/">Kalshi - Prediction Market for Trading the Future</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prediction_market">Prediction market - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#prediction markets`, `#regulation`, `#political betting`, `#Kalshi`, `#oversight`

---

<a id="item-18"></a>
## [Tesla just increased its capex to $25B. Here’s where the money is going.](https://techcrunch.com/2026/04/22/tesla-just-increased-its-capex-to-25b-heres-where-the-money-is-going/) ⭐️ 5.0/10

Tesla has announced plans to triple its capital expenditure to $25 billion in 2026, representing three times its historical spending levels. The company's CFO confirmed that as a result of this aggressive investment, Tesla will generate negative free cash flow for the remainder of the year. This massive capital commitment signals Tesla's aggressive expansion strategy across its electric vehicle and energy businesses. For investors tracking Tesla's EV and energy initiatives, the negative free cash flow indicates the company is prioritizing long-term growth over short-term profitability, which could reshape competitive dynamics in the EV market. The $25 billion capex figure is significantly higher than Tesla's historical capital expenditure levels, marking a substantial shift in the company's investment approach. According to the CFO's statement, the expanded spending will result in negative free cash flow, suggesting Tesla is willing to absorb short-term financial pressure to fund its operational expansion.

rss · TechCrunch AI · Apr 22, 23:56

**Background**: Capital expenditure (CapEx) refers to funds companies use to acquire, upgrade, or maintain physical assets such as property, equipment, and technology, with the goal of increasing operational capacity. Free cash flow represents the amount by which a company's operating cash flow exceeds its working capital needs and expenditures on fixed assets—positive free cash flow means a company has surplus cash to reinvest or distribute to shareholders, while negative free cash flow indicates the company is spending more than it earns from operations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.investopedia.com/terms/c/capitalexpenditure.asp">Capital Expenditure (CapEx): Definitions, Formulas, and Real ...</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#Capital Expenditure`, `#Electric Vehicles`, `#Financial Strategy`, `#Investment`

---

<a id="item-19"></a>
## [Hands on with X’s new AI-powered custom feeds](https://techcrunch.com/2026/04/22/hands-on-with-xs-new-ai-powered-custom-feeds/) ⭐️ 5.0/10

X is replacing its Communities feature with AI-powered custom timelines curated by Grok, the chatbot developed by xAI, while introducing new advertising opportunities on the platform. This shift represents a fundamental change in how X users discover content, moving from topic-based community engagement to algorithmic curation. It also signals X's strategy to monetize its platform through AI-personalized advertising while competing with other social media platforms leveraging AI feeds. Grok offers features including AI Voice Chatbot, Natural Language Understanding, and image/video generation capabilities, providing real-time X data integration for content curation. The transition from Communities suggests X is prioritizing AI-driven personalization over community-based features that previously functioned similarly to Reddit.

rss · TechCrunch AI · Apr 22, 22:25

**Background**: X Communities was a feature launched to let users connect and engage in discussions around specific topics, each with its own dedicated space and timeline similar to Reddit. Grok, developed by Elon Musk's xAI, is known for its real-time X data access, conversational capabilities, and bold personality compared to other AI chatbots. The feature has been getting updates since 2023, including new filters and pinned community tabs.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2025/03/04/x-updates-communities-with-new-filters-sorting-options-and-a-way-to-see-your-own-posts/">X updates Communities with new filters, sorting options, and a way to see your own posts | TechCrunch</a></li>
<li><a href="https://www.eweek.com/news/grok-cheat-sheet-complete-guide/">Grok Cheat Sheet: A Complete Guide to Elon Musk’s Chatbot</a></li>

</ul>
</details>

**Tags**: `#social media`, `#AI feeds`, `#X platform`, `#Grok`, `#product updates`

---

<a id="item-20"></a>
## [Google Cloud launches two new AI chips to compete with Nvidia](https://techcrunch.com/2026/04/22/google-cloud-next-new-tpu-ai-chips-compete-with-nvidia/) ⭐️ 5.0/10

Google Cloud announced faster, cheaper TPU chips while maintaining its Nvidia partnership in cloud AI services.

rss · TechCrunch AI · Apr 22, 18:39

**Tags**: `#AI hardware`, `#Google Cloud`, `#TPU`, `#cloud computing`, `#Nvidia`

---

<a id="item-21"></a>
## [Crypto scam lures ships into Strait of Hormuz, falsely promising safe passage](https://arstechnica.com/security/2026/04/crypto-scam-lures-ships-into-strait-of-hormuz-falsely-promising-safe-passage/) ⭐️ 5.0/10

据报道，一个加密货币骗局向航行于霍尔木兹海峡的船只提供虚假的安全通行承诺，诱使这些船只可能遭遇伊朗的袭击。该骗局利用加密货币作为支付手段，声称可以为船只提供安全保障。 这一事件标志着加密货币被用于危险的地缘政治操纵，将无辜的船员置于严重的人身危险之中。随着海上网络攻击事件在2025年翻倍增长，此类骗局揭示了航运业面临的新兴安全威胁。 霍尔木兹海峡是全球最重要的石油运输咽喉要道之一，每日约有1700万桶石油从此通过。伊朗过去曾扣押和袭击过在该海域航行的船只，而加密货币骗局可能是攻击的前置手段。

rss · Ars Technica · Apr 22, 22:07

**Background**: 霍尔木兹海峡连接波斯湾与阿曼湾，是全球最繁忙的石油运输通道。由于其战略重要性，该区域长期存在地缘政治紧张局势。网络安全公司Cytur报告显示，2025年海上网络攻击事件翻倍增长，主要由恶意软件和分布式拒绝服务（DDoS）攻击驱动。加密货币的匿名性使其成为网络犯罪和此类骗局中支付手段的理想选择。

<details><summary>References</summary>
<ul>
<li><a href="https://maritime-executive.com/article/report-maritime-cyberattacks-doubled-in-2025">Report: Maritime Cyberattacks Doubled in 2025</a></li>
<li><a href="https://en.wikipedia.org/wiki/Spoofing_attack">Spoofing attack - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#cryptocurrency`, `#scams`, `#geopolitics`, `#maritime-security`, `#phishing`

---

<a id="item-22"></a>
## [Lawsuit: Nintendo is getting tariff refunds—its customers should get them instead](https://arstechnica.com/tech-policy/2026/04/lawsuit-nintendo-is-getting-tariff-refunds-its-customers-should-get-them-instead/) ⭐️ 5.0/10

A lawsuit has been filed demanding that Nintendo pass on tariff refunds received from the Trump administration to its customers rather than retaining the financial benefits for itself. This case raises important questions about corporate responsibility and whether companies should share government-provided cost savings with consumers who paid higher prices during the tariff period. The lawsuit argues that customers effectively paid inflated prices to cover tariff costs, so they—rather than Nintendo—should benefit when those tariffs are refunded.

rss · Ars Technica · Apr 22, 20:27

**Background**: During the Trump administration, tariffs were imposed on various imported goods including electronics and gaming consoles, which typically increased costs for manufacturers. When the government later refunds these tariffs, the question arises as to who should receive the benefit—the company that paid the tariffs or the consumers who purchased the affected products at higher prices.

**Tags**: `#gaming`, `#tariffs`, `#consumer-protection`, `#nintendo`, `#tech-policy`

---

<a id="item-23"></a>
## [You want your Moon landings in HD? So does NASA—here's how it's happening.](https://arstechnica.com/space/2026/04/you-want-your-moon-landings-in-hdtv-so-does-nasa-heres-how-its-happening/) ⭐️ 5.0/10

NASA is implementing new communications technology, including laser-based optical communications, to enable high-definition video transmission from the Moon and beyond. The Deep Space Network is being upgraded with modern systems that can handle HD signals across vast interplanetary distances. This advancement is significant for future lunar missions, including crewed Artemis missions, as high-definition video will allow Earth audiences to experience Moon landings with unprecedented visual clarity. The improved bandwidth also supports more data-intensive scientific operations and better real-time monitoring of distant spacecraft. The Deep Space Optical Communications (DSOC) system can improve communications performance 10 to 100 times over traditional radio frequency technology without significant increases in mass, volume, or power. The upgraded infrastructure includes laser transceivers at ground stations and new optical terminals capable of capturing and processing signals transmitted across hundreds of millions of kilometers.

rss · Ars Technica · Apr 22, 19:42

**Background**: The NASA Deep Space Network (DSN) is a worldwide network of large radio antennas operated by the Jet Propulsion Laboratory, located in California, Madrid, and Canberra to provide continuous coverage as Earth rotates. DSN has historically relied on radio frequency communications, but NASA is now integrating laser optical communications technology to meet growing bandwidth demands from increasingly sophisticated scientific instruments and imaging systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/NASA_Deep_Space_Network">NASA Deep Space Network</a></li>
<li><a href="https://en.wikipedia.org/wiki/Deep_Space_Optical_Communications">Deep Space Optical Communications - Wikipedia</a></li>
<li><a href="https://www.nasa.gov/mission/deep-space-optical-communications-dsoc/">Deep Space Optical Communications (DSOC) - NASA</a></li>

</ul>
</details>

**Tags**: `#space exploration`, `#NASA`, `#deep space communications`, `#video technology`, `#lunar missions`

---

<a id="item-24"></a>
## [Sam Altman’s Orb Company Promoted a Bruno Mars Partnership That Doesn't Exist](https://www.wired.com/story/sam-altman-orb-company-bruno-mars-partnership-fake/) ⭐️ 5.0/10

Worldcoin, Sam Altman's eye-scanning crypto project, promoted a partnership with pop star Bruno Mars that never existed. Bruno Mars' representatives confirmed to WIRED that they were never approached for any discussions regarding a partnership or tour access. This incident raises serious questions about Worldcoin's marketing practices and corporate ethics, particularly for a project that relies on building global trust through its biometric identity verification system. It demonstrates how easily misinformation can spread in the crypto industry to attract users. The fake partnership was promoted by Worldcoin's Orb company, and when contacted by WIRED, Bruno Mars' representatives stated clearly: 'To be clear, we were never approached… nor were we in any discussions regarding a partnership or tour access.' This follows Worldcoin's history of controversy over its iris-scanning practices.

rss · Wired · Apr 22, 22:11

**Background**: Worldcoin, co-founded by Sam Altman in 2023, is a cryptocurrency project that uses biometric technology through spherical devices called Orbs to scan people's irises in exchange for digital tokens. The project has expanded to over 120 countries with more than 3.1 million verified users. Worldcoin aims to create a digital identity system by proving users are unique humans through iris recognition, while distributing its own WLD cryptocurrency token as an incentive. The project has faced significant regulatory scrutiny and criticism regarding privacy concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://time.com/6300522/worldcoin-sam-altman/">What to Know About Worldcoin and the Controversy Around It - TIME</a></li>
<li><a href="https://www.wired.com/story/worldcoin-sam-altman-orb/">Sam Altman’s Eye- Scanning Orb Has a New Look—and Will... | WIRED</a></li>

</ul>
</details>

**Tags**: `#worldcoin`, `#sam-altman`, `#misinformation`, `#tech-ethics`, `#scandal`

---

<a id="item-25"></a>
## [🚨 GSR LAUNCHES MULTI-ASSET CRYPTO ETF WITH STAKING](https://t.me/CoinBureau/12941) ⭐️ 5.0/10

American VC firm GSR launched a first-of-its-kind multi-asset crypto ETF (BESO) on Nasdaq offering exposure to Bitcoin, Ethereum, and Solana with weekly rebalancing, a 1% fee, and staking access.

telegram · CoinBureau · Apr 22, 17:33

**Tags**: `#crypto ETF`, `#staking`, `#Bitcoin`, `#Ethereum`, `#Solana`, `#financial products`

---

<a id="item-26"></a>
## [📊 ETHENA USDe SUPPLY DROPS $800M IN 3 DAYS](https://t.me/CoinBureau/12943) ⭐️ 5.0/10

Ethena's USDe stablecoin supply contracted by 14%, equivalent to approximately $800 million, over just three days, representing one of the largest redemption events in the protocol's history. The rapid liquidity exit spread pressure across DeFi markets, according to on-chain analytics firm CryptoQuant. A supply contraction of this magnitude signals potential instability in synthetic stablecoin protocols and raises questions about user confidence in delta-hedged structures during volatile market conditions. This event could prompt broader reassessment of risk exposure in DeFi liquidity pools and affect how traders manage stablecoin allocations. The 14% supply reduction in three days represents an unusually rapid contraction for USDe, suggesting either large-scale redemption pressure or a coordinated withdrawal of liquidity. CryptoQuant's monitoring indicates the outflow is impacting multiple DeFi markets simultaneously.

telegram · CoinBureau · Apr 22, 17:43

**Background**: USDe is Ethena's synthetic dollar stablecoin that maintains its peg through a delta-hedging strategy using short positions in perpetual and deliverable futures contracts to offset price volatility of underlying collateral. Unlike traditional stablecoins backed by fiat reserves, USDe is backed by crypto assets such as staked Ethereum (stETH) and holds USDC and USDT as part of its reserves. Ethena's adaptive model continuously adjusts its hedging positions to maintain peg stability while generating yield for holders through the funding rate differential on its derivatives positions.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.ethena.fi">Ethena Overview | Ethena</a></li>
<li><a href="https://coinmarketcap.com/cmc-ai/ethena-usde/what-is/">What Is Ethena USDe (USDe) And How Does It Work?</a></li>
<li><a href="https://cryptoquant.com/">CryptoQuant | On-Chain Actionable Insights</a></li>

</ul>
</details>

**Tags**: `#stablecoin`, `#DeFi`, `#Ethena`, `#USDe`, `#liquidity`

---

<a id="item-27"></a>
## [🚨AAVE STABLECOIN BORROW RATES SPIKE AFTER KELP DAO EXPLOIT](https://t.me/CoinBureau/12946) ⭐️ 5.0/10

AAVE V3's USDT and USDC stablecoin borrow rates spiked from approximately 3.4% to 14% following the April 19 exploit of Kelp DAO's rsETH token, as users rapidly withdrew liquidity and unwound their positions. This incident demonstrates how exploit events in liquid restaking protocols can create cascading liquidity crises across DeFi lending markets, with sudden withdrawal demand driving extreme interest rate spikes that can destabilize position management for leveraged users. The Kelp DAO exploit reportedly drained approximately $292 million from the protocol. The attack exploited a 1-of-1 verifier configuration weakness in the cross-chain LayerZero messaging infrastructure, where only a single node was responsible for validating messages before releasing funds.

telegram · CoinBureau · Apr 23, 00:05

**Background**: Kelp DAO is a liquid restaking protocol built on the EigenLayer platform that accepts user-deposited ETH, routes it through EigenLayer to earn additional yield on top of standard Ethereum staking rewards, and issues rsETH as a tradeable receipt token. Liquid restaking tokens like rsETH allow users to earn staking and restaking rewards while maintaining liquidity for DeFi participation. Aave V3 is a decentralized non-custodial liquidity market protocol where users can supply assets to earn interest or borrow assets by paying variable interest rates that fluctuate based on supply and demand dynamics.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coindesk.com/tech/2026/04/22/the-protocol-kelp-dao-exploited-for-usd292-million">The Protocol: Kelp DAO exploited for $292 million</a></li>
<li><a href="https://www.halborn.com/blog/post/explained-the-kelp-dao-hack-april-2026">Explained: The Kelp DAO Hack (April 2026)</a></li>
<li><a href="https://coinmarketcap.com/currencies/kelp-dao-restaked-eth/">Kelp DAO Restaked ETH price today, RSETH to USD... | CoinMarketCap</a></li>

</ul>
</details>

**Tags**: `#DeFi`, `#Aave`, `#Crypto Exploit`, `#Stablecoin`, `#Liquidity Crisis`

---

<a id="item-28"></a>
## [Billionaire backer sues Trump family's crypto firm over alleged extortion](https://www.bbc.com/news/articles/c8x7kxjgq9xo?at_medium=RSS&at_campaign=rss) ⭐️ 4.0/10

Billionaire crypto investor Justin Sun has filed a lawsuit against World Liberty Financial, the Trump family's cryptocurrency venture, seeking $45 million in damages. The suit alleges extortion related to Sun's purchases of World Liberty tokens. This lawsuit highlights the intersection of celebrity-endorsed crypto ventures and legal accountability in the digital asset space. It could set precedents for how token sales and alleged high-pressure tactics are treated legally, affecting investor protection standards across the crypto industry. Justin Sun, founder of the TRON blockchain and a prominent figure in the crypto space, reportedly invested $45 million in World Liberty Financial tokens before filing the lawsuit. World Liberty Financial was founded in 2024 by Zachary Folkman, Chase Herro, Alex Witkoff, Zach Witkoff, and Trump family members, with the Trump family receiving 75% of net proceeds from WLFI token sales.

rss · BBC World · Apr 22, 18:10

**Background**: Justin Sun is a Chinese-born Kittitian billionaire and the founder of TRON, a blockchain platform that hosts the Tronix (TRX) cryptocurrency and the USDD stablecoin. World Liberty Financial is the most prominent of several crypto businesses co-founded or controlled by the Trump family, which has reportedly made over $1 billion from the venture according to a Reuters analysis.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/c8x7kxjgq9xo">Trump family crypto firm sued over alleged 'extortion'</a></li>
<li><a href="https://en.wikipedia.org/wiki/World_Liberty_Financial">World Liberty Financial - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Justin_Sun">Justin Sun - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#cryptocurrency`, `#legal-dispute`, `#politics`, `#news`, `#business`

---

<a id="item-29"></a>
## [Warner Bros and Paramount merger could reshape US media landscape](https://www.aljazeera.com/economy/2026/4/22/warner-bros-and-paramount-merger-could-reshape-us-media-landscape?traffic_source=rss) ⭐️ 4.0/10

Warner Bros and Paramount have proposed a merger that is now facing regulatory scrutiny from US authorities. The deal is being reviewed for its potential impact on the US media landscape and concerns related to foreign investment funding. The merger could significantly reshape the US entertainment industry by combining two major studios. If approved, it would create one of the largest media conglomerates, potentially affecting competition, content diversity, and consumer choices in streaming and theatrical markets. Regulatory concerns center on two main issues: the merger's potential to reduce competition in the media industry, and questions about foreign investment involvement in the deal. These factors have prompted careful examination by relevant authorities.

rss · Al Jazeera · Apr 22, 19:53

**Background**: Media consolidation has been a significant trend in recent years as streaming platforms compete for content and audiences. Major studios have been merging or partnering to strengthen their market positions. Warner Bros (owned by Warner Bros Discovery) and Paramount (owned by Paramount Global) are two iconic Hollywood studios with extensive film libraries, television networks, and streaming services.

**Discussion**: This merger proposal has sparked debate about media consolidation and its effects on the entertainment industry. Concerns include potential reduction in competitive diversity and the implications of foreign investment in critical media assets.

**Tags**: `#media`, `#mergers`, `#regulation`, `#entertainment`, `#business`

---

<a id="item-30"></a>
## [Did UK universities pay to ‘spy’ on pro‑Palestine students?](https://www.aljazeera.com/video/the-take-2/2026/4/22/aje-onl-tt_gbr_unispying_av_v2-220426?traffic_source=rss) ⭐️ 4.0/10

A joint investigation by Al Jazeera and Liberty Investigates has revealed that twelve British universities paid at least £440,000 to Horus Security Consultancy Limited since 2022 to monitor student protesters and academics, particularly those expressing solidarity with Palestine. The security firm is led by former military intelligence officials and presents itself as an "intelligence-led consultancy." This surveillance raises serious concerns about academic freedom and civil liberties on UK campuses, as it effectively transforms educational institutions into instruments of state-style monitoring. The targeting of pro-Palestinian expression specifically suggests that political viewpoints are being treated as potential security threats, potentially chilling legitimate political discourse and protest. The investigation found that Horus scanned social media accounts and undertook direct surveillance of students and academics. The universities funnelled public money into monitoring their own student bodies, with the total amount paid being at least £440,000. The firm specifically focused on pro-Palestinian activism and solidarity with Palestine.

rss · Al Jazeera · Apr 22, 18:21

**Background**: This surveillance controversy is connected to the UK's PREVENT strategy, a counter-extremism framework introduced in 2011 that requires universities to report signs of radicalization. Critics have long argued that PREVENT creates a climate of suspicion on campuses and infringes on civil liberties. Universities UK, the main higher education sector body, has been examining ways to prevent extremism on campuses under this framework.

<details><summary>References</summary>
<ul>
<li><a href="https://libertyinvestigates.org.uk/articles/british-universities-paid-security-firm-monitor-pro-palestine-students/">British universities paid security firm to monitor pro ...</a></li>
<li><a href="https://www.aljazeera.com/news/2026/4/20/uk-universities-pay-to-spy-on-students-social-media-accounts">British universities paid security firm to spy on pro ...</a></li>
<li><a href="https://www.ukfactcheck.com/article/244/uk-universities-paid-private-firm-to-spy-on-pro-palestine-students-and-academics">UK Universities Paid Private Firm to Spy on Pro-Palestine ...</a></li>

</ul>
</details>

**Discussion**: Campaigners have described the surveillance as a "chilling crackdown on political dissent" that blurs the line between education and state-style surveillance. Critics argue that PREVENT is an untenable infringement on civil liberties and call for the strategy to be repealed. The evidence suggests that only the government continues defending the policy in defiance of expert opinion.

**Tags**: `#surveillance`, `#academic-freedom`, `#civil-liberties`, `#higher-education`, `#human-rights`

---

<a id="item-31"></a>
## [Ukraine restarts Russian oil to Europe, unblocking 90-billion-euro EU loan](https://www.aljazeera.com/news/2026/4/22/ukraine-restarts-russian-oil-flows-to-europe-unblocking-90bn-eu-loan?traffic_source=rss) ⭐️ 4.0/10

Ukraine has resumed pumping Russian oil through the Druzhba pipeline to Hungary and Slovakia, enabling Hungary to lift its veto and clearing the way for EU member states to formally approve a €90 billion loan package for Ukraine. This development resolves a months-long diplomatic deadlock and unlocks critical financial support for Ukraine amid its ongoing conflict with Russia. The pipeline's restart also addresses energy security concerns for landlocked Central European nations that depend on Russian oil supplies. Oil supplies through the Druzhba pipeline were halted at the end of January following a Russian drone strike that damaged the pipeline in western Ukraine. The €90 billion EU loan is to be repaid using proceeds from frozen Russian sovereign assets over a repayment period that can extend up to 35 years.

rss · Al Jazeera · Apr 22, 16:12

**Background**: The Druzhba pipeline, whose name means "friendship" in Russian, is the largest principal artery for transporting Russian and Kazakh oil across Europe. Built during the Soviet era in the 1960s, it remains a critical piece of energy infrastructure for several EU member states. Hungary and Slovakia have been particularly affected by the supply suspension due to their landlocked geography and limited alternative oil import options. The EU's €90 billion loan package was approved by MEPs in February 2026 to bolster Ukraine's defence against Russian aggression.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/cnv8l99r3yyo">EU approves €90bn loan for Ukraine as pipeline is turned on ending deadlock</a></li>
<li><a href="https://www.nbcnews.com/world/ukraine/druzhba-pipeline-restarts-russian-oil-flows-europe-unblocking-eu-loan-rcna341394">Druzhba pipeline restarts Russian oil flows to Europe, unblocking E.U. loan for Kyiv</a></li>
<li><a href="https://www.europarl.europa.eu/news/en/press-room/20260206IPR33903/parliament-approves-EU90-billion-ukraine-support-loan-package">Parliament approves €90 billion Ukraine support loan package</a></li>

</ul>
</details>

**Tags**: `#geopolitics`, `#energy-policy`, `#EU-politics`, `#oil-and-gas`, `#international-relations`

---

<a id="item-32"></a>
## [How Iran and the United States Are Planning Their Next Moves](https://foreignpolicy.com/2026/04/22/karim-sadjadpour-iran-regime-future-war-gulf-energy-hormuz-cease-fire/) ⭐️ 4.0/10

Foreign Policy published an interview with Iran expert Karim Sadjadpour discussing the extended cease-fire and ongoing naval blockade affecting the Strait of Hormuz, the world's most critical oil shipping chokepoint. The US continues its naval blockade of Iranian ports despite the declared truce, which Iran claims undermines the ceasefire agreement. The Strait of Hormuz handles approximately 20-25% of global oil shipments daily, making its continued blockade a critical energy security concern. Any escalation or prolonged blockade could dramatically impact global oil prices and destabilize international energy markets, affecting economies worldwide. On March 2, Iran's Islamic Revolutionary Guard Corps officially confirmed the Strait of Hormuz was closed and threatened to set fire to any ship entering the strait. About 100 ships passed through between March 1-20, and tensions have escalated since the October 7, 2023 Hamas attacks on Israel and subsequent Gaza war that led to Israel decimating Iran-backed regional militias.

rss · Foreign Policy · Apr 22, 21:23

**Background**: The Strait of Hormuz is a narrow waterway between the Arabian Gulf and Gulf of Oman, at its narrowest point lying entirely within Iranian and Omani territorial waters. It has been a flashpoint for US-Iran tensions, which intensified following the Gaza war and Israel's military operations against Iran-backed groups including Hamas, Hezbollah, and Houthis. Trump extended the ceasefire on day 54 of the conflict while maintaining the naval blockade as leverage.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Strait_of_Hormuz">Strait of Hormuz - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/2026_Iran_war">2026 Iran war - Wikipedia</a></li>
<li><a href="https://www.aljazeera.com/news/2026/4/22/iran-war-whats-happening-on-day-54-as-trump-extends-ceasefire">Iran war: What’s happening on day 54 as Trump extends... | Al Jazeera</a></li>

</ul>
</details>

**Tags**: `#geopolitics`, `#middle-east`, `#energy-security`, `#us-iran-relations`, `#international-affairs`

---

<a id="item-33"></a>
## [Europe Might Sit Out In An Indo-Pacific War — But It Can’t Escape the Fallout](https://warontherocks.com/europe-might-sit-out-in-an-indo-pacific-war-but-it-cant-escape-the-fallout/) ⭐️ 4.0/10

Strategic analysis examining how a Sino-American conflict over Taiwan would impact Europe even if European states attempt to remain militarily uninvolved.

rss · War on the Rocks · Apr 22, 17:30

**Tags**: `#geopolitics`, `#defense-policy`, `#europe`, `#indo-pacific`, `#taiwan`

---

<a id="item-34"></a>
## [New Low-Cost Cruise Missile Features Tomahawk-Like Range](https://www.twz.com/air/new-raacm-er-low-cost-cruise-missile-features-tomahawk-like-range) ⭐️ 4.0/10

CoAspire has unveiled the RAACM-ER (Rapidly Adaptable Affordable Cruise Missile Extended Range), a new low-cost cruise missile featuring a range exceeding 1,000 nautical miles, comparable to the Tomahawk missile. The missile is designed using additive manufacturing (3D printing) technology to keep production costs down while delivering long-range strike capabilities. The RAACM-ER addresses the U.S. Air Force's requirement for long-range anti-ship missiles at a fraction of traditional costs. By leveraging 3D printing to eliminate tooling and reduce touch labor, this missile could enable mass procurement of affordable long-range munitions, potentially changing the economics of naval strike operations. The original RAACM was designed to match the dimensions of a GBU-38 500-pound JDAM, measuring 92.6 inches long with a 14-inch wingspan. The missile incorporates a turbojet engine, warhead, and guidance package. The ER variant extends the range while maintaining the low-cost manufacturing approach that eliminates tooling during assembly.

rss · The Drive Warzone · Apr 22, 20:16

**Background**: The RAACM program was showcased at the Sea Air Space 2025 expo, where CoAspire demonstrated its approach to affordable long-range munitions using 3D printing technology. The missile fills a gap between inexpensive but short-range precision-guided munitions and expensive traditional cruise missiles like the Tomahawk, which cost over $1 million per unit. Additive manufacturing allows the missile to be produced without traditional tooling, significantly reducing assembly labor and unit costs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.twz.com/air/new-raacm-er-low-cost-cruise-missile-features-tomahawk-like-range">New Low-Cost Cruise Missile Features Tomahawk-Like Range</a></li>
<li><a href="https://www.coaspire.com/raacm">RAACM Cruise Missile — CoAspire</a></li>
<li><a href="https://www.navalnews.com/event-news/sea-air-space-2025/2025/04/coaspire-tests-raacm-rapidly-adaptable-affordable-cruise-missile/">CoAspire Tests RAACM Rapidly Adaptable Affordable Cruise Missile</a></li>

</ul>
</details>

**Tags**: `#defense-technology`, `#cruise-missiles`, `#military-systems`, `#aerospace`, `#weaponry`

---

<a id="item-35"></a>
## [F-15EX Buy Was Just Doubled By The USAF, Which Makes Perfect Sense](https://www.twz.com/air/f-15ex-buy-was-just-doubled-by-the-usaf-which-makes-perfect-sense) ⭐️ 4.0/10

The USAF has doubled its F-15EX procurement order, initially to replace F-15C fighters with potential future expansion to replace aging F-15E Strike Eagles.

rss · The Drive Warzone · Apr 22, 18:38

**Tags**: `#military-aviation`, `#defense-procurement`, `#USAF`, `#F-15EX`, `#boeing`

---

<a id="item-36"></a>
## [Ford Class Review Puts Navy’s Future Carrier Plans Into Question](https://www.twz.com/sea/ford-class-review-puts-navys-future-carrier-plans-into-question) ⭐️ 4.0/10

The US Navy is conducting a review comparing Ford-class and Nimitz-class carriers to evaluate operational performance, assessing what has been gained or lost in the transition between the two carrier designs. This review could significantly impact the US Navy's carrier acquisition strategy and affect billions of dollars in defense spending. The outcome may determine whether the Navy proceeds with additional Ford-class carriers or restructures its carrier program. The Ford-class features advanced technologies including the Electromagnetic Aircraft Launch System (EMALS), Advanced Arresting Gear (AAG), and Dual Band Radar. These systems were designed to increase sortie rates by 25% and triple electrical power generation, but have experienced reliability issues and developmental delays since the USS Gerald R. Ford was commissioned in 2017.

rss · The Drive Warzone · Apr 22, 17:01

**Background**: The Ford-class represents the next generation of US nuclear-powered aircraft carriers, designed to replace the aging Nimitz-class fleet. The lead ship, USS Gerald R. Ford, cost approximately $13 billion and incorporates revolutionary new launch and recovery systems. The EMALS uses electromagnetic linear induction motors rather than traditional steam catapults, while the AAG replaces hydraulic systems for aircraft recovery. The Dual Band Radar combines S-band and X-band capabilities for comprehensive air defense coverage.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gerald_R._Ford-class_aircraft_carrier">Gerald R. Ford-class aircraft carrier - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/USS_Gerald_R._Ford">USS Gerald R. Ford - Wikipedia</a></li>
<li><a href="https://www.19fortyfive.com/2026/04/the-ford-class-is-not-the-aircraft-carrier-you-think-it-is-we-should-call-it-a-13-billion-laboratory/">The Ford-Class Is Not the Aircraft Carrier You Think It Is: We Should Call It a $13 Billion 'Laboratory' - 19FortyFive</a></li>

</ul>
</details>

**Tags**: `#naval-defense`, `#aircraft-carriers`, `#military-procurement`, `#US-Navy`, `#defense-review`

---

<a id="item-37"></a>
## [Google updates Workspace to make AI your new office intern](https://techcrunch.com/2026/04/22/google-updates-workspace-to-make-ai-your-new-office-intern/) ⭐️ 4.0/10

Google has introduced Workspace Intelligence, a new AI system that powers automated functions across its productivity suite including Gmail, Docs, Sheets, Slides, and Chat. This update positions AI as an active participant in daily work tasks, potentially transforming how users interact with productivity tools and reducing repetitive manual work. Workspace Intelligence enables Gemini in Google Slides to generate presentations that adhere to company templates and visual styles in a single operation, while a new command-line interface is being introduced directly in Google Chat for work-related commands.

rss · TechCrunch AI · Apr 22, 22:44

**Background**: Google Workspace is the company's cloud-based productivity suite that includes Gmail, Docs, Drive, Calendar, Meet, and Chat. Gemini is Google's family of large language models that power AI features across Google products. Workspace Intelligence acts as a contextual layer that gives Gemini deeper understanding of user data and organizational context to generate more relevant and accurate outputs.

<details><summary>References</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lJaHBmOEVCR3Q3amN1OUEtd2NDZ0FQAQ?hl=en-US&gl=US&ceid=US:en">Google News - Google Workspace Intelligence for Gemini...</a></li>
<li><a href="https://workspace.google.com/blog/product-announcements/introducing-workspace-intelligence">New Workspace Intelligence delivers unified, real-time understanding...</a></li>
<li><a href="https://9to5google.com/2026/04/22/google-workspace-intelligence/">Google announces ' Workspace Intelligence ' and TPU 8t + 8i chips</a></li>

</ul>
</details>

**Tags**: `#Google Workspace`, `#AI Automation`, `#Productivity Tools`, `#Tech Industry News`, `#Google AI`

---

<a id="item-38"></a>
## [AI Overviews are coming to your Gmail at work](https://techcrunch.com/2026/04/22/ai-overviews-are-coming-to-your-gmail-at-work/) ⭐️ 4.0/10

Google is extending its AI Overviews feature to Gmail for Google Workspace users, enabling instant summarization pulled from across multiple emails in the inbox. This integration brings AI-powered email intelligence to enterprise users, potentially transforming how professionals manage high-volume inboxes and quickly extract key information from communications. The feature appears to mirror the AI Overviews functionality already rolled out in Google Drive, which allows users to get instant answers from files without manually searching through documents.

rss · TechCrunch AI · Apr 22, 16:46

**Background**: AI Overviews is Google's AI-powered search and summarization feature, initially launched in the US search experience. The feature is currently available in over 120 countries and 11 languages. Earlier this month, AI Overviews became generally available in Google Drive, and this announcement indicates Google's continued expansion of the technology across its productivity suite.

<details><summary>References</summary>
<ul>
<li><a href="https://workspaceupdates.googleblog.com/2026/04/ai-overviews-in-drive-now-generally-available.html">Google Workspace Updates: AI Overviews in Drive now generally ...</a></li>
<li><a href="https://www.search.google/ways-to-search/ai-overviews/">Google AI Overviews - Search anything, effortlessly</a></li>

</ul>
</details>

**Tags**: `#AI features`, `#Gmail`, `#Google Workspace`, `#product news`, `#workplace productivity`

---

<a id="item-39"></a>
## [Scientists Gave Cocaine to Salmon and You Will Absolutely Believe What Happened Next](https://www.wired.com/story/cocaine-fueled-wild-salmon-swam-twice-as-far-as-sober-ones/) ⭐️ 4.0/10

Scientists exposed wild salmon to cocaine and its primary metabolite benzoylecgonine, and observed that the contaminated fish swam approximately twice the distance compared to unexposed fish, demonstrating behavioral changes consistent with those previously documented in laboratory settings. This research highlights the growing problem of pharmaceutical pollution in aquatic environments, where drugs and their metabolites enter waterways through wastewater and affect wildlife behavior in ways that could disrupt ecosystems and fish survival. The study observed that cocaine-exposed salmon maintained hyperactivity similar to laboratory findings, with swimming distances doubling compared to controls. Benzoylecgonine, the main metabolite tested in most drug screenings, also produced measurable behavioral effects in the fish.

rss · Wired · Apr 22, 21:34

**Background**: Pharmaceutical pollution represents a global environmental threat, with concentrations of active pharmaceutical ingredients exceeding safe levels at over a quarter of sampled river sites worldwide. Research has documented that pollutants including psychoactive drugs can alter fish behavior, cognition, and movement patterns, potentially affecting their survival and predator avoidance capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pnas.org/doi/10.1073/pnas.2113947119">Pharmaceutical pollution of the world’s rivers | PNAS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Benzoylecgonine">Benzoylecgonine - Wikipedia</a></li>
<li><a href="https://www.frontiersin.org/journals/ecology-and-evolution/articles/10.3389/fevo.2020.00086/full">Effects of Pollution on Fish Behavior, Personality, and ...</a></li>

</ul>
</details>

**Tags**: `#environmental-science`, `#ecotoxicology`, `#wildlife-research`, `#pharmaceutical-pollution`, `#animal-behavior`

---

<a id="item-40"></a>
## [🇮🇷🇺🇸🇮🇱Hãng thông tấn IRIB: Iran đang xem xét nhiều khía cạnh khác nhau của việc ](https://t.me/quantin_vic/199838) ⭐️ 4.0/10

Iran's state news agency IRIB reports that Iran is reviewing multiple aspects of a potential ceasefire extension while officially denying rumors that it had agreed to President Trump's proposal. Foreign Ministry spokesman Esmaeil Baghaei has not commented on the matter, and reports attributing statements to him have been dismissed as inaccurate. This development highlights the delicate diplomatic dance in US-Iran relations, where ceasefire negotiations remain uncertain. The mutual denials and careful official language suggest both parties are testing boundaries while avoiding commitments that could be politically costly. IRIB, Iran's official state news agency, serves as the source for these reports. The denial specifically addresses rumors about Iran formally agreeing to Trump's ceasefire extension proposal, with officials maintaining a stance of official silence rather than explicit rejection or acceptance.

telegram · quantin_vic · Apr 22, 16:20

**Background**: Iran-US relations have been marked by decades of tension since the 1979 Islamic Revolution. Recent ceasefire efforts represent one of several diplomatic attempts to reduce hostilities. IRIB (Islamic Republic of Iran Broadcasting) is Iran's official state media outlet, and its reports are considered authoritative for Iranian government positions. Esmaeil Baghaei is the current spokesperson for Iran's Ministry of Foreign Affairs.

**Tags**: `#geopolitics`, `#Iran`, `#US-Iran relations`, `#ceasefire`, `#diplomacy`

---

