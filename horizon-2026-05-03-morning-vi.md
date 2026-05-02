# Horizon Daily - 2026-05-02

> From 48 items, 3 important content pieces were selected

---

1. [VS Code inserting 'Co-Authored-by Copilot' into commits regardless of usage](#item-1) ⭐️ 8.0/10
2. [Dav2d](#item-2) ⭐️ 7.0/10
3. [NetHack 5.0.0](#item-3) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [VS Code inserting 'Co-Authored-by Copilot' into commits regardless of usage](https://github.com/microsoft/vscode/pull/310226) ⭐️ 8.0/10

Microsoft's VS Code merged a pull request that automatically inserts 'Co-Authored-By Copilot' into git commit metadata even when users haven't used Copilot AI assistance. The change sets the default configuration to "all" for git.addAICoAuthor, triggering the automatic insertion regardless of actual AI usage. This raises serious concerns about commit integrity, as git commits serve as legal and technical records of code authorship. The precedent of inserting misleading attribution purely for branding and AI usage metrics represents a significant breach of developer trust and could affect auditing, compliance, and attribution systems across the industry. Ironically, Copilot itself commented on the PR noting the change creates inconsistency with runtime fallback code that still defaults to 'off', recommending the revert. The configuration schema was changed to default 'all' while the actual code path in extensions/git/src/repository.ts still calls config.get('addAICoAuthor', 'off'), creating a desync that can lead to unexpected behavior.

hackernews · indrora · May 2, 19:57

**Background**: Git trailers are metadata lines added at the end of commit messages, with 'Co-authored-by' being a standard format for attributing commits to multiple contributors. This feature is legitimate when accurately reflecting joint authorship, but becomes problematic when inserted without actual AI involvement. GitHub's commit history and blame systems rely on accurate authorship data for code review, security auditing, and license compliance.

<details><summary>References</summary>
<ul>
<li><a href="https://code.visualstudio.com/docs/sourcecontrol/staging-commits">Staging and committing changes</a></li>
<li><a href="https://docs.github.com/articles/creating-a-commit-with-multiple-authors">Creating a commit with multiple authors - GitHub Docs</a></li>
<li><a href="https://alchemists.io/articles/git_trailers">Git Trailers | Alchemists</a></li>

</ul>
</details>

**Discussion**: The community response is overwhelmingly negative, with critics comparing this to Microsoft's historical pattern of prioritizing marketing over user experience. Commenters highlight the irony that Copilot recommended reverting its own branding injection. There's widespread agreement that commit metadata should accurately reflect what actually happened, not what marketing departments want projected. The broader concern extends beyond Microsoft to a general pattern of AI hype overriding technical standards and ethics.

**Tags**: `#vscode`, `#github-copilot`, `#developer-tools`, `#ethics`, `#microsoft`

---

<a id="item-2"></a>
## [Dav2d](https://code.videolan.org/videolan/dav2d) ⭐️ 7.0/10

VideoLAN developers have published dav2d, an open-source, CPU-based AV2 video decoder claimed to be the fastest across all platforms, with cross-platform support planned for x86, ARM, and RISC-V architectures. As the first major open-source AV2 decoder, dav2d signals growing ecosystem support for AOMedia's next-generation codec, which promises 30% lower bitrates than AV1 while maintaining video quality—critical for streaming services and video delivery at scale. The decoder prioritizes correctness first, with performance optimizations planned as a secondary phase, and is designed to be small and portable across platforms.

hackernews · dabinat · May 2, 17:32

**Background**: AV2 is the next-generation video coding specification from the Alliance for Open Media (AOMedia), an industry consortium including Google, Apple, Netflix, Amazon, Intel, NVIDIA, and Microsoft. AV2 was announced in September 2025 on AOMedia's 10th anniversary, building on AV1's royalty-free foundation. The AV2 specification promises significant compression improvements over AV1, though encoder implementations like SVT-AV1 took years to become production-ready for AV1, suggesting similar timeline challenges for AV2.

<details><summary>References</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Dav2d-Open-Source-AV2-Decode">VideoLAN Publishes Dav2d For Open-Source AV2 Decoder - Phoronix</a></li>
<li><a href="https://en.wikipedia.org/wiki/AV2_(codec)">AV2 - Wikipedia</a></li>
<li><a href="https://av2.aomedia.org/">AV2 Specification</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive, with users expressing excitement about AV2's potential improvements over AV1. Concerns were raised about the timeline for viable AV2 encoders, echoing frustrations with how long SVT-AV1 took to become usable. One user raised an off-topic but relatable complaint about internet bot verification and cookie popups, while another praised the clean interface of the VideoLAN GitLab instance.

**Tags**: `#video-codec`, `#av2`, `#av1`, `#open-source`, `#performance`

---

<a id="item-3"></a>
## [NetHack 5.0.0](https://nethack.org/v500/release.html) ⭐️ 6.0/10

NetHack 5.0.0 has replaced its legacy yacc/lex-based level and dungeon compilers with Lua-based alternatives, and existing saved games and bones files will no longer be compatible with the new version. This release marks the end of an era for one of computing's oldest roguelike games, modernizing a decades-old codebase while acknowledging that some long-running save files from players may be permanently lost. The Lua-based configuration is loaded and processed during gameplay rather than at build time, and the quest text file processing previously handled by makedefs has also been migrated. Additionally, multiple gameplay balance changes affect Valkyrie characters, bag of holding mechanics, and amnesia effects.

hackernews · rsaarelm · May 2, 18:03

**Background**: NetHack is a classic roguelike dungeon crawler originally released in 1987, known for its ASCII graphics and punishing difficulty. Yacc (Yet Another Compiler-Compiler) and Lex (Lexical Analyzer) are traditional Unix tools for generating parsers and tokenizers used in compiler construction. Lua is a lightweight, embeddable scripting language first released in 1993 that has become popular in game development for configuration and modding, as seen in games like World of Warcraft and Roblox.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Yacc">Yacc - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lua">Lua - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community sentiment mixes nostalgia with appreciation for modernization. One player shared a touching story of having an old save file from 17 years ago with the Amulet of Yendor in hand, now lost to incompatibility. Others praised the Lua migration as technically sound while mourning the end of the yacc/lex era, and several noted specific gameplay balance changes with mixed reactions.

**Tags**: `#gaming`, `#roguelike`, `#open-source`, `#software-engineering`, `#legacy-code`

---

