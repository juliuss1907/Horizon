# Horizon Daily - 2026-04-26

> From 90 items, 6 important content pieces were selected

---

1. [Asahi Linux Progress Linux 7.0](#item-1) ⭐️ 7.0/10
2. [The West forgot how to make things, now it’s forgetting how to code](#item-2) ⭐️ 7.0/10
3. [Musk and Altman’s bitter feud over OpenAI to be laid bare in court](#item-3) ⭐️ 7.0/10
4. [Statecharts: hierarchical state machines](#item-4) ⭐️ 6.0/10
5. [Cannes AI film festival raises eyebrows – and questions about future](#item-5) ⭐️ 5.0/10
6. [Hồ sơ nghi phạm nổ súng tại bữa tiệc báo chí Nhà Trắng](#item-6) ⭐️ 5.0/10

---

<a id="item-1"></a>
## [Asahi Linux Progress Linux 7.0](https://asahilinux.org/2026/04/progress-report-7-0/) ⭐️ 7.0/10

Asahi Linux released Progress Report 7.0, detailing continued development of Linux support for Apple Silicon hardware. The report highlights audio driver work, including discussions about CS42L84 and CS42L42 codec compatibility, while community members express interest in Mac-like distribution experiences. This progress report demonstrates steady advancement in bringing Linux to Apple Silicon Macs without official Apple support. The work enables users to run Linux on hardware that was previously locked to macOS, expanding choice for developers and enthusiasts on ARM-based systems. The community discussion reveals technical insights about audio codec differences between CS42L84 and CS42L42 chips, with users proposing cross-chip sample rate value sharing. One commenter suggests creating an Asahi Remix spin with Mac-like UX defaults including cmd-based modifiers and gesture support.

hackernews · elisaado · Apr 26, 10:50

**Background**: Asahi Linux is a community project led by Hector Martin that ports Linux to Apple Silicon Macs by reverse-engineering the proprietary SoCs, since Apple provides no official documentation. The project has produced Fedora Asahi Remix as its flagship distribution, serving both as an end-user OS and a reference for other distributions. Apple Silicon uses ARM64 architecture, which requires specialized kernel support distinct from traditional x86_64 systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asahi_Linux">Asahi Linux - Wikipedia</a></li>
<li><a href="https://asahilinux.org/about/">About - Asahi Linux</a></li>

</ul>
</details>

**Discussion**: Community members show appreciation for the project's consistent breakthroughs and professional approach. Technical discussions focus on solving audio codec challenges, with one commenter suggesting cross-referencing datasheet values between CS42L84 and CS42L42 chips. Some express philosophical concerns about Apple's lack of openness, while others propose Mac-like UX customizations as a potential spin-off direction.

**Tags**: `#asahi-linux`, `#apple-silicon`, `#linux-on-mac`, `#open-source`, `#hardware-drivers`

---

<a id="item-2"></a>
## [The West forgot how to make things, now it’s forgetting how to code](https://techtrenches.dev/p/the-west-forgot-how-to-make-things) ⭐️ 7.0/10

一篇观点文章指出西方国家正在经历编程能力的衰退，类似于他们历史上失去制造业专业知识的过程，而人工智能编程助手如GitHub Copilot可能正在加速这一趋势。该文引发了开发者社区的激烈讨论，评论者从管理实践、个人责任和文章本身的人工智能生成性质等角度提供了多维度的观点。 这篇分析触及了软件工程行业的核心担忧：如果开发者过度依赖人工智能工具，可能会失去对底层原理的理解和手动编码能力。前特斯拉人工智能主管Andrej Karpathy已观察到手动编码技能的"萎缩"现象，称自己现在"主要用英语编程"，这表明即使是顶尖工程师也面临技能退化风险。 评论者指出了人工智能代码生成器的关键问题：它们产生自信且看似合理但实际部分错误的代码，使人类需要费力找出错误。缺乏手动编程经验意味着开发者无法识别人工智能输出中的错误，因为没有基准来判断什么是正确的。前OpenAI工程师Karpathy将这种人工智能辅助编程方式称为"vibe coding"。

hackernews · milkglass · Apr 26, 06:24

**Background**: GitHub Copilot是由GitHub和OpenAI开发的AI编程助手，集成在Visual Studio Code、Visual Studio、JetBrains IDE等主流开发环境中，通过自动补全代码帮助开发者更快地编写程序。技能萎缩（skill atrophy）指的是由于缺乏练习或使用，专业技能随时间退化的现象。Andrej Karpathy是著名的人工智能研究人员，曾在特斯拉领导自动驾驶项目，现为AI初创公司xAI的联合创始人，他最近公开谈论了人工智能编码工具对手动编程技能的影响。

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GitHub_Copilot">GitHub Copilot - Wikipedia</a></li>
<li><a href="https://www.businessinsider.com/andrej-karpathy-claude-code-manual-skills-atrophy-software-engineering-tesla-2026-1">Ex-Tesla AI Boss Notices ' Atrophy ' of Manual Coding Skills As AI Gains</a></li>

</ul>
</details>

**Discussion**: 社区讨论呈现出多个层次的批评：首先，管理层通过削减人员配置和组织冗余来追求短期利润，导致隐性知识无法传承，资深工程师没有余力教导新人；其次，有开发者选择主动抵抗人工智能依赖，坚持不借助编程助手来完成日常工作，以保持对底层技能的掌握；最后，一位评论者尖锐地指出，这篇讨论人工智能取代编程技能的文章本身明显是由人工智能生成的，充满了不自然的表达和"LLM腔"，讽刺地证明了写作能力同样会萎缩，建议不如直接阅读人工智能翻译版本。

**Tags**: `#skill-atrophy`, `#AI-development-tools`, `#knowledge-transfer`, `#software-industry-criticism`, `#engineering-culture`

---

<a id="item-3"></a>
## [Musk and Altman’s bitter feud over OpenAI to be laid bare in court](https://www.theguardian.com/technology/2026/apr/26/musk-altman-openai-court) ⭐️ 7.0/10

Elon Musk's lawsuit against Sam Altman and OpenAI begins its trial this week in Oakland, California, with the case focusing on whether OpenAI violated its original nonprofit founding agreement when it transitioned to a for-profit structure. The 2024 lawsuit alleges breach of fiduciary duty and breach of contract related to OpenAI's 2019 creation of a for-profit subsidiary and its subsequent restructuring. The trial outcome could set significant legal precedents for AI governance, corporate responsibility, and how technology companies balance profit motives with public benefit missions. If Musk prevails, it could force restructuring at OpenAI and other AI labs, fundamentally reshaping the industry's approach to nonprofit-to-profit transitions. The lawsuit claims Altman breached OpenAI's founding charter by pivoting toward commercializing technology for Microsoft's benefit rather than humanity's benefit as originally stated. Internal communications, board decisions, and the terms of Microsoft's multi-billion dollar investment are expected to be examined during the trial, with the court set to reveal details previously hidden behind settlement negotiations.

rss · The Guardian Life · Apr 26, 10:00

**Background**: OpenAI was founded in 2015 by Musk, Altman, Greg Brockman, and others as a nonprofit research laboratory with the stated mission of ensuring artificial general intelligence (AGI) benefits all of humanity. In 2019, OpenAI created a for-profit subsidiary structured as a limited liability company under the nonprofit parent, a move made necessary to attract the massive capital investments required for competitive AI development. The organization has since evolved to include a Public Benefit Corporation (PBC) structure, similar to those used by competitors Anthropic and x.ai.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI">OpenAI - Wikipedia</a></li>
<li><a href="https://openai.com/index/evolving-our-structure/">Evolving OpenAI ’s structure | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI">OpenAI - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#OpenAI`, `#Legal/Regulation`, `#Elon Musk`, `#Tech Industry`

---

<a id="item-4"></a>
## [Statecharts: hierarchical state machines](https://statecharts.dev/) ⭐️ 6.0/10

A comprehensive introduction to Statecharts (hierarchical state machines) has been published at statecharts.dev, featuring community discussion where XState creator David Khourshid shares that statecharts are most valuable when treated as executable behavior rather than documentation. Statecharts provide a formal way to model complex UI state and asynchronous behaviors, which remains a significant challenge in modern frontend development. Their hierarchical nature allows developers to organize state logic in a more maintainable way, though adoption in the frontend ecosystem has remained limited despite their proven utility in safety-critical industries. Key points include the tension between treating statecharts as executable behavior versus documentation, the difficulty of retrofitting them into existing codebases, and their established role in automotive software through tools like MATLAB/Simulink. The creator emphasizes that statecharts don't need to model everything—just where they provide the most value.

hackernews · sph · Apr 26, 09:32

**Background**: Statecharts were introduced by David Harel in 1987 as an extension of traditional finite state machines, adding hierarchical nesting of states, orthogonal (parallel) regions, and state actions like entry/exit behaviors. UML standardized a variant called UML state machines, combining characteristics of both Mealy machines (event-driven actions) and Moore machines (state-based actions). This formalism helps developers reason about complex systems where entities are always in exactly one of several possible states with well-defined conditional transitions between them.

<details><summary>References</summary>
<ul>
<li><a href="https://statecharts.dev/">Welcome to the world of Statecharts - Statecharts</a></li>
<li><a href="https://en.wikipedia.org/wiki/UML_state_machine">UML state machine - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments reveal mixed real-world experiences: while some developers find state machines invaluable for managing complex UI interactions and CSS transitions, others struggled with retrofitting XState into existing Vue/React codebases due to boundary issues between the statechart and the rest of the system. The creator himself acknowledges you don't need to use them everywhere. One commenter noted that while Statecharts once seemed to be gaining traction in the frontend ecosystem, that momentum eventually faded, though the automotive industry has long relied on them through tools like MATLAB/Simulink.

**Tags**: `#state-machines`, `#statecharts`, `#xstate`, `#frontend-development`, `#software-architecture`

---

<a id="item-5"></a>
## [Cannes AI film festival raises eyebrows – and questions about future](https://www.theguardian.com/technology/2026/apr/26/cannes-ai-film-festival-raises-eyebrows-questions-future) ⭐️ 5.0/10

The World AI Film Festival (WAIFF) held its debut edition at Cannes this week, featuring AI-generated films depicting surreal imagery like men with fish scales and armies sweeping battlefields, just as the main Cannes Film Festival banned AI from its Palme d'Or competition on the grounds that 'AI imitates very well but it will never feel deep emotions'. The WAIFF represents a significant cultural and industry moment, as Hollywood studios and big-tech companies like Google France are increasingly investing in AI filmmaking tools, creating a schism between traditional cinema institutions and the emerging AI creative movement that claims a 'nouvelle vague' is coming. The second WAIFF showcased films, shorts, advertising, and micro-series created using at least three generative AI tools, with entries from international satellite festivals in Japan, Korea, China, and Brazil. Google France's Gen AI Lead Johann Choron appeared as a speaker, supporting studios and producers in integrating generative AI from ideation to production.

rss · The Guardian Life · Apr 26, 06:00

**Background**: The Cannes Film Festival, entering its 76th year, is the world's most prestigious film competition, awarding the Palme d'Or to outstanding works. Traditional film festivals have generally banned or restricted AI-generated content from competition categories, citing concerns about authenticity and the human creative element. Meanwhile, AI filmmaking tools powered by platforms like Runway, Flux, Kling, and Luma have advanced rapidly, enabling creators to generate images, videos, and assets from text prompts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.screendaily.com/news/seven-talking-points-from-the-world-ai-film-festival-in-cannes/5215914.article">Seven talking points from the World AI Film Festival in Cannes</a></li>
<li><a href="https://worldaifilmfestival.com/">ACCUEIL 2026 - WAIFF</a></li>
<li><a href="https://melies.co/">Melies - AI Filmmaking Tools</a></li>

</ul>
</details>

**Tags**: `#AI-generated content`, `#film industry`, `#creative AI`, `#Cannes`, `#generative media`

---

<a id="item-6"></a>
## [Hồ sơ nghi phạm nổ súng tại bữa tiệc báo chí Nhà Trắng](https://kenh14.vn/ho-so-nghi-pham-no-sung-tai-bua-tiec-bao-chi-nha-trang-215260426184358978.chn) ⭐️ 5.0/10

The individual suspected of firing shots at the White House Press Corps dinner on Saturday, April 25, has been identified as a teacher and video game developer from Southern California. This incident represents a serious security breach at a high-profile journalism event attended by politicians, media professionals, and officials. The suspect's dual identity as an educator and game developer raises questions about access and motivations. The shooting occurred at the White House Press Corps dinner event on April 25. The suspect has been identified as a teacher and game developer from Southern California. No further details about the investigation or the suspect's motivations have been released.

rss · Kenh14 · Apr 26, 19:24

**Background**: The White House Press Corps dinner, organized by the White House Correspondents' Association, is an annual black-tie event that brings together journalists, politicians, celebrities, and government officials. It has been a target of controversy in recent years due to perceptions of excess and shifting attitudes toward press coverage of the administration. Security at such events is typically handled by the Secret Service.

**Discussion**: Discussions online have focused on the unusual profile of the suspect—a teacher and game developer—and questions about how someone with this background could allegedly carry out such an attack at a major political event.

**Tags**: `#White House`, `#shooting`, `#press corps`, `#breaking news`, `#crime`

---

