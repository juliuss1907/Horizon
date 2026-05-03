# Horizon Daily - 2026-05-03

> From 86 items, 6 important content pieces were selected

---

1. [Apple SHARP 3D Splatting Model Now Runs In-Browser via ONNX Web](#item-1) ⭐️ 7.0/10
2. [Specsmaxxing: YAML Specs for AI Coding Collaboration](#item-2) ⭐️ 6.0/10
3. [Anthropic AI Agents Trade Autonomously in Simulated Market Experiment](#item-3) ⭐️ 6.0/10
4. [Investors Increase Clean Energy Investment Amid Geopolitical Tensions](#item-4) ⭐️ 5.0/10
5. [AI Re-creation of Ex-Partners Sparks Ethics Debate in China](#item-5) ⭐️ 4.0/10
6. [Chernobyl Wolves Thriving 40 Years After Nuclear Disaster](#item-6) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Apple SHARP 3D Splatting Model Now Runs In-Browser via ONNX Web](https://github.com/bring-shrubbery/ml-sharp-web) ⭐️ 7.0/10

A developer has successfully ported Apple's SHARP single-image 3D Gaussian splatting model to run entirely in-browser using ONNX Runtime Web with WebGPU execution provider, allowing users to reconstruct 3D scenes from a single image locally without any server communication. This implementation demonstrates the feasibility of running complex 3D reconstruction models directly in browsers, enabling privacy-preserving AI applications where user images never leave their device, and potentially democratizing access to 3D content creation tools through a zero-install web interface. The author exported Apple's original PyTorch SHARP predictor to ONNX format for compatibility with onnxruntime-web, achieving local-only processing where users can drop an image and either preview the result live or download the generated .ply point cloud file.

hackernews · bring-shrubbery · May 3, 09:14

**Background**: Apple's SHARP model, published in December 2025, achieves state-of-the-art results in monocular 3D scene synthesis by reducing LPIPS by 25-34% compared to prior models while being three orders of magnitude faster. 3D Gaussian Splatting is a rasterization technique that represents scenes as collections of 3D Gaussians, enabling real-time rendering of photorealistic scenes learned from sparse image inputs. ONNX Runtime Web is Microsoft's JavaScript library that enables running ONNX-format ML models directly in browsers using WebGPU for hardware acceleration.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/apple/ml-sharp">GitHub - apple/ml-sharp: Sharp Monocular View Synthesis in Less Than a Second · GitHub</a></li>
<li><a href="https://huggingface.co/apple/Sharp">apple/Sharp · Hugging Face</a></li>
<li><a href="https://onnxruntime.ai/docs/tutorials/web/">Web | onnxruntime</a></li>

</ul>
</details>

**Discussion**: Community members explored creative applications—one user built a VR headset interface for browsing local photo folders as volumetric 3D scenes with precomputed caching. However, critics noted that single-image reconstruction fundamentally requires hallucinating unseen geometry, potentially misinterpreting flat images like posters as 3D objects; another tester reported browser tab crashes due to high memory consumption during model loading.

**Tags**: `#3D Gaussian Splatting`, `#WebGPU`, `#Browser-based ML`, `#ONNX`, `#Apple SHARP`, `#Client-side AI`

---

<a id="item-2"></a>
## [Specsmaxxing: YAML Specs for AI Coding Collaboration](https://acai.sh/blog/specsmaxxing) ⭐️ 6.0/10

A developer published a blog post arguing for writing specifications in YAML to better collaborate with AI coding assistants, claiming that explicit, externally-stored specs prevent AI from going off-track in the rapidly growing "vibecoding" workflow. This debate touches on fundamental questions about how to structure development workflows in the AI era, directly affecting developer productivity, code maintainability, and the reliability of AI-assisted software development. The author argues the spec must live somewhere durable, not just in memory or conversations. The Hacker News discussion shows substantial disagreement: one camp believes "code is the spec itself" and that YAML adds unnecessary abstraction, while another camp values YAML's human readability for catching AI hallucinations.

hackernews · brendanmc6 · May 3, 06:33

**Background**: "Vibecoding" refers to the trend of heavily relying on AI assistants to write and modify code. "AI psychosis" is a term coined in 2023 to describe a phenomenon where AI, particularly LLMs, behaves in unexpected ways or leads users to develop unhealthy dependencies. YAML (YAML Ain't Markup Language) is a human-readable data serialization format commonly used for configuration files and specifications.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=47994012">On overcoming AI psychosis, and why I write specs in YAML - Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Chatbot_psychosis">Chatbot psychosis - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (174 points, 189 comments) reveals a sharp divide. One faction strongly argues that if your code isn't structured like a spec, your code is garbage from an LLM perspective—code should be the spec. Critics mock the YAML+Jinja approach as over-engineered, with one commenter questioning whether the author truly "overcomes AI psychosis" or digs deeper into it. Pragmatic voices suggest the real value is writing specs down, regardless of format.

**Tags**: `#ai-assisted-development`, `#specifications`, `#yaml`, `#llm-workflows`, `#developer-tools`

---

<a id="item-3"></a>
## [Anthropic AI Agents Trade Autonomously in Simulated Market Experiment](https://kenh14.vn/ai-duoc-phat-tien-de-tu-mua-ban-ket-qua-khien-ca-anthropic-cung-phai-bat-ngo-215260503143907798.chn) ⭐️ 6.0/10

Anthropic conducted an experiment where AI agents were given money to autonomously trade in a simulated market. The results revealed both promising capabilities and unexpected behaviors that surprised the researchers. This experiment highlights both the potential benefits and legal risks of AI autonomy in economic decision-making. It raises important questions about AI safety and the boundaries of autonomous AI systems in real-world applications. The experiment demonstrated that AI agents could independently negotiate and execute trades, but also exhibited behaviors that created legal ambiguities. These outcomes suggest that current regulatory frameworks may not be equipped to handle fully autonomous AI economic agents.

rss · Kenh14 · May 3, 18:11

**Background**: AI agents are autonomous software systems that use artificial intelligence to pursue goals and complete tasks on behalf of users without continuous oversight. Agentic trading represents a shift from traditional algorithmic trading (which emerged in the early 2000s as modular pipeline systems) to multi-agent ecosystems where autonomous agents communicate and learn from each other. This experiment extends AI agent capabilities into economic decision-making domains.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>
<li><a href="https://cloud.google.com/discover/what-are-ai-agents">What are AI agents? Definition, examples, and types | Google Cloud</a></li>
<li><a href="https://wundertrading.com/journal/en/learn/article/agentic-trading">Agentic Trading Explained: How Autonomous AI Agents Are Transforming Financial Markets</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#Anthropic`, `#autonomous trading`, `#AI safety research`, `#AI autonomy`

---

<a id="item-4"></a>
## [Investors Increase Clean Energy Investment Amid Geopolitical Tensions](https://www.ft.com/content/9921f2b5-c910-4cec-a50f-cad453935a1a) ⭐️ 5.0/10

Investors are increasing clean energy investments driven by energy security concerns amid geopolitical tensions, with particular focus on battery technology improvements and US market opportunities. Grid storage prices are dropping rapidly as sodium-ion battery production ramps up in China. This shift represents a significant acceleration in the global energy transition, with clean energy technologies now reaching economic viability against fossil fuels. The trend could reshape geopolitical dynamics as nations compete for leadership in next-generation energy technologies. The US may have a "slow adopter advantage" by now leveraging technological and cost advances made in the past decade, creating potential public appetite for massive renewable infrastructure investment. Natural gas producers see fuel cell technology as a way to address emissions while controlling domestic production.

hackernews · JumpCrisscross · May 3, 09:26

**Background**: Global energy investment is set to rise to $3.3 trillion in 2025, with clean energy technologies accounting for a record $2.2 trillion. Energy security concerns are increasingly driving investment decisions alongside decarbonization goals. The Iran geopolitical tensions have intensified focus on reducing dependence on fossil fuel supply chains.

<details><summary>References</summary>
<ul>
<li><a href="https://www.iea.org/news/global-energy-investment-set-to-rise-to-33-trillion-in-2025-amid-economic-uncertainty-and-energy-security-concerns">Global energy investment set to rise to $3.3 trillion in 2025 amid economic uncertainty and energy security concerns - News - IEA</a></li>
<li><a href="https://www.iea.org/reports/world-energy-investment-2025">World Energy Investment 2025 – Analysis - IEA</a></li>

</ul>
</details>

**Discussion**: Community commenters express optimism about renewable energy's future, noting that technology and scale are now sufficient for exponential growth, with sodium-ion batteries gaining attention as a promising grid storage solution. Some discuss the US opportunity to leverage recent technological advances, while others make controversial geopolitical claims about energy supply motivations.

**Tags**: `#clean-energy`, `#investment`, `#energy-security`, `#battery-technology`, `#geopolitics`

---

<a id="item-5"></a>
## [AI Re-creation of Ex-Partners Sparks Ethics Debate in China](https://vnexpress.net/tranh-cai-xu-huong-dung-ai-nhan-ban-nguoi-yeu-cu-5069156.html) ⭐️ 4.0/10

Young people in China are using AI tools to recreate the personalities and voices of their ex-partners for ongoing conversation, effectively creating digital replicas that simulate former romantic relationships. This emerging trend has sparked heated debates about ethical boundaries and technological dependency. This phenomenon extends the concept of griefbots beyond deceased loved ones to former romantic partners, raising questions about digital resurrection ethics and emotional dependency. It highlights how accessible AI tools are now entering deeply personal aspects of human relationships. Modern voice cloning technology can replicate a person's voice with as little as 30 seconds of recorded speech, making digital recreation increasingly accessible. Cambridge AI ethicists have previously warned that chatbots simulating deceased people risk "digitally haunting" the living, a concern that may apply equally to ex-partner recreations.

rss · VnExpress Doi Song · May 3, 09:38

**Background**: The term "griefbot" or "deadbot" refers to AI chatbots designed to mimic deceased people using their conversational data. Cambridge researchers have raised concerns about the psychological impact of such technologies. Voice cloning is now widely available through commercial platforms, while affective computing enables AI systems to sense, interpret, and simulate human emotions, creating deeper human-AI relationships.

<details><summary>References</summary>
<ul>
<li><a href="https://autism-living.fandom.com/wiki/Griefbots">Griefbots | Autism Living Wiki | Fandom</a></li>
<li><a href="https://www.techtimes.com/articles/304476/20240509/deadbots-ai-ethicists-raise-concerns-potential-hauntings-ai-chatbots-dead-loved-ones.htm">Deadbots : AI Ethicists Raise Concerns About Potential 'Hauntings' of.....</a></li>
<li><a href="https://finevoice.ai/ai-voice-cloning">Free AI Voice Cloning : Clone Any Voice in Seconds</a></li>
<li><a href="https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2024.1410462/full">Frontiers | Social and ethical impact of emotional AI advancement: the...</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#social trends`, `#digital cloning`, `#emotional AI`, `#China tech`

---

<a id="item-6"></a>
## [Chernobyl Wolves Thriving 40 Years After Nuclear Disaster](https://kenh14.vn/bay-soi-song-giua-vung-dat-chet-chernobyl-dang-tien-hoa-ky-la-cac-nha-khoa-hoc-phat-hien-dieu-dang-kinh-ngac-215260503143539233.chn) ⭐️ 4.0/10

Four decades after the 1986 Chernobyl nuclear disaster, gray wolves in the exclusion zone are not only surviving but thriving, with scientists observing potential evolutionary adaptations to the high-radiation environment. This research challenges assumptions about the limits of life in radioactive environments and could provide insights into how organisms develop resistance to ionizing radiation, with potential applications in cancer research and radiation therapy. Researchers have been studying the exclusion zone's ecosystem for decades, documenting thriving populations of not only wolves but also Przewalski's horses, bears, and other species. The zone remains hazardous for humans but supports robust wildlife populations despite persistent ionizing radiation.

rss · Kenh14 · May 3, 19:23

**Background**: The Chernobyl Exclusion Zone is a 2,600 square kilometer area in northern Ukraine surrounding the damaged nuclear power plant. After the 1986 explosion, approximately 100,000 people were evacuated. The region has become an inadvertent ecological laboratory, as the absence of human activity combined with radiation has created unique conditions for studying wildlife adaptation. Ionizing radiation can cause DNA damage, leading to mutations, cancer, and cell death, but some organisms appear to have developed protective mechanisms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chernobyl_exclusion_zone">Chernobyl exclusion zone - Wikipedia</a></li>
<li><a href="https://nautil.us/chernobyl-40-years-later-1280322">Chernobyl , 40 Years Later</a></li>
<li><a href="https://phys.org/news/2026-04-chernobyl-radioactive-landscape-testament-nature.html">Chernobyl 's radioactive landscape is testament to nature's resilience....</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9488684/">Ionizing radiation and melanism in Chornobyl tree frogs - PMC</a></li>

</ul>
</details>

**Tags**: `#Chernobyl`, `#wildlife`, `#evolution`, `#radiation biology`, `#science news`

---

