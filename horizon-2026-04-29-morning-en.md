# Horizon Daily - 2026-04-28

> From 86 items, 12 important content pieces were selected

---

1. [Ghostty Terminal Emulator Leaves GitHub Amid Platform Concerns](#item-1) ⭐️ 8.0/10
2. [Critical GitHub Enterprise RCE Vulnerability CVE-2026-3854](#item-2) ⭐️ 8.0/10
3. [Your phone is about to stop being yours](#item-3) ⭐️ 8.0/10
4. [Google expands Pentagon’s access to its AI after Anthropic’s refusal](#item-4) ⭐️ 8.0/10
5. [OpenAI Models Arrive on Amazon Bedrock via AWS Partnership](#item-5) ⭐️ 7.0/10
6. [Warp Terminal Emulator Goes Open-Source](#item-6) ⭐️ 7.0/10
7. [UK's ARIA Pursues Brain-Computer Interface for Epilepsy, Alzheimer's](#item-7) ⭐️ 7.0/10
8. [Before GitHub: A Retrospective on Version Control Evolution](#item-8) ⭐️ 6.0/10
9. [Musk Testifies at OpenAI Trial, Claims Company Betrayed Mission](#item-9) ⭐️ 6.0/10
10. [China Blocks Meta's $2B Acquisition of AI Startup Manus](#item-10) ⭐️ 6.0/10
11. [Japan Airlines Tests Humanoid Robots for Airport Tasks](#item-11) ⭐️ 6.0/10
12. [GitHub Copilot Shifts to Usage-Based Pricing Model](#item-12) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Ghostty Terminal Emulator Leaves GitHub Amid Platform Concerns](https://mitchellh.com/writing/ghostty-leaving-github) ⭐️ 8.0/10

Mitchell Hashimoto, creator of Ghostty and former HashiCorp founder, announced that his terminal emulator project is leaving GitHub with an emotionally charged blog post where he admitted to crying while writing about the departure. This departure signals growing developer dissatisfaction with GitHub under Microsoft ownership, reflecting broader concerns about platform stability and resource allocation toward AI features over core development tools. Ghostty is a fast, feature-rich, cross-platform terminal emulator that uses platform-native UI and GPU acceleration. The community discussion highlights GitHub's perceived decline, including criticism of prioritization of Copilot over fundamental services.

hackernews · WadeGrimridge · Apr 28, 19:44

**Background**: Ghostty represents a new generation of terminal emulators focused on performance and modern features. Mitchell Hashimoto previously founded HashiCorp, known for infrastructure tools like Terraform and Vault. GitHub, acquired by Microsoft in 2018, has faced increasing criticism from developers regarding service quality and feature prioritization.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: 👻 Ghostty is a fast, feature-rich, and cross-platform terminal emulator that uses platform-native UI and GPU acceleration.</a></li>
<li><a href="https://ghostty.org/">Ghostty</a></li>
<li><a href="https://ghostty.org/docs">Ghostty Docs</a></li>
<li><a href="https://www.itpro.com/software/development/github-copilot-pricing-changes-premium-requests">‘Made the Pro plan worse’: GitHub just announced new pricing ...</a></li>

</ul>
</details>

**Discussion**: Developers express mixed reactions—some support Mitchell's emotional stance and acknowledge GitHub's service degradation, while others point to vendor lock-in concerns and question the sustainability of platform dependencies.

**Tags**: `#GitHub`, `#Ghostty`, `#MitchellHashimoto`, `#open-source`, `#devtools`, `#Microsoft`

---

<a id="item-2"></a>
## [Critical GitHub Enterprise RCE Vulnerability CVE-2026-3854](https://www.wiz.io/blog/github-rce-vulnerability-cve-2026-3854) ⭐️ 8.0/10

Wiz Research discovered CVE-2026-3854, a critical command injection vulnerability in GitHub Enterprise Server that allows attackers with push access to achieve remote code execution on the instance. At the time of disclosure, 88% of on-prem instances remained unpatched despite a security fix being available for 7 weeks. This vulnerability represents a severe security risk as it could allow any authenticated user to compromise backend servers and access millions of private repositories, potentially achieving full server takeover. The shockingly low patching rate highlights a critical gap in enterprise security hygiene and underscores how AI-accelerated vulnerability discovery is outpacing organizations' ability to respond. The flaw, tracked as CVE-2026-3854 with a CVSS score of 8.7, resides in GitHub's internal git infrastructure and affects both GitHub.com and GitHub Enterprise Server. Users are advised to upgrade to GHES version 3.19.3 or later. Wiz demonstrated how their AI-augmented reverse engineering methodology enabled rapid vulnerability discovery, representing what commentators called a 'watershed moment' in security research tooling.

hackernews · bo0tzz · Apr 28, 16:15

**Background**: Remote code execution (RCE) vulnerabilities allow attackers to execute arbitrary commands on a target system, representing among the most severe security flaws possible. GitHub Enterprise Server is the on-premises version of GitHub's platform, used by organizations requiring data residency or stricter security controls. Command injection occurs when user-controlled input is improperly sanitized before being passed to system commands, enabling attackers to inject malicious commands. Wiz Research is the security research arm of Wiz, an Israeli-American cloud security company acquired by Google Cloud in March 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wiz.io/blog/github-rce-vulnerability-cve-2026-3854">GitHub RCE Vulnerability: CVE-2026-3854 Breakdown | Wiz Blog</a></li>
<li><a href="https://thehackernews.com/2026/04/researchers-discover-critical-github.html">Researchers Discover Critical GitHub CVE-2026-3854 RCE Flaw Exploitable via Single Git Push</a></li>
<li><a href="https://cybersecuritynews.com/github-com-and-enterprise-server-rce/">Critical GitHub.com and Enterprise Server RCE Vulnerability Enables Full Server Compromise</a></li>

</ul>
</details>

**Discussion**: Community commenters praised Wiz's research capabilities, with one noting their AI-augmented reverse engineering methodology demonstrates how LLM agents trained extensively on code can vastly accelerate understanding complex system internals—a traditionally difficult component of security research. However, concerns were raised about the 88% unpatched rate, with one commenter stating that organizations failing to apply a critical security fix 7 weeks after release 'seems... bad.' Others debated GitHub alternatives, though some questioned whether any alternative platform would be fundamentally more secure.

**Tags**: `#security`, `#vulnerability`, `#CVE`, `#GitHub`, `#RCE`

---

<a id="item-3"></a>
## [Your phone is about to stop being yours](https://keepandroidopen.org/en/) ⭐️ 8.0/10

Google will begin blocking non-Play Store Android apps via silent updates starting September 2026, prompting community debate about platform openness, user freedom, and the implications for millions of Android users who chose the platform specifically for its openness.

hackernews · doener · Apr 28, 15:21

**Tags**: `#android`, `#google`, `#platform-policy`, `#user-freedom`, `#mobile-development`, `#app-stores`

---

<a id="item-4"></a>
## [Google expands Pentagon’s access to its AI after Anthropic’s refusal](https://techcrunch.com/2026/04/28/google-expands-pentagons-access-to-its-ai-after-anthropics-refusal/) ⭐️ 8.0/10

Google has signed a contract with the Pentagon to provide AI capabilities after Anthropic declined involvement due to concerns about domestic mass surveillance and autonomous weapons applications.

rss · TechCrunch AI · Apr 28, 18:15

**Tags**: `#AI Ethics`, `#Defense Contracts`, `#Google`, `#Anthropic`, `#AI Policy`

---

<a id="item-5"></a>
## [OpenAI Models Arrive on Amazon Bedrock via AWS Partnership](https://stratechery.com/2026/an-interview-with-openai-ceo-sam-altman-and-aws-ceo-matt-garman-about-bedrock-managed-agents/) ⭐️ 7.0/10

OpenAI and AWS announced a partnership bringing OpenAI models to Amazon Bedrock, with both the latest OpenAI models and the Codex coding agent now available in limited preview through the AWS platform. This partnership enables regulated industries with existing AWS contracts to access OpenAI models without separate data processing agreements, potentially shifting competitive dynamics in enterprise AI adoption. Models hosted on different inference platforms may perform differently due to factors like quantization, custom model serving silicon, batching, or inference optimizations, adding another layer of non-determinism to development.

hackernews · translocator · Apr 28, 19:24

**Background**: Amazon Bedrock is AWS's fully managed service for building and scaling generative AI applications, offering access to models from multiple AI providers along with security and governance tools. Anthropic's Claude models have been available on Bedrock since launch, giving them significant enterprise penetration in privacy-conscious organizations. OpenAI previously relied primarily on Azure for enterprise distribution.

<details><summary>References</summary>
<ul>
<li><a href="https://aws.amazon.com/bedrock/">Amazon Bedrock – Build genAI applications and agents at ...</a></li>
<li><a href="https://www.aboutamazon.com/news/aws/bedrock-openai-models">About Amazon News post</a></li>

</ul>
</details>

**Discussion**: Community members note that Claude gained significant enterprise traction because organizations could access it through their 'trusted' intermediate Amazon, while OpenAI was often rejected by privacy-focused organizations. One commenter observes this partnership could unlock regulated industries with existing AWS data residency commitments, though technical concerns remain about inference platform differences potentially causing inconsistent model behavior across different hosting environments.

**Tags**: `#OpenAI`, `#AWS`, `#cloud-computing`, `#enterprise-AI`, `#partnership`

---

<a id="item-6"></a>
## [Warp Terminal Emulator Goes Open-Source](https://github.com/warpdotdev/warp) ⭐️ 7.0/10

Warp, a venture-backed terminal emulator that previously raised $50 million in funding, has open-sourced their codebase on GitHub while facing significant community criticism over their practices and recent product changes. The open-sourcing of a well-funded commercial terminal emulator is relatively rare in the developer tools space and represents a significant shift in Warp's business strategy. The move raises questions about the company's future direction and whether open-sourcing will help rebuild trust with a skeptical community. The terminal emulator was forked from Alacritky, another popular open-source terminal project, and critics allege the company never contributed back to the parent project despite raising $50M in venture capital. Warp also recently redesigned their UI in a way that removed features and broke existing workflows for paying customers.

hackernews · doppp · Apr 28, 17:09

**Background**: Warp is a modern terminal emulator written in Rust, available for macOS, Windows and Linux, featuring AI-powered command suggestions and code generation capabilities. A terminal emulator is software that mimics physical computer terminals, providing a text-based interface for interacting with the operating system. Warp has partnered with OpenAI and claims over 700,000 developers use their platform, competing with alternatives like Ghostty and iTerm2.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Warp_(terminal)">Warp ( terminal ) - Wikipedia</a></li>
<li><a href="https://www.warp.dev/">Warp : The Agentic Development Environment</a></li>
<li><a href="https://www.geeksforgeeks.org/operating-systems/difference-between-terminal-console-shell-and-command-line/">Difference between Terminal, Console, Shell, and Command Line</a></li>

</ul>
</details>

**Discussion**: Community sentiment is predominantly negative, with critics still angry that Warp forked Alacritty to build their commercial product without contributing to the original open-source project they owe their foundation to. Former paying customers express frustration that recent UI changes removed intuitive features like the agent mode toggle and broke saved prompt templates. Some users appreciate the concept but find the current implementation too overwhelming, preferring simpler alternatives like Ghostty or iTerm2.

**Tags**: `#open-source`, `#terminal-emulator`, `#developer-tools`, `#venture-capital`, `#startup-drama`

---

<a id="item-7"></a>
## [UK's ARIA Pursues Brain-Computer Interface for Epilepsy, Alzheimer's](https://www.wired.com/story/kathleen-fisher-jacques-carolan-aria-wired-health/) ⭐️ 7.0/10

Wired has profiled ARIA (Advanced Research and Invention Agency), the UK's £800 million research agency, revealing its ambitious program to develop advanced neurotechnology and brain-computer interfaces targeting conditions like epilepsy and Alzheimer's. This profile highlights how the UK is positioning itself as a major player in neurotechnology research, directly challenging US dominance in the field. Success could lead to transformative treatments for millions suffering from neurological disorders worldwide. ARIA operates with a similar mandate to DARPA, funding "high-risk, high-reward" research including precision neurotechnologies, programmable systems, robotics, and AI. The agency gives programme directors unusual freedom to fund and pivot programs quickly without bureaucratic constraints.

rss · Wired · Apr 28, 17:58

**Background**: ARIA is a UK non-departmental public body formally established by an Act of Parliament on 26 January 2023, sponsored by the Department for Science, Innovation and Technology. Brain-computer interfaces (BCI) are systems that establish direct communication pathways between the brain and external devices, a technology gaining significant commercial attention following milestones like Neuralink's first human implant. The neurotechnology field is experiencing rapid growth, with BCI listed among MIT Technology Review's breakthrough technologies for 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Aria_(Advanced_Research_and_Invention_Agency)">Aria (Advanced Research and Invention Agency)</a></li>
<li><a href="https://www.technologyreview.com/2025/04/01/1114009/brain-computer-interfaces-10-breakthrough-technologies-2025/">Brain - computer interfaces face a critical test | MIT Technology Review</a></li>

</ul>
</details>

**Tags**: `#neurotechnology`, `#brain-computer-interfaces`, `#ARIA`, `#UK-research`, `#healthcare-AI`, `#neuroscience`

---

<a id="item-8"></a>
## [Before GitHub: A Retrospective on Version Control Evolution](https://lucumr.pocoo.org/2026/4/28/before-github/) ⭐️ 6.0/10

Armin Ronacher published a retrospective examining what GitHub changed about version control hosting, highlighting the shift from project-centric to person-centric repositories, comparing Fossil's all-in-one philosophy with Git's minimalist approach, and raising concerns about centralized platforms atrophying collective archival skills. GitHub's person-centric model fundamentally lowered the barrier for individual developers to share code publicly, transforming how open source projects are initiated and discovered. Understanding this historical shift helps contextualize today's developer ecosystem and the ongoing tradeoffs between convenience and distributed resilience. Fossil is a distributed version control system by D. Richard Hipp (creator of SQLite) that includes built-in wiki, forum, bug tracking, and chat features all versioned together in a single SQLite file, contrasting with Git's focused approach. The discussion notes that while Git may have performance advantages for massive codebases like the Linux kernel, most projects never encounter VCS performance limits.

hackernews · mlex · Apr 28, 21:17

**Background**: Before GitHub, SourceForge was the dominant open source hosting platform and required developers to go through a formal project registration process including coming up with a project name and reserving namespace, often with associated website, mailing lists, and issue tracking that felt overly serious for individual experimentation. CVS (Concurrent Versions System) and later SVN (Subversion) were the dominant version control systems before distributed version control systems (DVCS) like Git and Mercurial gained popularity. Git was created by Linus Torvalds in 2005 for Linux kernel development.

<details><summary>References</summary>
<ul>
<li><a href="https://fossil-scm.org/home">Fossil: A Coherent Software Configuration Management System</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fossil_(software)">Fossil (software) - Wikipedia</a></li>
<li><a href="https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/repository-access-and-collaboration/inviting-collaborators-to-a-personal-repository">Inviting collaborators to a personal repository - GitHub Docs</a></li>

</ul>
</details>

**Discussion**: Commenters express both appreciation for GitHub's democratizing effect and nostalgia for alternative approaches. Alastairp highlights the liberating reduction in mental overhead from person-centric repos. Wps remains salty that Fossil's integrated tooling (wiki, forum, tickets all versioned together) lost to Git's simplicity, noting they use Fossil for freelance work for its contextual recovery benefits. Lammy raises a provocative concern that GitHub's convenient centralized archival actually atrophies collective archival skills—if everyone had to manually seed and maintain copies, the community would be more resilient at preservation.

**Tags**: `#github`, `#version-control`, `#fossil`, `#software-history`, `#open-source`

---

<a id="item-9"></a>
## [Musk Testifies at OpenAI Trial, Claims Company Betrayed Mission](https://www.aljazeera.com/economy/2026/4/28/musk-testifies-at-openai-trial-its-not-ok-to-loot-a-charity?traffic_source=rss) ⭐️ 6.0/10

Elon Musk testified in his lawsuit against OpenAI, accusing the company and its cofounder of betraying him and the public by abandoning its original non-profit mission to become a profit-seeking enterprise. Musk argued that transforming a charitable organization into a commercial entity amounts to 'looting a charity.' This lawsuit raises critical questions about the governance of AI organizations that blend charitable missions with commercial operations. The outcome could set precedents for how non-profit technology ventures handle structural transitions and fiduciary responsibilities when pivoting toward profit models. OpenAI transitioned from its original non-profit structure in 2019 by creating a capped-profit subsidiary (OpenAI LP), allowing external investors while capping returns. Musk alleges this transformation violated fiduciary duties owed to the non-profit's original mission and supporters.

rss · Al Jazeera · Apr 28, 22:35

**Background**: OpenAI was founded in 2015 as a non-profit AI research lab with Musk as a founding donor. The organization pivoted to a 'capped-profit' model in 2019, creating OpenAI LP to attract capital while limiting investor returns. Non-profit board members have fiduciary duties requiring them to act in the organization's best interest rather than personal or commercial interests, and breaching these duties can result in legal liability.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/our-structure/">Our structure - OpenAI</a></li>
<li><a href="https://www.techrepublic.com/article/news-openai-structure-explained/">How OpenAI’s Corporate Structure Works and Why Changing It ...</a></li>
<li><a href="https://www.boardeffect.com/blog/fiduciary-responsibilities-nonprofit-board-directors/">Fiduciary Responsibilities of a Nonprofit Board of Directors | BoardEffect</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Elon Musk`, `#AI Industry`, `#Legal/Court`, `#Tech Policy`

---

<a id="item-10"></a>
## [China Blocks Meta's $2B Acquisition of AI Startup Manus](https://foreignpolicy.com/2026/04/28/china-blocks-ai-meta-manus-deal-national-security/) ⭐️ 6.0/10

China has blocked Meta's acquisition of the AI startup Manus, reversing a deal announced in late December 2025 that was estimated to be worth approximately $2 billion. China's National Development and Reform Commission (NDRC) issued a one-line statement prohibiting the acquisition, requiring all parties to immediately withdraw and cancel the transaction. The blocking signals a significant escalation in China's approach to protecting domestic AI technology from foreign ownership, extending well beyond US-China tensions into the broader global AI industry. This marks one of the most significant interventions in a cross-border technology deal, potentially setting a precedent for future foreign acquisitions of Chinese AI companies. Manus is a general-purpose AI agent startup founded by Chinese engineers. The deal was announced in late December 2025, and regulators have now cited national security concerns as the basis for prohibition. China's NDRC also indicated the decision extends to bar foreign investment in the Manus AI project.

rss · Foreign Policy · Apr 28, 21:24

**Background**: China established a formal national security review mechanism for foreign investments in 2014, which was further strengthened in subsequent years. The Foreign Investment Security Review Working Mechanism authorizes reviews of foreign investments in covered sectors. This recent intervention aligns with broader efforts, including reported plans to restrict top Chinese technology firms—including leading AI startups—from accepting US capital without government approval.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/china-meta-manus-ai-acquisition-5f8012791f86f719a24a3ebac06d9b0a">China blocks Meta from acquiring AI startup Manus | AP News</a></li>
<li><a href="https://www.bbc.com/news/articles/cj0v0gr2yz7o">China blocks Meta's $2bn acquisition of AI start-up Manus</a></li>
<li><a href="https://technode.com/2026/04/27/china-bars-foreign-investment-in-manus-ai-project-as-scrutiny-on-ai-exports-grows/">China bars foreign investment in Manus AI project as scrutiny on AI exports grows · TechNode</a></li>

</ul>
</details>

**Tags**: `#AI Policy`, `#Geopolitics`, `#US-China Relations`, `#Tech Regulation`, `#National Security`

---

<a id="item-11"></a>
## [Japan Airlines Tests Humanoid Robots for Airport Tasks](https://arstechnica.com/ai/2026/04/japan-airlines-tests-having-robots-instead-of-humans-handle-travelers-luggage/) ⭐️ 6.0/10

Japan Airlines has begun testing humanoid robots at Haneda Airport in Tokyo to handle luggage loading, cargo operations, and aircraft cabin cleaning tasks. The pilot program aims to address Japan's persistent labor shortages in the transportation sector. This deployment represents one of the first large-scale commercial applications of humanoid robots in airport logistics, potentially setting a precedent for automation in high-labor-demand industries. If successful, similar robots could appear in airports, hotels, and warehouses worldwide as countries with aging populations seek solutions to workforce gaps. The robots are being evaluated for their ability to perform precision tasks in confined aircraft cabin spaces and handle luggage with varying weights and shapes. The test phase will determine whether the technology can meet the reliability and safety standards required for commercial airport operations.

rss · Ars Technica · Apr 28, 18:01

**Background**: Japan faces one of the world's most severe labor shortages due to its rapidly aging population and declining birth rate. The country's unemployment rate remains extremely low, making it difficult for companies in labor-intensive industries to fill positions. Humanoid robots with advanced sensors and manipulation capabilities are increasingly seen as a potential solution for tasks that have traditionally required human dexterity and judgment.

**Tags**: `#humanoid-robots`, `#robotics`, `#airport-automation`, `#labor-shortage`, `#Japan`

---

<a id="item-12"></a>
## [GitHub Copilot Shifts to Usage-Based Pricing Model](https://arstechnica.com/ai/2026/04/github-will-start-charging-copilot-users-based-on-their-actual-ai-usage/) ⭐️ 6.0/10

GitHub announced it will transition Copilot from a flat-rate subscription model to usage-based pricing. The change comes as GitHub can no longer absorb the escalating inference costs from its heaviest AI users. This pricing shift could significantly impact development teams' budgets, especially those heavily reliant on AI coding assistance. It also signals a broader industry trend where AI service providers are moving away from flat-rate models to better align costs with actual usage. AI inference costs represent approximately 95% of total compute costs in LLM operations. The decode phase is memory-bandwidth bound rather than compute-bound, making optimization particularly challenging for services with high query volumes.

rss · Ars Technica · Apr 28, 15:41

**Background**: GitHub Copilot is an AI-powered code completion tool launched in 2021, developed by GitHub in partnership with Microsoft and OpenAI. The current pricing model charges $10/month for individuals and $19/month per user for business plans. The shift reflects the economics of running large language models, where inference expenses can quickly add up as usage increases.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/inside-llm-black-box-true-architecture-latency-cost-aneel-kanuri-pqn4e">Inside the LLM Black Box: The True Architecture of Latency and Cost</a></li>

</ul>
</details>

**Tags**: `#AI pricing`, `#GitHub Copilot`, `#developer tools`, `#SaaS pricing`, `#AI costs`

---

