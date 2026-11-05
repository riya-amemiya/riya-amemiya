<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3178C6,100:4B8BF5&height=200&section=header&text=Riya%20Amemiya&fontSize=56&fontColor=ffffff&fontAlignY=36&desc=V8%20Contributor%20%2F%20Platform%20Engineer%20at%20Dinii%20Inc.&descSize=18&descAlignY=58&animation=fadeIn" alt="Riya Amemiya" width="100%" />

[![X](https://img.shields.io/badge/@riya__amemiya-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/riya_amemiya)
[![Zenn](https://img.shields.io/badge/Zenn-3EA8FF?style=for-the-badge&logo=zenn&logoColor=white)](https://zenn.dev/riya_amemiya)
[![connpass](https://img.shields.io/badge/connpass-D93A00?style=for-the-badge)](https://connpass.com/user/riya-amemiya/)
[![Slides](https://img.shields.io/badge/Slides-2B90B6?style=for-the-badge&logo=slidev&logoColor=white)](https://riya-amemiya.github.io/amemiya_riya_slide_data/)
[![Links](https://img.shields.io/badge/Links-334155?style=for-the-badge)](https://riya-amemiya-links.tokidux.com/)
[![Sponsor](https://img.shields.io/badge/Sponsor-EA4AAA?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/riya-amemiya)

[![wakatime](https://wakatime.com/badge/user/eae142f3-5e4b-4e20-b3ca-d5d6d5a13e07.svg)](https://wakatime.com/@eae42f3-5e4b-4e20-b3ca-d5d6d5a13e07)
 
**日本語** | [English](./README-en.md)
 
</div>

## 👋 About
 
初めまして、Riya です。<br/>
株式会社ダイニーで Platform Engineer として働いています。<br/>
V8 のコントリビューターとして、主に `Array.prototype` 系 Builtin の高速化に取り組んでいます。<br/>
TSKaigi のスタッフとしてカンファレンス運営に関わるほか、Zenn での執筆や勉強会、カンファレンスでの登壇も続けています。
 
## ⚙️ V8 へのコントリビューション
 
V8 の Builtin の高速化と不具合修正をしています。<br/>
高速化の経緯と計測結果は Zenn にまとめています。
 
| 対象 | 変更 | 効果 | 記事 |
| --- | --- | --- | --- |
| `Array.prototype.flat` | Torque による高速パスを追加 | 最大約5倍 | [Zenn](https://zenn.dev/dinii/articles/675d47a6c21c83) |
| `Array.prototype.flat` | 高速パスにバルクコピーを導入 | さらに約5倍 | [Zenn](https://zenn.dev/dinii/articles/e12fbacc8e761c) |
| `Array.prototype.copyWithin` | Torque による高速パスを追加 | 最大約450倍 | [Zenn](https://zenn.dev/dinii/articles/a272b7c3b60ab8) |
| `Array.prototype.fill` | Smi と double の値で要素ごとの書き込みを省略 | 最大約7倍 | [Zenn](https://zenn.dev/dinii/articles/5b8edc7856c25b) |
| `Array.prototype.lastIndexOf` | ElementsKind ごとに処理を特殊化 | 最大約26000倍 | [Zenn](https://zenn.dev/dinii/articles/2f66b147007cf8) |
 
高速化のほかに、`Intl.DateTimeFormat` と Temporal の不具合修正や、direct eval でのスプレッド引数への対応なども入っています。<br/>
すべての変更は [V8 のコミット履歴](https://github.com/v8/v8/commits/main/?author=riya-amemiya)で確認できます。
 
### V8 関連のツール
 
| リポジトリ | 説明 |
| --- | --- |
| [vscode-torque-fork](https://github.com/riya-amemiya/vscode-torque-fork) | V8 Torque 用の VS Code 拡張。Rust 製の Torque コンパイラを WebAssembly で動かし、定義ジャンプ、補完、診断、整形を提供 |
| [v8-performance-viewer](https://github.com/riya-amemiya/v8-performance-viewer) | 複数の V8 バージョンで同じベンチマークを実行し、速度差を Web で可視化 |
| [v8-deep-dive](https://github.com/riya-amemiya/v8-deep-dive) | V8 の内部実装、メモリ管理、Torque、配列、`Array.prototype.flat` を解説する単一ページの技術資料 |
 
## 📦 自作 OSS
 
| リポジトリ | 説明 | パッケージ |
| --- | --- | --- |
| [UMT](https://github.com/riya-amemiya/UMT) | 依存ゼロの汎用関数集。TypeScript の実装を基準に、Python、Rust、WebAssembly 向けの移植も提供 | [![npm](https://img.shields.io/npm/v/umt?style=flat-square&logo=npm&label=umt)](https://www.npmjs.com/package/umt) |
| [agrb](https://github.com/riya-amemiya/agrb) | ブランチを別のブランチへ安全に載せ替える対話型 CLI。cherry-pick と `git rebase` の2方式に対応 | [![npm](https://img.shields.io/npm/v/agrb?style=flat-square&logo=npm&label=agrb)](https://www.npmjs.com/package/agrb) |
| [agbd](https://github.com/riya-amemiya/agbd) | 不要な Git ブランチを確認しながら削除する対話型 CLI | [![npm](https://img.shields.io/npm/v/agbd?style=flat-square&logo=npm&label=agbd)](https://www.npmjs.com/package/agbd) |
| [chtr](https://github.com/riya-amemiya/chtr) | HTML 文字列を React 要素へ変換するライブラリ | [![npm](https://img.shields.io/npm/v/chtr?style=flat-square&logo=npm&label=chtr)](https://www.npmjs.com/package/chtr) |
| [mojiyose](https://github.com/riya-amemiya/mojiyose) | Shift_JIS などの日本語レガシーエンコーディングと UTF-8 を相互変換する依存ゼロのライブラリ | [![npm](https://img.shields.io/npm/v/mojiyose?style=flat-square&logo=npm&label=mojiyose)](https://www.npmjs.com/package/mojiyose) |
| [happy-cracking](https://github.com/riya-amemiya/happy-cracking) | 70 以上のコマンドを備えた Rust 製の CTF ツールキット | [![crates.io](https://img.shields.io/crates/v/happy-cracking?style=flat-square&logo=rust&label=happy-cracking)](https://crates.io/crates/happy-cracking) |
| [links](https://github.com/riya-amemiya/links) | 各種アカウントへのリンク集 | [Web](https://riya-amemiya-links.tokidux.com/) |
 
## 🎤 登壇
 
スライドの一覧は [amemiya_riya_slide_data](https://riya-amemiya.github.io/amemiya_riya_slide_data/) にあります。
 
| 分野 | タイトル |
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
 
## ✍️ 執筆
 
記事は [Zenn](https://zenn.dev/riya_amemiya) に書いています。<br/>
原稿は [amemiya_riya_zenn_data](https://github.com/riya-amemiya/amemiya_riya_zenn_data) で管理しています。<br/>
V8 の高速化に関する記事は、上の [V8 へのコントリビューション](#️-v8-へのコントリビューション) にまとめています。
 
- [最近のHTMLを改めてちゃんと学んでみた](https://zenn.dev/dinii/articles/16b3e71b580b6c)
- [最近のCSSを改めてちゃんと学んでみた](https://zenn.dev/gmomedia/articles/6ed3718b4c6bc1)
- [え？まだgit checkoutしてるの？](https://zenn.dev/gmomedia/articles/d9366fa84aadfd)
- [TryHackMeでHackerになった話](https://zenn.dev/gmomedia/articles/6a90805a1e9936)
- [git rebaseが難しすぎたので、自動化CLI作った](https://zenn.dev/riya_amemiya/articles/c080705b331456)
- [V8に初めてパッチを出すための手引き](https://zenn.dev/riya_amemiya/articles/44e6ed7d381304)
## 🛠️ 技術スタック
 
得意領域は Web フロントエンドで、特に TypeScript と React です。
 
| 分野 | 技術 |
| --- | --- |
| 言語 | ![Languages](https://go-skill-icons.vercel.app/api/icons?i=ts,js,python,rust,go,cpp,c,zig,ruby,php,html,css,sass,wasm,graphql&perline=8) |
| フロントエンド | ![Frontend](https://go-skill-icons.vercel.app/api/icons?i=react,nextjs,remix,astro,gatsby,angular,redux,jquery,tailwindcss,mui,bootstrap&perline=8) |
| バックエンド | ![Backend](https://go-skill-icons.vercel.app/api/icons?i=nodejs,express,nestjs,django,flask,fastapi,rails,laravel,rocket&perline=8) |
| データベースと ORM（あまり得意ではない） | ![Databases and ORM](https://go-skill-icons.vercel.app/api/icons?i=postgresql,mysql,sqlite,redis,prisma&perline=8) |
| インフラ | ![Infrastructure](https://go-skill-icons.vercel.app/api/icons?i=gcp,firebase,supabase,vercel,cloudflare,docker&perline=8) |
| テスト | ![Tests](https://go-skill-icons.vercel.app/api/icons?i=jest,cypress&perline=8) |
| 開発ツール | ![Tools](https://go-skill-icons.vercel.app/api/icons?i=git,github,ghactions,npm,yarn,pnpm,bun,webpack,vite,babel&perline=8) |
| エディタとデザイン | ![Editors and Design](https://go-skill-icons.vercel.app/api/icons?i=vscode,vim,figma,notion&perline=8) |
| OS | ![OS](https://go-skill-icons.vercel.app/api/icons?i=apple,linux,ubuntu,kali,windows&perline=8) |
 
## 🎓 資格
 
| 資格 | |
| --- | --- |
| G検定（2023#4） | <img src="./img/general2023_4_regular.png" alt="G検定" width="160" /> |
| Python 3 エンジニア認定実践試験 | 合格 |
| TryHackMe | <img src="https://tryhackme-badges.s3.amazonaws.com/riyaamemiya.png" alt="TryHackMe" /> |
 
## 📊 GitHub Stats
 
<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github_dark/0-profile-details.svg" />
  <img src="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github/0-profile-details.svg" alt="プロフィールの概要" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github_dark/2-most-commit-language.svg" />
  <img src="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github/2-most-commit-language.svg" alt="コミットの多い言語" width="49%" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github_dark/3-stats.svg" />
  <img src="https://raw.githubusercontent.com/riya-amemiya/riya-amemiya/main/profile-summary-card-output/github/3-stats.svg" alt="GitHub の統計" width="49%" />
</picture>
<img src="https://wakatime.com/share/@riya_amemiya/d0f95094-22a7-4aff-aff7-25a43506cc2f.svg" alt="WakaTime の統計" height="250" />
<img src="https://wakatime.com/share/@riya_amemiya/21948023-0285-4b79-ba4d-6c2a8fad15a8.svg" alt="WakaTime の統計" height="250" />
</div>
<details>
<summary>コントリビューションカレンダー</summary>

![Metrics](./metrics.plugin.calendar.full.svg)
 
</details>
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3178C6,100:4B8BF5&height=120&section=footer" alt="" width="100%" />
