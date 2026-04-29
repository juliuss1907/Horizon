# Horizon Daily - 2026-04-29

> From 135 items, 12 important content pieces were selected

---

1. [HashiCorp co-founder says GitHub 'no longer a place for serious work'](#item-1) ⭐️ 7.0/10
2. [Tangled – We need a federation of forges](#item-2) ⭐️ 6.0/10
3. [He asked AI to count carbs 27000 times. It couldn't give the same answer twice](#item-3) ⭐️ 6.0/10
4. [Indie music has been invaded by fake fans and cynical viral campaigns​. Here’s how deep it all goes](#item-4) ⭐️ 6.0/10
5. [Meet the AI jailbreakers: ‘I see the worst things humanity has produced’](#item-5) ⭐️ 6.0/10
6. [Soft launch of open-source code platform for government](#item-6) ⭐️ 5.0/10
7. [Show HN: Rip.so – a graveyard for dead internet things](#item-7) ⭐️ 5.0/10
8. [HardenedBSD Is Now Officially on Radicle](#item-8) ⭐️ 5.0/10
9. [Howdy, Roku’s $2.99 Streamer, Appears to Have More Than 1 Million Subscribers](#item-9) ⭐️ 5.0/10
10. [How to turn old pitta into spiced chips – recipe | Waste not](#item-10) ⭐️ 4.0/10
11. [Shall We Play a Game?](#item-11) ⭐️ 4.0/10
12. [Cảnh báo: Sinh trắc học không còn an toàn, tội phạm mạng có thể vượt qua hệ thống bảo mật của ngân hàng](#item-12) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [HashiCorp co-founder says GitHub 'no longer a place for serious work'](https://www.theregister.com/2026/04/29/mitchell_hashimoto_ghostty_quitting_github/) ⭐️ 7.0/10

HashiCorp联合创始人Mitchell Hashimoto（GitHub第1299号用户，2008年2月加入）公开表示GitHub已"不再是认真工作的地方"，引发社区关于平台稳定性问题的大规模讨论。 Hashimoto作为DevOps和基础设施工具领域的知名人物，他的批评在开发者社区中具有相当的分量。这场讨论反映出人们对于平台在大规模场景下可靠性的日益担忧，以及迁移关键开发基础设施所面临的实际挑战。 有社区用户反映，在从CircleCI向GitHub迁移的过程中，平台稳定性明显下降。有用户指出Azure Repos和Pipelines在某些方面反而表现更好，尽管其迁移工作仍在进行中。部分早期用户认为GitHub的核心功能仍然可用，强调"写软件不一定需要GitHub"。

hackernews · terminalbraid · Apr 29, 11:42

**Background**: HashiCorp成立于2012年，由Mitchell Hashimoto和Armon Dadgar联合创立，是Terraform、Vault、Consul等知名开源基础设施工具的开发商，在DevOps和云原生领域具有重要影响力。GitHub则是全球最大的代码托管平台，拥有超过1亿开发者用户，其稳定性对全球软件开发工作流至关重要。

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HashiCorp">HashiCorp - Wikipedia</a></li>
<li><a href="https://www.hashicorp.com/en/products/vault">HashiCorp Vault | Identity-based secrets management</a></li>

</ul>
</details>

**Discussion**: 社区反应呈现明显分歧：一派用户分享了GitHub稳定性下降带来的真实挫折感，特别是在迁移期间；另一派则对Hashimoto的批评表示质疑，认为GitHub的核心功能仍能满足需求。讨论还涉及对Azure Repos等替代平台的关注，以及关于GitHub用户编号的好奇询问。

**Tags**: `#developer-tools`, `#github`, `#hashiCorp`, `#platform-stability`, `#devops`

---

<a id="item-2"></a>
## [Tangled – We need a federation of forges](https://blog.tangled.org/federation/) ⭐️ 6.0/10

The Tangled project has published a proposal calling for a federation of code forges to address the growing fragmentation in developer collaboration infrastructure, sparking community debate about technical approaches including email-based federation and comparisons to existing protocols like ActivityPub. Code forges like GitHub, GitLab, and Forgejo host millions of open source projects, and their fragmentation creates silos that hinder collaboration and lock developers into single platforms; a unified federation standard could restore interoperability and reduce vendor dependency across the open source ecosystem. Community commenters raised questions about why existing decentralized communication protocols like ActivityPub cannot solve the forge federation problem, with some suggesting email as a proven foundation that has worked for decades, while others compared the challenge to BitTorrent's success in decentralized file sharing for git repositories.

hackernews · icy · Apr 29, 14:00

**Background**: A code forge is a web-based collaborative platform for software development and sharing, with examples including GitHub, GitLab, and the community-driven Forgejo fork from Gitea. Federation in distributed systems allows different servers to communicate and share data while maintaining their autonomy, similar to how email or the Matrix protocol enable cross-platform communication.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Forge_(software)">Forge (software) - Wikipedia</a></li>
<li><a href="https://forgejo.org/">Forgejo – Beyond coding. We forge.</a></li>
<li><a href="https://matrix.org/">Matrix, the open protocol for secure decentralised communications</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed, with some agreeing that the proliferation of competing federation standards creates unnecessary complexity, while others question whether a new standard is needed when ActivityPub already exists. One commenter noted that Tangled's integration with Jujutsu (a version control system) is its most important feature, highlighting that technical differentiation may matter more than federation protocol details.

**Tags**: `#federation`, `#open-source-infrastructure`, `#git`, `#decentralization`, `#forge`

---

<a id="item-3"></a>
## [He asked AI to count carbs 27000 times. It couldn't give the same answer twice](https://www.diabettech.com/i-asked-ai-to-count-my-carbs-27000-times-it-couldnt-give-me-the-same-answer-twice/) ⭐️ 6.0/10

A diabetic user conducted an extensive test by asking AI models to count carbohydrates from identical food photos 27,000 times, receiving a different answer each time despite using the lowest randomness settings available. The experiment yielded wildly inconsistent results, including a suggested insulin dose of 42.9 units from a single photo, highlighting fundamental unpredictability in LLM outputs. This experiment underscores a critical safety concern: people with diabetes rely on accurate carbohydrate counts to dose insulin, and incorrect calculations can lead to life-threatening hypoglycemia or hyperglycemia. As AI-powered carb-counting apps proliferate in app stores, this test serves as an important warning about the dangers of relying on probabilistic language models for medical nutrition guidance. The author explicitly set randomness to the minimum available across all tested models, attempting to minimize variance in responses. Critics in the discussion pointed out that this test may be fundamentally unreasonable, as LLMs cannot extract nutritional information from photons alone—factors like portion size, ingredient composition, and oil content are invisible in food images.

hackernews · sarusso · Apr 29, 12:38

**Background**: Large Language Models (LLMs) are AI systems trained on massive datasets to generate human-like text by predicting token probabilities. Unlike deterministic programs, LLMs produce probabilistic outputs, meaning identical prompts can yield different responses even at low temperature settings. For diabetic patients, carbohydrate counting is essential for calculating insulin doses, as accurate dosing prevents dangerous blood sugar fluctuations. AI carb-counting applications have recently emerged in app stores, raising concerns about their safety in medical contexts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/large-language-model-llm/">What is a Large Language Model ( LLM ) - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: Community reactions were divided: some critics dismissed the experiment as fundamentally unreasonable, arguing that expecting nutritional data from photos alone is impossible since photons cannot capture internal food composition. Others acknowledged the value of demonstrating AI unreliability as a warning against using such tools for diabetes management. Several commenters noted the irony of the author using an LLM to write an article about LLM limitations, while others warned that commercial AI diabetes apps may use even less reliable models than those tested.

**Tags**: `#LLM-limitations`, `#AI-reliability`, `#healthcare`, `#AI-testing`, `#machine-learning`

---

<a id="item-4"></a>
## [Indie music has been invaded by fake fans and cynical viral campaigns​. Here’s how deep it all goes](https://www.theguardian.com/music/2026/apr/29/geese-outcry-phoney-virality-music-fans-hype) ⭐️ 6.0/10

The Guardian investigates how marketing agencies like Chaotic Good create artificial viral moments for indie artists through fake fans and influencer campaigns.

rss · The Guardian Music · Apr 29, 09:15

**Tags**: `#music industry`, `#astroturfing`, `#social media marketing`, `#indie music`, `#viral culture`

---

<a id="item-5"></a>
## [Meet the AI jailbreakers: ‘I see the worst things humanity has produced’](https://www.theguardian.com/technology/2026/apr/29/meet-the-ai-jailbreakers-i-see-the-worst-things-humanity-has-produced) ⭐️ 6.0/10

The Guardian profiles Valen Tagliabui, an AI red teamer who spent two years deliberately manipulating LLMs like Claude and ChatGPT to bypass safety rules, successfully eliciting dangerous outputs including instructions for creating lethal pathogens. As LLMs become increasingly integrated into critical infrastructure and daily life, understanding how malicious actors might exploit these systems becomes essential for developing effective defenses, making the work of red teamers vital to AI safety. Tagliabui describes falling into a 'dark flow' state where he mastered manipulation techniques including being cruel, vindictive, sycophantic, and abusive toward models to trigger harmful outputs—the work revealed both the technical ingenuity required and the psychological toll on testers.

rss · The Guardian Life · Apr 29, 09:00

**Background**: AI red teaming involves systematically probing large language models for safety vulnerabilities through techniques like prompt injection, role-play scenarios, and incremental context building. Unlike automated testing approaches, human red teamers use social engineering, psychological manipulation, and creative framing to bypass model safety guardrails. Jailbreaking techniques have evolved from simple prompt tricks to multi-turn conversations that gradually desensitize models, with modern attacks employing tactics like passive history framing and seed collection to generate and mutate bypass prompts at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@shafiqulsumon007/red-teaming-large-language-models-how-to-break-ai-before-attackers-do-ad3f6a8c3dde">Red Teaming Large Language Models: How to Break AI ... | Medium</a></li>
<li><a href="https://www.confident-ai.com/blog/how-to-jailbreak-llms-one-step-at-a-time">How to Jailbreak LLMs One Step at a Time: Top Techniques and Strategies - Confident AI</a></li>
<li><a href="https://startup-house.com/blog/llm-jailbreak-techniques">LLM Jailbreaks 2024–2026: Techniques, Risks & Defense Strategies | Startup House</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#red teaming`, `#LLM security`, `#jailbreaking`, `#AI alignment`

---

<a id="item-6"></a>
## [Soft launch of open-source code platform for government](https://www.nldigitalgovernment.nl/news/soft-launch-for-government-open-source-code-platform/) ⭐️ 5.0/10

The Dutch government has soft-launched an open-source code platform at code.overheid.nl, moving away from third-party hosting. The platform features the RegelRecht system, which encodes legal texts as structured YAML and executes them as deterministic decision logic. This platform marks a significant step toward digital sovereignty in Dutch government IT infrastructure, reducing dependency on external platforms like GitHub. It also enables citizens and developers to access, audit, and contribute to publicly funded code, promoting transparency in government software development. The RegelRecht system takes legal regulations and input data, evaluates the decision logic, and returns results with full explanation trails. It compares favorably to Germany's similar portal opencode.de, which is built on GitLab and provides hardened base container images at container.gov.de.

hackernews · e12e · Apr 29, 09:14

**Background**: Machine-readable law initiatives aim to convert legislation into code that computers can read, interpret, and execute consistently. New Zealand and Estonia have similar programs to digitize their entire legislative corpus. By encoding laws as structured data, governments can enable automated compliance checking, reduce ambiguity in legal interpretation, and create transparent audit trails for decision-making.

<details><summary>References</summary>
<ul>
<li><a href="https://code.overheid.nl/RegelRecht/regelrecht">RegelRecht/regelrecht: RegelRecht - Forgejo: Beyond coding. We forge.</a></li>
<li><a href="https://www.jd-shapiro.com/policy/machine-readable-laws-macro-considerations-for-government-digitization-strategy">Machine Readable Laws : Macro-considerations for government...</a></li>

</ul>
</details>

**Discussion**: Community comments reveal mixed sentiments. Dutch users express pride in the migration from third-party hosting but also frustration about past government unresponsiveness to open-source contributors. One commenter described being ghosted after applying for an open-source contributor role. Others requested clearer use cases for the RegelRecht system, while comparing it favorably to Germany's opencode.de portal built on GitLab.

**Tags**: `#open-source`, `#government`, `#netherlands`, `#policy`, `#digital-government`

---

<a id="item-7"></a>
## [Show HN: Rip.so – a graveyard for dead internet things](https://rip.so/) ⭐️ 5.0/10

Rip.so is a community-curated graveyard cataloging dead, zombie, and deprecated internet services with user debates about categorization accuracy and mentions of spiritual successors.

hackernews · bozdemir · Apr 29, 09:21

**Tags**: `#internet-history`, `#web-archive`, `#digital-nostalgia`, `#community-curation`, `#defunct-services`

---

<a id="item-8"></a>
## [HardenedBSD Is Now Officially on Radicle](https://hardenedbsd.org/article/shawn-webb/2026-04-26/hardenedbsd-officially-radicle) ⭐️ 5.0/10

HardenedBSD has officially migrated its code collaboration to Radicle, a decentralized, peer-to-peer Git forge built on Git. This move positions HardenedBSD among projects embracing sovereign code hosting without relying on centralized platforms like GitHub. This migration highlights growing interest in decentralized code hosting as an alternative to centralized platforms. For security-focused projects like HardenedBSD, peer-to-peer collaboration could provide greater autonomy and resilience against platform-level censorship or shutdowns. Radicle differentiates itself by ensuring commits are cryptographically signed by current maintainers and giving users full control over their data. However, discoverability remains a challenge—projects exist on the network but may not appear in visible search results without active node hosting and linking to external websites.

hackernews · lftherios · Apr 29, 06:38

**Background**: Git forges are web-based platforms that host Git repositories and provide collaboration tools like issue tracking and pull requests. Traditional forges like GitHub, GitLab, and Gitea are centralized, meaning a single company controls the network. Radicle takes a different approach by replicating repositories across peer nodes, eliminating dependence on any single entity while maintaining compatibility with standard Git workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://radicle.dev/">Radicle: the sovereign forge</a></li>
<li><a href="https://en.wikipedia.org/wiki/Forge_(software)">Forge (software) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community members raised practical questions about the migration rationale—specifically what platform HardenedBSD moved from and why Radicle was chosen over alternatives. Some compared Radicle to ATProto and Fossil for distributed version control, noting that peer-to-peer solutions still require highly available servers. While Radicle is recognized as a legitimate project with five years of development, concerns remain about project discoverability in a decentralized environment.

**Tags**: `#hardenedbsd`, `#radicle`, `#decentralization`, `#git-forge`, `#p2p`

---

<a id="item-9"></a>
## [Howdy, Roku’s $2.99 Streamer, Appears to Have More Than 1 Million Subscribers](https://www.hollywoodreporter.com/business/digital/howdy-roku-subscribers-1236579351/) ⭐️ 5.0/10

Roku's budget streaming service 'Howdy' has apparently crossed the 1 million subscriber milestone, with streaming research firm Antenna validating the numbers. The $2.99/month service reportedly shows better retention rates compared to other streaming services. This milestone suggests there is significant demand for ultra-low-cost streaming options in an increasingly crowded market. The strong retention rates indicate that budget-conscious consumers are finding value in affordable content offerings, potentially reshaping competitive dynamics in the streaming industry. Antenna's data triangulation confirms the subscriber count, though Roku has not officially disclosed these figures independently. The $2.99 price point positions 'Howdy' as one of the most affordable streaming options currently available in the market.

rss · The Hollywood Reporter · Apr 29, 14:00

**Background**: The streaming landscape has become increasingly competitive, with major platforms like Netflix, Disney+, and HBO Max dominating the market. In response to this crowded environment, companies like Roku have introduced budget-friendly alternatives to attract price-sensitive consumers. Low-cost streaming services typically offer more limited content libraries compared to premium platforms, trading breadth of content for accessibility.

**Tags**: `#streaming`, `#roku`, `#subscription services`, `#entertainment industry`, `#digital media`

---

<a id="item-10"></a>
## [How to turn old pitta into spiced chips – recipe | Waste not](https://www.theguardian.com/food/2026/apr/29/how-to-turn-old-pitta-into-spiced-chips-recipe-zero-waste-cooking) ⭐️ 4.0/10

The Guardian published a recipe guide for transforming stale pitta bread into seasoned spiced chips, developed by chef Sam Webb of Babette street food stall in Cornwall. The recipe uses sumac, za'atar, and sea salt as seasonings and takes only minutes to prepare. This recipe represents a practical approach to reducing food waste at the household level, turning bread that might otherwise be discarded into an appealing snack. While not technically groundbreaking, such zero-waste cooking tips can contribute to changing consumer habits around food waste reduction. The pitta chips are seasoned with a combination of sumac, za'atar, and sea salt just before serving, giving them a distinctive Middle Eastern flavor profile. Webb and his team at Babette source local Cornish produce and make everything from scratch, with food waste reduction being a key priority in their operation.

rss · The Guardian Life · Apr 29, 12:00

**Background**: Zero-waste cooking has gained traction as awareness grows about the environmental and economic impact of food waste. In the UK alone, millions of tonnes of food are wasted each year, with bread products representing a significant portion of household food waste. Pitta bread, when stale, becomes ideal for chip-making because its flat shape and texture hold seasonings well and crisp up quickly when heated. Sumac and za'atar are common spices in Middle Eastern and Mediterranean cuisines, with sumac providing a lemony tang and za'atar adding a complex herbal mixture typically including oregano, thyme, and sesame seeds.

**Tags**: `#food waste`, `#cooking`, `#zero-waste`, `#recipes`, `#sustainability`

---

<a id="item-11"></a>
## [Shall We Play a Game?](https://longreads.com/2026/04/29/wargames-tabletop-rpg-history/) ⭐️ 4.0/10

A long-form historical overview by gaming historian Jon Peterson traces the evolution of wargaming from its origins in Prussian military headquarters to the creation of modern tabletop RPGs like Dungeons & Dragons, ultimately connecting military strategy gaming to Gary Gygax's basement innovations. This piece illuminates the often-overlooked military heritage underlying modern recreational gaming culture, showing how serious military training tools eventually became foundational to one of the world's most influential hobby industries. Understanding this lineage reveals how formal discipline transformed into imaginative play. Jon Peterson is widely recognized as the authority on gaming history, having authored seminal works including 'Playing at the World' and 'Game Wizards.' The article specifically connects Prussian Kriegsspiel wargaming traditions through Chainmail (1971) to Gary Gygax's eventual creation of Dungeons & Dragons (1974).

rss · Longreads · Apr 29, 11:00

**Background**: Wargaming originated in 19th-century Prussia as a military training tool to simulate battlefield conditions and test strategic concepts without real casualties. The term 'Kriegsspiel' (German for 'war game') referred to both official Prussian military exercises and later commercial variants. Chainmail was a medieval miniatures wargame published by Gary Gygax and Jeff Perren in 1971, which served as the immediate predecessor to Dungeons & Dragons by introducing fantasy elements and dungeon exploration mechanics. Jon Peterson's 'Playing at the World' (2012) is considered the definitive scholarly history of how these military simulations evolved into role-playing games.

<details><summary>References</summary>
<ul>
<li><a href="https://www.penguinrandomhouse.com/authors/2155959/jon-peterson/">Jon Peterson | Penguin Random House</a></li>
<li><a href="https://www.amazon.com/Playing-at-World-Jon-Peterson/dp/0615642047">Playing at the World: A History of Simulating Wars, People and Fantastic Adventures, from Chess to Role-Playing Games: Peterson, Jon: 9780615642048: Amazon.com: Books</a></li>

</ul>
</details>

**Tags**: `#gaming-history`, `#tabletop-rpg`, `#culture`, `#wargaming`, `#dungeons-and-dragons`

---

<a id="item-12"></a>
## [Cảnh báo: Sinh trắc học không còn an toàn, tội phạm mạng có thể vượt qua hệ thống bảo mật của ngân hàng](https://kenh14.vn/canh-bao-sinh-trac-hoc-khong-con-an-toan-toi-pham-mang-co-the-vuot-qua-he-thong-bao-mat-cua-ngan-hang-215260429180306706.chn) ⭐️ 4.0/10

MIT Technology Review has identified nearly two dozen channels and groups claiming the ability to breach major cryptocurrency exchanges and well-known banks by bypassing biometric security systems. This development poses a significant threat to the financial sector, which increasingly relies on biometric authentication to protect customer accounts. With traditional passwords being phased out, the integrity of biometric systems is now critical for maintaining security in digital banking and cryptocurrency platforms. Security researchers have documented AI-generated deepfake images being used to bypass biometric verification systems. Traditional liveness detection methods are increasingly vulnerable to sophisticated spoofing attacks, leaving mobile banking applications and cryptocurrency exchanges exposed to account takeovers and fraud.

rss · Kenh14 · Apr 29, 18:11

**Background**: Biometric authentication has become a cornerstone of modern digital security, using unique physical characteristics like fingerprints and facial features to verify user identity. Financial institutions have widely adopted these systems as more secure alternatives to traditional passwords. However, the emergence of AI-generated deepfakes has created new attack vectors that can fool facial recognition systems by presenting synthetic but highly realistic images or videos.

<details><summary>References</summary>
<ul>
<li><a href="https://www.forbes.com/sites/daveywinder/2024/12/04/ai-bypasses-biometric-security-in-1385-million-financial-fraud-risk/">Now AI Can Bypass Biometric Banking Security, Experts Warn</a></li>
<li><a href="https://www.appdome.com/dev-sec-blog/protecting-the-integrity-of-biometric-authentication-from-deepfake-attacks/">Protecting the Integrity of Biometric Authentication from Deepfake ...</a></li>
<li><a href="https://www.secureworld.io/industry-news/mobile-malware-deepfakes-biometric-authentication">Mobile Malware Uses Deepfakes , Social Engineering to Bypass ...</a></li>

</ul>
</details>

**Discussion**: Security experts widely agree that biometric authentication alone is insufficient against evolving AI-powered threats. The consensus calls for layered security approaches combining multiple verification methods. Industry professionals emphasize that organizations must implement multi-factor authentication to mitigate these emerging risks effectively.

**Tags**: `#cybersecurity`, `#biometrics`, `#banking-security`, `#threat-intelligence`, `#cryptocurrency`

---

