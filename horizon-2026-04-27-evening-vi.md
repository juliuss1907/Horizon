# Horizon Daily - 2026-04-27

> From 113 items, 8 important content pieces were selected

---

1. [Pgbackrest is no longer being maintained](#item-1) ⭐️ 8.0/10
2. [4TB of voice samples just stolen from 40k AI contractors at Mercor](#item-2) ⭐️ 8.0/10
3. [Show HN: OSS Agent I built topped the TerminalBench on Gemini-3-flash-preview](#item-3) ⭐️ 7.0/10
4. [Quarkdown – Markdown with Superpowers](#item-4) ⭐️ 6.0/10
5. [France's Mistral Built a $14B AI Empire by Not Being American](#item-5) ⭐️ 6.0/10
6. [Men Who Stare at Walls](#item-6) ⭐️ 5.0/10
7. [Is it true that … it’s harder for women to build muscle than men?](#item-7) ⭐️ 5.0/10
8. [Tin vui cho người đi xe điện](#item-8) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Pgbackrest is no longer being maintained](https://github.com/pgbackrest/pgbackrest) ⭐️ 8.0/10

The creator of pgBackRest announced the discontinuation of the widely-used PostgreSQL backup tool after 13 years of development, citing lack of sustainable financial support as the primary reason for ending the project. This discontinuation leaves the PostgreSQL community without a premier open-source backup solution, raising broader concerns about open source sustainability and the economics of maintaining critical infrastructure software without proper funding. pgBackRest was considered the premier backup solution for PostgreSQL, distinguished by its serious approach to restore validation alongside backup functionality. The maintainer cited years of late nights and weekends invested in the project, even with corporate sponsorship during certain periods.

hackernews · c0l0 · Apr 27, 10:56

**Background**: pgBackRest is a reliable backup and restore solution for PostgreSQL designed to scale to the largest databases and workloads. It offers features including incremental backups, parallel operations, and checksumming/validation. The project gained significant adoption in production environments due to its focus on data integrity and robust restore capabilities, differentiating itself from simpler backup approaches that only focus on taking backups without proper validation.

<details><summary>References</summary>
<ul>
<li><a href="https://pgbackrest.org/">pgBackRest - Reliable PostgreSQL Backup & Restore</a></li>
<li><a href="https://github.com/pgbackrest/pgbackrest">GitHub - pgbackrest/pgbackrest: Reliable PostgreSQL Backup & Restore · GitHub</a></li>

</ul>
</details>

**Discussion**: The community response mixed gratitude with concern about open source sustainability. Users praised pgBackRest as the premier PostgreSQL backup solution and thanked the maintainer for 13 years of work, while some noted the irony of companies relying on free infrastructure tools without supporting their creators. Others suggested a for-profit company could step in to maintain the project given its commercial value.

**Tags**: `#postgresql`, `#open-source-sustainability`, `#pgbackrest`, `#backup-recovery`, `#maintainer-burnout`

---

<a id="item-2"></a>
## [4TB of voice samples just stolen from 40k AI contractors at Mercor](https://app.oravys.com/blog/mercor-breach-2026) ⭐️ 8.0/10

A 4TB breach at AI contractor platform Mercor exposed voice samples paired with ID documents from 40k contractors, creating a comprehensive deepfake toolkit for banking voiceprint bypass, video impersonation, and insurance fraud.

hackernews · Oravys · Apr 27, 09:57

**Tags**: `#data-breach`, `#deepfake`, `#voice-spoofing`, `#ai-security`, `#privacy`

---

<a id="item-3"></a>
## [Show HN: OSS Agent I built topped the TerminalBench on Gemini-3-flash-preview](https://github.com/dirac-run/dirac) ⭐️ 7.0/10

Dirac, an open-source coding agent built by dirac-run, achieved 65.2% on TerminalBench 2.0, outperforming Google's official result of 47.8% and the closed-source Junie CLI's 64.3%. The agent employs Hash-Anchored edits, AST-based context fetching, and batched operations to achieve this benchmark score. This result demonstrates that an entirely open-source agent can outperform both Google's official benchmark and a major closed-source competitor. The novel techniques introduced—Hash-Anchored edits, AST-based context selection, and batched operations—offer a new architectural approach that other developers can study and build upon. Hash-Anchored edits use content hashes in LINE#ID format to ensure agents reference the exact version of code they read, eliminating edit failures caused by stale line numbers. AST-based context fetching leverages the language's abstract syntax tree to select relevant code snippets, completely avoiding large file reads. The developer has clarified the agent ran in fully leaderboard-compliant mode with no agents/skills.md files or resource modifications.

hackernews · GodelNumbering · Apr 27, 12:35

**Background**: TerminalBench is a benchmark that tests whether AI agents can interact with a real shell environment to complete concrete tasks, ranging from compiling code repositories and training ML models to setting up servers and debugging system configurations. Hash-Anchored edits represent a technique to prevent code editing failures by using content hashes instead of line numbers as references. AST-based context fetching uses the abstract syntax tree structure of code to enable semantic navigation and selective context retrieval, which is particularly useful for large codebases where reading entire files would exceed context window limits.

<details><summary>References</summary>
<ul>
<li><a href="https://mcpbr.org/terminalbench">TerminalBench : Shell & Terminal Task Evaluation for AI Agents</a></li>
<li><a href="https://deepwiki.com/code-yeongyu/oh-my-opencode/9.3-hash-anchored-edit-system">Hash-Anchored Edit System | code-yeongyu/oh-my-opencode | DeepWiki</a></li>
<li><a href="https://github.com/can1357/oh-my-pi">GitHub - can1357/oh-my-pi: ⌥ AI Coding agent for the terminal — hash-anchored edits, optimized tool harness, LSP, Python, browser, subagents, and more</a></li>

</ul>
</details>

**Discussion**: Community members are curious about comparing Dirac to existing tools like pi.dev for day-to-day coding tasks outside benchmarks. One commenter noted that static analysis in tools like Claude Code can be frustrating when it triggers mid-edit, and questioned whether this has been an issue for Dirac. Another asked whether the project builds on top of Cline and retains features like plan and act modes. There's also interest in understanding why a new harness was built rather than implementing these techniques as extensions in pi.

**Tags**: `#ai-agents`, `#open-source`, `#coding-assistants`, `#benchmarking`, `#llm-tools`

---

<a id="item-4"></a>
## [Quarkdown – Markdown with Superpowers](https://quarkdown.com/) ⭐️ 6.0/10

Quarkdown, a new markup language that extends CommonMark and GitHub Flavored Markdown (GFM) with programmable features similar to LaTeX, has been officially released. The tool allows a single project to compile into multiple output formats including print-ready books, academic papers, knowledge bases, and interactive presentations. As LaTeX's complexity drives users toward alternatives, Quarkdown enters a competitive landscape alongside Typst and Quarto. Its approach of extending familiar Markdown syntax rather than inventing entirely new syntax could lower the learning curve for technical writers seeking programmable document generation without full LaTeX complexity. Quarkdown builds on existing Markdown standards, meaning users only need to learn the new programmable extensions rather than entire syntax. Community members have raised concerns about whether Quarkdown has an appropriate evaluation model for iterative text layout, noting that Typst uses a 'context' concept for handling layout passes that adjust document formatting recursively.

hackernews · amai · Apr 27, 08:54

**Background**: Markdown is a lightweight markup language originally designed for web writing, using simple syntax to format text. LaTeX, widely used in academia, offers programmable document generation through macros and packages but has a steep learning curve. Typst emerged as a modern LaTeX alternative with built-in scripting and fast incremental compilation. Quarto and Pandoc serve as document conversion tools that process Markdown into various output formats using the Pandoc Markdown dialect. These tools represent a fragmented ecosystem where users must choose between simplicity (standard Markdown), power (LaTeX), or modern alternatives (Typst, Quarto).

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/iamgio/quarkdown">GitHub - iamgio/quarkdown: Markdown with superpowers: from ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Typst">Typst - Wikipedia</a></li>
<li><a href="https://typst.app/docs/">Typst Documentation</a></li>

</ul>
</details>

**Discussion**: The community discussion reveals a fragmented ecosystem where users compare Quarkdown against Typst, Quarto, Pandoc, and MyST. While some appreciate Quarkdown's approach of extending Markdown rather than creating new syntax, others argue this defeats Markdown's purpose of simplicity. Technical concerns have emerged about evaluation models for layout iteration, with one commenter noting they switched from pandoc/md/LaTeX to Typst for better handling of document layout passes. There is also interest in practical features like CV formatting with version control capabilities.

**Tags**: `#markdown`, `#markup-languages`, `#documentation-tools`, `#technical-writing`, `#latex-alternatives`

---

<a id="item-5"></a>
## [France's Mistral Built a $14B AI Empire by Not Being American](https://www.forbes.com/sites/iainmartin/2026/04/16/how-frances-mistral-built-a-14-billion-ai-empire-by-not-being-american/) ⭐️ 6.0/10

French AI company Mistral has achieved a $14 billion valuation by positioning itself as a European-hosted alternative to American AI providers, capitalizing on EU data sovereignty requirements and compliance needs. This valuation signals growing demand for region-specific AI infrastructure where data residency is mandatory, potentially reshaping how multinational companies evaluate AI vendor relationships across the Atlantic. Mistral was founded in April 2023 by former researchers from Google DeepMind and Meta, and currently relies on Nvidia chips for training despite its European identity. The company offers both open-weight and proprietary models including the Le Chat assistant.

hackernews · rzk · Apr 27, 10:14

**Background**: EU data sovereignty regulations, particularly GDPR since 2018, establish strict controls over data residency and cross-border transfers. The EU's recent SEAL-2 certification requires cloud providers to abide by EU laws without requiring additional customer technical measures. For many European businesses, routing API requests through US-based endpoints is no longer acceptable, especially for privacy-sensitive data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mistral_AI">Mistral AI - Wikipedia</a></li>
<li><a href="https://commission.europa.eu/news-and-media/news/commission-advances-cloud-sovereignty-through-strategic-procurement-2026-04-17_en">Commission advances cloud sovereignty through strategic procurement</a></li>

</ul>
</details>

**Discussion**: Community commenters debate whether Mistral's positioning is sustainable long-term. Supporters argue EU-based hosting is non-negotiable for business customers handling sensitive data, where 'pinky swearing' from OpenAI doesn't provide hard guarantees. Skeptics counter that Mistral still depends on American Nvidia chips, and if geopolitical separation occurs, reliance on any American technology becomes untenable. One commenter notes $14B is 'table stakes' in AI, while others report positive experiences with Mistral's Le Chat Pro offering.

**Tags**: `#Mistral AI`, `#European AI`, `#AI industry`, `#data sovereignty`, `#AI business strategy`

---

<a id="item-6"></a>
## [Men Who Stare at Walls](https://www.alexselimov.com/posts/men_who_stare_at_walls/) ⭐️ 5.0/10

A personal blog post titled 'Men Who Stare at Walls' explores wall-staring as a low-barrier mental break technique, suggesting that simply looking at a blank wall can provide cognitive rest without requiring special equipment, natural surroundings, or formal training. This discussion highlights a critical accessibility gap in wellness culture—many people cannot easily access parks or nature during breaks due to urban living conditions or long commutes. The post generated significant engagement on Hacker News (98 points, 50 comments), revealing strong community interest in practical mental well-being techniques that work regardless of one's environment. The blog post describes wall-staring as a 'rest' state where the mind can recover from information overload. Unlike traditional meditation, it doesn't require any special technique—just looking at a wall and allowing thoughts to settle naturally.

hackernews · aselimov3 · Apr 27, 11:08

**Background**: Wellness and mindfulness culture often promote nature-based practices like forest bathing, park walks, or outdoor meditation. However, this assumes accessibility to green spaces—something not available to many urban workers, shift laborers, or those in densely populated metropolitan areas with limited public parks. Wall-staring represents an alternative that democratizes mental health practices by removing environmental prerequisites.

**Discussion**: The Hacker News discussion revealed a clear split in perspectives. Some commenters drew parallels to meditation, arguing that wall-staring essentially serves the same purpose of quiet mental rest. Others advocated for nature-based alternatives like walks, but faced strong pushback from users pointing out accessibility issues—many people commute 1.5 hours to work in urban areas without parks or fresh air. Several commenters shared personal experiences of 'staring into the distance' or zoning out to solve difficult problems, supporting the technique's validity.

**Tags**: `#productivity`, `#mental-health`, `#meditation`, `#mindfulness`, `#self-care`

---

<a id="item-7"></a>
## [Is it true that … it’s harder for women to build muscle than men?](https://www.theguardian.com/lifeandstyle/2026/apr/27/is-it-true-harder-women-build-muscle-than-men-resistance-training) ⭐️ 5.0/10

A Guardian article featuring Prof Leigh Breen from the University of Leicester explains that while men typically have higher muscle-to-fat ratios due to testosterone differences established during puberty, women respond just as well to resistance training when measuring relative percentage change in muscle mass. This challenges a widespread fitness myth and can help women approach strength training with greater confidence, potentially improving public health outcomes by encouraging more inclusive participation in resistance training. Women have approximately 15-20 times lower testosterone levels than men. Despite this, research shows both sexes experience similar percentage increases in muscle mass from resistance training. Androgen receptors in muscle tissue, which bind testosterone, do not significantly limit women's muscle-building potential.

rss · The Guardian Life · Apr 27, 07:00

**Background**: Muscle growth from resistance training involves muscle protein synthesis, stimulated by mechanical tension and metabolic stress. Testosterone is an anabolic hormone that influences muscle protein synthesis, and men produce substantially more of it naturally. The distribution of androgen receptors in muscle tissue also differs between sexes. Understanding these physiological mechanisms helps explain why relative training adaptations can be similar despite baseline hormonal differences.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Androgen">Androgen - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC4810760/">Androgen Receptor Structure, Function and Biology: From Bench to...</a></li>

</ul>
</details>

**Tags**: `#fitness`, `#muscle building`, `#gender differences`, `#resistance training`, `#health science`

---

<a id="item-8"></a>
## [Tin vui cho người đi xe điện](https://kenh14.vn/tin-vui-cho-nguoi-di-xe-dien-215260427173944695.chn) ⭐️ 4.0/10

A new report analyzing over 1 billion real-world miles of driving data reveals that modern electric vehicles experience minimal range degradation after years of use, challenging common concerns about battery longevity. This finding addresses one of the primary barriers to EV adoption by demonstrating that battery degradation fears may be overstated. For consumers and fleet operators, this data supports the long-term economic viability of electric vehicles. The research, conducted by Recurrent Auto, tracked thousands of EVs including popular models like the Hyundai Ioniq 5 and Ford Mustang Mach-E. Separate studies from the same researchers found that DC fast charging does not accelerate battery degradation compared to slower charging methods.

rss · Kenh14 · Apr 27, 18:00

**Background**: Battery degradation in lithium-ion batteries occurs through mechanisms including solid-electrolyte interphase growth, lithium plating, and transition metal dissolution. These processes gradually reduce battery capacity over charge cycles. Recurrent Auto monitors EV battery health by comparing manufacturer-reported range estimates against real-world performance data collected from connected vehicles.

<details><summary>References</summary>
<ul>
<li><a href="https://www.greencars.com/expert-insights/research-shows-ev-battery-replacements-very-rare">Research Shows EV Battery Replacements Very Rare | GreenCars</a></li>
<li><a href="https://www.linkedin.com/pulse/new-study-shows-fast-charging-wont-harm-your-ev-battery-6c4ge">New Study Shows Fast Charging Won't Harm Your EV Battery</a></li>

</ul>
</details>

**Tags**: `#electric-vehicles`, `#battery-technology`, `#ev-range`, `#clean-energy`, `#consumer-tech`

---

