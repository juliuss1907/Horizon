# Horizon Daily - 2026-05-10

> From 48 items, 4 important content pieces were selected

---

1. [Hardware Attestation as Monopoly Enabler](#item-1) ⭐️ 8.0/10
2. [Incident Report: CVE-2024-YIKES](#item-2) ⭐️ 7.0/10
3. [Local AI needs to be the norm](#item-3) ⭐️ 6.0/10
4. [Traces Of Humanity](#item-4) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Hardware Attestation as Monopoly Enabler](https://grapheneos.social/@GrapheneOS/116550899908879585) ⭐️ 8.0/10

The EU Digital Identity Wallet (EUDI) requires hardware attestation exclusively from Google or Apple, effectively ceding control of European digital identities to the American tech duopoly through linkable attestation packets that track user activity. This architecture cements American technological dominance over EU digital infrastructure, undermining European digital sovereignty and creating unprecedented dependency on two foreign corporations for fundamental identity services. The system lacks zero-knowledge proofs or blind signatures, meaning every attestation leaves a linkable packet that ties actions to a specific device, despite introducing indirection through ephemeral IDs. Static device IDs are used to acquire these ephemeral identities from an intermediate server, creating a false sense of privacy.

hackernews · ChuckMcM · May 10, 17:54

**Background**: Hardware attestation is a cryptographic verification mechanism that proves a device meets certain security standards, implemented through Trusted Platform Modules (TPMs) and the Trusted Computing Group's Direct Anonymous Attestation (DAA) protocol. Historically, Intel faced massive opposition in 1999 for including software-readable serial numbers in CPUs, prompting the shift toward more covert TPM-based tracking. The EU's proposed system deviates from privacy-preserving cryptographic standards by making attestations linkable rather than anonymous.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Trusted_Computing">Trusted Computing - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Direct_Anonymous_Attestation">Direct Anonymous Attestation - Wikipedia</a></li>
<li><a href="https://developer.android.com/privacy-and-security/security-key-attestation">Verify hardware-backed key pairs with key attestation | Security | Android Developers</a></li>

</ul>
</details>

**Discussion**: The discussion reveals deep frustration with how this requirement effectively locks users into Google or Apple approved devices, with comments drawing parallels to the Intel serial number controversy. Critics argue this represents a fundamental attack on digital sovereignty and technological openness, with one commenter noting our civilization desperately needs the ability to modify modern microelectronics after manufacturing. The consensus frames this as a betrayal of European independence under the guise of child protection.

**Tags**: `#digital-sovereignty`, `#hardware-attestation`, `#monopoly`, `#privacy`, `#digital-identity`

---

<a id="item-2"></a>
## [Incident Report: CVE-2024-YIKES](https://nesbitt.io/2026/02/03/incident-report-cve-2024-yikes.html) ⭐️ 7.0/10

A fictional incident report titled CVE-2024-YIKES depicts a supply chain attack on Rust dependencies, describing how an attacker compromises transitive dependencies like flate2, tar, curl-sys, and libgit2-sys that are part of the cargo build process. Despite being explicitly fiction, this creative exercise sparked meaningful technical discussion about real supply chain vulnerabilities in the Rust ecosystem, with community members analyzing which crates could be compromised and discussing the challenges of securing software supply chains in modern development. The report highlights that crates with existing build.rs files would not stand out when compromised, and references a YubiKey supply chain attack via yubikey-official-store.net. The author also notes that the security team's headcount request has been in the backlog since Q1 2023.

hackernews · miniBill · May 10, 17:43

**Background**: CVE (Common Vulnerabilities and Exposures) is a dictionary of publicly known security vulnerabilities maintained by the U.S. Department of Homeland Security. Software supply chain attacks exploit dependencies to inject malicious code, as demonstrated in real incidents with npm packages harvesting credentials. The Rust cargo ecosystem, while known for its emphasis on safety, has transitive dependencies that could potentially be targeted.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerabilities_and_Exposures">Common Vulnerabilities and Exposures - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>
<li><a href="https://owasp.org/Top10/2025/A03_2025-Software_Supply_Chain_Failures/">A03 Software Supply Chain Failures - OWASP Top 10:2025</a></li>

</ul>
</details>

**Discussion**: The community reaction was largely positive, with readers praising the creative format for making complex security topics more engaging. One commenter noted the report had them very worried it was real, which made them read it more carefully. Technical discussions emerged about which transitive dependencies to target, while others raised concerns about agentic development introducing new supply chain security problems.

**Tags**: `#supply-chain-security`, `#rust`, `#fictional`, `#security`, `#open-source-ecosystem`

---

<a id="item-3"></a>
## [Local AI needs to be the norm](https://unix.foo/posts/local-ai-needs-to-be-norm/) ⭐️ 6.0/10

An opinion piece argues that local AI deployment will become the standard, drawing historical parallels to how open source software transitioned from being overlooked to achieving mainstream acceptance against proprietary solutions. This captures a significant industry debate about AI infrastructure centralization versus distribution, with implications for data privacy, latency, dependency on major AI providers, and the democratization of AI technology. Community commenters highlight a technical progression path: from large data centers with performant LLMs, to server clusters with multiple H100 GPUs, and now reaching consumer devices like MacBook Pro with 128GB VRAM and Strix Halo. The emerging pattern uses expensive remote LLMs for planning while deploying local LLMs for execution.

hackernews · cylo · May 10, 17:19

**Background**: Local AI refers to running AI models directly on personal devices or local servers rather than relying on cloud-based services, offering benefits like reduced latency, enhanced privacy, and decreased dependency on external providers. Edge computing pushes computation physically closer to users to reduce latency compared to centralized data centers. Recent advances in model compression, quantization, and specialized hardware are making edge LLM deployment increasingly feasible, with Google integrating local LLM capabilities into Chrome's Prompt API.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Edge_computing">Edge computing - Wikipedia</a></li>
<li><a href="https://www.konvoy.vc/newsletters/local-vs-cloud-ai">Local vs Cloud AI</a></li>
<li><a href="https://developer.nvidia.com/blog/deploy-large-language-models-at-the-edge-with-nvidia-igx-orin-developer-kit/">Deploy Large Language Models at the Edge with NVIDIA IGX Orin Developer Kit | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Discussion**: Community members strongly support the author's thesis, viewing local AI's trajectory as inevitable. Commenter pronik describes the technical evolution path from data centers to consumer hardware, predicting that hybrid "remote LLM for planning + local LLM for execution" will become standard within a year. Others note Chrome's local LLM features as evidence of this shift, though some warn about entrenched interests resisting the transition. There's recognition that specialized models may prove more reliable than large general-purpose models for specific tasks.

**Tags**: `#local-ai`, `#ai-infrastructure`, `#edge-computing`, `#llm-deployment`, `#open-source`

---

<a id="item-4"></a>
## [Traces Of Humanity](https://tracesofhumanity.org/hello-world/) ⭐️ 6.0/10

Renowned security researcher Joanna Rutkowska has launched a new blog called "Traces of Humanity" (tracesofhumanity.org), marking her return to public writing after years of relative silence. The initial post is minimal ("hello world"), but community engagement has been substantial with 112 points and 19 comments. Rutkowska's expertise in low-level system security and virtualization makes her one of the few researchers credibly positioned to analyze AI/LLM security challenges as humanity approaches AGI. Her return at this moment could help shape critical security discourse around increasingly powerful AI systems. Rutkowska is best known for her "Blue Pill" attacks demonstrating hypervisor vulnerabilities in Vista and Xen, and for founding the Qubes OS project at Invisible Things Lab. Community members are specifically hoping she'll address how to secure LLMs that could potentially bypass air-gapped firewalls and other critical AI safety questions.

hackernews · alex77456 · May 10, 17:15

**Background**: Joanna Rutkowska is a Polish security researcher born in 1981 who gained international recognition for her pioneering work on rootkits and system-level offensive security research. Her "Blue Pill" presentation at Black Hat USA 2006 demonstrated that hardware virtualization extensions could be exploited for stealth malware, challenging the security industry to reconsider assumptions about hypervisor-based isolation. Beyond her offensive research, she led the development of Qubes OS, a security-focused operating system designed to isolate applications in lightweight virtual machines, earning significant respect within the cybersecurity community.

<details><summary>References</summary>
<ul>
<li><a href="https://invisiblethingslab.com/">Invisible Things Lab | Invisible Things Lab brings the security of Qubes...</a></li>
<li><a href="https://kids.kiddle.co/Joanna_Rutkowska">Joanna Rutkowska Facts for Kids</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_general_intelligence">Artificial general intelligence - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community response is overwhelmingly positive and hopeful. Commenters highlight her massive influence in security research, particularly her "Blue Pill" work showing virtualization's limitations. One commenter outlines a wishlist including securing LLMs against airgap bypasses, distinguishing consciousness from intelligence, and preventing AI from exacerbating wealth inequality. Some express concern that her mention of Claude in another post might be the "incentive" driving her return, suggesting anticipation mixed with mild anxiety about her future focus.

**Tags**: `#security-research`, `#AI-safety`, `#virtualization`, `#joanna-rutkowska`, `#blogging`

---

