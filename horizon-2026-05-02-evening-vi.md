# Horizon Daily - 2026-05-02

> From 87 items, 5 important content pieces were selected

---

1. [How fast is a macOS VM, and how small could it be?](#item-1) ⭐️ 6.0/10
2. [Why are there both TMP and TEMP environment variables? (2015)](#item-2) ⭐️ 6.0/10
3. [Strength in numbers: what have 50 years of labor union documentaries shown us?](#item-3) ⭐️ 4.0/10
4. [Chưa từng có: Trung Quốc đặt lò phản ứng hạt nhân lên xe tải, di chuyển khắp nơi, hoạt động trong nhiều thập kỷ mà không cần tiếp nhiên liệu](#item-4) ⭐️ 4.0/10
5. [Nam sinh dựng ảnh nhạy cảm bạn học nữ, công an vào cuộc](#item-5) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [How fast is a macOS VM, and how small could it be?](https://eclecticlight.co/2026/05/02/how-fast-is-a-macos-vm-and-how-small-could-it-be/) ⭐️ 6.0/10

Howard Oakley published practical benchmarks demonstrating that macOS virtual machines can run efficiently with as little as 2 virtual cores and 4 GB of RAM, with actual memory usage dropping to around 3.1 GB during lightweight tasks, compared to 5 GB usage with 4 cores and 8 GB configuration. This challenges assumptions about minimum macOS VM resource requirements, potentially enabling more efficient CI/CD pipelines, cost reduction for Mac-based cloud infrastructure, and better resource utilization for developers working with macOS VMs on Apple Silicon. The benchmarks reveal that each virtual core consumes a baseline amount of memory (approximately for page cache and concurrency handling), but even a 2-core/4GB VM handles typical workloads well. However, GPU passthrough limitations remain: virtio-gpu provides graphics GPU support but not compute GPU acceleration, making PyTorch and ML workloads essentially impossible in current macOS VMs.

hackernews · moosia · May 2, 09:30

**Background**: Apple Silicon Macs use the Virtualization.framework with paravirtualized GPUs (virtio-gpu) to enable GPU access inside VMs, supporting Metal APIs. However, this approach differs from traditional GPU passthrough used in data centers—compute workloads requiring CUDA or similar acceleration cannot utilize Apple Silicon GPUs through standard virtualization. The community notes historical precedent: early iPhones ran trimmed macOS Tiger with only 128 MiB of RAM, suggesting modern macOS could be similarly optimized if motivated.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/cirruslabs/tart/discussions/344">Is GPU passthrough possible on macOS VMs ? · Discussion #344...</a></li>
<li><a href="https://macstadium.com/blog/gpu-passthrough-virtualization-with-mac-private-clouds">GPU Passthrough & Virtualization with Mac Private Clouds</a></li>
<li><a href="https://eclecticlight.co/2026/04/29/virtualisation-on-apple-silicon-macs-is-different/">Virtualisation on Apple silicon Macs is different – The Eclectic Light...</a></li>

</ul>
</details>

**Discussion**: The discussion highlights practical trade-offs: commenters confirm that GPU compute acceleration remains impossible in VMs (virtio-gpu passes through graphics but not compute capabilities), making PyTorch unusable. One commenter references the Lume library project as an alternative approach, while another points to historical precedent showing macOS can scale down significantly—the original iPhone ran a trimmed macOS Tiger with just 128 MiB, suggesting modern deployments are similarly optimizable.

**Tags**: `#virtualization`, `#macos`, `#vm-performance`, `#benchmarking`, `#apple-silicon`

---

<a id="item-2"></a>
## [Why are there both TMP and TEMP environment variables? (2015)](https://devblogs.microsoft.com/oldnewthing/20150417-00/?p=44213) ⭐️ 6.0/10

Raymond Chen's Old New Thing blog explains why Windows maintains both TMP and TEMP environment variables, tracing the legacy back to CP/M's dual file naming convention and early DOS compatibility decisions made decades ago. This quirk demonstrates how early software decisions can have enduring consequences. Understanding these historical roots helps developers appreciate why certain 'oddities' persist in modern systems and underscores the importance of backward compatibility in operating system design. The post notes that CP/M programs were typically configured through patching—users would modify specific bytes in the executable to customize behavior, a practice foreign to modern configuration paradigms. One commenter also corrected the timeline, noting that CP/M only ran on a simulator in 1973, with practical microcomputer availability coming later.

hackernews · ankitg12 · May 2, 08:23

**Background**: CP/M (Control Program for Microcomputers) was the dominant operating system for early personal computers in the late 1970s, created by Gary Kildall's Digital Research. When IBM developed the PC that would become the IBM PC, they initially planned to use CP/M-86, but negotiations with Digital Research failed. IBM instead turned to Microsoft, which delivered PC DOS based on 86-DOS. The TMP and TEMP distinction stems from CP/M's handling of temporary files and has persisted through decades of Windows evolution.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CP/M">CP / M - Wikipedia</a></li>
<li><a href="https://dfarq.homeip.net/cpm-operating-system/">CPM operating system - The Silicon Underground</a></li>
<li><a href="https://www.britannica.com/technology/CP-M">CP / M | operating system | Britannica</a></li>

</ul>
</details>

**Discussion**: The discussion highlights several valuable insights: corrections to the historical timeline (some noting 1973 is too early for practical CP/M use), the interesting practice of configuring CP/M programs through byte patching (with WordStar mentioned as an example), and practical wisdom that developers should ensure both variables point to the same path to avoid potential issues.

**Tags**: `#windows`, `#environment-variables`, `#retro-computing`, `#legacy-systems`, `#tech-history`

---

<a id="item-3"></a>
## [Strength in numbers: what have 50 years of labor union documentaries shown us?](https://www.theguardian.com/film/2026/may/02/50-years-of-labor-union-documentaries) ⭐️ 4.0/10

The Guardian published a retrospective analyzing 50 years of labor union documentaries, from Barbara Kopple's seminal Harlan County, USA (1976) to American Dream (1990), examining how these films have documented workers' struggles and solidarity against corporate power. These documentaries serve as historical records of labor movements, offering crucial perspectives on workers' rights and corporate accountability that remain relevant to contemporary labor relations. They document how workers organized and resisted corporate pressure during periods of declining union power. American Dream (1990) documents the 1985-86 strike at Hormel Foods Corporation in Austin, Minnesota, where workers faced drastic wage and benefit cuts. The film depicts the broader Reagan-era context of anti-union policies, including the 1981 PATCO strike where President Reagan fired over 11,000 air traffic controllers, and the loss of 2.7 million union members from 1980 to 1984.

rss · The Guardian Culture · May 2, 09:00

**Background**: Labor union documentaries emerged as a powerful medium to capture workers' resistance and solidarity. Harlan County, USA (1976) won the Academy Award for Best Documentary Feature and chronicled the Brookside Strike of 180 coal miners and their wives against the Duke Power Company. Barbara Kopple, who directed both films, became known for her intimate portrayals of labor struggles that balanced personal stories with broader political and economic contexts.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Harlan_County,_USA">Harlan County, USA - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/American_Dream_(film)">American Dream (film) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Professional_Air_Traffic_Controllers_Organization_(1968)">Professional Air Traffic Controllers Organization (1968) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#documentary`, `#film-history`, `#labor-unions`, `#cultural-analysis`, `#cinema`

---

<a id="item-4"></a>
## [Chưa từng có: Trung Quốc đặt lò phản ứng hạt nhân lên xe tải, di chuyển khắp nơi, hoạt động trong nhiều thập kỷ mà không cần tiếp nhiên liệu](https://kenh14.vn/chua-tung-co-trung-quoc-dat-lo-phan-ung-hat-nhan-len-xe-tai-di-chuyen-khap-noi-hoat-dong-trong-nhieu-thap-ky-ma-khong-can-tiep-nhien-lieu-215260502194226034.chn) ⭐️ 4.0/10

A Vietnamese entertainment news outlet reported that China has developed a mobile nuclear reactor with 10 MW capacity capable of operating for decades without refueling, describing it as unprecedented. If verified, such technology could provide flexible nuclear power for remote locations or disaster relief, but the extraordinary claims require rigorous verification given the source's limited nuclear expertise. The article only mentions a 10 MW electrical output capacity and no refueling requirement, with no technical specifications, expert sources, or official documentation to verify the claims.

rss · Kenh14 · May 2, 20:19

**Background**: Small Modular Reactors (SMRs) are nuclear reactors typically under 300 MWe designed with modular construction for factory fabrication and shorter build times. While some SMR designs like Westinghouse's eVinci are being developed for transportability, claims of decades-long operation without refueling would require advanced fuel technologies not widely deployed commercially. Most nuclear reactors require periodic refueling, typically every 18-24 months for light water reactors.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Small_modular_reactor">Small modular reactor - Wikipedia</a></li>
<li><a href="https://world-nuclear.org/information-library/nuclear-power-reactors/small-modular-reactors/small-modular-reactors">Small Modular Reactors - World Nuclear Association</a></li>

</ul>
</details>

**Discussion**: The news has not generated substantial technical community discussion, as the article from an entertainment-focused outlet lacks the credibility and technical depth that would prompt nuclear engineering experts to engage.

**Tags**: `#nuclear-energy`, `#mobile-reactors`, `#China`, `#small-modular-reactors`, `#energy-technology`

---

<a id="item-5"></a>
## [Nam sinh dựng ảnh nhạy cảm bạn học nữ, công an vào cuộc](https://kenh14.vn/nam-sinh-dung-anh-nhay-cam-ban-hoc-nu-cong-an-vao-cuoc-21526050216515433.chn) ⭐️ 4.0/10

Vietnamese police have launched an investigation into a male student from Tân Hưng commune in Đồng Nai city, who allegedly created AI-generated intimate images of female classmates. The case has raised alarms about the misuse of AI technology and social media among minors, causing serious psychological and reputational harm to victims. This case highlights the growing problem of AI misuse among young people, demonstrating how accessible AI tools can be weaponized for harassment and cyberbullying. It underscores the urgent need for better education about AI ethics and stronger legal protections for victims of non-consensual intimate imagery in the digital age. The incident occurred in a school setting, affecting minors, which complicates legal proceedings and raises questions about parental supervision and school responsibility. Deepfake technology enables the creation of highly realistic fake images using neural networks and GANs (Generative Adversarial Networks), making it increasingly difficult to distinguish real from fabricated content.

rss · Kenh14 · May 2, 16:51

**Background**: Deepfakes are media synthesized via AI depicting events that did not occur, using advanced algorithms to swap faces or generate entirely fabricated images. Laws such as the U.S. TAKE IT DOWN Act criminalize the creation and distribution of non-consensual intimate imagery, with penalties including charges for threats to publish, extort, harass, or coerce. AI-generated intimate images cause significant psychological harm to victims, affecting their well-being and digital reputation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.researchgate.net/publication/365467804_Deepfakes_Technology_Using_AI">(PDF) Deepfakes Technology Using AI</a></li>
<li><a href="https://learn-prompting.fr/blog/take-it-down-act-explained">TAKE IT DOWN Act: US Law Against AI - Generated Intimate</a></li>
<li><a href="https://www.linkedin.com/pulse/emergence-deepfakes-technical-basis-documented-harms-detection-olang-y2n3f">The Emergence of Deepfakes : Technical Basis, Documented Harms...</a></li>

</ul>
</details>

**Discussion**: The incident has drawn strong condemnation from the public, with many calling for stricter enforcement of laws against AI-generated harassment. Discussions emphasize the need for comprehensive sex education and digital literacy programs to prevent such misuse. Some users also highlight the importance of platform-level interventions to detect and remove non-consensual intimate content.

**Tags**: `#AI ethics`, `#deepfakes`, `#cybercrime`, `#social media safety`, `#digital privacy`

---

