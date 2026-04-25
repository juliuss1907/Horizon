# Horizon Daily - 2026-04-25

> From 32 items, 5 important content pieces were selected

---

1. [Replace IBM Quantum back end with /dev/urandom](#item-1) ⭐️ 8.0/10
2. [New 10 GbE USB adapters are cooler, smaller, cheaper](#item-2) ⭐️ 6.0/10
3. [Turbo Vision 2.0 – a modern port](#item-3) ⭐️ 6.0/10
4. [OpenAI’s Sam Altman apologises over failure to report Canadian mass shooter](#item-4) ⭐️ 6.0/10
5. [This is who's developing Golden Dome's orbital interceptors—if they're ever built](#item-5) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Replace IBM Quantum back end with /dev/urandom](https://github.com/yuvadm/quantumslop/blob/25ad2e76ae58baa96f6219742459407db9dd17f5/URANDOM_DEMO.md) ⭐️ 8.0/10

Developer Yuval Adam demonstrated that recovering a 17-bit ECC key can be achieved using /dev/urandom instead of actual IBM Quantum hardware. The replacement still successfully recovered the key, revealing that small quantum benchmarks can be trivially matched by classical random number generation. This exposes a fundamental flaw in quantum computing benchmarks for small problems. When a problem is small enough, quantum computers can succeed for the wrong reasons, essentially imitating random number generators. This undermines the validity of such benchmarks for measuring actual quantum progress. A 17-bit key has only 131,072 possible values, making it trivially brute-forceable by classical computers. Project Eleven had awarded 1 BTC for this 'largest quantum attack on ECC to date,' but the demonstration proves the solution is purely classical and does not require quantum computation. When quantum circuits are too long for the hardware's error rate, the quantum computer essentially becomes a random number generator.

hackernews · pigeons · Apr 25, 00:58

**Background**: Elliptic Curve Cryptography (ECC) is a public-key encryption method based on the algebraic structure of elliptic curves over finite fields. Project Eleven is a quantum computing advocacy group that offered Bitcoin rewards for quantum attacks on ECC. This demonstration critiques the validation of quantum computing claims rather than quantum computing technology itself. Modern cryptographic keys typically use 256 bits or larger, providing security against both classical and quantum attacks, in stark contrast to the trivially small 17-bit key used in this benchmark.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Elliptic-curve_cryptography">Elliptic-curve cryptography - Wikipedia</a></li>
<li><a href="https://unix.stackexchange.com/questions/324209/when-to-use-dev-random-vs-dev-urandom">devices - When to use /dev/ random vs / dev / urandom - Unix & Linux...</a></li>

</ul>
</details>

**Discussion**: The community clarifies this is not an attack on quantum computing itself, but a critique of Project Eleven's validation practices. Strilanc references his April Fool's paper explaining that for small numbers, Shor's algorithm succeeds quickly when fed random samples, and when circuits are too long for the hardware's error rate, quantum computers effectively imitate random number generators. Commenters note that brute-forcing a 17-bit key is not challenging for classical computers, making this a validation failure rather than a quantum breakthrough.

**Tags**: `#quantum-computing`, `#cryptography`, `#benchmarking`, `#ecc`, `#ibm-quantum`

---

<a id="item-2"></a>
## [New 10 GbE USB adapters are cooler, smaller, cheaper](https://www.jeffgeerling.com/blog/2026/new-10-gbe-usb-adapters-cooler-smaller-cheaper/) ⭐️ 6.0/10

Jeff Geerling reviews new USB 10GbE ethernet adapters that offer improved thermal efficiency, reduced physical size, and lower prices compared to previous generations, enabling 10 gigabit per second wired networking over standard USB-C connections. These improvements make 10GbE networking more accessible for users seeking high-speed wired connections without expensive Thunderbolt docks or PCIe cards, particularly benefiting laptop users and compact workstation setups where thermal management and port density matter. Community members report mixed real-world performance, with one user noting a Xikestor 10G adapter with Realtek chipset underperformed their cheaper 5G alternative. Discussion also covers Framework expansion card alternatives, PoE++ power delivery possibilities (up to 100W), and Thunderbolt dock limitations where 2.5GbE remains common.

hackernews · calcifer · Apr 25, 05:56

**Background**: 10GbE (10 Gigabit Ethernet) represents a tenfold bandwidth increase over standard 1GbE, enabling faster file transfers, media production workflows, and network-attached storage access. USB-based 10GbE adapters provide a portable and relatively affordable alternative to Thunderbolt docks or PCIe network cards. Power over Ethernet (PoE) technology can deliver up to 100W via PoE++ standard, potentially enough to power laptops through compatible adapters.

<details><summary>References</summary>
<ul>
<li><a href="https://frame.work/marketplace/expansion-cards">Framework Marketplace | Expansion Cards</a></li>
<li><a href="https://en.wikipedia.org/wiki/Power_over_Ethernet">Power over Ethernet - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters discuss practical alternatives including Framework's announced 10GbE expansion card. Users debate PoE power delivery possibilities and note that Thunderbolt 4/5 docks often still have 2.5GbE limitations, with the premium CalDigit TS5 Plus being one of few 10GbE options at ~$500. One user recommends HP Thunderbolt 4 G4 refurb docks as affordable alternatives with good display outputs.

**Tags**: `#networking`, `#hardware`, `#usb`, `#ethernet`, `#10gbe`

---

<a id="item-3"></a>
## [Turbo Vision 2.0 – a modern port](https://github.com/magiblot/tvision) ⭐️ 6.0/10

Turbo Vision 2.0 has been released as a modern, cross-platform C++ port of Borland's classic 1990s text-mode UI framework, featuring full Unicode support and compatibility with code written over three decades ago. This release brings a piece of retro computing history back to life for modern developers, making it useful for building terminal applications with rich text-based user interfaces while preserving compatibility with legacy code. The port maintains the original architecture while adding Unicode support across Windows and other platforms. A .NET wrapper is actively being developed, enabling use from managed code on macOS. Community members note the build complexity (CMake) contrasts sharply with the original "hit F9 to compile" simplicity of Turbo Pascal.

hackernews · andsoitis · Apr 25, 04:18

**Background**: Turbo Vision was a character-mode text user interface framework included with Borland Pascal, Turbo Pascal, and Borland C++ around 1990. Borland itself used Turbo Vision to build the integrated development environments (IDEs) for these programming languages. The framework featured a distinctive bluish TUI aesthetic and an event-driven architecture that made it easy for developers to create text-based applications. Multiple ports of Turbo Vision exist today, including versions in Rust and Pascal.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Turbo_Vision">Turbo Vision - Wikipedia</a></li>
<li><a href="https://github.com/magiblot/tvision">GitHub - magiblot/tvision: A modern port of Turbo Vision 2.0, the classical framework for text-based user interfaces. Now cross-platform and with Unicode support. · GitHub</a></li>

</ul>
</details>

**Discussion**: Community response is overwhelmingly positive with strong nostalgic appreciation. Developers share stories of discovering Turbo Vision books in the '90s and falling in love with its bluish TUIs. A .NET wrapper developer reports magical experiences running Turbo Vision under .NET on macOS. However, some comments critique modern build complexity—CMake instructions versus the simple "hit F9" compilation of Turbo Pascal—as demonstrating "our incompetence" with modern tooling. Others note this is one of several existing Turbo Vision ports, including Rust and Pascal implementations.

**Tags**: `#retro-computing`, `#tui`, `#c++`, `#terminal-apps`, `#open-source`

---

<a id="item-4"></a>
## [OpenAI’s Sam Altman apologises over failure to report Canadian mass shooter](https://www.aljazeera.com/economy/2026/4/25/chkopenaissamaltmanapologises-over-failure-to-report-canadian-mass-shooter?traffic_source=rss) ⭐️ 6.0/10

OpenAI CEO Sam Altman publicly apologized after the company suspended a Canadian mass shooter's ChatGPT account before the attacks occurred but failed to notify law enforcement authorities about the potential threat. The incident has prompted scrutiny over AI companies' obligations when they detect dangerous user behavior on their platforms. This case raises critical questions about the responsibilities AI companies have when threat detection systems flag dangerous users. As AI platforms become increasingly ubiquitous, the incident highlights gaps in corporate safety protocols and legal frameworks governing how technology firms should respond when they identify potential mass violence threats. While OpenAI's systems successfully detected and suspended the individual's account prior to the attacks, the company did not escalate the information to law enforcement, a gap in their threat response protocol. According to corporate compliance research, companies face increasingly complex reporting obligations under evolving AI regulations, but clear guidelines for sharing threat information with authorities remain unclear.

rss · Al Jazeera · Apr 25, 02:07

**Background**: AI content monitoring systems use machine learning algorithms to identify potential threats, including violent content, hate speech, and indicators of planned attacks. Corporate reporting obligations for AI companies have become more complex as regulators worldwide implement new rules requiring disclosure of cybersecurity incidents and AI-related risks. However, existing legal frameworks often lack clear guidance on when companies should proactively notify law enforcement about detected threats versus merely terminating user access.

<details><summary>References</summary>
<ul>
<li><a href="https://www.corporatecomplianceinsights.com/data-authenticity-accountability-crucial-ai-age/">Data Authenticity & Accountability Crucial in the AI Age | Corporate Compliance Insights</a></li>
<li><a href="https://law-ai.org/balancing-safety-and-privacy-regulatory-models-for-ai-misuse/">Balancing Safety and Privacy: Regulatory Models for AI Misuse - Institute for Law & AI</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#corporate responsibility`, `#law enforcement`, `#AI policy`, `#accountability`

---

<a id="item-5"></a>
## [This is who's developing Golden Dome's orbital interceptors—if they're ever built](https://arstechnica.com/space/2026/04/this-is-whos-developing-golden-domes-orbital-interceptors-if-theyre-ever-built/) ⭐️ 6.0/10

Ars Technica报道了正在为金穹（Golden Dome）导弹防御计划开发天基拦截器的承包商名单，同时指出技术界对这些拦截器能否以可承受的成本实现规模化部署持怀疑态度。 如果无法实现可负担且可扩展的天基助推段拦截能力，整个金穹系统的战略价值将大打折扣，这将影响美国应对洲际弹道导弹威胁的国防战略。 助推段拦截是导弹防御中最难实现的方案，因为拦截器必须在导弹发动机工作的短短几分钟内进入攻击范围。据估计，仅应对液体燃料洲际弹道导弹就需要至少700枚大型轨道拦截器。

rss · Ars Technica · Apr 25, 02:52

**Background**: 金穹计划是特朗普总统于2025年1月签署行政命令后启动的多层导弹防御系统，旨在探测并摧毁弹道导弹、高超音速导弹和巡航导弹。该系统计划覆盖美国本土及军事设施，2027财年预算申请据报高达1.5万亿美元。助推段拦截是指在导弹发射后、发动机仍在工作阶段进行拦截，此时导弹飞行速度较慢、飞行高度较低，被认为是理论上最有效的拦截窗口，但实际部署面临极大的技术和成本挑战。

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Golden_Dome_(missile_defense_system)">Golden Dome (missile defense system) - Wikipedia</a></li>
<li><a href="https://www.axios.com/2026/04/22/trump-guetlein-golden-dome-interceptors">The ups and downs of Trump's Golden Dome gambit</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ballistic_missile_flight_phases">Ballistic missile flight phases - Wikipedia</a></li>
<li><a href="https://www.csis.org/analysis/boost-phase-missile-defense">Boost-Phase Missile Defense | CSIS</a></li>

</ul>
</details>

**Tags**: `#defense`, `#missile-defense`, `#space`, `#golden-dome`, `#policy`

---

