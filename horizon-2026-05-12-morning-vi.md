# Horizon Daily - 2026-05-11

> From 83 items, 8 important content pieces were selected

---

1. [TanStack NPM Packages Compromised](#item-1) ⭐️ 9.0/10
2. [UCLA discovers first stroke rehabilitation drug to repair brain damage (2025)](#item-2) ⭐️ 7.0/10
3. [GitLab Announces Workforce Reduction and End of Their CREDIT Values](#item-3) ⭐️ 7.0/10
4. [Linux bitten by second severe vulnerability in as many weeks](#item-4) ⭐️ 7.0/10
5. [Can someone please explain whether Cloudflare blackmailed Canonical?](#item-5) ⭐️ 6.0/10
6. [Three things in AI to watch, according to a Nobel-winning economist](#item-6) ⭐️ 6.0/10
7. [Data center guzzled 30 million gallons of water and nobody noticed for months](#item-7) ⭐️ 6.0/10
8. [Starlink shuts down its GPS-style cheat code. Researchers may unlock it anyway.](#item-8) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [TanStack NPM Packages Compromised](https://github.com/TanStack/router/issues/7383) ⭐️ 9.0/10

Popular TanStack NPM packages were compromised with malicious code that installs a dead-man's-switch mechanism. The malware monitors stolen GitHub tokens by polling api.github.com/user every 60 seconds, and if the token is revoked (returning an HTTP 40x error), it executes rm -rf ~/ to delete the user's entire home directory. This attack represents a dangerous evolution in supply chain attacks, combining data exfiltration with a punitive kill-switch that destroys user data if victims attempt recovery by revoking their compromised credentials. Developers using affected packages face potential data loss simply for trying to protect their accounts. The malicious payload uses a "prepare" lifecycle hook to execute via bun, though bun itself is immune to this attack vector. The malware achieves persistence by installing as a systemd user service on Linux (at ~/.local/bin/gh-token-monitor.sh) or as a LaunchAgent (com.user.gh-token-monitor) on macOS. The attack exploited Trusted Publishing mechanisms, demonstrating that OIDC-based publishing alone cannot prevent compromised CI pipelines from publishing malicious packages.

hackernews · varunsharma07 · May 11, 21:08

**Background**: A dead man's switch is a mechanism designed to trigger an automatic response if the operator fails to take action within a specified timeframe—in this case, activating if a GitHub token is revoked. Supply chain attacks compromise trusted software distribution channels to deliver malware, often exploiting npm's lifecycle scripts like "postinstall" or "prepare" which execute arbitrary code during package installation. Trusted Publishing is npm's mechanism to publish packages from CI using OIDC tokens instead of long-lived secrets, but it cannot protect against attacks originating from within the CI pipeline itself.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem</a></li>
<li><a href="https://ru.wikipedia.org/wiki/Переключатель_мертвеца">Переключатель мертвеца — Википедия</a></li>

</ul>
</details>

**Discussion**: The community expressed strong concerns about the attack's sophistication and design. jonchurch_ argued that Trusted Publishing alone is insufficient because attackers with access to CI credentials or repo admin rights can easily publish malicious packages, noting this isn't new information but represents a serious risk. chrisweekly criticized GitHub's architecture for making commits in forks reachable via URIs indistinguishable from legitimate repos, calling this "bonkers" and placing significant blame on GitHub. Multiple developers recommended using pnpm as a safer alternative to npm, with chuckadams stating that enabling lifecycle scripts in dependencies by default in 2026 is "plain malpractice."

**Tags**: `#security`, `#npm`, `#supply-chain-attack`, `#malware`, `#open-source`

---

<a id="item-2"></a>
## [UCLA discovers first stroke rehabilitation drug to repair brain damage (2025)](https://stemcell.ucla.edu/news/ucla-discovers-first-stroke-rehabilitation-drug-repair-brain-damage) ⭐️ 7.0/10

UCLA researchers have identified compounds that restore gamma oscillations and repair lost connections of parvalbumin neurons in stroke-damaged mouse brains, representing what they claim is the first drug candidate capable of repairing brain tissue after stroke rather than merely preventing further damage. Stroke is a leading cause of long-term disability worldwide, and current treatments focus primarily on preventing immediate damage rather than promoting actual brain repair. If this approach translates to humans, it could fundamentally change stroke rehabilitation by enabling actual regeneration of neural connections and restoration of brain function. The study (PubMed ID 39106304) demonstrates that successful physical rehabilitation brings gamma oscillations back into the brain, and the identified compounds work through the same neural mechanism involving parvalbumin neurons. However, all current testing has been conducted in mouse models, and significant regulatory hurdles remain before human trials could begin.

hackernews · bookofjoe · May 11, 17:53

**Background**: Gamma oscillations are rhythmic patterns of neural activity (typically around 40 Hz) that help synchronize neural populations and enable coordinated brain networks for behaviors like movement. Parvalbumin neurons are a specific type of inhibitory neuron crucial for generating these gamma oscillations. When stroke occurs, blood supply to part of the brain is blocked, causing rapid cell death and loss of gamma oscillations. Neural oscillations drive various cognitive functions including attention, and restoring these rhythms has shown promise in other neurological conditions through both pharmaceutical and sensory stimulation approaches.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Neural_oscillation">Neural oscillation - Wikipedia</a></li>
<li><a href="https://www.frontiersin.org/journals/medicine/articles/10.3389/fmed.2026.1730333/full">Frontiers | Light-based 40 Hz sensory therapy for brain disorders...</a></li>

</ul>
</details>

**Discussion**: Community commenters raised important questions about the 'first' claim, with one noting Clinuvel's afamelanotide treatment showed positive results though regulatory challenges halted progression. Others engaged with the neuroscience, discussing gamma oscillations and parvalbumin neurons, while some questioned the mouse model limitations with one humorous observation that it could be 'life changing for male mice.' References to Ted Chiang's 'Understand' story suggest readers find the concept of neural enhancement through drug-induced gamma restoration conceptually resonant with science fiction themes.

**Tags**: `#medical-research`, `#neuroscience`, `#stroke-rehabilitation`, `#drug-discovery`, `#brain-repair`

---

<a id="item-3"></a>
## [GitLab Announces Workforce Reduction and End of Their CREDIT Values](https://about.gitlab.com/blog/gitlab-act-2/) ⭐️ 7.0/10

GitLab announces workforce reduction and replaces their CREDIT company values with a new 'Speed with Quality' framework, removing diversity commitments.

hackernews · AnonGitLabEmpl · May 11, 20:51

**Tags**: `#corporate-culture`, `#workforce-reduction`, `#dei`, `#gitlab`, `#tech-industry`

---

<a id="item-4"></a>
## [Linux bitten by second severe vulnerability in as many weeks](https://arstechnica.com/security/2026/05/linux-bitten-by-second-severe-vulnerability-in-as-many-weeks/) ⭐️ 7.0/10

Ars Technica reports that a new severe security vulnerability in Linux has emerged, requiring immediate patching, following another critical flaw disclosed just weeks prior. Production-version patches are now coming online and users are urged to install them urgently. Linux powers a vast portion of the internet's servers, cloud infrastructure, and critical systems, making any severe vulnerability a major concern for the entire technology ecosystem. The fact that this is the second high-severity flaw in as many weeks suggests a concerning pattern of increased vulnerability discovery, potentially indicating systemic security challenges or heightened scrutiny. The vulnerability appears to be severe enough to warrant 'pronto' patching language, indicating active exploitation risk or high potential impact. Organizations running Linux-based systems should prioritize applying these production patches immediately to mitigate potential attacks.

rss · Ars Technica · May 11, 22:28

**Background**: Zero-day vulnerabilities are security flaws unknown to developers and for which no patch exists until they are discovered and addressed. These vulnerabilities are particularly dangerous because threat actors can exploit them before defenses are developed. Linux, as an open-source kernel, powers everything from web servers and cloud platforms to mobile devices and embedded systems, making vulnerabilities in it far-reaching. When a zero-day is disclosed, vendors create patches or workarounds, but the actual protection depends on users deploying those mitigations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability</a></li>
<li><a href="https://grokipedia.com/page/Zero-day_vulnerability">Zero-day vulnerability</a></li>

</ul>
</details>

**Tags**: `#Linux`, `#Cybersecurity`, `#Vulnerabilities`, `#Patches`, `#Zero-Day`

---

<a id="item-5"></a>
## [Can someone please explain whether Cloudflare blackmailed Canonical?](https://www.flyingpenguin.com/can-someone-please-explain-whether-cloudflare-blackmailed-canonical/) ⭐️ 6.0/10

The Hacker News community is debating whether Cloudflare should act as a content moderator after allegations emerged about the company pressuring Canonical during a DDoS attack situation. The discussion centers on whether Cloudflare's free tier inadvertently helps attackers while their paid protection services profit from the victims. This case highlights the broader question of platform responsibility for internet infrastructure companies. As a critical CDN and security provider, Cloudflare's decisions about which customers to serve can significantly impact both victims and perpetrators of cyber attacks. Community commenters point out significant inaccuracies in the original article, specifically that it conflates hosting an attacker's informational website with actually hosting the attack infrastructure. Some defenders argue Cloudflare should host 'everything unless and until a lawful order is received.'

hackernews · speckx · May 11, 18:12

**Background**: Cloudflare provides CDN, DNS, and DDoS protection services to millions of websites globally. The controversy touches on the 'double-edged' nature of their free tier, which can protect both legitimate websites and potentially malicious actors. The debate reflects broader tensions between free internet principles and the need to prevent abuse.

**Discussion**: Commenters are divided: some defend Cloudflare's hands-off approach as principled and consistent with free internet values, while others question whether the DDoS protection business model creates perverse incentives where the company profits from attacks on non-customers. One commenter describes the model as a 'digital protection racket.'

**Tags**: `#cloudflare`, `#content-moderation`, `#platform-responsibility`, `#internet-infrastructure`, `#ddos`

---

<a id="item-6"></a>
## [Three things in AI to watch, according to a Nobel-winning economist](https://www.technologyreview.com/2026/05/11/1137090/three-things-in-ai-to-watch-according-to-a-nobel-winning-economist/) ⭐️ 6.0/10

MIT Technology Review summarizes Nobel Prize-winning economist Daron Acemoglu's three key trends to watch in AI, drawing from his influential if controversial research on technology's economic impact. The article, published in May 2026, previews insights from his work that has drawn attention from both the academic community and Silicon Valley. Acemoglu received the 2024 Nobel Prize in Economic Sciences jointly with Simon Johnson and James A. Robinson for their studies on how institutions are formed and affect prosperity. His critical perspective on AI's macroeconomic impact carries significant weight, especially given that his AI paper reportedly earned him few fans in Silicon Valley, making this analysis particularly valuable for understanding the tension between tech industry optimism and academic scrutiny. In his paper 'The Simple Macroeconomics of AI,' Acemoglu uses a task-based model to evaluate claims about AI's large macroeconomic implications, working through automation and task complementarities. The paper establishes that as long as AI's microeconomic effects are driven by cost savings and productivity improvements at the task level, its macroeconomic consequences will follow a version of Hulten's theorem.

rss · MIT Tech Review · May 11, 17:35

**Background**: The Nobel Memorial Prize in Economic Sciences was awarded to Acemoglu, Johnson, and Robinson in 2024 for their comparative studies on prosperity among nations, specifically highlighting how institutions set up during colonization have had an enduring impact on economic outcomes. Their work contrasts with the often techno-optimistic narratives prevalent in Silicon Valley, which typically predict transformative productivity gains from AI. Acemoglu's more measured stance on AI's economic potential challenges these prevailing assumptions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Daron_Acemoglu">Daron Acemoglu - Wikipedia</a></li>
<li><a href="https://news.mit.edu/2024/mit-economists-daron-acemoglu-simon-johnson-nobel-prize-economics-1014">MIT economists Daron Acemoglu and Simon Johnson share Nobel Prize | MIT News | Massachusetts Institute of Technology</a></li>
<li><a href="https://www.nobelprize.org/prizes/economic-sciences/2024/acemoglu/facts/">Sveriges Riksbank Prize in Economic Sciences in Memory of Alfred Nobel 2024</a></li>
<li><a href="https://economics.mit.edu/sites/default/files/2024-04/The+Simple+Macroeconomics+of+AI.pdf">The Simple Macroeconomics of AI - Massachusetts Institute of ...</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#economic perspective`, `#Nobel Laureate`, `#technology regulation`, `#industry analysis`

---

<a id="item-7"></a>
## [Data center guzzled 30 million gallons of water and nobody noticed for months](https://arstechnica.com/tech-policy/2026/05/data-center-used-30-million-gallons-of-water-without-initially-paying/) ⭐️ 6.0/10

An Ars Technica investigation has revealed that a data center consumed 30 million gallons of water over several months without proper billing or oversight, sparking concerns about accountability in the rapidly expanding AI infrastructure sector. This incident highlights the growing environmental and resource challenges posed by AI data centers, which can consume as much water as a town of 10,000 to 50,000 people. As AI adoption accelerates, such resource consumption patterns demand greater transparency and regulatory scrutiny. The oversight persisted for months before discovery, with the facility consuming approximately 30 million gallons of water used for cooling systems. US data centers consumed approximately 17 billion gallons of water in 2023 alone, with hyperscale facilities accounting for 84% of this consumption.

rss · Ars Technica · May 11, 20:37

**Background**: Data centers require substantial cooling systems to manage heat generated by computing equipment. Water cooling is an efficient method that uses liquid to absorb and dissipate heat, though this process can consume significant volumes of water. The AI industry has faced increasing scrutiny over its environmental footprint, with water consumption becoming a key concern alongside energy usage. By 2028, hyperscale data centers are projected to consume up to 33 billion gallons of water annually.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eesi.org/articles/view/data-centers-and-water-consumption">Data Centers and Water Consumption | Article | EESI</a></li>
<li><a href="https://harvardsciencereview.org/2026/02/28/re-architecting-the-ai-server-the-hidden-water-cost-of-data-centers-part-ii/">Re-Architecting the AI Server: The Hidden Water Cost of Data ...</a></li>
<li><a href="https://www.aitooldiscovery.com/ai-infra/how-much-water-does-ai-use">How Much Water Does AI Use? The Real Numbers for 2026</a></li>

</ul>
</details>

**Discussion**: The incident has fueled ongoing debates about AI sustainability and accountability, with many calling for stronger regulations on data center resource consumption. Environmental advocates argue that the industry must adopt more efficient cooling technologies to reduce its ecological footprint.

**Tags**: `#data centers`, `#AI infrastructure`, `#environmental impact`, `#water consumption`, `#tech policy`

---

<a id="item-8"></a>
## [Starlink shuts down its GPS-style cheat code. Researchers may unlock it anyway.](https://arstechnica.com/gadgets/2026/05/starlink-blocks-access-to-its-gps-alternative-ahead-of-spacex-ipo/) ⭐️ 6.0/10

Starlink has closed public access to its satellite-based positioning system that was being developed as a potential GPS alternative. Researchers in the navigation community have indicated they may find ways to circumvent this restriction and continue accessing the system. The closure of Starlink's positioning service highlights the growing strategic importance of GPS alternatives for both civilian and military applications. With GPS vulnerability becoming a recognized national security concern, restrictions on backup navigation systems could impact critical infrastructure and defense capabilities ahead of SpaceX's potential IPO. Starlink's positioning system utilized signals from low Earth orbit (LEO) satellites and employed algorithms analyzing Doppler shifts and timing data to calculate user location. The system was based on research published in February 2025 that revealed the full Starlink orthogonal frequency division multiplexing (OFDM) beacon structure spanning the entire time-frequency resource grid.

rss · Ars Technica · May 11, 17:55

**Background**: Traditional GPS relies on medium Earth orbit satellites positioned approximately 20,000 kilometers above Earth, while Starlink and other LEO mega-constellations operate at much lower altitudes of around 550 kilometers. LEO-based positioning offers potential advantages including stronger signal strength, reduced latency, and better indoor penetration compared to traditional GPS. The U.S. Space Force is actively fostering an ecosystem of commercial LEO navigation providers including TrustPoint and Xona as part of a broader strategy to reduce dependence on legacy GPS systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Starlink">Starlink - Wikipedia</a></li>
<li><a href="https://navi.ion.org/content/72/1/navi.685">Unveiling Starlink for PNT | NAVIGATION: Journal of the Institute of Navigation</a></li>
<li><a href="https://www.airandspaceforces.com/space-force-ecosystem-gps-alternatives-leo/">Space Force Boosts Ecosystem of GPS Alternatives in LEO</a></li>
<li><a href="https://spacenews.com/trustpoint-sets-2027-target-for-initial-rollout-of-leo-based-navigation-services/">TrustPoint sets 2027 target for initial rollout of LEO-based ...</a></li>

</ul>
</details>

**Discussion**: The navigation research community has expressed interest in developing workarounds to access Starlink's positioning signals, viewing the closure as a challenge rather than a definitive barrier. Researchers note that the underlying satellite signals remain technically accessible, and independent analysis of the Starlink OFDM beacon structure could enable continued positioning experiments without official cooperation. The sentiment suggests strong continued interest in LEO-based navigation research despite the access restrictions.

**Tags**: `#satellite-navigation`, `#GPS-alternatives`, `#Starlink`, `#positioning-systems`, `#space-technology`

---

