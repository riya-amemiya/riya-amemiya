<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3178C6,100:4B8BF5&height=200&section=header&text=Riya%20Amemiya&fontSize=56&fontColor=ffffff&fontAlignY=36&desc=V8%20Contributor%20%2F%20Platform%20Engineer%20at%20Dinii%20Inc.&descSize=18&descAlignY=58&animation=fadeIn" alt="Riya Amemiya" width="100%" />

[![X](https://img.shields.io/badge/@riya__amemiya-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/riya_amemiya)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yuta-nishi-499738262/)
[![Zenn](https://img.shields.io/badge/Zenn-3EA8FF?style=for-the-badge&logo=zenn&logoColor=white)](https://zenn.dev/riya_amemiya)
[![connpass](https://img.shields.io/badge/connpass-D93A00?style=for-the-badge)](https://connpass.com/user/riya-amemiya/)
[![Slides](https://img.shields.io/badge/Slides-2B90B6?style=for-the-badge&logo=slidev&logoColor=white)](https://riya-amemiya.github.io/amemiya_riya_slide_data/)
[![Links](https://img.shields.io/badge/Links-334155?style=for-the-badge)](https://riya-amemiya-links.tokidux.com/)
[![Sponsor](https://img.shields.io/badge/Sponsor-EA4AAA?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/riya-amemiya)
 
[![wakatime](https://wakatime.com/badge/user/eae142f3-5e4b-4e20-b3ca-d5d6d5a13e07.svg)](https://wakatime.com/@eae142f3-5e4b-4e20-b3ca-d5d6d5a13e07)
 
[日本語](./README-ja.md) | **English**
 
</div>

## 👋 About
 
Hi, I'm Riya.<br/>
I work as a Platform Engineer at Dinii Inc.<br/>
As a V8 contributor, I mainly work on speeding up `Array.prototype` builtins.<br/>
I also help run conferences as a TSKaigi staff member, write articles on Zenn, and speak at meetups and conferences.
 
## ⚙️ V8 Contributions
 
I work on performance improvements and bug fixes for V8 builtins.<br/>
The background and benchmark results of each optimization are written up on Zenn (in Japanese).
 
| Target | Change | Result | Article |
| --- | --- | --- | --- |
| `Array.prototype.flat` | Added a Torque fast path | Up to ~5x faster | [Zenn](https://zenn.dev/dinii/articles/675d47a6c21c83) |
| `Array.prototype.flat` | Added bulk copy to the fast path | A further ~5x faster | [Zenn](https://zenn.dev/dinii/articles/e12fbacc8e761c) |
| `Array.prototype.copyWithin` | Added a Torque fast path | Up to ~450x faster | [Zenn](https://zenn.dev/dinii/articles/a272b7c3b60ab8) |
| `Array.prototype.fill` | Skipped per-element stores for Smi and double values | Up to ~7x faster | [Zenn](https://zenn.dev/dinii/articles/5b8edc7856c25b) |
| `Array.prototype.lastIndexOf` | Specialized by ElementsKind | Up to ~26000x faster | [Zenn](https://zenn.dev/dinii/articles/2f66b147007cf8) |
 
Beyond performance work, my changes include fixes for `Intl.DateTimeFormat` and Temporal, and support for spread arguments in direct eval.<br/>
All of my changes are listed in [the V8 commit history](https://github.com/v8/v8/commits/main/?author=riya-amemiya).
 
### V8 Tools
 
| Repository | Description |
| --- | --- |
| [vscode-torque-fork](https://github.com/riya-amemiya/vscode-torque-fork) | VS Code extension for V8 Torque. Runs a Torque compiler written in Rust as WebAssembly to provide go to definition, completion, diagnostics, and formatting |
| [v8-performance-viewer](https://github.com/riya-amemiya/v8-performance-viewer) | Runs the same benchmarks on multiple V8 versions and visualizes the speed difference on the web |
| [v8-deep-dive](https://github.com/riya-amemiya/v8-deep-dive) | A single-page technical guide to V8 internals, memory management, Torque, arrays, and `Array.prototype.flat` |
 
## 📦 My OSS
 
| Repository | Description | Package |
| --- | --- | --- |
| [UMT](https://github.com/riya-amemiya/UMT) | A dependency-free collection of useful functions. The TypeScript implementation is the source of truth, with ports for Python, Rust, and WebAssembly | [![npm](https://img.shields.io/npm/v/umt?style=flat-square&logo=npm&label=umt)](https://www.npmjs.com/package/umt) |
| [agrb](https://github.com/riya-amemiya/agrb) | Interactive CLI to safely rebase a branch onto another, using either cherry-pick or `git rebase` | [![npm](https://img.shields.io/npm/v/agrb?style=flat-square&logo=npm&label=agrb)](https://www.npmjs.com/package/agrb) |
| [agbd](https://github.com/riya-amemiya/agbd) | Interactive CLI to inspect and safely delete unnecessary Git branches | [![npm](https://img.shields.io/npm/v/agbd?style=flat-square&logo=npm&label=agbd)](https://www.npmjs.com/package/agbd) |
| [chtr](https://github.com/riya-amemiya/chtr) | Converts HTML strings into React elements | [![npm](https://img.shields.io/npm/v/chtr?style=flat-square&logo=npm&label=chtr)](https://www.npmjs.com/package/chtr) |
| [mojiyose](https://github.com/riya-amemiya/mojiyose) | A tiny, dependency-free library that converts between Japanese legacy encodings such as Shift_JIS and UTF-8 | [![npm](https://img.shields.io/npm/v/mojiyose?style=flat-square&logo=npm&label=mojiyose)](https://www.npmjs.com/package/mojiyose) |
| [happy-cracking](https://github.com/riya-amemiya/happy-cracking) | A CTF toolkit written in Rust with 70+ commands | [![crates.io](https://img.shields.io/crates/v/happy-cracking?style=flat-square&logo=rust&label=happy-cracking)](https://crates.io/crates/happy-cracking) |
| [links](https://github.com/riya-amemiya/links) | Links to my accounts | [Web](https://riya-amemiya-links.tokidux.com/) |
 
## 🎤 Talks
 
All slides are available at [amemiya_riya_slide_data](https://riya-amemiya.github.io/amemiya_riya_slide_data/). The talks are in Japanese.
 
| Topic | Title |
| --- | --- |
| V8 | [V8のArray.prototype.flatを最大約20倍速くするまでと、巨大OSSへの大規模コミットの道のり](https://riya-amemiya.github.io/amemiya_riya_slide_data/v8_array_flat/) |
| V8 | [そのJavaScript、V8が泣いてます。V8の気持ちを理解して書くパフォーマンス最適化](https://riya-amemiya.github.io/amemiya_riya_slide_data/frontend_conf_tokyo_2025/) |
| V8 | [JavaScriptのNumberは1つじゃない？V8内部の型システムを覗く](https://riya-amemiya.github.io/amemiya_riya_slide_data/v8_number_internals/) |
| V8 | [V8のTorqueを語りたい](https://riya-amemiya.github.io/amemiya_riya_slide_data/v8_torque/) |
| V8 | [V8コントリビュート超入門](https://riya-amemiya.github.io/amemiya_riya_slide_data/v8_contribute_intro/) |
| JavaScript | [知ってた？JavaScriptの"正しさ"を検証するテストが5万以上もあること(Test262)](https://riya-amemiya.github.io/amemiya_riya_slide_data/frontend_conf_nagoya_2026/) |
| JavaScript | [Temporal 最高!でも改めて「日付」について調べたら人類の負債すぎる件](https://riya-amemiya.github.io/amemiya_riya_slide_data/temporal_calendar/) |
| TypeScript | [IsAny はなぜ any だけを見抜けるのか](https://riya-amemiya.github.io/amemiya_riya_slide_data/typescript_isany/) |
| HTML | [「え？！それ今ではHTMLだけでできるの！？」驚きの進化を遂げたモダンHTML](https://riya-amemiya.github.io/amemiya_riya_slide_data/frontend_conf_kansai_2025/) |
| CSS | [「え？！それ今ではCSSだけでできるの！？」驚きの進化を遂げたモダンCSS](https://riya-amemiya.github.io/amemiya_riya_slide_data/frontend_conf_hokkaido_2025/) |
 
## ✍️ Writing
 
I write articles in Japanese on [Zenn](https://zenn.dev/riya_amemiya).<br/>
The drafts are managed in [amemiya_riya_zenn_data](https://github.com/riya-amemiya/amemiya_riya_zenn_data).<br/>
Articles about V8 optimizations are listed in [V8 Contributions](#️-v8-contributions) above.
 
- [最近のHTMLを改めてちゃんと学んでみた](https://zenn.dev/dinii/articles/16b3e71b580b6c)
- [最近のCSSを改めてちゃんと学んでみた](https://zenn.dev/gmomedia/articles/6ed3718b4c6bc1)
- [え？まだgit checkoutしてるの？](https://zenn.dev/gmomedia/articles/d9366fa84aadfd)
- [TryHackMeでHackerになった話](https://zenn.dev/gmomedia/articles/6a90805a1e9936)
- [git rebaseが難しすぎたので、自動化CLI作った](https://zenn.dev/riya_amemiya/articles/c080705b331456)
- [V8に初めてパッチを出すための手引き](https://zenn.dev/riya_amemiya/articles/44e6ed7d381304)
## 🛠️ Tech Stack
 
My area of expertise is web frontend, especially TypeScript and React.
 
| Area | Technologies |
| --- | --- |
| Languages | ![Languages](https://go-skill-icons.vercel.app/api/icons?i=ts,js,python,rust,go,cpp,c,zig,ruby,php,html,css,sass,wasm,graphql&perline=8) |
| Frontend | ![Frontend](https://go-skill-icons.vercel.app/api/icons?i=react,nextjs,remix,astro,gatsby,angular,redux,jquery,tailwindcss,mui,bootstrap&perline=8) |
| Backend | ![Backend](https://go-skill-icons.vercel.app/api/icons?i=nodejs,express,nestjs,django,flask,fastapi,rails,laravel,rocket&perline=8) |
| Databases and ORM (not my strongest area) | ![Databases and ORM](https://go-skill-icons.vercel.app/api/icons?i=postgresql,mysql,sqlite,redis,prisma&perline=8) |
| Infrastructure | ![Infrastructure](https://go-skill-icons.vercel.app/api/icons?i=gcp,firebase,supabase,vercel,cloudflare,docker&perline=8) |
| Testing | ![Tests](https://go-skill-icons.vercel.app/api/icons?i=jest,cypress&perline=8) |
| Dev Tools | ![Tools](https://go-skill-icons.vercel.app/api/icons?i=git,github,ghactions,npm,yarn,pnpm,bun,webpack,vite,babel&perline=8) |
| Editors and Design | ![Editors and Design](https://go-skill-icons.vercel.app/api/icons?i=vscode,vim,figma,notion&perline=8) |
| OS | ![OS](https://go-skill-icons.vercel.app/api/icons?i=apple,linux,ubuntu,kali,windows&perline=8) |
 
## 🎓 Certifications
 
| Certification | |
| --- | --- |
| JDLA Deep Learning for GENERAL (2023#4) | <img src="./img/general2023_4_regular.png" alt="JDLA Deep Learning for GENERAL" width="160" /> |
| Python 3 Certified Practical Engineer | Passed |
| TryHackMe | <img src="https://tryhackme-badges.s3.amazonaws.com/riyaamemiya.png" alt="TryHackMe" /> |
 
## 📊 GitHub Stats
 
<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github_dark/0-profile-details.svg" />
  <img src="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github/0-profile-details.svg" alt="Profile details" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github_dark/2-most-commit-language.svg" />
  <img src="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github/2-most-commit-language.svg" alt="Top languages by commit" width="49%" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github_dark/3-stats.svg" />
  <img src="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github/3-stats.svg" alt="GitHub stats" width="49%" />
</picture>
<img src="https://wakatime.com/share/@riya_amemiya/d0f95094-22a7-4aff-aff7-25a43506cc2f.svg" alt="WakaTime stats" height="250" />
<img src="https://wakatime.com/share/@riya_amemiya/21948023-0285-4b79-ba4d-6c2a8fad15a8.svg" alt="WakaTime stats" height="250" />
</div>
<details>
<summary>Contribution calendar</summary>

![Metrics](./metrics.plugin.calendar.full.svg)
 
</details>
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3178C6,100:4B8BF5&height=120&section=footer" alt="" width="100%" />
