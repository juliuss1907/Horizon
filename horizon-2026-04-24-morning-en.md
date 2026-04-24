# Horizon Daily - 2026-04-24

> From 79 items, 7 important content pieces were selected

---

1. [First Ransomware Confirmed Using Post-Quantum Cryptography](#item-1) ⭐️ 8.0/10
2. [OpenAI releases GPT-5.5, bringing company one step closer to an AI ‘super app’](#item-2) ⭐️ 7.0/10
3. [Researchers Decode Fast16, 2005 Malware Predating Stuxnet](#item-3) ⭐️ 7.0/10
4. [DL Research RWAfi Q1 2026: $25.2B Market with 5x Growth](#item-4) ⭐️ 7.0/10
5. [U.S. Soldier Charged with Insider Trading via Prediction Markets](#item-5) ⭐️ 6.0/10
6. [Rednote Separates Chinese and International Users](#item-6) ⭐️ 6.0/10
7. [Lido DAO Proposes 2,500 stETH for rsETH Relief](#item-7) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [First Ransomware Confirmed Using Post-Quantum Cryptography](https://arstechnica.com/security/2026/04/now-even-ransomware-is-using-post-quantum-cryptography/) ⭐️ 8.0/10

Security researchers have confirmed that a ransomware family has become the first to implement post-quantum cryptography (PQC) in its encryption scheme, marking an unprecedented development in cyber threat capabilities. This development signals that threat actors are proactively future-proofing their malware against quantum computing threats, even though quantum computers capable of breaking current encryption do not yet exist. Organizations should consider that ransomware attacks may soon become resistant to post-quantum decryption efforts by authorities. The ransomware uses PQC algorithms that are currently believed to be secure against quantum attacks, though there is no immediate practical advantage for attackers today. Analysts suggest the adoption may be driven by software compliance standards, future-proofing, or potential integration with nation-state sponsored threat groups that have access to advanced quantum capabilities.

rss · Ars Technica · Apr 23, 20:41

**Background**: Post-quantum cryptography refers to cryptographic algorithms designed to resist attacks from powerful quantum computers, which could theoretically break widely-used public-key encryption methods like RSA and elliptic curve cryptography. NIST released its first finalized post-quantum encryption standards in August 2024, recommending organizations begin transitioning to these new standards. The paradox of ransomware adopting PQC is that while it offers no benefit against current security measures, it demonstrates threat actors are closely monitoring and adapting to emerging cryptographic technologies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography - Wikipedia</a></li>
<li><a href="https://www.nist.gov/news-events/news/2024/08/nist-releases-first-3-finalized-post-quantum-encryption-standards">NIST Releases First 3 Finalized Post-Quantum Encryption ...</a></li>

</ul>
</details>

**Discussion**: Security community members have expressed both concern and skepticism about the development. While some view it as clear evidence that ransomware operators are investing in long-term capability development, others question whether the implementation was intentional or merely the result of an upstream software library update. The general consensus is that this represents a notable evolution in the sophistication of cybercriminal operations.

**Tags**: `#post-quantum cryptography`, `#ransomware`, `#cybersecurity`, `#threat intelligence`, `#cryptography`

---

<a id="item-2"></a>
## [OpenAI releases GPT-5.5, bringing company one step closer to an AI ‘super app’](https://techcrunch.com/2026/04/23/openai-chatgpt-gpt-5-5-ai-model-superapp/) ⭐️ 7.0/10

OpenAI announces GPT-5.5, a new model with broad capability improvements positioning the company toward an AI 'super app' vision.

rss · TechCrunch AI · Apr 23, 18:29

**Tags**: `#AI`, `#OpenAI`, `#LLM`, `#GPT`, `#Product Announcement`

---

<a id="item-3"></a>
## [Researchers Decode Fast16, 2005 Malware Predating Stuxnet](https://www.wired.com/story/fast16-malware-stuxnet-precursor-iran-nuclear-attack/) ⭐️ 7.0/10

Researchers have finally reverse-engineered Fast16, a mysterious sabotage malware created in 2005 that was capable of silently tampering with calculation and simulation software. The malware, likely deployed by the US or an ally, appears to have targeted Iran's nuclear program before the infamous Stuxnet worm became public. This discovery reveals that sophisticated sabotage tools targeting nuclear programs existed years before Stuxnet, providing new insights into the evolution of nation-state cyber operations. It also raises concerns about the long-term use of covert malware campaigns in geopolitical conflicts. Fast16 was specifically designed to silently corrupt scientific calculations and simulations, potentially causing nuclear research facilities to produce flawed results without detection. The malware remained undeciphered for nearly two decades until recent reverse-engineering efforts finally cracked its code.

rss · Wired · Apr 23, 22:00

**Background**: Stuxnet, discovered in 2010, was the first publicly known cyberweapon designed to physically destroy infrastructure by targeting Iran's uranium enrichment centrifuges. Unlike Stuxnet's direct physical sabotage, Fast16 represents a different approach—silently corrupting computational results. Both malware instances reflect long-standing cyber operations targeting Iran's nuclear program and demonstrate the evolution of state-sponsored hacking capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wired.com/story/fast16-malware-stuxnet-precursor-iran-nuclear-attack/">Newly Deciphered Sabotage Malware May Have Targeted... | WIRED</a></li>

</ul>
</details>

**Tags**: `#malware`, `#cyberwarfare`, `#nation-state-hacking`, `#stuxnet`, `#reverse-engineering`

---

<a id="item-4"></a>
## [DL Research RWAfi Q1 2026: $25.2B Market with 5x Growth](https://x.com/dl_research/status/2047364085503901866?s=20) ⭐️ 7.0/10

DL Research released its Q1 2026 RWAfi market report showing the tokenized real-world assets market grew 5x year-over-year to $25.2B market cap, with tokenized funds ($13.5B), gold ($5.9B), private credit ($4.6B), and stocks ($1.2B) accounting for 95%+ of the market, while only ~$2.8B is actually deployed in DeFi. This report highlights a critical phase transition in the RWAfi ecosystem: while issuance has exploded, actual DeFi usage remains nascent at only 11% of total market cap. The distinction between issuance and usage phases signals that the next growth driver will be integrating tokenized assets into DeFi composability rather than simply creating more tokens. Gold leads in DeFi maturity through yield-bearing products like thGOLD and pmUSD, enabling collateralization, perps, and yield generation; private credit grew 93x from $49M to $4.57B led by Maple Finance's SyrupUSDC integration with Spark and Morpho; stocks consolidated around custody-backed models (Ondo, xStocks) with native issuance (Galaxy's GLXY) emerging; real estate and carbon credits remain non-composable.

telegram · ahboyashreads · Apr 23, 18:15

**Background**: RWAfi (Real World Assets Finance) represents the convergence of tokenized real-world assets and DeFi, enabling off-chain assets like gold, private credit, and stocks to be represented on-chain and used within decentralized financial applications. Theo launched thGOLD in January 2026 as a yield-bearing tokenized gold product based on FundBridge Capital's MG999 on-chain gold fund, which uses physical gold reserves as collateral for retail lending. Maple Finance's SyrupUSDC has become a flagship private credit product, integrating with major DeFi protocols like Spark and Morpho to provide institutional-quality yields on-chain. Unlike traditional stablecoins, yield-bearing tokens generate returns through strategies like cash-and-carry trades using gold futures.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tokenized_real-world_asset">Tokenized real-world asset - Wikipedia</a></li>
<li><a href="https://www.theblock.co/post/385152/theo-launches-yield-bearing-tokenized-gold-built-work-defi">Theo launches yield-bearing tokenized gold built to 'work in DeFi' | The Block</a></li>
<li><a href="https://messari.io/project/syrup">Maple Price, SYRUP to USD, Research, News & Fundraising | Messari</a></li>

</ul>
</details>

**Tags**: `#RWA tokenization`, `#Real World Assets`, `#DeFi`, `#market analysis`, `#private credit`

---

<a id="item-5"></a>
## [U.S. Soldier Charged with Insider Trading via Prediction Markets](https://www.justice.gov/usao-sdny/pr/us-soldier-charged-using-classified-information-profit-prediction-market-bets?bm-verify=AAQAAAAN_____y6To7sZYZ502biZwIHXlr-7zXZUqV4H0xLTfW__wDA3SjNLqifXRaQwsikyuz6IJknyuL8xfVYRkesxcDk5V10m-HoXl2K93f17rygBphL77WVFoQ_XvlmUo922IwM_DQ66137X6wWMtpdHslcEjpJG7KbBmUw9Su4kDENpDt_yv2spThQZehgv-X1Adk5U2VHfp41co2s_QJGjRj4y0KmL1mhSCyVaE7MC1LHG0mtP-xYmD0xBOQwn6PlHkPiP5Nt46h5ZIjLGXgCZDEVD42i7rIEM379DKLPUPX0PDNmOAwFSuTqcTDVnT_UUV8vxpHLRMb7rUxPxKUPcIB23iZTRJddWDDtPHMXadpwv67xr-f1sKDLZT9NgHCO4iuC2EthmAt0) ⭐️ 6.0/10

A U.S. Army Special Forces soldier has been charged by federal prosecutors in the Southern District of New York with using classified information from a government operation to place bets on Polymarket, generating over $400,000 in profit from approximately $33,000 in wagers. This case represents one of the first federal prosecutions involving insider trading on prediction markets, raising critical questions about the regulation of these platforms and the application of existing securities and commodities laws to a rapidly evolving financial landscape. The 5-count indictment includes charges of unlawful use of confidential government information, theft of nonpublic government information, commodities fraud, wire fraud, and engaging in monetary transactions with proceeds from specified unlawful activity. The soldier was directly involved in the operation about which he placed bets on Polymarket, according to the DOJ announcement.

hackernews · paulpauper · Apr 23, 22:37

**Background**: Prediction markets like Polymarket allow users to trade contracts on real-world event outcomes, functioning as information markets where participants speculate on results ranging from elections to geopolitical events. These platforms operate in a regulatory gray area, and federal prosecutors have indicated increasing scrutiny of insider trading activities on such markets. The Southern District of New York has specifically stated it is reviewing applicable laws for pursuing criminal charges involving prediction market insider trading.

<details><summary>References</summary>
<ul>
<li><a href="https://www.congress.gov/crs-product/LSB11406">Prediction Markets and Insider Trading Law - Congress.gov</a></li>
<li><a href="https://www.businessinsider.com/states-clamp-down-prediction-market-insider-trading-2026-4">States Are Clamping Down on Prediction Market Insider Trading ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong skepticism about selective enforcement, arguing that wealthy and politically connected individuals regularly engage in similar activities without consequences. One commenter questioned how many congressional members made identical bets on the same information legally, while another suggested this prosecution protects major prediction market investors. Several comments highlighted perceived double standards in the justice system, with one characterizing it as "nabbing the little guy for show."

**Tags**: `#prediction-markets`, `#classified-information`, `#legal`, `#insider-trading`, `#policy`

---

<a id="item-6"></a>
## [Rednote Separates Chinese and International Users](https://www.wired.com/story/rednote-draws-a-line-between-china-and-the-world/) ⭐️ 6.0/10

Rednote (Xiaohongshu) is implementing measures to separate Chinese users from its international audience as the platform experiences rapid growth abroad, following the influx of 'TikTok refugees' in early 2025. This separation reflects the fundamental tension Chinese platforms face between global expansion and compliance with domestic regulations on data localization and content governance. The move signals how geopolitics increasingly shapes platform architecture and user experience. The platform now appears to restrict international users from viewing content from Chinese users, creating a bifurcated experience. This architectural change comes as Rednote climbed to the top of Apple's U.S. App Store ranking in January 2025 during the TikTok ban crisis.

rss · Wired · Apr 23, 20:23

**Background**: Xiaohongshu (Rednote) is a Chinese social networking and e-commerce platform that allows users to share lifestyle content and product recommendations. During the TikTok ban uncertainty, millions of American users flocked to the platform, temporarily making it the top free app in the U.S. App Store. China maintains strict data localization laws that require certain user data to be stored domestically, complicating how Chinese platforms handle international user bases.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Xiaohongshu">Xiaohongshu - Wikipedia</a></li>
<li><a href="https://www.nytimes.com/2025/01/16/arts/tiktok-red-note-china.html">TikTok Refugees Get Wry Welcome on RedNote , Another Chinese...</a></li>
<li><a href="https://womeninlocalization.com/data-localization-laws-around-the-world/">Data Localization Laws Around the World - Women in Localization</a></li>

</ul>
</details>

**Tags**: `#social-media`, `#platform-governance`, `#china-tech`, `#international-expansion`, `#content-moderation`

---

<a id="item-7"></a>
## [Lido DAO Proposes 2,500 stETH for rsETH Relief](https://research.lido.fi/t/lido-dao-contribution-to-coordinated-rseth-relief-effort/11483) ⭐️ 6.0/10

Lido DAO proposes allocating up to 2,500 stETH as part of a coordinated multi-party relief effort to address the approximately 100,000+ ETH rsETH backing deficit caused by the KelpDAO exploit, which threatens EarnETH vault depositors with potential losses of up to ~9,000 ETH. This represents a significant governance action by the largest liquid staking protocol to address a major protocol-level security incident affecting the broader DeFi ecosystem. The conditional nature of the allocation—requiring full funding of the relief package—demonstrates responsible stewardship of DAO resources while addressing systemic risk from the $292 million KelpDAO hack. The contribution is contingent on the relief package achieving complete funding to close the entire deficit, is separate from the EGG 2026 budget, and will be routed through the Lido Labs Foundation multisig as a pass-through mechanism with unused funds returned to the DAO Agent. The forwarding transaction hash must be published within 48 hours of release.

telegram · ahboyashreads · Apr 23, 18:15

**Background**: KelpDAO suffered a $292 million exploit that caused the rsETH backing deficit, leading to Aave freezing rsETH markets and a wider liquidity crunch in DeFi. Lido Finance confirmed its EarnETH vault carries approximately 9% direct exposure to rsETH, though the core Lido staking system remains unaffected. Liquid staking protocols enable users to stake ETH while receiving liquid tokens that can be used in DeFi applications.

<details><summary>References</summary>
<ul>
<li><a href="https://research.lido.fi/t/lido-dao-contribution-to-coordinated-rseth-relief-effort/11483">Lido DAO contribution to coordinated rsETH relief... - Lido Governance</a></li>
<li><a href="https://coincentral.com/lido-finance-flags-9-rseth-exposure-as-kelpdao-exploit-fallout-spreads/">Lido Finance Flags 9% rsETH Exposure as KelpDAO Exploit ...</a></li>
<li><a href="https://www.coindesk.com/tech/2026/04/21/the-usd292-million-kelp-dao-exploit-shows-why-crypto-bridges-are-still-one-of-the-industry-s-weakest-links">The $292 million Kelp DAO exploit shows why crypto bridges are still one of the industry's weakest links</a></li>

</ul>
</details>

**Tags**: `#Lido DAO`, `#DeFi`, `#Governance`, `#rsETH`, `#Protocol Security`

---

