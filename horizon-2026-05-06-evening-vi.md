# Horizon Daily - 2026-05-06

> From 122 items, 6 important content pieces were selected

---

1. [Inside the Enhanced Games, Where Athletes Compete on Steroids. And Growth Hormones. And Adderall.](#item-1) ⭐️ 7.0/10
2. [Show HN: Red Squares – GitHub outages as contributions](#item-2) ⭐️ 5.0/10
3. [Setting up a Sun Ray server on OpenIndiana Hipster 2025.10](#item-3) ⭐️ 4.0/10
4. [CNN founder Ted Turner dies at 87](#item-4) ⭐️ 4.0/10
5. [‘Call of Duty’ Launches Military Appreciation Month Campaign With New In-Game Pack (Gaming News Roundup)](#item-5) ⭐️ 4.0/10
6. [Xiaomi 17 Ultra chinh phục thử thách chụp đêm và telephoto qua góc nhìn nhiếp ảnh gia](#item-6) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Inside the Enhanced Games, Where Athletes Compete on Steroids. And Growth Hormones. And Adderall.](https://longreads.com/2026/05/06/enhanced-games-peptides-abu-dhabi/) ⭐️ 7.0/10

The Enhanced Games, a new global sports competition backed by Peter Thiel, Donald Trump Jr., and Saudi royalty, explicitly permits the use of steroids, growth hormones, and Adderall. World Aquatics has banned athletes participating in Enhanced Games events from their own competitions, calling the enterprise 'a circus built on shortcuts.' 这场竞赛对国际体育伦理提出了根本性挑战，可能会使人体的药物增强成为常态。知名科技和政治人物的支持表明，一个价值数十亿美元的“增强人类”产业可能正在形成。 The organizers claim to have medical staff on-site for safety monitoring, but anti-doping agencies warn that many negative health effects from banned substances can occur during training or manifest years later. The June 2025 announcement by World Aquatics specifically targets athletes connected to TEG (The Enhanced Games) for lifetime bans from their events.

rss · Longreads · May 6, 11:01

**Background**: Traditional elite sports operate under strict anti-doping regimes enforced by organizations like WADA (World Anti-Doping Agency), which ban substances including anabolic steroids, growth hormones, and stimulants like Adderall. Transhumanism is a philosophical movement advocating for the enhancement of human capabilities through science and technology, including extending longevity and cognitive abilities. The Enhanced Games directly challenges the established sports establishment by creating an alternative where pharmaceutical and technological enhancement is not just permitted but central to the competition's identity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Enhanced_Games">Enhanced Games - Wikipedia</a></li>
<li><a href="https://www.usada.org/spirit-of-sport/need-know-enhanced-games/">What Athletes Need to Know About the Enhanced Games</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transhumanism">Transhumanism - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The sports community has responded with strong criticism. World Aquatics characterized the Enhanced Games as antithetical to core sporting values of 'honesty, fairness and equity.' Anti-doping authorities emphasize that the claimed safety measures cannot prevent long-term health consequences that often emerge years after substance use. Some transhumanist advocates, however, view the competition as a necessary step toward legitimizing human enhancement technologies.

**Tags**: `#bioethics`, `#doping`, `#sports`, `#transhumanism`, `#technology`, `#regulation`

---

<a id="item-2"></a>
## [Show HN: Red Squares – GitHub outages as contributions](https://red-squares.cian.lol/) ⭐️ 5.0/10

A developer created a web visualization that maps GitHub's public incidents from the past year as red contribution squares on a GitHub-style heatmap grid, using the familiar green-square aesthetic to display downtime instead of code commits. The visualization sparked a broader discussion about whether GitHub itself or third-party AI code assistant providers (Copilot, Claude, Gemini) should bear responsibility for incidents labeled as 'GitHub' disruptions, raising questions about platform reliability transparency. Many incidents attributed to GitHub in the visualization are actually AI code assistant provider issues (e.g., Copilot Grok Code Fast 1, Claude Opus 4, Gemini 2.5 Pro disruptions). Enterprise GitHub users report significantly better uptime than public GitHub users, according to community commenters.

hackernews · cianmm · May 6, 10:28

**Background**: GitHub displays user activity as a heatmap called a 'contribution graph' or 'green squares' — colored squares where darker green indicates more commits or contributions. This visualization inverts that concept by using red to represent outages instead of activity. 'Show HN' is a Hacker News category where developers showcase projects they've created to receive community feedback.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hacker_News">Hacker News - Wikipedia</a></li>
<li><a href="https://github.com/pdb/git-squares">GitHub - pdb/git-squares: Populate GitHub contribution graphs ...</a></li>
<li><a href="https://gitblend.com/kb/understanding-github-contribution-graphs">Understanding GitHub Contribution Graphs - gitblend.com</a></li>

</ul>
</details>

**Discussion**: The community discussion revealed a key nuance: many incidents labeled as 'GitHub' problems are actually AI code assistant failures from providers like Anthropic, Google, and xAI, which GitHub cannot control. Commenters also noted that enterprise GitHub instances maintain much better uptime than the public service. Humorous comments joked that outages decrease on weekends 'when the team leaves it alone.'

**Tags**: `#github`, `#visualization`, `#devops`, `#uptime`, `#humor`

---

<a id="item-3"></a>
## [Setting up a Sun Ray server on OpenIndiana Hipster 2025.10](https://catstret.ch/202605/srss-hipster202510/) ⭐️ 4.0/10

一篇技术教程发布了，展示了如何在 OpenIndiana Hipster 2025.10 上配置 Oracle Sun Ray 瘦客户机服务器软件（SRSS），使传统的 Sun Ray 客户端能够连接到基于 illumos 的现代服务器环境。 本指南帮助爱好者和企业维护老化的 Sun Ray 基础设施，通过提供现代化的操作系统路径，保留了原本可能需要昂贵更换或迁移到专有 VDI 解决方案的瘦客户机部署。 SRSS（Sun Ray Server Software）原本为 Oracle Solaris 设计，现在可在 OpenIndiana 的 illumos 基础架构上运行；用户报告了使用 libvirt 虚拟机时 1024x768 以上分辨率显示不完整的问题。社区评论者指出该架构与 Linux Terminal Server Project（LTSP）在概念上相似。

hackernews · jandeboevrie · May 6, 10:53

**Background**: Sun Ray 是 Oracle（前 Sun Microsystems）推出的超低功耗（约 4 瓦）瘦客户机设备，采用专有协议连接服务器上运行的会话。OpenIndiana 是一个基于 illumos 内核的开源操作系统，旨在保持与 Oracle Solaris 的二进制兼容性。许多企业曾在 Oracle 收购 Sun 之前部署这些系统，现在爱好者通过 OpenIndiana 继续维护这些遗留基础设施。

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sun_Ray">Sun Ray - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenIndiana">OpenIndiana - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Linux_Terminal_Server_Project">Linux Terminal Server Project - Wikipedia</a></li>

</ul>
</details>

**Discussion**: 社区评论充满了对 Sun 时代硬件的怀旧情绪，多位用户回忆 JavaStation 等经典设备，表达了对丢弃珍贵硬件的遗憾。评论者 alexellisuk 将 Sun Ray 与他学生时代使用的 LTSP 进行比较，指出两者在瘦客户机网络启动概念上的相似性。也有用户（ktm5j）分享了在 libvirt 虚拟机中使用 OpenIndiana 时遇到的显示问题。

**Tags**: `#openindiana`, `#sun-ray`, `#thin-client`, `#legacy-systems`, `#tutorial`

---

<a id="item-4"></a>
## [CNN founder Ted Turner dies at 87](https://www.bbc.com/news/articles/c1k2jnx8gmlo?at_medium=RSS&at_campaign=rss) ⭐️ 4.0/10

Ted Turner, the media mogul who founded CNN in 1980 and pioneered 24-hour news broadcasting, has died at age 87 in Georgia. Turner launched the Cable News Network with just $20 million in funding and built it into a global news powerhouse. Turner's creation of CNN revolutionized global news consumption, establishing the 24-hour news cycle that modern media depends on. His pioneering approach fundamentally changed how people around the world access and engage with breaking news and current events. Beyond CNN, Turner also founded Headline News and was the largest private landowner in the United States, owning approximately 2 million acres. He was known for his bold vision and willingness to challenge established media practices.

rss · BBC Culture · May 6, 14:26

**Background**: Ted Turner built his media empire starting with a small television station in Atlanta, Georgia. CNN launched on June 1, 1980, becoming the first 24-hour cable news channel. The concept of continuous news coverage was initially met with skepticism from established broadcasters who questioned whether there would be enough news to fill 24 hours. Turner's model eventually became the standard for news broadcasting worldwide.

**Tags**: `#media`, `#news`, `#obituary`, `#broadcasting`, `#history`

---

<a id="item-5"></a>
## [‘Call of Duty’ Launches Military Appreciation Month Campaign With New In-Game Pack (Gaming News Roundup)](https://variety.com/2026/gaming/news/gaming-news-roundup-1236738760/) ⭐️ 4.0/10

Activision launches a Military Appreciation Month campaign for Call of Duty featuring in-game content proceeds benefiting the Call of Duty Endowment's veteran employment initiatives.

rss · Variety · May 6, 14:15

**Tags**: `#gaming`, `#call-of-duty`, `#activision`, `#corporate-campaign`, `#veterans`

---

<a id="item-6"></a>
## [Xiaomi 17 Ultra chinh phục thử thách chụp đêm và telephoto qua góc nhìn nhiếp ảnh gia](https://kenh14.vn/xiaomi-17-ultra-chinh-phuc-thu-thach-chup-dem-va-telephoto-qua-goc-nhin-nhiep-anh-gia-215260506190024303.chn) ⭐️ 4.0/10

Vietnamese media outlet Kenh14.vn tested the Xiaomi 17 Ultra's camera capabilities by placing it in extreme low-light conditions, including nighttime Saigon street scenes and the traditional firewalking ceremony of the Pà Thẻn indigenous people. This consumer review provides real-world insights into how flagship smartphone cameras perform under challenging conditions rather than controlled lab environments, helping potential buyers understand practical mobile photography capabilities. The tests focused on night photography and telephoto capabilities, two areas where smartphone cameras traditionally struggle. Professional photographers evaluated the device's performance in real-world scenarios rather than controlled conditions.

rss · Kenh14 · May 6, 19:30

**Background**: Smartphone camera technology has advanced rapidly, with flagship devices now featuring sophisticated multi-lens setups and AI-powered computational photography. Night photography particularly challenges camera sensors due to limited light, requiring larger apertures and sensor pixel sizes to capture usable images. Telephoto lenses on smartphones typically offer fixed zoom levels (such as 3x or 5x optical zoom) rather than continuous optical zoom, though software interpolation helps bridge the gap.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gsmarena.com/xiaomi_17_ultra_5g-14380.php">Xiaomi 17 Ultra - Full phone specifications</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_longest_smartphone_telephoto_lenses">List of longest smartphone telephoto lenses - Wikipedia</a></li>
<li><a href="https://www.mi.com/global/product/xiaomi-17-ultra/specs/">Xiaomi 17 Ultra Specs</a></li>

</ul>
</details>

**Tags**: `#smartphone cameras`, `#Xiaomi`, `#mobile photography`, `#product review`, `#night photography`

---

