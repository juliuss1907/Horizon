# Horizon Daily - 2026-05-08

> From 128 items, 10 important content pieces were selected

---

1. [Meshtastic Introduction Sparks Interest in Off-Grid Mesh Communication](#item-1) ⭐️ 6.0/10
2. [ClojureScript Gains Native Async/Await Support](#item-2) ⭐️ 6.0/10
3. [GeoJSON Practical Limitations Revealed in Developer Discussion](#item-3) ⭐️ 5.0/10
4. [Microsoft Discontinues Gaming Copilot on Xbox and Mobile](#item-4) ⭐️ 5.0/10
5. [Nintendo Switch 2 Price Increase to $499.99 in U.S.](#item-5) ⭐️ 5.0/10
6. [The Eye in Your Pocket: Digital Devices as Surveillance Tools](#item-6) ⭐️ 5.0/10
7. [Experts Propose Transforming Parking into Green Spaces](#item-7) ⭐️ 4.0/10
8. [ReelShort CEO Joey Jia to Speak at Vertical Media Summit](#item-8) ⭐️ 4.0/10
9. [AMC Global Media Q1 2026: Streaming Revenue Rises Despite Subscriber Dip](#item-9) ⭐️ 4.0/10
10. [Gawker's Collapse: Former Staff Reflect a Decade Later](#item-10) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Meshtastic Introduction Sparks Interest in Off-Grid Mesh Communication](https://meshtastic.org/docs/introduction/) ⭐️ 6.0/10

A Hacker News post introducing Meshtastic, a LoRa-based mesh networking protocol, has attracted significant community engagement with 101 points and 37 comments. The project enables encrypted peer-to-peer text messaging over ISM radio bands without requiring amateur radio licenses. The discussion highlights growing interest in decentralized, censorship-resistant communication as internet infrastructure becomes increasingly centralized. Meshtastic provides a practical solution for emergency communication and off-grid connectivity, with community members noting its potential value in regions facing internet restrictions like Russia. Meshtastic operates on license-free ISM (Industrial, Scientific, Medical) radio bands, which limits transmit power but notably does not prohibit encryption—the inverse of most amateur radio regulations. Users report that coverage varies significantly by location, with cities like the poster's area having thriving communities. Some community members note a perceived shift from Meshtastic toward Meshcore.io in recent months.

hackernews · ColinWright · May 8, 11:22

**Background**: Meshtastic is a decentralized wireless mesh networking protocol built on LoRa (Long Range) technology, which is a spread spectrum modulation technique derived from chirp spread spectrum (CSS). LoRa enables long-range communication with low power consumption, making it ideal for off-grid applications where small amounts of data need to be transmitted. Unlike amateur radio, which requires licenses and prohibits encryption on certain frequencies, ISM bands allow unlicensed operation but have power restrictions. The project runs on inexpensive hardware and has attracted users who compare its community-driven, experimental nature to the early internet.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LoRa">LoRa - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Meshtastic">Meshtastic - Wikipedia</a></li>
<li><a href="https://www.thethingsnetwork.org/docs/lorawan/what-is-lorawan/">What are LoRa and LoRaWAN? | The Things Network</a></li>

</ul>
</details>

**Discussion**: The community response is overwhelmingly positive, with long-term users sharing multi-year experiences running nodes and noting that Meshtastic encouraged them to obtain HAM licenses. Multiple commenters draw parallels to the early internet's ethos of select communities and high signal-to-noise ratio, with one stating 'nobody trying to monetize your attention.' There's also discussion of related projects like Meshcore and Reticulum, with some suggesting Meshcore may be gaining traction. One commenter highlights the technology's importance for regions with limited internet access like Russia.

**Tags**: `#mesh-networking`, `#lora-radio`, `#peer-to-peer`, `#decentralized-communication`, `#amateur-radio`

---

<a id="item-2"></a>
## [ClojureScript Gains Native Async/Await Support](https://clojurescript.org/news/2026-05-07-release) ⭐️ 6.0/10

ClojureScript 1.12.145 officially shipped with native async/await support on May 7, 2026. The new ^:async function hint generates JavaScript async functions directly, eliminating the need for additional dependencies when working with modern Browser APIs and libraries. This enhancement significantly improves ClojureScript's JavaScript interoperability, addressing the #1 requested feature from community surveys for years. It closes a major gap that made interacting with Promise-heavy JavaScript ecosystems cumbersome, potentially making ClojureScript more accessible to developers working on front-end projects. ClojureScript implements async/await through the ^:async function hint rather than dedicated keywords, staying true to Lisp's expression-based syntax. Notably, ClojureScript already had core.async (CSP-style concurrency) long before JavaScript received async/await in ES2017, demonstrating how libraries can add features unavailable in the host language.

hackernews · Borkdude · May 8, 07:04

**Background**: ClojureScript is a dialect of the Lisp programming language that compiles to JavaScript, enabling developers to write browser-based applications using Clojure syntax and idioms. Unlike Clojure running on the JVM, ClojureScript targets JavaScript runtimes and emphasizes interoperability with existing JS code. JavaScript introduced native async/await support in ES2017 (ECMAScript 2017), approximately a decade ago, revolutionizing asynchronous programming in that ecosystem. ClojureScript's core.async library previously offered an alternative CSP-style approach to asynchronous programming inspired by Go's concurrency model.

<details><summary>References</summary>
<ul>
<li><a href="https://clojurescript.org/news/2026-05-07-release">ClojureScript - 1.12.145 Release</a></li>
<li><a href="https://byteiota.com/clojurescript-async-await-bridging-fp-and-javascript-2026/">ClojureScript Async/Await: Bridging FP and JavaScript (2026)</a></li>

</ul>
</details>

**Discussion**: The community response is mixed, with celebration alongside concerns about adoption. Commenters note the irony that ClojureScript had CSP-style async via core.async before JavaScript got async/await, but also raise concerns about front-end adoption challenges—some wishing alternatives to JavaScript would catch on while questioning whether ClojureScript is practical for anything beyond personal projects. There is speculation about whether recent attention is due to agentic coding workflows.

**Tags**: `#ClojureScript`, `#Async/Await`, `#Functional Programming`, `#JavaScript Interop`, `#Lisp`

---

<a id="item-3"></a>
## [GeoJSON Practical Limitations Revealed in Developer Discussion](https://geojson.org/) ⭐️ 5.0/10

A Hacker News discussion revealed practical limitations of GeoJSON format, including polygon simplification problems with shared boundaries causing "slivers," CRS handling risks when tools assume world coordinate systems, and lack of z+m coordinate support. The community discussed alternatives like the SQLite-based GeoPackage format. These limitations impact GIS practitioners and developers using GeoJSON in production environments for mapping, logistics, and spatial analysis. Understanding these trade-offs helps teams make informed decisions when choosing geospatial data formats for their applications. When simplifying adjacent polygons (e.g., US state boundaries), GeoJSON treats each polygon separately rather than encoding shared boundary points, leading to misalignment artifacts. Additionally, the format assumes WGS84 lon/lat coordinates, and many tools will malfunction if users apply flatland CRS projections. GeoPackage offers binary storage advantages with more flexible geometry support.

hackernews · tosh · May 8, 09:55

**Background**: GeoJSON (RFC 7946) is a JSON-based open standard for encoding geographic features and their attributes, widely adopted due to its human-readable format and JavaScript ecosystem compatibility. However, it lacks native support for topology (shared boundaries), forces a single CRS per file, and has limited 3D coordinate support. GeoPackage, defined by the Open Geospatial Consortium in 2014, uses SQLite as a container to store vector features, rasters, and tile pyramids in a serverless, platform-independent format.

<details><summary>References</summary>
<ul>
<li><a href="https://geojson.org/">GeoJSON</a></li>
<li><a href="https://en.wikipedia.org/wiki/GeoPackage">GeoPackage - Wikipedia</a></li>
<li><a href="https://www.geopackage.org/">OGC GeoPackage</a></li>

</ul>
</details>

**Discussion**: Community members shared practical production experiences. DarkNova6 recommended GeoPackage as "the best format in geospatial data analysis" despite its binary nature requiring extra testing steps. Stratoscope highlighted the polygon simplification problem specifically for the 48 contiguous US states. Waterluvian warned about CRS assumptions causing calculation errors in warehouse robot monitoring systems. Nobleach mentioned TopoJSON as a workaround that adds arcs to reduce shared boundary points.

**Tags**: `#geojson`, `#gis`, `#spatial-data`, `#json`, `#coordinate-systems`

---

<a id="item-4"></a>
## [Microsoft Discontinues Gaming Copilot on Xbox and Mobile](https://variety.com/2026/gaming/news/gaming-news-roundup-may-4-1236738760/) ⭐️ 5.0/10

Microsoft's new Xbox CEO Asha Sharma announced the company is stopping development of Copilot on Xbox consoles and winding down the AI service for mobile gaming. Gaming Copilot, which was still in beta testing, will have its features retired as they don't align with the company's future plans. This marks a significant strategic pivot for Microsoft's gaming division under its new leadership. The discontinuation signals a potential reallocation of resources away from AI辅助 gaming features toward other Xbox priorities, which could reshape the company's approach to integrating AI in its gaming ecosystem. Gaming Copilot was designed as a personal gaming sidekick offering in-game assistance, gameplay recommendations, and help with play history. The feature had been available through Xbox Game Bar and the Xbox app beta. The announcement was made via Sharma's post on X (formerly Twitter), and leadership changes accompanied this decision.

rss · Variety · May 8, 12:22

**Background**: Microsoft introduced Gaming Copilot as an AI-powered feature designed to help players with personalized game recommendations, seamless game setup, and in-game tips. Unlike standard Microsoft Copilot, Gaming Copilot was optimized specifically for gaming scenarios. The feature represented Microsoft's broader attempt to integrate AI capabilities into its Xbox gaming ecosystem across both console and mobile platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/video-games/xbox/xbox-ceo-asha-sharma-kills-copilot-for-gaming">Xbox CEO Asha Sharma kills Copilot for Gaming — overhauls ...</a></li>
<li><a href="https://www.geekwire.com/2026/microsofts-new-xbox-chief-nixes-gaming-copilot-for-mobile-and-console-shakes-up-leadership/">Microsoft’s new Xbox chief nixes Gaming Copilot for mobile ...</a></li>
<li><a href="https://www.xbox.com/en-US/gaming-copilot">Gaming Copilot (Beta): Your personal gaming sidekick | Xbox</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#Xbox`, `#Gaming Copilot`, `#AI Assistants`, `#Product Discontinuation`

---

<a id="item-5"></a>
## [Nintendo Switch 2 Price Increase to $499.99 in U.S.](https://variety.com/2026/gaming/news/nintendo-switch-2-price-increase-20-million-sold-1236741441/) ⭐️ 5.0/10

Nintendo is raising the Switch 2 price from $449.99 to $499.99 starting September 1, citing increased memory and storage costs. The console, which launched in June 2025, is approaching 20 million units sold since its release. This $50 price increase marks the first major pricing adjustment for the Switch 2 and could affect consumer purchasing decisions in a competitive gaming market against devices like the Steam Deck. It may also signal broader hardware cost pressures affecting the gaming industry. The price adjustment brings the U.S. price closer to parity with Japanese pricing when converted, suggesting Nintendo is adjusting for currency fluctuations. The timing coincides with Switch 2 approaching 20 million units sold since its June 2025 launch.

rss · Variety · May 8, 11:34

**Background**: Nintendo's previous console, the original Switch, launched at $299.99 in 2017 and became one of the best-selling gaming consoles of all time. Gaming console pricing typically remains stable throughout a generation, making this adjustment notable. The yen has weakened significantly against the dollar since 2022, pressuring Japanese companies to adjust pricing to maintain profitability.

**Discussion**: Community reactions are mixed: some users criticize Nintendo's pricing as overpriced and question the timing, noting they have switched to alternatives like the Steam Deck. Others point out that yen weakness since 2022 and the dollar's global value changes since April 2025 have pressured Nintendo to adjust pricing to equalize costs. One user notes the Switch 2's hardware bill of materials is actually more costly relative to its predecessor, making this price increase somewhat justified despite poor timing.

**Tags**: `#gaming`, `#nintendo`, `#hardware`, `#pricing`, `#industry-news`

---

<a id="item-6"></a>
## [The Eye in Your Pocket: Digital Devices as Surveillance Tools](https://aeon.co/essays/things-have-jobs-and-digital-devices-are-made-to-track-you) ⭐️ 5.0/10

隐私伦理学家卡丽莎·维利兹在Aeon杂志上发表文章，指出数字设备的核心设计目的是追踪用户，与枕头用于舒适、剪刀用于剪切等日常物品的固有功能形成类比。 随着智能手机和物联网设备无处不在，理解它们作为监控工具而非中立技术的本质，对于知情同意、政策监管和个人隐私保护至关重要。 这篇文章的核心论点是将数字设备的追踪功能视为其根本属性，如同其他物品的固有用途一样，而非可选功能或偶然副作用。

rss · Aeon · May 8, 10:00

**Background**: Carissa Véliz是牛津大学的隐私伦理学者，著有《隐私即保护》一书并专注于数字时代的隐私问题。物联网设备通过传感器和网络连接持续收集用户数据，从位置追踪到睡眠模式无所不包。数字追踪是当前技术伦理讨论的核心议题，涉及数据收集、知情同意和监控资本主义等概念。

**Tags**: `#privacy`, `#digital surveillance`, `#technology ethics`, `#internet of things`, `#data tracking`

---

<a id="item-7"></a>
## [Experts Propose Transforming Parking into Green Spaces](https://www.theguardian.com/environment/2026/may/08/cities-cars-experts-green-spaces-cyclists) ⭐️ 4.0/10

Urban planning experts recommend converting parking bays into green spaces and prioritizing cycling infrastructure as the fastest routes to improving city life, citing benefits including cleaner air, safer streets, and climate stability. Reducing car dependency addresses public health, urban livability, and climate goals simultaneously, though cities like those in the US have become so car-dependent that opting out is nearly impossible for most residents. The article notes that while some cities with world-class public transport are debating how to tackle the stubborn minority of journeys still made by car, others have infrastructure that makes car-free living practically impossible.

rss · The Guardian Life · May 8, 10:00

**Background**: Car dependency is a pattern in urban planning where infrastructure favors automobiles over other transport modes like public transit, bicycles, and walking. This dependency places significant financial burdens on individuals living in car-dependent areas. Meanwhile, urban green infrastructure—comprising parks, green roofs, urban forests, wetlands, and green corridors integrated within city fabric—can provide ecological benefits while supporting biodiversity and urban communities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wikiwand.com/en/articles/Automobile_dependency">Car dependency - Wikiwand</a></li>
<li><a href="https://www.epa.gov/green-infrastructure/community-planning-and-green-infrastructure">Community Planning and Green Infrastructure - US EPA</a></li>

</ul>
</details>

**Tags**: `#urban-planning`, `#sustainability`, `#environment`, `#public-transport`, `#cities`

---

<a id="item-8"></a>
## [ReelShort CEO Joey Jia to Speak at Vertical Media Summit](https://variety.com/2026/biz/news/reelshort-joey-jia-vertical-media-summit-owl-co-1236740243/) ⭐️ 4.0/10

Joey Jia, founder and CEO of ReelShort, is scheduled to speak at Owl & Co.'s Vertical Media Summit in Hollywood on June 3, in conversation with Hernan Lopez, the former Fox executive and company chief. The summit brings together key players in the rapidly growing vertical video space, where ReelShort has emerged as a major competitor to platforms like TikTok in the microdrama segment. Jia's appearance signals continued industry interest in short-form mobile content. The event will be held at Owl & Co.'s venue in Hollywood, with Hernan Lopez—founder of a media company whose name was cut off in the source—as the interviewer. ReelShort is recognized by Times100 for movie reels innovation.

rss · Variety · May 8, 13:15

**Background**: ReelShort is a Chinese short-form video streaming app specializing in microdramas, owned by Crazy Maple Studio and backed by COL Group. The platform offers vertical TV mini series with one-minute episodes designed for mobile viewing, featuring rapid plot twists and heightened emotional conflicts. The vertical video format uses a 9:16 aspect ratio optimized for smartphone screens, distinguishing it from traditional horizontal video content.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ReelShort">ReelShort - Wikipedia</a></li>
<li><a href="https://www.backstage.com/magazine/article/vertical-video-explained-78419/">Vertical Video Explained: What You Need to Know About the ...</a></li>

</ul>
</details>

**Tags**: `#vertical-video`, `#streaming`, `#media-industry`, `#ReelShort`, `#industry-events`

---

<a id="item-9"></a>
## [AMC Global Media Q1 2026: Streaming Revenue Rises Despite Subscriber Dip](https://variety.com/2026/tv/news/amc-global-media-earnings-4-million-charge-streaming-sales-1236741415/) ⭐️ 4.0/10

AMC Global Media (formerly AMC Networks) reported Q1 2026 earnings showing streaming revenue growth despite a 1% year-over-year decline in paid subscribers to 10.1 million. The company also recorded a $4 million restructuring charge and reported that ad-supported AMC+ hard-bundle agreements surged 200% year-over-year to 1.8 million. This earnings report highlights a critical shift in streaming economics, where bundled partnerships and ad-supported tiers are becoming primary growth engines even as traditional subscriber counts stagnate. The 200% surge in hard-bundle agreements suggests telecom and cable partnerships are increasingly central to AMC's strategy amid intensifying competition in the streaming market. The 1.8 million hard-bundle agreements are counted separately from AMC's 10.1 million streaming subscriber total, meaning they represent distinct distribution channels rather than overlapping users. AMC recently completed a rebranding from AMC Networks to AMC Global Media, reflecting the company's broader strategic shift toward a diversified media operations model.

rss · Variety · May 8, 11:13

**Background**: A "hard bundle" refers to an arrangement where multiple streaming applications are integrated into a single interface and offered as a unified package, typically through partnerships with telecommunications or cable companies. This model has gained traction across the streaming industry as platforms seek to reduce customer acquisition costs and combat subscription fatigue among consumers. AMC+ specifically offers an ad-supported tier that can be distributed through these bundled agreements, allowing the company to monetize its content through multiple revenue streams including advertising.

<details><summary>References</summary>
<ul>
<li><a href="https://variety.com/2026/tv/news/amc-global-media-earnings-4-million-charge-streaming-sales-1236741415/">AMC Global Media Takes $4 Million Restructuring Charge in Q1, Streaming Revenue Rises</a></li>
<li><a href="https://www.filmtake.com/streaming/piecing-together-the-future-of-streaming-the-rise-of-bundling-and-aggregation/">Piecing Together the Future of Streaming: The Rise of Bundling and Aggregation – FilmTake</a></li>

</ul>
</details>

**Tags**: `#streaming`, `#media-industry`, `#earnings`, `#subscription-services`, `#entertainment`

---

<a id="item-10"></a>
## [Gawker's Collapse: Former Staff Reflect a Decade Later](https://www.hollywoodreporter.com/business/digital/inside-gawker-legacy-1236585677/) ⭐️ 4.0/10

The Hollywood Reporter published a retrospective examining Gawker Media's downfall ten years after Peter Thiel secretly funded Hulk Hogan's lawsuit against the media company, leading to a $140 million verdict in March 2016 that forced Gawker's closure and sale. Former staff members share how the site's demise continues to affect their careers and mental health. The Gawker case became a landmark example of how billionaire-funded litigation can be weaponized against media organizations, fundamentally changing how journalists approach controversial content and source protection. Its aftermath raises ongoing questions about press freedom, legal strategy, and the power dynamics between tech wealth and traditional media. Peter Thiel confirmed spending millions to finance Hulk Hogan's case, using what became known as 'litigation as a business strategy.' The approach was groundbreaking because Thiel's funding remained secret during the trial, only revealed afterward when Gawker was already facing financial collapse from the verdict.

rss · The Hollywood Reporter · May 8, 13:00

**Background**: Gawker Media was founded by British journalist Nick Denton in October 2003 and grew into a network of blogs known for aggressive, often provocative coverage of media, tech, and celebrity scandals. The site gained notoriety for its 'weaponized wit' and willingness to publish stories other outlets avoided. The 2012 Hulk Hogan sex tape story became the trigger for Thiel's legal campaign, though critics argued the broader motive was retaliation for Gawker's previous coverage of Thiel's private life. The case established a precedent where wealthy individuals could effectively shut down media companies through strategic litigation financing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hollywoodreporter.com/business/digital/inside-gawker-legacy-1236585677/">Inside Gawker's Legacy: Stories, Scandals, and Lasting Impact</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bollea_v._Gawker">Bollea v. Gawker - Wikipedia</a></li>
<li><a href="https://www.forbes.com/sites/mattdrange/2016/06/21/peter-thiels-war-on-gawker-a-timeline/">Peter Thiel 's War On Gawker : A Timeline</a></li>

</ul>
</details>

**Discussion**: The retrospective prompted discussions about the chilling effect on journalism, with commentators noting that many former Gawker writers have since moved to more cautious positions at mainstream outlets. Some argue the site was genuinely problematic and deserved scrutiny, while others see its destruction as a dangerous precedent for press freedom. The case continues to be cited in debates about billionaire influence over media.

**Tags**: `#media industry`, `#journalism`, `#business history`, `#legal battles`, `#tech culture`

---

