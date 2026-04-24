# Horizon Daily - 2026-04-24

> From 44 items, 4 important content pieces were selected

---

1. [DeepSeek v4 Pro Released with 1.6T Parameters](#item-1) ⭐️ 8.0/10
2. [White House Memo Accuses China of AI Model Theft](#item-2) ⭐️ 6.0/10
3. [US Soldier Charged with Insider Trading on Polymarket Using Classified Intel](#item-3) ⭐️ 6.0/10
4. [Saildrone Spectre Enters Navy's Medium-Sized USV Competition](#item-4) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [DeepSeek v4 Pro Released with 1.6T Parameters](https://api-docs.deepseek.com/) ⭐️ 8.0/10

DeepSeek released its v4 Pro model with 1.6 trillion parameters on HuggingFace, featuring competitive API pricing at $1.74 per million input tokens and $3.48 per million output tokens on OpenRouter. The model is already available with both base and Pro versions accessible to developers. This release raises questions about AI model economics, as community members debate whether such a large model can be profitable at these price points. The pricing challenges assumptions about inference costs for massive models and could pressure competitors to lower their prices. The model architecture appears to use Mixture of Experts (MoE), a technique that allows activating only subset of parameters for each inference, enabling efficient handling of the 1.6T parameter model. The Pro version on OpenRouter offers superior performance compared to the Flash version ($0.14/$0.28 per million tokens).

hackernews · impact_sy · Apr 24, 03:01

**Background**: DeepSeek is a Chinese AI company based in Hangzhou, Zhejiang, owned and funded by High-Flyer, a Chinese hedge fund. The company gained significant attention earlier in 2025 when it released models rivaling US tech giants but built at a fraction of the cost. Mixture of Experts (MoE) architecture divides a model into multiple specialized expert networks, with a gating mechanism selecting the appropriate expert for each input, dramatically reducing computational requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/mixture-of-experts">What is mixture of experts? | IBM</a></li>
<li><a href="https://www.gmicloud.ai/blog/comparing-gpu-pricing-large-language-models">Compare GPU Cloud Pricing for LLM Inference Workloads</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed but largely positive. Users debate whether the $4 per million output tokens pricing is profitable for such a large model, with some arguing that subscription models alone would be profitable. There is appreciation for the developer documentation being released before any press release, and cautious optimism about truly open source models coming from China. Some users remain skeptical about potential ulterior motives.

**Tags**: `#deepseek`, `#ai-models`, `#llm`, `#pricing`, `#open-source`

---

<a id="item-2"></a>
## [White House Memo Accuses China of AI Model Theft](https://www.bbc.com/news/articles/cpqxgxx9nrqo?at_medium=RSS&at_campaign=rss) ⭐️ 6.0/10

A memo from Michael Kratsios, a former White House official, alleges that companies, primarily based in China, are wrongfully extracting and copying US AI models through a process called model distillation. This accusation highlights escalating tensions between the US and China in the AI sector, and could trigger new export controls or policy measures targeting Chinese tech firms. If proven, it could fundamentally reshape international AI partnerships and technology transfer agreements. The memo specifically targets "distillation" as the method used to extract knowledge from US AI models. Model distillation is a legitimate technique that transfers knowledge from large models to smaller, more efficient ones, but the memo claims it is being weaponized to replicate proprietary US AI technology without authorization.

rss · BBC World · Apr 24, 00:58

**Background**: Model distillation, also known as knowledge distillation, is a machine learning technique where a large, complex model transfers its learned patterns to a smaller model. While this process is widely used legitimately to create efficient AI systems, security researchers have documented 'model extraction attacks' where adversaries systematically query AI APIs to replicate a model's behavior. The US has already implemented various semiconductor export restrictions to China, and this memo suggests extending scrutiny to AI model intellectual property.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://www.praetorian.com/blog/stealing-ai-models-through-the-api-a-practical-model-extraction-attack/">Stealing AI Models Through the API: A Practical Model Extraction Attack | Praetorian</a></li>

</ul>
</details>

**Tags**: `#AI_policy`, `#geopolitics`, `#China_US_relations`, `#IP_theft`, `#tech_competition`

---

<a id="item-3"></a>
## [US Soldier Charged with Insider Trading on Polymarket Using Classified Intel](https://www.aljazeera.com/economy/2026/4/23/us-soldier-charged-with-using-polymarket-to-bet-on-nicolas-maduro-abduction?traffic_source=rss) ⭐️ 6.0/10

Gannon Ken Van Dyke, a 38-year-old US Army master sergeant, has been charged with using Polymarket, a cryptocurrency-based prediction market platform, to allegedly profit $400,000 by betting on the capture of Venezuelan President Nicolás Maduro based on classified military intelligence. This marks the first US arrest for insider trading involving a prediction market. This case sets a precedent as the first prosecution of insider trading on a prediction market platform, exposing the unique vulnerabilities of these decentralized betting systems to exploitation by those with access to classified information. It raises critical questions about regulatory oversight for crypto-based prediction markets and their susceptibility to manipulation by bad actors in positions of trust. The DOJ is prosecuting the case under securities or commodities fraud statutes, though insider trading charges specifically apply only to securities. Polymarket operates using theCelo blockchain and USDC stablecoin, functioning in a regulatory gray area. The Venezuelan operation allegedly targeted Maduro but did not result in his capture, yet the soldier allegedly traded based on classified information about the planned operation.

rss · Al Jazeera · Apr 23, 23:04

**Background**: Prediction markets are open markets where participants trade contracts based on the likelihood of future events, using financial incentives to aggregate information. Polymarket claims to be the world's largest prediction market, enabling traders to profit from their knowledge of real-world outcomes across political, economic, and military events. In the US, insider trading laws prohibit trading based on material non-public information, and these regulations apply to securities and potentially commodities trading.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Polymarket">Polymarket - Wikipedia</a></li>
<li><a href="https://polymarket.com/">Polymarket | The World's Largest Prediction Market™</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prediction_market">Prediction market - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#prediction-markets`, `#polymarket`, `#insider-trading`, `#crypto`, `#crime`

---

<a id="item-4"></a>
## [Saildrone Spectre Enters Navy's Medium-Sized USV Competition](https://www.twz.com/sea/saildrones-missile-toting-spectre-enters-navys-medium-sized-unmanned-ship-competition) ⭐️ 6.0/10

Saildrone has partnered with defense companies to develop a larger missile-armed variant called Spectre for the Navy's medium-sized unmanned surface vessel (MUSV) program. The 52-meter Spectre combines anti-submarine warfare sensors with vertical launch strike capabilities, aiming to close critical gaps in both areas. This entry positions Spectre to address critical gaps in anti-submarine warfare and distributed maritime strike operations. As the Navy seeks to sustain presence in contested waters without relying on scarce crewed ships, unmanned vessels like Spectre could become essential force multipliers for the Golden Fleet initiative. The Spectre can reach speeds up to 27 knots (50 km/h) using twin 5,000-horsepower Caterpillar diesel engines for higher-speed operations. The Navy recently cancelled the Modular Attack Surface Craft (MASC) program and is creating a new acquisition strategy for unmanned vessels, opening additional opportunities for competitors like Saildrone.

rss · The Drive Warzone · Apr 23, 23:18

**Background**: Medium Unmanned Surface Vessels (MUSVs) are autonomous surface ships operated by the U.S. Navy as part of its broader unmanned systems strategy. Sea Hunter and Seahawk are the first MUSVs in Navy service, both developed under the Overlord program. The Navy's Golden Fleet initiative aims to deliver several production-ready, multi-role unmanned ships capable of working with the containerized capability campaign plan. Saildrone has previously demonstrated its autonomous surface vessel technology through hurricane tracking missions with NOAA.

<details><summary>References</summary>
<ul>
<li><a href="https://www.navy.mil/Resources/Fact-Files/Display-FactFiles/Article/4288073/medium-unmanned-surface-vessel-musv/">Medium Unmanned Surface Vessel (MUSV) - United States Navy</a></li>
<li><a href="https://www.navalnews.com/naval-news/2026/03/u-s-navy-unveils-unmanned-centerpiece-of-golden-fleet-initiative/">U.S. Navy Unveils Unmanned Centerpiece of Golden Fleet ...</a></li>
<li><a href="https://nextgendefense.com/saildrone-usv-anti-submarine/">30 Knots at Sea: Saildrone Reveals New USV Built for Anti-Submarine...</a></li>
<li><a href="https://www.armyrecognition.com/news/navy-news/2026/u-s-unveils-saildrone-spectre-unmanned-vessel-for-anti-submarine-warfare-and-vertical-launch-strike">U.S. Unveils Saildrone Spectre Unmanned Vessel for Anti Submarine ...</a></li>

</ul>
</details>

**Tags**: `#unmanned-systems`, `#naval-technology`, `#defense-industry`, `#autonomous-weapons`, `#military-procurement`

---

