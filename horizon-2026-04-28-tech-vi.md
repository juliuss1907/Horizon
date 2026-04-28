# Horizon Daily - 2026-04-28

> From 33 items, 20 important content pieces were selected

---

1. [Elon Musk and Sam Altman are going to court over OpenAI’s future](#item-1) ⭐️ 8.0/10
2. [High Performance Git](#item-2) ⭐️ 7.0/10
3. [AI-Generated APIs Have an IDOR Problem: 3 Patterns Cursor Misses](#item-3) ⭐️ 7.0/10
4. [Anti-bot without the arms race: what Camoufox does differently](#item-4) ⭐️ 7.0/10
5. [https://www.wsj.com/tech/ai/openai-misses-key-revenue-user-targets-in-high-stake](#item-5) ⭐️ 7.0/10
6. [Wire Claude into Hashlock Markets in 10 minutes: a hands-on MCP tutorial](#item-6) ⭐️ 6.0/10
7. [I Had a Free Oracle Cloud ARM Box With 24GB RAM — So I Got Weird With It](#item-7) ⭐️ 6.0/10
8. [Google is testing AI chatbot search for YouTube](#item-8) ⭐️ 5.0/10
9. [Put it in pencil: NASA's Artemis III mission will launch no earlier than late 2027](#item-9) ⭐️ 5.0/10
10. [Some Musk v. Altman Jurors Don't Like Elon Musk](#item-10) ⭐️ 5.0/10
11. [🤖 SWE-agent — Deep Dive & Build-Your-Own Guide](#item-11) ⭐️ 5.0/10
12. [Top 10 Code Review Mistakes That Let Performance Issues Slip](#item-12) ⭐️ 5.0/10
13. [Building Real HMI Interfaces with a 4.3-inch ESP32-S3 Touch Display (WiFi + LVGL)](#item-13) ⭐️ 5.0/10
14. [Gemini-3-Flash: My ai agent benchmark terminalbench Win & 3 Fixes](#item-14) ⭐️ 5.0/10
15. [The Capital Suck](#item-15) ⭐️ 5.0/10
16. [Introducing Agentic Trading on Gemini: The Future of Crypto Is Autonomous](#item-16) ⭐️ 5.0/10
17. [Integrated by Design](#item-17) ⭐️ 4.0/10
18. [India’s Snabbit closes $56M round as investor interest in on-demand home services heats up](#item-18) ⭐️ 4.0/10
19. [Thoughts on crypto VC](#item-19) ⭐️ 4.0/10
20. [🚨 Zetachain Exploit 🚨](#item-20) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Elon Musk and Sam Altman are going to court over OpenAI’s future](https://www.technologyreview.com/2026/04/27/1136466/elon-musk-and-sam-altman-are-going-to-court-over-openais-future/) ⭐️ 8.0/10

Elon Musk and OpenAI CEO Sam Altman are heading to trial this week in Northern California after years of legal disputes, with the court set to decide whether OpenAI can legally operate as a for-profit enterprise ahead of its anticipated IPO. The outcome could fundamentally reshape OpenAI's corporate structure and set precedent for how AI companies organize themselves commercially. This trial carries enormous implications for the entire AI industry, as it will determine whether AI companies can transition from nonprofit origins to fully commercial enterprises while retaining their original missions. The ruling could establish legal precedent affecting how AI organizations worldwide structure their operations, fundraising, and governance, potentially influencing hundreds of billions in investment flows. OpenAI was originally founded as a 501(c)(3) nonprofit in 2015, then created a capped-profit subsidiary OpenAI LP in 2019 to attract capital. The company has since been transitioning its for-profit entity to a Public Benefit Corporation structure, a process that has drawn scrutiny from Delaware Attorney General Kathy Jennings and opposition from a coalition of California-based foundations and nonprofits.

rss · MIT Tech Review · Apr 27, 22:52

**Background**: OpenAI's unique hybrid structure was designed to attract investment while preventing AI from being developed purely for commercial gain. Under the capped-profit model, investors and employees receive returns up to a predetermined cap, with any profits beyond that threshold funneled back into the nonprofit's mission of developing safe AGI. This structure allowed OpenAI to raise billions from Microsoft and other investors while theoretically maintaining its founding purpose.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/evolving-our-structure/">Evolving OpenAI's structure</a></li>
<li><a href="https://news.delaware.gov/2025/10/28/ag-jennings-completes-review-of-openai-recapitalization/">AG Jennings completes review of OpenAI recapitalization - State of Delaware News</a></li>
<li><a href="https://openai.com/our-structure/">Our structure - OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI Industry`, `#Legal Battle`, `#Elon Musk`, `#Corporate Structure`

---

<a id="item-2"></a>
## [High Performance Git](https://gitperf.com/) ⭐️ 7.0/10

A comprehensive guide to Git performance internals that helps developers understand plumbing commands and optimize their workflow.

hackernews · gnabgib · Apr 28, 00:32

**Tags**: `#git`, `#performance`, `#developer-tools`, `#version-control`, `#tutorials`

---

<a id="item-3"></a>
## [AI-Generated APIs Have an IDOR Problem: 3 Patterns Cursor Misses](https://dev.to/chandan_karn_fb750e731394/ai-generated-apis-have-an-idor-problem-3-patterns-cursor-misses-4ji6) ⭐️ 7.0/10

A developer documented how AI code editors like Cursor generate APIs that include authentication middleware but omit per-resource ownership checks, creating Insecure Direct Object Reference (IDOR) vulnerabilities. Any authenticated user can access another user's data by simply guessing or incrementing the object ID in the request. This vulnerability affects the rapidly growing number of developers adopting AI coding assistants, potentially exposing sensitive user data across countless AI-generated projects. Since AI-generated code often passes tests and appears secure due to authentication middleware, developers may deploy vulnerable applications without realizing the authorization gap. The article identifies three common vulnerability patterns in AI-generated APIs, with the most critical being CWE-862: Missing Authorization. The root cause is that AI models are trained on tutorials that teach authentication but rarely cover authorization—the verification that an authenticated user is actually allowed to access a specific record. The recommended fix is to scope ownership directly into database queries.

rss · Dev.to · Apr 28, 06:25

**Background**: IDOR (Insecure Direct Object Reference) is an access control vulnerability listed in the OWASP Top Ten that occurs when an application exposes internal object identifiers (such as database keys or record IDs) and fails to verify that the requesting user is authorized to access the referenced object. Cursor is an AI-first code editor built as a fork of VS Code, with AI integrated throughout the editing experience, including multi-line autocomplete and autonomous agent mode for building features. Similar issues have been observed in Claude Code and GitHub Copilot outputs.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/Security/Attacks/IDOR">Insecure Direct Object Reference (IDOR) - Security | MDN</a></li>
<li><a href="https://owasp.org/www-community/attacks/insecure_direct_object_reference">Insecure Direct Object Reference (IDOR) | OWASP Foundation</a></li>
<li><a href="https://cursor.com/">Cursor: The best way to code with AI</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI-tools`, `#IDOR`, `#API-development`, `#vulnerability`

---

<a id="item-4"></a>
## [Anti-bot without the arms race: what Camoufox does differently](https://dev.to/tokozen/anti-bot-without-the-arms-race-what-camoufox-does-differently-e67) ⭐️ 7.0/10

Camoufox is a modified Firefox build that patches browser fingerprinting evasion at the C++ and Rust engine level, rather than using JavaScript shims. The tool addresses runtime fingerprinting signals including canvas rendering hashes, WebGL vendor strings, screen geometry, navigator.webdriver, and font enumeration without leaving detectable artifacts. This approach breaks the traditional cat-and-mouse cycle where detection vendors update their logic faster than developers can patch. For developers working on web scraping or browser automation, Camoufox provides a sustainable solution where fingerprint corrections live in the compiled binary itself, making them harder to detect than JS-layer tampering. Camoufox injects controlled noise at the canvas rendering level so hashes vary realistically across sessions, spoofs WebGL vendor strings to plausible hardware values instead of revealing Mesa software rendering in containers, and allows configuration of screen sizes and reported fonts to match common real-world distributions. The Python wrapper handles launching the patched browser and configuring fingerprint parameters without requiring developers to write custom JavaScript injection code.

rss · Dev.to · Apr 28, 06:18

**Background**: Browser fingerprinting is a tracking technique that aggregates dozens of weak signals—canvas rendering, WebGL vendor strings, AudioContext API behavior, font metrics, screen geometry, and navigator properties—into a probabilistic identifier. Unlike behavioral analysis, runtime fingerprinting checks what the browser actually is at the code level. Headless browsers like standard Playwright or Puppeteer produce consistent, recognizable signatures that differ from real user sessions, such as canvas hashes from Linux servers with software rendering or viewport sizes that don't match any physical screen.

<details><summary>References</summary>
<ul>
<li><a href="https://scrapfly.io/blog/posts/how-browser-fingerprinting-works">How Browser Fingerprinting Works and How to Defend Against It ...</a></li>
<li><a href="https://www.browserless.io/blog/device-fingerprinting">Browser Fingerprinting Guide: Detection & Bypass Methods ...</a></li>
<li><a href="https://fingerprint.com/blog/browser-fingerprinting-techniques/">Browser Fingerprinting Techniques: 6 Top Methods Explained</a></li>

</ul>
</details>

**Tags**: `#browser-automation`, `#web-scraping`, `#fingerprinting`, `#anti-bot`, `#playwright`

---

<a id="item-5"></a>
## [https://www.wsj.com/tech/ai/openai-misses-key-revenue-user-targets-in-high-stake](https://www.wsj.com/tech/ai/openai-misses-key-revenue-user-targets-in-high-stakes-sprint-toward-ipo-94a95273?mod=e2tw) ⭐️ 7.0/10

OpenAI reportedly missed key revenue and user growth targets as the company pushes toward a potential initial public offering, according to Wall Street Journal reporting on the company's financial performance. The missed targets highlight the challenges AI companies face in converting massive user bases into sustainable revenue streams, and raise questions about OpenAI's valuation and IPO prospects in an increasingly competitive market. The company has been racing to demonstrate financial viability to investors as it pursues public markets, with revenue growth放缓ing while operational costs remain high due to expensive AI model training and deployment.

telegram · ahboyashreads · Apr 28, 03:26

**Background**: OpenAI, founded in 2015 as a non-profit AI research laboratory, transitioned to a commercial structure and gained worldwide attention after launching ChatGPT in November 2022. The company has raised billions in funding from Microsoft and other investors, achieving a reported valuation exceeding $80 billion, making it one of the most valuable private companies in the AI sector. IPO preparation typically requires companies to show consistent growth and clear paths to profitability.

**Tags**: `#OpenAI`, `#AI Industry`, `#IPO`, `#Business News`, `#Revenue`

---

<a id="item-6"></a>
## [Wire Claude into Hashlock Markets in 10 minutes: a hands-on MCP tutorial](https://dev.to/barissozen/wire-claude-into-hashlock-markets-in-10-minutes-a-hands-on-mcp-tutorial-45n6) ⭐️ 6.0/10

A hands-on tutorial demonstrates how to connect Claude or other MCP-capable AI agents to Hashlock Markets for autonomous cross-chain crypto trading, using either stdio or Streamable HTTP transport with SIWE authentication. This tutorial enables fully autonomous AI-driven DeFi trading by connecting AI agents directly to a sealed-bid RFQ and HTLC-based trading system, eliminating human intervention from the trading lifecycle and potentially reducingMEV arbitrage risks through private quotes. The MCP server exposes six tools for the trading lifecycle, supporting two authentication methods: local stdio transport (fastest for development via npx @hashlock-tech/mcp) or hosted Streamable HTTP (accessible at https://hashlock.markets/mcp for custom orchestrators). The platform uses HTLC atomic settlement to ensure cross-chain trades either complete or revert entirely without intermediary escrow.

rss · Dev.to · Apr 28, 06:22

**Background**: Hashlock Markets implements sealed-bid RFQ (Request for Quote) where quotes remain private until execution, protecting traders from front-running. HTLC (Hashed Time-Lock Contract) is the cryptographic primitive underlying atomic swaps, Lightning Network, and non-oracle cross-chain bridges, using hashlocks and timelocks to ensure either both parties complete the swap or neither does. MCP (Model Context Protocol) is an open standard that enables AI agents to connect with external tools and data sources in a standardized way.

<details><summary>References</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/specification/2025-11-25">Specification - Model Context Protocol</a></li>
<li><a href="https://www.emergentmind.com/topics/hash-time-lock-htl-contracts">Hash-Time-Lock Contracts - emergentmind.com</a></li>
<li><a href="https://chainscorelabs.com/en/glossary/defi-protocols/defi-aggregators-and-routing/request-for-quote-rfq">What is RFQ (Request for Quote) in DeFi? | Chainscore Glossary</a></li>

</ul>
</details>

**Tags**: `#MCP`, `#DeFi`, `#crypto trading`, `#AI agents`, `#tutorial`

---

<a id="item-7"></a>
## [I Had a Free Oracle Cloud ARM Box With 24GB RAM — So I Got Weird With It](https://dev.to/tedtalk/i-had-a-free-oracle-cloud-arm-box-with-24gb-ram-so-i-got-weird-with-it-390d) ⭐️ 6.0/10

A developer published a practical guide demonstrating how to use Oracle Cloud's free ARM instance (4 cores, 24GB RAM, 200 Mbps) for self-hosted LLM inference via Ollama, running models like Llama 3.2 3B or Mistral 7B with Q4_K_M quantization on a reverse-proxied endpoint. This enables developers to run local LLM APIs without per-token costs, leveraging underutilized free-tier cloud resources for production-grade inference. The 24GB RAM configuration supports concurrent models and leaves headroom for a 13B model alongside a 3B model, making self-hosted AI economically viable. The author highlights that llama.cpp has native ARM/NEON SIMD optimizations making inference genuinely fast on ARM hardware. A 7B model with Q4_K_M quantization fits in ~4.5GB RAM, consuming 15-25% CPU during inference and ~5-8GB RAM at rest, dropping to near-zero when idle. Resource-efficient tools like Bazel Remote Cache (1-3% CPU idle) and Airbyte are also demonstrated.

rss · Dev.to · Apr 28, 06:20

**Background**: Oracle Cloud Infrastructure (OCI) offers a permanently free tier with ARM Ampere A1 cores, making it attractive for running compute-intensive workloads. Ollama is an open-source tool that simplifies running LLMs locally by handling model weights, configuration, and inference runtime in a single package, supporting GGUF-formatted quantized models. Q4_K_M is a 4-bit quantization method using k-means clustering that balances model size reduction with quality preservation.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@paul.ilvez/demystifying-llm-quantization-suffixes-what-q4-k-m-q8-0-and-q6-k-really-mean-0ec2770f17d3">Demystifying LLM Quantization Suffixes: What Q4_K_M, Q8_0, and Q6_K Really Mean | by Paul Ilvez | Medium</a></li>
<li><a href="https://www.neurealm.com/blogs/practical-approach-to-arm-neon-optimization/">Practical approach to Arm Neon Optimization | Neurealm</a></li>

</ul>
</details>

**Tags**: `#self-hosted-llm`, `#ollama`, `#oracle-cloud`, `#arm-inference`, `#infrastructure-optimization`

---

<a id="item-8"></a>
## [Google is testing AI chatbot search for YouTube](https://www.theverge.com/streaming/919441/google-ask-youtube-ai-chatbot-search) ⭐️ 5.0/10

Google is testing a new conversational search experience on YouTube that aggregates content from longform videos, Shorts, and text-based results, similar to its AI Mode feature in Google Search. The feature, currently available as an experiment, allows users to interact with search results in a more natural, dialogue-like format. This development signals Google's intent to extend its AI-powered search capabilities beyond traditional web search into its video platform, potentially changing how users discover and engage with content on YouTube. With YouTube being the world's largest video platform, any major interface change could affect billions of users and content creators. The feature appears to pull results from multiple content types on YouTube, including full-length videos, Shorts, and textual descriptions, providing a unified conversational interface. This mirrors the AI Mode functionality launched in Google Search in March 2025, which uses Gemini 2.0 for advanced reasoning and multimodal understanding.

rss · The Verge · Apr 28, 00:01

**Background**: AI Mode is an experimental generative AI search feature that Google introduced in March 2025, enabling users to input complex, multi-part queries and receive AI-generated responses. The feature leverages Gemini 2.0 technology to combine advanced reasoning capabilities with Google's information systems, allowing for more nuanced and comprehensive search experiences. Google appears to be adapting this technology for YouTube's unique content ecosystem, which includes both short-form and long-form video content alongside text metadata.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_AI_Mode">AI Mode - Wikipedia</a></li>
<li><a href="https://blog.google/products-and-platforms/products/search/ai-mode-search/">AI Mode is a new generative AI experiment in Google Search .</a></li>

</ul>
</details>

**Tags**: `#AI`, `#YouTube`, `#Google`, `#Search`, `#Product News`

---

<a id="item-9"></a>
## [Put it in pencil: NASA's Artemis III mission will launch no earlier than late 2027](https://arstechnica.com/space/2026/04/put-it-in-pencil-nasas-artemis-iii-mission-will-launch-no-earlier-than-late-2027/) ⭐️ 5.0/10

SpaceX and Blue Origin have separately confirmed to NASA that their respective lunar landers will be ready for the Artemis III mission. As a result, NASA has officially pushed the target launch date to no earlier than late 2027, marking another schedule adjustment for the historic lunar return mission. The Artemis III mission represents NASA's first crewed lunar landing since Apollo 17 in 1972, making any schedule shift significant for the broader goal of establishing a sustainable human presence on the Moon. The confirmation from both commercial partners provides clarity on the program's path forward after years of uncertainty. Artemis III will launch aboard NASA's Space Launch System (SLS) rocket carrying the Orion spacecraft, which will rendezvous in lunar orbit with either SpaceX's Starship HLS or Blue Origin's Blue Moon lander for the descent to the surface. SpaceX's Starship HLS design relies on on-orbit propellant transfer using tanker vehicles and depot spacecraft before lunar transit.

rss · Ars Technica · Apr 28, 00:14

**Background**: The Artemis program is NASA's successor to the Apollo missions, designed to land the first woman and first person of color on the Moon. SpaceX was selected in April 2020 to develop its Starship Human Landing System as one of the competing lunar lander designs, with Blue Origin later selected as a second provider. The program aims to establish a long-term human presence on the lunar surface as a stepping stone for future Mars missions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artemis_III">Artemis III - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Starship_HLS">Starship HLS - Wikipedia</a></li>
<li><a href="https://www.nasa.gov/mission/artemis-iii/">Artemis III - NASA</a></li>

</ul>
</details>

**Tags**: `#NASA`, `#Artemis`, `#SpaceX`, `#Blue Origin`, `#Space Exploration`

---

<a id="item-10"></a>
## [Some Musk v. Altman Jurors Don't Like Elon Musk](https://www.wired.com/story/some-musk-v-altman-jurors-dont-like-elon-musk/) ⭐️ 5.0/10

During jury selection for Elon Musk's lawsuit against OpenAI and CEO Sam Altman, several potential jurors openly expressed unfavorable opinions about Musk himself, potentially complicating the case proceedings. The jurors' expressed bias against Musk could impact how the case is perceived and decided, as a favorable jury pool is crucial for any civil lawsuit. This development highlights the challenges of selecting an impartial jury in a high-profile case involving controversial public figures. The lawsuit challenges OpenAI's evolution from its original non-profit, open-source mission to a more commercially-oriented structure under Altman's leadership. The negative juror sentiment toward Musk adds another layer of complexity to an already contentious legal battle.

rss · Wired · Apr 28, 00:39

**Background**: Elon Musk was one of the original co-founders of OpenAI in 2015 but left the organization in 2018. His lawsuit alleges that OpenAI has abandoned its founding mission of developing AI for the benefit of humanity, instead pursuing profit-making activities. Jury selection is a critical phase in any trial where potential jurors are questioned to identify any biases that might affect their impartiality.

**Tags**: `#legal`, `#openai`, `#elon-musk`, `#sam-altman`, `#tech-news`

---

<a id="item-11"></a>
## [🤖 SWE-agent — Deep Dive & Build-Your-Own Guide](https://dev.to/truongpx396/swe-agent-deep-dive-build-your-own-guide-ade) ⭐️ 5.0/10

A dev.to tutorial providing a deep dive and build-your-own guide for SWE-agents (AI agents for software engineering tasks) failed to render properly due to a Liquid template syntax error (Unknown tag 'endraw'). SWE-agents represent a significant application of LLMs in automating complex software engineering tasks, such as bug fixing and code comprehension. Access to clear tutorials is crucial for developers looking to implement or improve such systems, making this content gap particularly notable for the developer community. The actual tutorial content remains inaccessible due to a Liquid syntax error involving the 'endraw' tag, which is commonly used in markdown code blocks. The technical depth, practical value, and educational quality of the guide cannot be evaluated at this time.

rss · Dev.to · Apr 28, 06:36

**Background**: SWE-agent (Software Engineering Agent) is a system introduced in a 2024 arXiv paper that enables LLM-based autonomous agents to interact with computers to solve real-world software engineering tasks. It utilizes custom Agent-Computer Interfaces (ACI) specifically designed to improve how AI systems navigate development environments, search through codebases, and execute engineering tasks. The system represents the intersection of LLM capabilities and practical software development automation.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2405.15793">[2405.15793] SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#software-engineering`, `#tutorial`, `#llm`, `#automation`

---

<a id="item-12"></a>
## [Top 10 Code Review Mistakes That Let Performance Issues Slip](https://dev.to/jhavtech/top-10-code-review-mistakes-that-let-performance-issues-slip-88p) ⭐️ 5.0/10

An article by jhavtech outlines the top 10 mistakes in code review processes that allow performance issues to bypass detection and reach production environments. The piece emphasizes that while code reviews often catch typos and readability issues, they frequently miss algorithmic efficiency, scalability concerns, and resource utilization problems. According to recent estimates, the cost of poor software quality in the United States alone has grown to at least $2.41 trillion, with the average data breach costing $4.45 million in 2023. When performance issues slip past review, they accumulate as technical debt that makes future development more expensive and systems more fragile. The article discusses the importance of examining algorithmic complexity (distinguishing between efficient O(n log n) versus performance-killing O(n²) implementations) and leveraging caching strategies during code review. It emphasizes separating correctness-focused reviews from dedicated performance optimization efforts.

rss · Dev.to · Apr 28, 06:31

**Background**: Code review is a collaborative quality assurance process where developers examine each other's code before it reaches production, serving as a final checkpoint for robustness and maintainability. Technical debt represents the implied cost of future rework caused by choosing expedient solutions over better approaches, accruing interest in the form of debugging time and system fragility. Performance optimization involves improving algorithmic efficiency, resource utilization, and reducing latency in software systems.

**Tags**: `#code-review`, `#performance-optimization`, `#software-engineering`, `#best-practices`, `#quality-assurance`

---

<a id="item-13"></a>
## [Building Real HMI Interfaces with a 4.3-inch ESP32-S3 Touch Display (WiFi + LVGL)](https://dev.to/alan12/building-real-hmi-interfaces-with-a-43-inch-esp32-s3-touch-display-wifi-lvgl-14o9) ⭐️ 5.0/10

A developer tutorial demonstrates how to build touch-based HMI interfaces using ESP32-S3 with the LVGL graphics library on a 4.3-inch 800×480 display with integrated WiFi and Bluetooth connectivity. As IoT and embedded applications demand more sophisticated user interfaces, this tutorial addresses the growing need for developers to create modern touchscreen HMIs without expensive high-end hardware, democratizing GUI development for resource-constrained devices. The ESP32-S3's dual-core Xtensa LX7 CPU, PSRAM support, and native USB make it well-suited for LVGL-based UI rendering. Typical architecture combines touch input, LVGL UI logic, WiFi connectivity for MQTT/REST APIs, and dashboard display on 800×480 panels.

rss · Dev.to · Apr 28, 06:28

**Background**: HMI (Human Machine Interface) refers to the interface through which humans interact with machines. LVGL (Light and Versatile Graphics Library) is an open-source C library widely used for embedded GUI development due to its low resource consumption, strong portability, and rich widget support including buttons, sliders, charts, and animations. ESP32-S3 is Espressif's latest flagship microcontroller featuring dual-core processing, integrated WiFi and Bluetooth, and improved performance for graphics-intensive applications.

<details><summary>References</summary>
<ul>
<li><a href="https://lvgl.io/">LVGL — Light and Versatile Embedded UI Ecosystem</a></li>
<li><a href="https://github.com/lvgl/lvgl">GitHub - lvgl / lvgl : Embedded graphics library to create beautiful UIs...</a></li>
<li><a href="https://documentation.espressif.com/esp32-s3_datasheet_en.pdf">[PDF] ESP32-S3 Series</a></li>

</ul>
</details>

**Tags**: `#ESP32`, `#LVGL`, `#HMI`, `#Embedded Systems`, `#Touch Display`, `#IoT`

---

<a id="item-14"></a>
## [Gemini-3-Flash: My ai agent benchmark terminalbench Win & 3 Fixes](https://dev.to/umair24171/gemini-3-flash-my-ai-agent-benchmark-terminalbench-win-3-fixes-44eb) ⭐️ 5.0/10

A developer documented their experience benchmarking Google's Gemini 3 Flash on TerminalBench, a rigorous benchmark for AI agents performing real CLI tasks. They shared practical solutions for three common issues: tool call problems, silent API failures, and multi-agent architecture challenges in a Node.js environment. This practical debugging guide addresses the gap between theoretical LLM capabilities and real-world AI agent deployment. By testing on TerminalBench's 89 challenging tasks, developers can validate actual reasoning, tool-use, and error handling capabilities rather than relying on token count metrics alone. The agent architecture consists of four components: an orchestrator (agent.js) for conversation management, a tool registry (tools.js) exposing shell commands via Node.js child processes, a state manager (state.js), and prompt templates (prompts.js) for guiding model behavior. The developer wrapped common shell commands like ls, cd, cat, mkdir, and curl as callable tools.

rss · Dev.to · Apr 28, 06:27

**Background**: TerminalBench is an AI agent benchmark that evaluates models on complex command-line interface tasks, including file operations, network requests, and package management. Unlike synthetic benchmarks, it tests real-world CLI navigation capabilities. Function calling (or tool calling) enables LLMs to interact with external tools and APIs beyond their training data, which is essential for AI agents to perform actionable tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2601.11868v1">Terminal-Bench: Benchmarking Agents on Hard, Realistic Tasks in Command Line Interfaces</a></li>
<li><a href="https://github.com/harbor-framework/terminal-bench">GitHub - harbor-framework/terminal-bench: A benchmark for LLMs on complicated tasks in the terminal · GitHub</a></li>
<li><a href="https://www.promptingguide.ai/agents/function-calling">Function Calling in AI Agents | Prompt Engineering Guide</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#gemini`, `#benchmarking`, `#terminalbench`, `#llm-debugging`

---

<a id="item-15"></a>
## [The Capital Suck](https://x.com/jonah_b/status/2048837866038415690?s=20) ⭐️ 5.0/10

A social media analysis by Jonah B claims that each $1B of new stablecoins generates approximately $122B in annual economic activity with 122x velocity, producing roughly $19M in protocol revenue. The post further states that stablecoin supply has grown 60x since early 2020 to approximately $300B, with institutional capital and tokenized RWAs increasingly migrating onchain. These figures suggest that stablecoins function as a powerful economic engine, with a relatively small capital base generating substantial onchain activity. If accurate, this analysis demonstrates that stablecoins are becoming a critical infrastructure for digital asset economies, potentially accelerating institutional adoption and RWA tokenization trends. The analysis highlights a 'flywheel' effect where stablecoin issuance drives economic activity, which in turn generates protocol revenue. Visa's research indicates that stablecoin daily velocity typically ranges from 0.15–0.25 in real-world usage, suggesting the 122x multiplier figure may represent annualized or aggregated velocity rather than single-day transactions. The methodology behind these calculations is not specified in the post.

telegram · ahboyashreads · Apr 28, 03:26

**Background**: Stablecoins are cryptocurrencies designed to maintain a stable value, typically pegged to the US dollar or other fiat currencies. RWA (Real World Assets) tokenization refers to representing physical assets like real estate, treasuries, or private credit as blockchain-based tokens. McKinsey reports that stablecoins currently process significant cross-border payment volumes, while the tokenization market is projected to accelerate in 2025-2026 as the technology matures from pilot stages to production-scale deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://corporate.visa.com/en/sites/visa-economic-empowerment-institute/stablecoin-velocity.html">Assessing stablecoin velocity and its economic impact | Visa</a></li>
<li><a href="https://rwa.xyz/">RWA .xyz | Tokenized Real - World Asset Analytics</a></li>
<li><a href="https://www.mckinsey.com/industries/financial-services/our-insights/the-stable-door-opens-how-tokenized-cash-enables-next-gen-payments">Stablecoins payments infrastructure for modern finance | McKinsey</a></li>

</ul>
</details>

**Tags**: `#stablecoins`, `#defi`, `#rwa-tokenization`, `#onchain-economy`, `#institutional-adoption`

---

<a id="item-16"></a>
## [Introducing Agentic Trading on Gemini: The Future of Crypto Is Autonomous](https://www.gemini.com/en-SG/blog/introducing-agentic-trading-on-gemini-the-future-of-crypto-is-autonomous) ⭐️ 5.0/10

Gemini has launched Agentic Trading, a feature that allows users to connect AI agents like Claude and ChatGPT to their trading accounts via the Model Context Protocol (MCP), enabling autonomous trade execution, market monitoring, and risk management through the full Gemini API. This represents a significant step in the convergence of agentic AI and cryptocurrency trading, potentially transforming how retail and institutional traders interact with crypto markets by delegating strategy execution to AI agents while maintaining human oversight of defined parameters. The feature integrates with existing AI assistants through the open MCP standard, allowing AI agents to access real-time market data, execute trades, and manage positions autonomously. Users define strategies and risk parameters while the AI handles continuous market monitoring and execution.

telegram · ahboyashreads · Apr 28, 03:26

**Background**: The Model Context Protocol (MCP) is an open JSON-RPC standard that provides AI applications with a unified way to call tools, access resources, and integrate with external systems like APIs. Agentic trading differs from traditional automated trading by allowing AI agents to not just execute pre-defined instructions but to dynamically analyze markets, make decisions, and adapt strategies based on changing conditions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gemini.com/blog/introducing-agentic-trading-on-gemini-the-future-of-crypto-is-autonomous">Introducing Agentic Trading on Gemini: The Future of Crypto ...</a></li>
<li><a href="https://modelcontextprotocol.io/docs/getting-started/intro">What is the Model Context Protocol (MCP)?</a></li>
<li><a href="https://www.theblock.co/post/399001/gemini-rolls-out-agentic-trading-allowing-ai-bots-to-directly-manage-crypto-exchange-trading-accounts">Gemini rolls out Agentic Trading allowing AI bots to directly ...</a></li>

</ul>
</details>

**Tags**: `#agentic-ai`, `#crypto-trading`, `#gemini`, `#MCP-protocol`, `#autonomous-systems`

---

<a id="item-17"></a>
## [Integrated by Design](https://vivianvoss.net/blog/integrated-by-design-launch) ⭐️ 4.0/10

A book promotion post titled 'Integrated by Design' that promotes FreeBSD over Linux has attracted skepticism from the HN community due to suspected AI-generated content and suspicious domain history, despite some praise for the technical comparison.

hackernews · vermaden · Apr 27, 23:14

**Tags**: `#freebsd`, `#linux`, `#operating-systems`, `#books`, `#ai-generated-content`

---

<a id="item-18"></a>
## [India’s Snabbit closes $56M round as investor interest in on-demand home services heats up](https://techcrunch.com/2026/04/27/indias-snabbit-closes-56m-round-as-investor-interest-heats-up-in-on-demand-home-services/) ⭐️ 4.0/10

Indian on-demand home services startup Snabbit has closed a $56 million funding round. The company now processes over 40,000 daily jobs and has achieved significant cost reductions while expanding across multiple cities. This funding highlights growing investor confidence in India's home services market, which has seen increased competition among on-demand platforms. The investment signals continued venture capital interest in aggregating fragmented local service providers at scale. Snabbit has demonstrated operational scalability by maintaining 40,000 daily job processing while driving down costs across its multi-city footprint. The fresh capital will likely fund further geographic expansion and service category additions to compete with established players in the Indian market.

rss · TechCrunch · Apr 28, 03:30

**Background**: India's on-demand home services market has grown rapidly as smartphone penetration increases and consumer trust in digital platforms improves. Major players like Urban Company have established category leadership, while newer entrants compete on pricing, service quality, and technology. The market opportunity spans home cleaning, repairs, beauty services, and appliance maintenance across urban centers.

**Tags**: `#startup-funding`, `#india-tech`, `#on-demand-services`, `#home-services`, `#venture-capital`

---

<a id="item-19"></a>
## [Thoughts on crypto VC](https://x.com/bennypjacobs/status/2048753204473549144?s=20) ⭐️ 4.0/10

An opinion piece outlines three strategic paths for crypto VCs expanding into non-crypto sectors like AI without domain expertise: sticking to crypto/fintech with clear PMF, diversifying thoughtfully with LP approval, or avoiding off-mandate deals falsely labeled as having "crypto ethos". This framework highlights the strategic risks crypto VCs face when diversifying beyond core competencies without proper domain knowledge, offering guidance on maintaining competitive advantage in unfamiliar sectors. The author emphasizes that crypto VCs often lack competitive edge beyond crypto-native opportunities when entering frontier tech like AI, and the framework suggests focusing on proven areas like stablecoins, payments, tokenization, and DeFi rather than forcing ill-fitting investments.

telegram · ahboyashreads · Apr 28, 03:26

**Background**: Crypto venture capital refers to funds that invest in blockchain and cryptocurrency startups, including infrastructure, DeFi protocols, Web3 projects, and NFT platforms. Product-Market Fit (PMF) is the degree to which a product fulfills a market need, meaning people genuinely want what the product offers. DeFi (Decentralized Finance) is a financial system built on blockchain technology that enables direct peer-to-peer transactions without traditional intermediaries like banks. Stablecoins are cryptocurrencies designed to maintain a stable value, typically pegged to a reserve asset like the US dollar.

<details><summary>References</summary>
<ul>
<li><a href="https://www.investopedia.com/decentralized-finance-defi-5113835">Understanding Decentralized Finance (DeFi): Basics and ...</a></li>
<li><a href="https://ethereum.org/defi/">What is DeFi? | Benefits and Use of Decentralised Finance ...</a></li>

</ul>
</details>

**Tags**: `#crypto-vc`, `#venture-capital`, `#investment-strategy`, `#ai-investment`, `#fintech`

---

<a id="item-20"></a>
## [🚨 Zetachain Exploit 🚨](https://x.com/ZetaChain/status/2048854107633631356?s=20) ⭐️ 4.0/10

ZetaChain disclosed a targeted attack on its GatewayEVM contract that drained approximately $300,000 from internal team wallets. The team has blocked the exploit vector and paused all cross-chain transactions as a precaution, confirming that no user funds were impacted. This incident highlights the ongoing security challenges in cross-chain infrastructure, even when financial losses remain relatively contained. While the $300k loss is modest compared to major exploits, the pause in cross-chain activity affects ZetaChain's core functionality and user experience. The attack targeted the GatewayEVM contract, which serves as a unified entry point for cross-chain interactions between external EVM-compatible blockchains and applications deployed on ZetaChain. The team acted quickly to mitigate further damage by halting all cross-chain transactions while investigations and security fixes continue.

telegram · ahboyashreads · Apr 28, 03:26

**Background**: ZetaChain is a Layer-1 blockchain designed to support omnichain message passing and fund transfer, enabling smart contract interactions across multiple blockchain networks including non-smart contract chains like Bitcoin. The GatewayEVM contract functions as a critical infrastructure component for ZetaChain's cross-chain operations, making it a high-value target for potential exploits.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cryptotimes.io/2026/04/28/zetachain-halts-cross-chain-activity-after-gatewayevm-smart-contract-exploit/">ZetaChain Halts Cross-Chain Activity After GatewayEVM Smart ...</a></li>
<li><a href="https://www.theblock.co/post/399092/zetachain-attack-smart-contract">ZetaChain halts cross-chain transactions following attack on ...</a></li>
<li><a href="https://www.zetachain.com/blog/introducing-omnichain-accounts">Introducing Omnichain Accounts | ZetaChain Blog</a></li>

</ul>
</details>

**Tags**: `#blockchain`, `#security-exploit`, `#cryptocurrency`, `#web3`, `#defi`

---

