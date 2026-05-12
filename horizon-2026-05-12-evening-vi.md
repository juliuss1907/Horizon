# Horizon Daily - 2026-05-12

> From 128 items, 8 important content pieces were selected

---

1. [Rendering the Sky, Sunsets, and Planets](#item-1) ⭐️ 7.0/10
2. [Learning Software Architecture](#item-2) ⭐️ 6.0/10
3. [EU to crack down on TikTok, Instagram's 'addictive design' targeting kids](#item-3) ⭐️ 6.0/10
4. [Coursera and Udemy are now one company](#item-4) ⭐️ 6.0/10
5. [UnDUNE II](#item-5) ⭐️ 5.0/10
6. [Chasing Utopia review – renegade Google exec Mo Gawdat searches for ethical AI in alarming insider warning](#item-6) ⭐️ 5.0/10
7. [Một nhân viên tài chính đã ‘tự nguyện’ chuyển 25 triệu USD cho kẻ lừa đảo chỉ sau cuộc họp qua Zoom: Chuyên gia Hiếu PC cảnh báo hiểm họa trong kỷ nguyên AI](#item-7) ⭐️ 5.0/10
8. [Cannes Juror Paul Laverty Says ‘Shame on Hollywood’ for Blacklisting Susan Sarandon and More Actors Who Oppose War in Gaza: ‘They’re the Best of Us’](#item-8) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Rendering the Sky, Sunsets, and Planets](https://blog.maximeheckel.com/posts/on-rendering-the-sky-sunsets-and-planets/) ⭐️ 7.0/10

Maxime Heckel published a technical blog post exploring the physics and implementation of rendering realistic skies, sunsets, and planetary atmospheres, covering Rayleigh scattering, Mie scattering, and phase functions for atmospheric simulation. This post makes complex atmospheric physics accessible to WebGL and shader developers, providing practical implementation guidance for creating photorealistic skies. The high community engagement (92 points, 6 comments) indicates strong demand for quality educational content on real-time graphics rendering. The blog explains how Rayleigh scattering causes the blue sky color while Mie scattering is responsible for the red and orange hues during sunsets. It also covers phase functions that determine the probability distribution of light scattering in different directions, which is essential for accurate atmosphere rendering.

hackernews · ibobev · May 12, 13:26

**Background**: Atmospheric scattering occurs when particles in the atmosphere diffuse light in various directions. Rayleigh scattering describes light interaction with small particles (like air molecules), predominantly scattering shorter blue wavelengths, creating a blue sky. Mie scattering deals with larger particles (like dust and aerosols), scattering longer wavelengths and producing the characteristic orange and red colors at sunrise and sunset. Phase functions mathematically describe the angular distribution of scattered light, critical for realistic sky rendering in real-time graphics applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mie_scattering">Mie scattering - Wikipedia</a></li>
<li><a href="https://blog.maximeheckel.com/posts/on-rendering-the-sky-sunsets-and-planets/">On Rendering the Sky, Sunsets, and Planets - The Blog of Maxime Heckel</a></li>
<li><a href="https://cpp-rendering.io/sky-and-atmosphere-rendering/">Sky and Atmosphere rendering: A physical approach - CPP Rendering - Antoine MORRIER</a></li>

</ul>
</details>

**Discussion**: Community response is overwhelmingly positive and enthusiastic. Commenters reference related resources including Sebastian Lague's video on planet generation atmospheres and SpaceEngine as examples of impressive atmospheric rendering. One commenter notes the post was impressive even though they only understood about 5% of it, highlighting the educational value. Another comment brings up the Perez All-Weather and Preetham sky models as alternative approaches, suggesting interest in comparing different atmospheric simulation techniques.

**Tags**: `#graphics`, `#rendering`, `#atmospheric-simulation`, `#webgl`, `#shader-programming`

---

<a id="item-2"></a>
## [Learning Software Architecture](https://matklad.github.io/2026/05/12/software-architecture.html) ⭐️ 6.0/10

A comprehensive blog post titled "Learning Software Architecture" compiles essential software design principles, emphasizing minimizing surprise, isolating data transformations from data usage, and avoiding coupling. The article has garnered 319 upvotes and 63 substantive comments, indicating meaningful community engagement with the content. These principles provide practical guidance for developers making architectural decisions, helping teams build systems that are easier to maintain, understand, and evolve over time. The principles apply broadly across different programming paradigms and can serve as a foundation for both individual coding practices and team-level architectural reviews. A key insight from the community is the "articulation technique" proposed by user luodaint: explaining your system to an AI agent with no prior context forces you to make implicit constraints explicit. CSMasterMind distilled the principles into a cheat sheet format, while mpweiher noted that many recommendations apply to general software development rather than architecture specifically, recommending classic texts like Shaw and Garlan's "Software Architecture: Perspectives on an Emerging Discipline."

hackernews · surprisetalk · May 12, 09:30

**Background**: Software architecture principles guide how components are structured, communicate, and evolve within a system. The "minimize surprise" principle, related to the SOLID design philosophy, suggests that software behavior should align with user expectations and developer intuitions. Isolating data transformations is a common pattern in software architecture, where data models outlive the code that transforms them. Coupling reduction is a fundamental principle across software engineering, as tightly coupled systems become difficult to maintain and extend.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SOLID">SOLID - Wikipedia</a></li>
<li><a href="https://www.getdbt.com/blog/data-transformation">Data transformation: methods, workflows, and best practices | dbt Labs</a></li>

</ul>
</details>

**Discussion**: Community responses were overwhelmingly positive and added significant value. CSMasterMind's "cheat sheet" condensed the principles into memorable bullet points. Luodaint contributed a valuable technique: using AI agents to expose implicit system constraints through forced articulation. Woodydesign offered a philosophical comparison between Confucian learning-as-cultivation and Laozi's Taoist wisdom about "dropping" rather than always adding. Some readers, like mpweiher, provided constructive critique suggesting the principles overlap with general software development rather than architecture specifically, recommending complementary readings from Mary Shaw.

**Tags**: `#software-architecture`, `#software-design`, `#engineering-principles`, `#best-practices`, `#system-design`

---

<a id="item-3"></a>
## [EU to crack down on TikTok, Instagram's 'addictive design' targeting kids](https://www.cnbc.com/2026/05/12/tiktok-instagram-social-media-addictive-eu-crack-down.html) ⭐️ 6.0/10

The European Union announced measures to crack down on TikTok and Instagram's addictive design practices targeting children, marking a significant enforcement action under the Digital Services Act. The regulation focuses on dark patterns such as infinite scroll, algorithmic recommendation systems, and variable reward mechanisms designed to maximize user engagement. This represents the first major regulatory action specifically targeting addictive design features on social media platforms, potentially setting a global precedent. If enforced, it could force platforms to fundamentally redesign their interfaces and algorithms for younger users, potentially affecting billions of users worldwide. The crackdown targets specific UX dark patterns including infinite scroll, push notifications designed to re-engage users, and algorithmic content curation that personalizes feeds based on behavior tracking. Platforms found non-compliant could face fines of up to 6% of their global annual turnover under the Digital Services Act.

hackernews · thm · May 12, 11:00

**Background**: The Digital Services Act (DSA) is a European Union regulation that came into full application in 2024, establishing comprehensive rules for digital platforms to protect users, especially minors. 'Dark patterns' or 'deceptive patterns' refer to manipulative design techniques that trick users into actions they didn't intend, such as infinite scroll that removes natural stopping points. Algorithmic content curation uses AI to select and arrange content based on inferred user interests and engagement metrics, often optimizing for time spent on platform rather than user well-being.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Algorithmic_curation">Algorithmic curation - Wikipedia</a></li>
<li><a href="https://www.deceptive.design/">Deceptive Patterns (aka Dark Patterns ) - spreading awareness since...</a></li>
<li><a href="https://www.fastcompany.com/90369183/deceptive-design-tricks-and-dark-patterns-that-steer-your-clicks">These are the deceptive design tricks and dark patterns that steer...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion reveals strong technical engagement, with multiple developers sharing personal projects building algorithm blockers for Safari and iOS. Commenters widely agree that addictive design harms everyone, not just children, with one user noting 'social media is actually crazy how much more pleasant social media is without recommendation algorithms.' A key philosophical debate emerged about why regulation targets minors specifically when these design patterns are equally harmful to adults. Some commenters proposed legal frameworks distinguishing algorithmic curation from neutral platform status, suggesting platforms that actively curate content lose 'common carrier' protections.

**Tags**: `#tech-regulation`, `#social-media`, `#addictive-design`, `#eu-policy`, `#algorithms`

---

<a id="item-4"></a>
## [Coursera and Udemy are now one company](https://blog.coursera.org/coursera-and-udemy-are-now-one-company-creating-the-worlds-most-comprehensive-skills-platform/) ⭐️ 6.0/10

Coursera and Udemy have officially merged to create a combined skills platform, bringing together two of the largest online learning providers under one corporate umbrella. The merger combines Coursera's university partnership model with Udemy's course marketplace approach. This merger creates one of the largest consolidated players in the online education market, potentially reducing competition and choice for learners. The combined entity will control a significant portion of the digital learning market, raising questions about pricing, course quality, and platform access going forward. The merger brings together Coursera's approximately 77 million learners and partnerships with over 300 universities with Udemy's 50 million students and over 210,000 courses. Community feedback indicates both platforms have shifted toward paywall-heavy models, with courses like NAND to Tetris becoming premium-only after years of free access.

hackernews · Anon84 · May 12, 10:37

**Background**: Coursera, founded in 2012 by Stanford professors Andrew Ng and Daphne Koller, pioneered free online courses from top universities. Udemy launched the same year as a course marketplace allowing anyone to teach. Both platforms initially offered free or low-cost educational content but have increasingly moved toward subscription and paywall models in recent years as investor pressure for profitability has grown.

**Discussion**: Community sentiment is largely nostalgic and critical, with users mourning the decline of both platforms from their earlier, more accessible days. Multiple commenters cite specific examples like NAND to Tetris being placed behind paywalls as emblematic of broader quality degradation. Concerns about subscription-only models replacing one-time purchases were frequently raised, with one commenter dismissing the consolidation as 'competition is for losers.'

**Tags**: `#online-learning`, `#edtech`, `#mergers-acquisitions`, `#coursera`, `#udemy`

---

<a id="item-5"></a>
## [UnDUNE II](https://liquidream.itch.io/undune2) ⭐️ 5.0/10

Liquidream released UnDUNE II, a fan-made demake of the classic 1992 RTS game Dune II, on itch.io. The project recreates Westwood Studios' pioneering real-time strategy game with nostalgic appeal for longtime fans. Dune II is considered one of the foundational titles of the RTS genre, and this demake preserves its legacy for modern audiences. Fan projects like this keep classic gaming history accessible while showcasing the enduring appeal of 1990s game design. The demake runs in a web browser via itch.io, making it easily accessible without original hardware. Community members noted specific nostalgic details like the unit 'reporting' and 'acknowledged' sound effects, and how the original soundtrack (stored in .adl files) remains memorable.

hackernews · tosh · May 12, 12:38

**Background**: A demake is a game remake that targets older or less capable platforms, often converting modern games to retro styles—but in this case, converting Dune II to a more accessible format. Dune II: The Building of a Dynasty was developed by Westwood Studios and published by Virgin Games in 1992, establishing many mechanics that became standard in the RTS genre. The game featured resource harvesting from spice fields and base-building across three playable factions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dune_II">Dune II - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Category:Video_game_demakes">Category: Video game demakes - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The discussion was dominated by nostalgic memories rather than technical analysis. Users fondly recalled the iconic soundtrack (with one sharing a tool to play original .adl music files) and characteristic unit sounds. One commenter appreciated quality-of-life improvements like not needing to manually click move commands on the sidebar. A newcomer asked what a demake is, highlighting that the term isn't universally known.

**Tags**: `#retro-gaming`, `#dune`, `#demake`, `#game-development`, `#rts`

---

<a id="item-6"></a>
## [Chasing Utopia review – renegade Google exec Mo Gawdat searches for ethical AI in alarming insider warning](https://www.theguardian.com/film/2026/may/12/chasing-utopia-review-renegade-google-exec-mo-gawdat-searches-for-ethical-ai-in-alarming-insider-warning) ⭐️ 5.0/10

A documentary titled "Chasing Utopia" features former Google X executive Mo Gawdat's campaign for ethical AI development, with directors Alex Holmes and Lina Zilinskaite presenting an 83-minute exploration of AI dangers including job displacement, power concentration, and brain organoid computing. The documentary represents an insider warning from someone who once oversaw advanced projects at one of the world's largest tech companies, lending credibility to concerns about AI development accelerating without adequate moral safeguards. It raises questions about whether empathy and benevolence can be successfully integrated into neural networks to prevent technological catastrophe. The film covers organoid intelligence (OI), an emerging field developing biological wetware computing using 3D cultures of human brain cells that can be integrated with brain-machine interface technologies. Mo Gawdat argues that humanity's capacity for benevolence is the training resource needed to prevent AI from causing catastrophe.

rss · The Guardian Film · May 12, 12:00

**Background**: Organoid intelligence represents a convergence of computer science and biology, where researchers use miniature brain-like structures grown from stem cells as computational substrates. This biocomputing approach addresses concerns about AI's ballooning demands for data storage and energy by leveraging biological neural networks' adaptive reservoir computation capabilities. The technology can perform tasks like speech recognition and nonlinear equation prediction through these biological systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Organoid_intelligence">Organoid intelligence - Wikipedia</a></li>
<li><a href="https://www.nature.com/articles/s41928-023-01069-w">Brain organoid reservoir computing for artificial intelligence | Nature Electronics</a></li>
<li><a href="https://www.scientificamerican.com/article/these-living-computers-are-made-from-human-neurons/">These Living Computers Are Made from Human Neurons</a></li>

</ul>
</details>

**Tags**: `#AI Ethics`, `#Documentary`, `#Tech Industry`, `#AI Safety`, `#Media Review`

---

<a id="item-7"></a>
## [Một nhân viên tài chính đã ‘tự nguyện’ chuyển 25 triệu USD cho kẻ lừa đảo chỉ sau cuộc họp qua Zoom: Chuyên gia Hiếu PC cảnh báo hiểm họa trong kỷ nguyên AI](https://kenh14.vn/mot-nhan-vien-tai-chinh-da-tu-nguyen-chuyen-25-trieu-usd-cho-ke-lua-dao-chi-sau-cuoc-hop-qua-zoom-chuyen-gia-hieu-pc-canh-bao-hiem-hoa-trong-ky-nguyen-ai-215260512195900222.chn) ⭐️ 5.0/10

A Vietnamese news outlet reports on a Deepfake-enabled fraud incident where a financial employee transferred $25 million after a fake Zoom meeting, with cybersecurity expert Hiếu PC providing basic safety advice against AI-powered scams.

rss · Kenh14 · May 12, 20:10

**Tags**: `#deepfake`, `#ai-security`, `#fraud-prevention`, `#cybersecurity`, `#phishing`

---

<a id="item-8"></a>
## [Cannes Juror Paul Laverty Says ‘Shame on Hollywood’ for Blacklisting Susan Sarandon and More Actors Who Oppose War in Gaza: ‘They’re the Best of Us’](https://variety.com/2026/film/news/paul-laverty-cannes-hollywood-blacklisting-susan-sarandon-gaza-1236745839/) ⭐️ 4.0/10

Cannes jury member Paul Laverty criticized Hollywood for blacklisting actors like Susan Sarandon who have spoken out against the war in Gaza, calling such actors 'the best of us.'

rss · Variety · May 12, 14:21

**Tags**: `#entertainment-industry`, `#political-speech`, `#hollywood`, `#censorship`, `#film-festival`

---

