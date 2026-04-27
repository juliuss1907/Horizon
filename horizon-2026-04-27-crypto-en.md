# Horizon Daily - 2026-04-27

> From 44 items, 20 important content pieces were selected

---

1. [Fast16: State-Sponsored Sabotage Tool Predating Stuxnet](#item-1) ⭐️ 8.0/10
2. [AI Should Elevate Thinking, Not Replace It](#item-2) ⭐️ 7.0/10
3. [AI Memory with Biological Decay Achieves 52% Recall](#item-3) ⭐️ 7.0/10
4. [Developer Revives Friendster Domain After $30k Purchase](#item-4) ⭐️ 6.0/10
5. [Study: 3% of Polymarket Traders Drive Price Discovery, Others Subsidize Gains](#item-5) ⭐️ 6.0/10
6. [DeFi Lost $13B This Month; KelpDAO Rescue Raised 69,550 ETH](#item-6) ⭐️ 6.0/10
7. [Google Bets on AI to Narrow Cloud Gap with AWS and Azure](#item-7) ⭐️ 5.0/10
8. [OpenAI Image Model Highlights Deepfake Crypto Scam Threat](#item-8) ⭐️ 5.0/10
9. [Litecoin DoS Attack Patched After Zero-Day Vulnerability Exploited](#item-9) ⭐️ 5.0/10
10. [Bitcoin Community Questions US Military's Crypto Readiness](#item-10) ⭐️ 5.0/10
11. [Aave DeFi Protocol Launches on Solana Blockchain](#item-11) ⭐️ 5.0/10
12. [Bitcoin Bottom May Hit $57K Based on Historical Averages: Analyst](#item-12) ⭐️ 4.0/10
13. [Coachella Tests Google DeepMind AI for Future Live Entertainment](#item-13) ⭐️ 4.0/10
14. [Iran Claims Oil Supply Potential as Hormuz Exports Drop 95%](#item-14) ⭐️ 4.0/10
15. [Scallop DeFi Protocol Loses 150K SUI in Deprecated Contract Exploit](#item-15) ⭐️ 4.0/10
16. [Senator Cruz Calls to Index Capital Gains to Inflation](#item-16) ⭐️ 4.0/10
17. [Unverified Claim: Bitmine to Acquire 10,000 ETH from Ethereum Foundation](#item-17) ⭐️ 4.0/10
18. [Bloomberg Allegedly Timed Iran Strait Story Until US Market Open](#item-18) ⭐️ 4.0/10
19. [Arthur Hayes Predicts $1M Bitcoin Driven by $15T Credit Expansion](#item-19) ⭐️ 4.0/10
20. [Babylon Foundation Deposits 3M USDT into Aave V3 and V4](#item-20) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Fast16: State-Sponsored Sabotage Tool Predating Stuxnet](https://www.sentinelone.com/labs/fast16-mystery-shadowbrokers-reference-reveals-high-precision-software-sabotage-5-years-before-stuxnet/) ⭐️ 8.0/10

SentinelLabs security researchers have uncovered Fast16, a sophisticated cyberweapon that remained undetected for 21 years and predates Stuxnet by approximately five years. The malware is designed to silently corrupt high-precision mathematical calculations in specialized domains such as civil engineering, physics, and nuclear process simulations, making scientists trust results that have been quietly compromised. This discovery reveals that nation-state actors were conducting precision software sabotage operations years before the publicly known Stuxnet attacks, fundamentally reshaping our understanding of the evolution of state-sponsored cyber weapons. The implications for scientific research integrity are profound, as any calculation-dependent industry—from nuclear facilities to civil engineering—could be silently undermined without detection. Analysis revealed that Fast16 uses SCCS/RCS source control notation—an extremely outdated system equivalent to finding a rotary phone in a modern office—suggesting the authors' programming backgrounds originated in government and military computing environments. Unlike typical malware that destroys systems, Fast16 functions as a precision instrument that spreads across networks and introduces subtle calculation errors that appear completely normal to affected systems.

hackernews · dd23 · Apr 26, 20:18

**Background**: Stuxnet, discovered in 2010, was a groundbreaking state-sponsored cyberweapon that specifically targeted Iranian nuclear centrifuge operations by causing them to spin out of control. Fast16 represents an even earlier precedent of cyber sabotage methodology, suggesting that sophisticated nation-state attackers had already developed and deployed precision-targeted malware capable of undermining scientific integrity before Stuxnet became public knowledge.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/SentinelOneXDR/comments/1sunwbb/sentinellabs_just_cracked_a_20yearold_mystery/">r/SentinelOneXDR on Reddit: SentinelLABS just cracked a 20-year-old mystery: Fast16, a state-grade sabotage tool that predates Stuxnet by five years</a></li>
<li><a href="https://hackingpassion.com/fast16-pre-stuxnet-cyber-sabotage/">Fast16: The Cyberweapon That Predates Stuxnet by Five Years - HackingPassion.com : root@HackingPassion.com-[~]</a></li>

</ul>
</details>

**Discussion**: Commenters expressed fascination with the technical findings, with one user highlighting the SCCS/RCS discovery as particularly insightful and sharing their experience at an astrophysics lab still using similarly outdated systems in 2006. Another user provided a malware sample download link for those wanting to conduct their own analysis, while a third questioned whether SCCS was truly that rare in 2005. Several commenters also speculated about the specific targets and whether the sabotage would only manifest in highly specialized simulated conditions.

**Tags**: `#malware-analysis`, `#cybersecurity`, `#stuxnet`, `#nation-state-threats`, `#historical-research`

---

<a id="item-2"></a>
## [AI Should Elevate Thinking, Not Replace It](https://www.koshyjohn.com/blog/ai-should-elevate-your-thinking-not-replace-it/) ⭐️ 7.0/10

A blog post arguing AI should augment human thinking rather than replace it has generated substantial Hacker News discussion, accumulating 289 points and 246 comments with the debate centered on AI usage models and the evolution of engineering roles. This discussion matters for software engineers navigating how to incorporate AI tools responsibly while maintaining professional competency. The community's engagement indicates widespread concern about preserving critical thinking skills as AI becomes more integrated into development workflows. Commenters identified two distinct modes of AI usage: using AI to help write code you still 'own' and fully understand, versus treating AI as an abstraction layer where code becomes a 'compile target' and maintenance is delegated to the machine. The consensus was that the latter approach is suitable only for short-lived prototypes.

hackernews · koshyjohn · Apr 26, 20:03

**Background**: AI coding assistants have become increasingly prevalent in software development, raising fundamental questions about professional identity and skill development. Hacker News serves as a major forum for tech professionals to debate these issues. The phrase 'elevate your thinking' frames AI as a cognitive tool rather than an autonomous agent, reflecting a broader philosophy of human-machine collaboration in knowledge work.

**Discussion**: Community sentiment was largely thoughtful and nuanced. Some commenters drew pragmatic parallels between AI dependency and other developer tools like IDEs or package managers, suggesting the shift is gradual and perhaps inevitable. Others expressed concern that junior developers relying on AI without understanding underlying logic might not develop essential problem-solving skills. A notable point was that AI won't help engineers who cannot think independently anyway.

**Tags**: `#AI`, `#software-engineering`, `#productivity-tools`, `#human-AI-collaboration`, `#technology-dependency`

---

<a id="item-3"></a>
## [AI Memory with Biological Decay Achieves 52% Recall](https://github.com/sachitrafa/YourMemory) ⭐️ 7.0/10

A GitHub project called YourMemory implements AI memory management using the Ebbinghaus forgetting curve and a graph layer over vector stores. Benchmarked on the LoCoMo dataset, it achieved 52% Recall@5—nearly double the accuracy of stateless vector stores—while reducing token waste by approximately 84%. This approach addresses a critical pain point in production RAG systems: context window noise caused by storing every transient detail indefinitely. By treating memory as a living substrate that can be pruned, developers can maintain reasoning quality while controlling token costs—a practical concern as context window usage directly impacts API expenses. The implementation assigns each memory a "strength" score that increases with recall and decreases over time, following the Ebbinghaus curve. The graph layer solves the "logical neighbor" problem where semantic search fails to find relevant but non-similar nodes. Built as a local-first MCP server using DuckDB, the system experiments with the hypothesis that for long-running agents, "what to forget" is equally important as "what to remember."

hackernews · SachitRafa · Apr 26, 20:58

**Background**: RAG (Retrieval-Augmented Generation) systems combine large language models with external knowledge retrieval. Traditional RAG stores all retrieved information permanently, causing context windows to fill with noise over time—a problem called "context pollution." The Ebbinghaus forgetting curve, established by Hermann Ebbinghaus in 1885, describes how memory retention declines exponentially without reinforcement, forming the basis of spaced repetition learning systems. The LoCoMo (Long Conversation Memory) benchmark specifically evaluates long-term conversational memory capabilities using annotated multi-session dialogue data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ebbinghaus_forgetting_curve">Ebbinghaus forgetting curve</a></li>
<li><a href="https://github.com/snap-research/locomo">GitHub - snap-research/locomo · GitHub</a></li>
<li><a href="https://modelcontextprotocol.io/docs/getting-started/intro">What is the Model Context Protocol (MCP)? - Model Context Protocol</a></li>

</ul>
</details>

**Discussion**: The HN discussion reveals practical concerns about AI memory implementations. Users report that existing memory systems often hurt productivity by causing agents to "second guess" based on outdated context or mix unrelated projects. One commenter described building a 4B model to actively curate and rank memories for injection, highlighting the challenge of deciding what information deserves storage. Some philosophically questioned whether mimicking human forgetting is the right approach, arguing it could inherit human cognitive limitations. The consensus suggests memory curation—not just retention—remains an unsolved problem in AI agent design.

**Tags**: `#ai-memory`, `#rag-systems`, `#spaced-repetition`, `#knowledge-graphs`, `#llm-agents`

---

<a id="item-4"></a>
## [Developer Revives Friendster Domain After $30k Purchase](https://ca98am79.medium.com/i-bought-friendster-for-30k-heres-what-i-m-doing-with-it-d5e8ddb3991d) ⭐️ 6.0/10

A developer purchased the Friendster domain (friendster.com) for approximately $30,000 through a combination of Bitcoin and a domain trade, and is now attempting to revive the pioneering social network that operated from 2002 to 2015. The app was rejected by Apple's App Store under Guideline 4.2 for Minimum Functionality. This revival attempt highlights debates about platform power, as the app rejection raises questions about whether Apple should dictate what apps users can install on their phones. It also tests whether nostalgic brand revival can compete against established social media giants, and whether unique features like the 'tapping phones' decay mechanic can attract users seeking alternatives to mainstream platforms. The deal structure involved $20,000 in Bitcoin plus a domain generating approximately $9,000/year in ad revenue. The proposed Friendster revival includes a 'tapping phones' feature where connections decay over time based on user interaction—a design that has drawn criticism from community members who find it potentially annoying and inappropriate for maintaining connections with deceased friends.

hackernews · ca98am79 · Apr 26, 20:41

**Background**: Friendster was one of the earliest social networking services, founded by Jonathan Abrams and launched in March 2002 in Mountain View, California. It pioneered features like friend connections and content sharing that would later become standard in social platforms. However, the service declined after being outcompeted by MySpace and Facebook, eventually shutting down in 2015. Domain name trading is a separate investment market where valuable domains are bought, sold, and traded as digital assets that can appreciate significantly over time.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Friendster">Friendster - Wikipedia</a></li>
<li><a href="https://blog.tangerines.io/remember-friendster-me-neither-f8d9814b24d6">Remember Friendster ? Me neither. Social networking has become...</a></li>
<li><a href="https://www.financialpoise.com/whats-in-a-domain-name-an-explainer-on-domain-investing/">What’s In a Domain Name ? An Explainer on Domain Investing</a></li>

</ul>
</details>

**Discussion**: Community comments reveal diverse concerns: one user argues Apple should not control what apps users can install, calling for laws regulating mobile platforms; another finds the 'tapping phones' decay feature potentially annoying and inappropriate, especially for connections with deceased loved ones; a third user notes difficulty finding the app in the App Store amid sponsored ads for competing platforms. Overall sentiment suggests skepticism about both the platform regulation issues and the product design viability.

**Tags**: `#social-networks`, `#startup-stories`, `#platform-regulation`, `#app-store-policies`, `#revival-projects`

---

<a id="item-5"></a>
## [Study: 3% of Polymarket Traders Drive Price Discovery, Others Subsidize Gains](https://www.theblock.co/post/398902/skilled-polymarket-traders-are-a-3-minority-and-everyone-else-funds-their-gains-study?utm_source=rss&utm_medium=rss) ⭐️ 6.0/10

A working paper analyzing all Polymarket trades from 2023 to 2025 found that approximately 3% of accounts are responsible for generating the bulk of price discovery, while the remaining 97% of accounts essentially subsidize their gains. This finding highlights significant inequality in prediction market participation, where the vast majority of traders act as effective liquidity providers for a skilled minority. It has implications for market design, retail trader protection, and understanding how information gets incorporated into prices in crypto-based markets. The study analyzed the complete trade history across all markets on Polymarket, a decentralized prediction market built on the Polygon blockchain. The concentration of price discovery in just 3% of accounts suggests that most participants lack the skills or information edge needed to consistently contribute to price formation.

rss · The Block · Apr 26, 22:40

**Background**: Polymarket is a cryptocurrency-based prediction market platform that allows users to trade shares on the outcomes of real-world events. Price discovery refers to the process by which buyers and sellers interact to determine acceptable prices for assets, reflecting the balance of supply and demand. Prediction markets are designed to aggregate information and generate forecasts, with the assumption that market prices reflect collective wisdom. However, this study suggests that in practice, price discovery on Polymarket is driven by a small group of skilled participants rather than broad market participation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Polymarket">Polymarket - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Price_discovery">Price discovery - Wikipedia</a></li>
<li><a href="https://www.investopedia.com/terms/p/pricediscovery.asp">Price Discovery Explained: Process, Factors, and Comparison with Valuation</a></li>

</ul>
</details>

**Tags**: `#prediction-markets`, `#market-structure`, `#polymarket`, `#trading-analysis`, `#crypto-markets`

---

<a id="item-6"></a>
## [DeFi Lost $13B This Month; KelpDAO Rescue Raised 69,550 ETH](https://cryptoslate.com/defi-lost-13b-this-month-as-the-kelpdao-rescue-shows-both-the-best-and-worst-of-defi/) ⭐️ 6.0/10

DeFi suffered $13 billion in losses this month, while the KelpDAO community successfully raised 69,550 ETH from 222 wallets across 1,623 transfers to restore rsETH backing after a hack exploited the LayerZero cross-chain bridge on April 20, 2026. This event reveals the dual nature of DeFi: extreme systemic vulnerability alongside emergent community-organized resilience that can mobilize capital without any central authority, regulator, or formal mandate. The rescue effort is being described as the closest thing the industry has built to a 'lender of last resort,' functioning as DeFi's emergency recapitalization desk. The hack targeted rsETH's LayerZero bridge, marking the largest DeFi exploit of 2026 to date.

rss · CryptoSlate · Apr 26, 20:35

**Background**: KelpDAO is a decentralized protocol on Ethereum that enables restaking through liquid restaked tokens (LRTs), with rsETH serving as its primary restaking asset built on EigenLayer. Liquid staking derivatives (LSDs) allow users to earn additional yield on staked assets by using them as collateral in DeFi applications. The concept of a 'lender of last resort' traditionally refers to central banks providing emergency liquidity to stabilize financial systems, but in this case, the crypto community self-organized such a function without any institutional backing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bitrue.com/blog/what-is-kelpdao">What Is KelpDAO ?</a></li>
<li><a href="https://lookonchain.com/feeds/54296">rsETH Hack Event Protocol Responses Overview: Multi-Party Pause of...</a></li>
<li><a href="https://www.coingecko.com/learn/what-is-liquid-staking-liquid-staked-derivatives-you-need-to-know">What is Liquid Staking? 5 Liquid Staked Derivatives You Need To Know</a></li>

</ul>
</details>

**Discussion**: The crypto community is analyzing this event as a pivotal test of DeFi's capacity for self-healing. While the successful 69,550 ETH raise demonstrates remarkable solidarity, critics question whether ad-hoc community rescues create moral hazard by making risky protocols 'too big to fail.'

**Tags**: `#DeFi`, `#KelpDAO`, `#Decentralized Finance`, `#Crypto Markets`, `#Community Rescue`

---

<a id="item-7"></a>
## [Google Bets on AI to Narrow Cloud Gap with AWS and Azure](https://www.ft.com/content/2429f0f0-b685-4747-b425-bf8001a2e94c) ⭐️ 5.0/10

Google is leveraging its AI capabilities to compete more aggressively with Amazon and Microsoft in the cloud computing market, according to Financial Times reporting. The company is positioning AI as a key differentiator in its efforts to close the market share gap with these competitors. The cloud infrastructure market has become one of the most competitive sectors in technology, with AWS holding approximately 29% and Azure around 20-24% of global market share. Google's push with AI could reshape the competitive landscape and affect enterprise cloud spending decisions worth billions of dollars annually. According to Q1 2024 data from Canalys, global cloud infrastructure services spending surged 21% to $79.8 billion. Edge AI technology is increasingly relevant to this competition, enabling local data processing without full reliance on centralized cloud infrastructure, which may play into Google's technological strengths.

hackernews · donsupreme · Apr 27, 00:34

**Background**: The cloud computing market is dominated by three major players—Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform—controlling approximately 66% of the global market. AWS leads with over 250 services, while Microsoft Azure has shown strong growth with 14.2% customer base expansion. Google Cloud has historically ranked third but is investing heavily in AI integration to gain competitive advantage. Edge AI, which processes data closer to its source rather than in distant data centers, represents a growing area of differentiation in cloud services.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Edge_computing">Edge computing - Wikipedia</a></li>
<li><a href="https://hginsights.com/blog/microsoft-azure-market-share-report/">Microsoft Azure Market Share & Buyer Landscape Report | HG Insights</a></li>
<li><a href="https://www.cisco.com/site/us/en/learn/topics/artificial-intelligence/what-is-edge-ai.html">What is Edge Computing in AI? - Cisco</a></li>

</ul>
</details>

**Discussion**: Community comments reflect both humor and genuine concern about big tech concentration. One commenter quoted the famous Dune line 'Whoever controls the spice, controls the universe,' drawing a parallel to tech companies' control over critical infrastructure. Another expressed visceral unease about the growing power of these companies, suggesting a broader public awareness of how deeply these cloud providers have embedded themselves in critical digital infrastructure.

**Tags**: `#cloud-computing`, `#google`, `#artificial-intelligence`, `#tech-industry`, `#business-strategy`

---

<a id="item-8"></a>
## [OpenAI Image Model Highlights Deepfake Crypto Scam Threat](https://cryptoslate.com/ai-scams-in-crypto-are-hitting-a-breaking-point-openais-new-image-model-shows-why-they-could-get-worse/) ⭐️ 5.0/10

A crypto founder's laptop was compromised during a Microsoft Teams call featuring an AI-generated deepfake impersonating Pierre Kaklamanos from the Cardano Foundation. The attack illustrates how OpenAI's advanced image generation capabilities are being weaponized for social engineering attacks targeting the cryptocurrency industry. This incident demonstrates the increasingly sophisticated nature of AI-powered scams targeting crypto users, with financial losses from AI-driven hacks and deepfake threats already exceeding $600 million in 2026. As deepfake technology becomes more accessible, traditional trust-based verification methods in the crypto space are becoming dangerously unreliable. North Korean threat actors known as UNC1069 have been identified targeting the cryptocurrency sector using AI-enabled social engineering tactics including deepfakes and ClickFix techniques. CertiK has warned that real-time deepfakes, AI-powered phishing, and supply chain compromises are the primary drivers of these massive crypto losses.

rss · CryptoSlate · Apr 26, 19:00

**Background**: Deepfakes use AI algorithms, particularly Generative Adversarial Networks (GANs), to create highly realistic fake audio and video content. ChatGPT Images 2.0, OpenAI's latest image generation model, features improved text rendering and multilingual support, making it increasingly difficult to distinguish AI-generated content from authentic media. The cryptocurrency industry is particularly vulnerable to these attacks due to its pseudonymous nature and irreversible transactions.

<details><summary>References</summary>
<ul>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/unc1069-targets-cryptocurrency-ai-social-engineering">UNC1069 Targets Cryptocurrency Sector with New Tooling and AI ...</a></li>
<li><a href="https://www.msn.com/en-us/news/other/ai-driven-hacks-and-deepfake-threats-push-2026-crypto-losses-past-600m/gm-GML08D5CEC">AI-driven hacks and deepfake threats push 2026 crypto ... - MSN</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT_Image">GPT Image - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Security experts have expressed growing concerns about the convergence of advanced AI tools and cryptocurrency attacks. The community widely agrees that traditional verification methods such as video calls are no longer sufficient to confirm identity, with some calling for the adoption of cryptographic verification methods like zero-knowledge proofs.

**Tags**: `#AI scams`, `#Deepfakes`, `#Crypto security`, `#Social engineering`, `#OpenAI`

---

<a id="item-9"></a>
## [Litecoin DoS Attack Patched After Zero-Day Vulnerability Exploited](https://bitcoinist.com/litecoin-suffer-denial-of-service-attack-due-to-bug/) ⭐️ 5.0/10

Major Litecoin mining pools were hit by a Denial-of-Service attack on April 25 due to a zero-day vulnerability in the network. The Litecoin Foundation confirmed that the bug has been patched and the network is fully operational, while the attacker also attempted to exploit cross-chain protocols for double-spend attacks. This incident highlights the ongoing security vulnerabilities in major blockchain networks, even when quickly patched. The combination of DoS attacks with attempted cross-chain protocol exploits demonstrates increasingly sophisticated attack vectors targeting cryptocurrency infrastructure. The attack specifically targeted major mining pools rather than individual nodes, suggesting a focused effort to disrupt Litecoin's mining infrastructure. Cross-chain protocols, also known as bridges, enable users to send cryptocurrencies between different blockchains, creating potential security vectors when exploited.

rss · Bitcoinist · Apr 26, 22:00

**Background**: Litecoin is one of the oldest cryptocurrencies, created in 2011 as a 'silver to Bitcoin's gold.' It uses a proof-of-work consensus mechanism similar to Bitcoin. Denial-of-service attacks flood a network with traffic to make it unavailable, while zero-day vulnerabilities are unknown security flaws that can be exploited before patches are developed. Cross-chain protocols enable interoperability between different blockchain networks, allowing for atomic swaps and asset transfers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Double-spending">Double-spending - Wikipedia</a></li>
<li><a href="https://medium.com/@jossif.elefteriadis/bridging-the-divide-an-in-depth-look-at-cross-chain-protocols-in-defi-b47b48d9fbe0">Bridging the Divide: An In-depth Look at Cross - Chain Protocols in DeFi</a></li>

</ul>
</details>

**Tags**: `#cryptocurrency`, `#Litecoin`, `#security`, `#DoS attack`, `#blockchain`

---

<a id="item-10"></a>
## [Bitcoin Community Questions US Military's Crypto Readiness](https://bitcoinist.com/bitcoin-community-questions-us-militarys-role-in-the-network/) ⭐️ 5.0/10

Iran has begun accepting Bitcoin as payment for oil shipping tolls through the Strait of Hormuz, reviving debate in Washington about whether the US military comprehends cryptocurrency sufficiently to leverage it as a tool of national power. The US military has confirmed it is running a Bitcoin node for cybersecurity testing and operational defense purposes. This development highlights the growing intersection of cryptocurrency and geopolitics, as nation-states increasingly recognize Bitcoin's potential as a strategic asset. The US military's engagement with Bitcoin infrastructure signals recognition that understanding and potentially leveraging cryptocurrency could be crucial for future national security and power projection. Admiral Samuel Paparo, head of US Indo-Pacific Command, disclosed during House Armed Services Committee hearings that the command is monitoring the Bitcoin network and running operational tests tied to defense systems. The military's approach appears pragmatic rather than ideological, evaluating tools based on their utility for power projection versus China.

rss · Bitcoinist · Apr 26, 20:00

**Background**: Bitcoin, created in 2009, is a decentralized digital currency that operates on a peer-to-peer network without central authority control. The Strait of Hormuz is a critical global oil shipping route, with approximately 21 million barrels passing through daily. As nations like Iran, Russia, and China explore cryptocurrency for international transactions, the US faces pressure to understand and potentially weaponize this technology for strategic advantage.

<details><summary>References</summary>
<ul>
<li><a href="https://www.forbes.com/sites/digital-assets/2026/04/26/top-admiral-calls-bitcoin-a-tool-of-power-projection-amid-us-china-clash/">Top Admiral Calls Bitcoin A Tool Of ‘Power Projection’ Amid ...</a></li>
<li><a href="https://www.analyticsinsight.net/news/us-military-confirms-bitcoin-node-use-for-cybersecurity-testing">US Military Confirms Bitcoin Node Use for Cybersecurity Testing</a></li>

</ul>
</details>

**Discussion**: The discussion reflects growing concern about whether traditional military doctrine can adapt to cryptocurrency's unique characteristics. Some observers view the US military's Bitcoin node as a pragmatic step toward understanding emerging technologies, while others question whether running a single node provides meaningful strategic capability. The broader debate centers on whether cryptocurrency expertise should be integrated into military planning or treated as a separate domain.

**Tags**: `#cryptocurrency`, `#geopolitics`, `#bitcoin-adoption`, `#US-policy`, `#energy-trade`

---

<a id="item-11"></a>
## [Aave DeFi Protocol Launches on Solana Blockchain](https://t.me/DegenerateNews/3323) ⭐️ 5.0/10

Aave, one of the largest decentralized finance (DeFi) lending protocols, has officially launched on the Solana blockchain network, marking its expansion beyond its primary Ethereum-based ecosystem. This launch brings Aave's proven lending infrastructure to Solana's high-performance blockchain, potentially opening the protocol to millions of new users and expanding its total value locked (TVL) beyond Ethereum. For Solana users, it means access to one of the most established DeFi lending platforms with its audited smart contracts and governance model. While the announcement lacks specific technical details such as supported tokens, initial TVL targets, or fee structures, Aave's Solana deployment reportedly leverages the blockchain's high throughput and low transaction costs. As one of the first major DeFi blue-chip protocols to expand to Solana, this deployment may set a precedent for further institutional DeFi adoption on the network.

telegram · DegenerateNews · Apr 27, 01:08

**Background**: Aave is a decentralized non-custodial liquidity market protocol where users can deposit crypto assets into pools to earn interest, or borrow against their collateral. When users deposit tokens, they receive aTokens (like aETH for ETH deposits), which accrue interest automatically. The protocol operates through governance where AAVE token holders vote on risk parameters. Solana is a high-performance blockchain using Proof of History consensus, known for processing thousands of transactions per second with low fees, making it attractive for DeFi applications that require frequent interactions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Aave">Aave - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/pulse/ultimate-guide-multi-chain-token-deployment-defi-web3-anu-geethan-g2cke">Ultimate Guide to Multi- Chain Token Deployment</a></li>

</ul>
</details>

**Tags**: `#DeFi`, `#Aave`, `#Solana`, `#Blockchain`, `#Cryptocurrency`

---

<a id="item-12"></a>
## [Bitcoin Bottom May Hit $57K Based on Historical Averages: Analyst](https://cointelegraph.com/news/bitcoin-bottom-57k-level-october?utm_source=rss_feed&utm_medium=rss&utm_campaign=rss_partner_inbound) ⭐️ 4.0/10

An analyst suggests Bitcoin's bottom could settle around $57,000 based on historical price averages, following the cryptocurrency's rejection from the $80,000 resistance level on its path toward reclaiming the $100,000 psychological mark. This analysis provides traders and investors with a potential support level to watch, helping them gauge risk and set entry points. Understanding where historical averages align with price action can inform decisions in a market known for volatility. The $80,000 level represents Bitcoin's immediate resistance zone, while $100,000 serves as the next major psychological milestone. Historical moving averages are commonly used in technical analysis to identify potential support and resistance zones based on prior price behavior.

rss · CoinTelegraph · Apr 26, 22:30

**Background**: Bitcoin is the largest cryptocurrency by market capitalization, frequently traded against the US dollar (BTC/USD). Moving averages are calculated by taking the average of Bitcoin's price over a specific period—such as 50, 100, or 200 days—to smooth out price fluctuations and identify trends. Support levels indicate where buying pressure historically exceeds selling pressure, while resistance levels mark zones where selling pressure tends to cap further gains.

<details><summary>References</summary>
<ul>
<li><a href="https://www.investing.com/crypto/bitcoin/historical-data">Bitcoin Historical Data - Investing.com</a></li>
<li><a href="https://www.tradingview.com/symbols/BTCUSD/">BTC USD — Bitcoin Price and Chart — TradingView</a></li>
<li><a href="https://www.barchart.com/crypto/quotes/^BTCUSD/cheat-sheet">BTCUSD Trader's Cheat Sheet for Bitcoin - Barchart.com</a></li>

</ul>
</details>

**Tags**: `#cryptocurrency`, `#bitcoin`, `#price-analysis`, `#market-prediction`, `#trading`

---

<a id="item-13"></a>
## [Coachella Tests Google DeepMind AI for Future Live Entertainment](https://decrypt.co/365532/coachella-google-deepmind-ai-test-future-live-entertainment?utm_source=telegram&amp;utm_medium=social&amp;utm_campaign=smt) ⭐️ 4.0/10

The Coachella Valley Music Festival has announced a collaboration with Google DeepMind to explore AI-powered artist tools, immersive digital worlds, and 3D performance archives designed to enhance future fan experiences. This partnership represents one of the most high-profile experiments with AI in live entertainment, potentially setting a precedent for how major music festivals leverage advanced technology to create more interactive and personalized fan engagement. The initiative focuses on three main areas: developing AI tools to assist artists in creation, building immersive digital environments for fans, and establishing 3D archives that preserve performances in three-dimensional digital form. However, specific technical implementation details remain limited in the current announcement.

telegram · Decrypt · Apr 26, 19:05

**Background**: Google DeepMind is the AI research division of Google, focused on developing advanced artificial intelligence systems with capabilities spanning language models, image generation, and multimodal AI. The Coachella Valley Music and Arts Festival is an annual music event held in Indio, California, known for featuring diverse artists across multiple genres. Immersive digital experiences typically leverage technologies such as virtual reality, augmented reality, and mixed reality to create interactive environments that blend digital content with physical spaces. Digital archiving through 3D scanning involves using specialized hardware to capture the physical dimensions and appearance of objects or spaces, creating comprehensive digital records that can be preserved and revisited over time.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_DeepMind">Google DeepMind - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/3D_scanning">3 D scanning - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI in entertainment`, `#Google DeepMind`, `#live events`, `#immersive technology`, `#digital experience`

---

<a id="item-14"></a>
## [Iran Claims Oil Supply Potential as Hormuz Exports Drop 95%](https://beincrypto.com/iran-oil-cards-us-gasoline-summer/) ⭐️ 4.0/10

Iran claims it has untapped oil supply capabilities while exports through the Strait of Hormuz remain down approximately 95%. This claim comes as the United States enters its peak summer gasoline demand season, typically the highest consumption period of the year for American drivers. The Strait of Hormuz handles over 20% of global oil exports, making any disruption highly significant for global energy markets. If Iran can actually deploy additional oil supply despite current sanctions, it could affect global crude prices and complicate U.S. energy policy during a politically sensitive period. According to EIA assessments, if all oil sanctions on Iran were lifted, the country's crude oil production could return to full capacity of approximately 3.8 million barrels per day. The U.S. has recently intensified sanctions targeting Iran's oil trade network, including Chinese teapot refineries and approximately 40 shipping vessels and associated firms.

rss · BeInCrypto · Apr 26, 21:05

**Background**: The Strait of Hormuz is a critical maritime chokepoint approximately 35 to 60 miles wide that serves as the primary export route for oil produced by Saudi Arabia, the UAE, Kuwait, Qatar, Iraq, Bahrain, and Iran. If shipping through this strait were significantly disrupted for an extended period, it could trigger a major oil supply crisis for major Asian importers including Japan, India, South Korea, and China. The United States has been actively working to disrupt Iran's illicit oil trade, which the State Department describes as the Iranian regime's primary revenue stream funding regional destabilization.

<details><summary>References</summary>
<ul>
<li><a href="https://www.iea.org/about/oil-security-and-emergency-response/strait-of-hormuz">Strait of Hormuz - About - IEA</a></li>
<li><a href="https://www.eia.gov/international/content/analysis/countries_long/Iran/pdf/Iran+CAB+2024.pdf">Country Analysis Brief: Iran</a></li>
<li><a href="https://home.treasury.gov/news/press-releases/sb0472">Economic Fury Targets Global Network Fueling Iran’s Oil Trade ...</a></li>

</ul>
</details>

**Tags**: `#oil-markets`, `#geopolitics`, `#energy-trading`, `#iran`, `#gasoline-demand`

---

<a id="item-15"></a>
## [Scallop DeFi Protocol Loses 150K SUI in Deprecated Contract Exploit](https://beincrypto.com/scallop-sui-defi-exploit-150k/) ⭐️ 4.0/10

Scallop, a DeFi protocol built on the Sui blockchain, suffered an exploit that drained approximately 150,000 SUI from a deprecated rewards contract. The Scallop team has committed to covering the full amount of user losses from the incident. This incident highlights the persistent security risks of failing to properly sunset deprecated smart contracts in DeFi protocols. It underscores a common but critical failure in operational security hygiene, where old contract code remains exploitable even after being replaced. For Sui DeFi users, the event raises questions about how rigorously protocols manage their contract lifecycles. The exploit targeted the sSUI rewards pool, and the MEXC report mentions the attack revealed a decades-old bug lurking in the deprecated contract code. At current prices, the 150,000 SUI loss represents approximately $300,000. Unlike some DeFi exploits, the team has taken responsibility and pledged to reimburse affected users directly.

rss · BeInCrypto · Apr 26, 20:16

**Background**: Sui is a Layer 1 blockchain developed by Mysten Labs that uses the Move programming language and features parallel transaction execution for high throughput. Smart contracts on blockchains like Sui are immutable by design, meaning once deployed they cannot be directly modified or shut down—only deprecated or replaced with new versions. Deprecated contracts can still hold user funds and remain vulnerable to exploits if not properly secured or migrated. Scallop is a DeFi lending and yield protocol on the Sui ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mexc.com/news/1055078">Scallop Exploit Drains 150K SUI Through Deprecated Contract ...</a></li>
<li><a href="https://coincentral.com/sui-guide/">Sui Blockchain Explained: How It Works and What You Need to Know</a></li>
<li><a href="https://chainscorelabs.com/guides/developer-experience-dx-blockchain-tools-and-analytics/smart-contract-lifecycle/setting-up-a-contract-end-of-life-and-sunsetting-procedure">How to Sunset a Smart Contract: End-of-Life Procedure</a></li>

</ul>
</details>

**Tags**: `#DeFi Security`, `#Sui Blockchain`, `#Smart Contract Exploit`, `#Cryptocurrency Hack`, `#DeFi Protocol`

---

<a id="item-16"></a>
## [Senator Cruz Calls to Index Capital Gains to Inflation](https://t.me/CoinBureau/13110) ⭐️ 4.0/10

Senator Ted Cruz publicly called for indexing capital gains to inflation as an economic measure to support the economy and improve affordability, expressing desire for implementation before Election Day. This proposal could significantly affect crypto investors and traditional asset holders by reducing their effective tax burden on investment gains. The initiative is part of a broader conservative coalition pushing the Treasury Department to implement capital gains indexation unilaterally through executive action. Capital gains indexation adjusts the purchase price of assets for inflation, meaning investors would only pay taxes on real gains rather than nominal gains inflated away. Analysis indicates the top 0.1% by income would receive an average tax cut of approximately $350,000, while the bottom two income quintiles would not benefit at all, making the proposal regressive.

telegram · CoinBureau · Apr 26, 20:04

**Background**: Capital gains tax is currently levied on the nominal profit from selling assets, which can create an unfair burden when inflation erodes the real value of gains. Indexing capital gains to inflation would adjust the cost basis of assets to account for inflation, reducing the taxable gain. This policy has been debated for years, with proponents arguing it is a fair tax reform and opponents warning it would disproportionately benefit wealthy individuals and add hundreds of billions to the national debt. Previous House bills have included provisions for capital gains indexation alongside rate reductions.

<details><summary>References</summary>
<ul>
<li><a href="https://tax.thomsonreuters.com/news/debate-over-indexing-capital-gains-to-inflation-reignites/">Debate Over Indexing Capital Gains to Inflation Reignites</a></li>
<li><a href="https://bipartisanpolicy.org/article/should-the-treasury-department-index-capital-gains-for-inflation/">Should the Treasury Department Index Capital Gains for Inflation?</a></li>
<li><a href="https://budgetlab.yale.edu/research/indexing-capital-gains-inflation">Indexing Capital Gains to Inflation | The Budget Lab</a></li>

</ul>
</details>

**Tags**: `#crypto-regulation`, `#capital-gains`, `#tax-policy`, `#us-politics`, `#inflation`

---

<a id="item-17"></a>
## [Unverified Claim: Bitmine to Acquire 10,000 ETH from Ethereum Foundation](https://t.me/CoinBureau/13119) ⭐️ 4.0/10

A Telegram channel (CoinBureau) reports that Bitmine Immersion Technologies, associated with Tom Lee, plans to acquire an additional 10,000 ETH from the Ethereum Foundation through an OTC transaction valued at $23.9 million. The deal would bring Bitmine's total holdings to 4.98 million ETH. This claim, if true, would represent a significant institutional accumulation of ETH and could signal Ethereum Foundation's ongoing treasury management strategy. However, the unverified nature of this report highlights the prevalence of unconfirmed rumors circulating in crypto Telegram channels, which can influence market sentiment. The news item rates 4.0/10 due to lack of verification from either party involved. Bitmine Immersion Technologies is not a widely recognized entity in the crypto space, and a private company's goal to reach '5% supply' represents an extraordinary claim that would be difficult to achieve without broader market attention.

telegram · CoinBureau · Apr 27, 01:42

**Background**: OTC (Over-The-Counter) trading is common in cryptocurrency for large transactions, allowing parties to trade directly without affecting market prices through standard exchanges. Cointelegraph previously reported a confirmed $10.2 million OTC deal where the Ethereum Foundation sold 5,000 ETH to BitMine, suggesting a pattern may exist. The Ethereum Foundation has conducted corporate ETH treasury sales as part of reserve management.

<details><summary>References</summary>
<ul>
<li><a href="https://cointelegraph.com/news/ethereum-foundation-sells-eth-to-bitmine-otc-deal">BitMine Buys 5,000 ETH From Ethereum Foundation in $10.2M OTC ...</a></li>
<li><a href="https://samouraiwallet.com/blog/otc-meaning-crypto">OTC Meaning in Crypto: How OTC Trading Works, Benefits, Risks</a></li>

</ul>
</details>

**Discussion**: Given the low credibility score and unverified nature of this claim, the crypto community is likely to treat this with significant skepticism. No confirmation has been provided by the Ethereum Foundation or Bitmine Immersion Technologies, and the extraordinary nature of the 5% supply target raises doubts about the authenticity of this report.

**Tags**: `#ethereum`, `#OTC deal`, `#institutional`, `#unverified rumor`, `#ethereum foundation`

---

<a id="item-18"></a>
## [Bloomberg Allegedly Timed Iran Strait Story Until US Market Open](https://t.me/CoinBureau/13121) ⭐️ 4.0/10

A post claims Bloomberg deliberately delayed reporting an Iran proposal about reopening the Strait of Hormuz until US markets opened, even though the same story was published by Axios 11 hours earlier. Markets reportedly pumped on the Bloomberg headline, suggesting significant market impact from the timed release. This raises serious questions about media timing practices and potential market manipulation by financial news organizations. If verified, such coordinated timing could undermine trust in financial news as an impartial information source and highlight how information asymmetry affects retail investors versus institutional players. The claims remain unverified and lack substantive evidence beyond the poster's assertion. The content is brief and lacks documentation of the 11-hour gap. The post reads more as engagement-bait than rigorous investigative journalism, offering no verifiable proof of deliberate market manipulation.

telegram · CoinBureau · Apr 27, 02:15

**Background**: The Strait of Hormuz is one of the world's most critical maritime chokepoints, carrying approximately 25% of global seaborne oil trade and about 20% of global LNG trade. Bloomberg is a major financial news and data company whose headlines can move markets. Axios is a digital news outlet founded in 2016 by former Politico journalists, known for its concise reporting style. Any disruption to this strait would have enormous consequences for world oil markets, making headlines about it particularly market-sensitive.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Axios_(website)">Axios (website) - Wikipedia</a></li>
<li><a href="https://www.iea.org/about/oil-security-and-emergency-response/strait-of-hormuz">Strait of Hormuz - About - IEA</a></li>
<li><a href="https://www.eia.gov/todayinenergy/detail.php?id=65504">Amid regional conflict, the Strait of Hormuz remains critical ...</a></li>

</ul>
</details>

**Tags**: `#media-manipulation`, `#market-timing`, `#financial-markets`, `#news-analysis`, `#conspiracy-theory`

---

<a id="item-19"></a>
## [Arthur Hayes Predicts $1M Bitcoin Driven by $15T Credit Expansion](https://x.com/WuBlockchain/status/2048477212177793402) ⭐️ 4.0/10

BitMEX创始人Arthur Hayes在2025年9月23日的韩国区块链周上表示，美国政府通过Genius Act和稳定币监管政策寻找短期美国国债的价格非弹性买家，这种策略可能导致2028年前信贷扩张规模达到15.2万亿美元，并推动比特币价格突破100万美元大关。 这一预测将比特币走势与美国货币政策和稳定币立法直接挂钩，暗示加密货币市场将受到政府债务管理策略的深刻影响。如果Hayes的判断准确，传统金融市场与加密货币之间的界限将进一步模糊，对投资者和政策制定者都具有重要意义。 Hayes声称美国政府因担心发行长期债务而选择利用稳定币持有短期国债，并预测这种极端的宏观经济宽松政策将打破传统的四年周期。他将比特币目标价定在100万美元以上，但这一预测缺乏具体的技术分析支撑，主要依赖于对货币政策走向的假设。

telegram · wublockchainenglish · Apr 27, 00:13

**Background**: GENIUS Act（美国稳定币创新与监管法案）于2025年7月颁布，旨在为支付稳定币建立监管框架，允许符合条件的发行机构发行稳定币供美国居民使用。根据最新进展，该法案的实施规则将在2027年前逐步完善。Arthur Hayes是BitMEX交易所的创始人，近年来以对宏观经济的激进预测而闻名加密货币社区，但其预测的准确性和方法论一直存在争议。

<details><summary>References</summary>
<ul>
<li><a href="https://www.congress.gov/bill/119th-congress/senate-bill/1582">S.1582 - 119th Congress (2025-2026): GENIUS Act</a></li>
<li><a href="https://www.morganlewis.com/pubs/2026/04/genius-act-implementation-key-proposals-and-what-comes-next">GENIUS Act Implementation: Key Proposals and What Comes Next</a></li>

</ul>
</details>

**Tags**: `#Bitcoin`, `#Arthur Hayes`, `#Macroeconomics`, `#Federal Reserve`, `#Stablecoin Regulation`

---

<a id="item-20"></a>
## [Babylon Foundation Deposits 3M USDT into Aave V3 and V4](https://wublockchain.xyz/news/news-18884) ⭐️ 4.0/10

Babylon Foundation announced it will deposit 3 million USDT into Aave, with 2 million USDT allocated to V3 and 1 million USDT to V4. Any interest earned will be returned to the Aave ecosystem through Aave x Babylon integration incentives. While the amount is relatively small compared to Aave's $23.8 billion total value locked, this deposit demonstrates institutional confidence in Aave's dominant DeFi lending protocol and signals support for ecosystem recovery and future adoption. The deposit is split evenly between Aave V3 and V4, with V4 recently launching on Ethereum mainnet with a Hub-and-Spoke architecture that separates lending markets while sharing liquidity. Babylon plans to redirect all earned interest back to the ecosystem through integration incentives.

telegram · wublockchainenglish · Apr 27, 01:33

**Background**: Aave is a leading decentralized finance lending protocol that dominates the DeFi lending space with approximately 60%-67% market share. The protocol allows users to earn interest on deposits and borrow assets, with USDT being one of the most widely used stablecoins in DeFi. USDT (Tether) is a fiat-backed stablecoin pegged 1:1 to the US dollar.

<details><summary>References</summary>
<ul>
<li><a href="https://www.btcc.com/en-US/academy/research-analysis/what-is-babylon-baby-everything-you-need-to-know">What is Babylon (BABY)? Everything You Need To Know - BTCC</a></li>
<li><a href="https://coinpedia.org/news/aave-v4-goes-live-on-ethereum-mainnet-with-new-lending-architecture/">Aave V4 Goes Live on Ethereum Mainnet - Coinpedia</a></li>
<li><a href="https://www.oobit.com/stablecoin/usdt">USDT Explained | A Simple Guide to the #1 Stablecoin - Oobit</a></li>

</ul>
</details>

**Tags**: `#DeFi`, `#Aave`, `#Crypto Investment`, `#USD Stablecoin`, `#Blockchain Ecosystem`

---

