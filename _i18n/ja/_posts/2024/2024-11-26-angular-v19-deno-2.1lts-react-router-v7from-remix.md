---
title: "2024-11-26のJS: Angular v19、Deno 2.1(LTS)、React Router v7(from Remix)"
author: "azu"
layout: post
date: 2024-11-26T02:04:02.199Z
category: JSer
tags:
- React
- nodejs
- playwright
- TypeScript
- tool

---

JSer.info #716 - Angular v19がリリースされました。

- [Meet Angular v19. In the past two years we doubled down… | by Minko Gechev | Nov, 2024 | Angular Blog](https://blog.angular.dev/meet-angular-v19-7b29dfd05b84)
- [Release v19.0.0 · angular/angular](https://github.com/angular/angular/releases/tag/19.0.0)
- [Angular v19 Developer Event - YouTube](https://www.youtube.com/watch?v=JvkX2_46gUY)

Developer previewとして新しいIncremental Hydrationの仕組みを追加、ServerRouteでレンダリングモードを指定できるように、HMRのサポートが追加されています。

Incremental Hydrationは、`@defer`でHydrationを遅延実行でき、Hydrationがするまでは`@placeholder`でプレースホルダーを表示することができます。Qwikの[Resumable](https://qwik.dev/docs/concepts/resumable/)とやや似た概念ですが、`@defer`ではHydrationするタイミングも指定できるようになっています。

- [Incremental Hydration • Angular](https://angular.dev/guide/incremental-hydration)
- [[Complete] RFC: Incremental Hydration · angular/angular · Discussion #57664](https://github.com/angular/angular/discussions/57664)

また、Standalone componentがデフォルトで`true`に変更、`linkedSignal`の追加、`resource()` APIの追加なども行われています。


----

Deno v2.1がリリースされました。

- [Deno 2.1: Wasm Imports and other enhancements](https://deno.com/blog/v2.1)

Deno 2.1はLTSとなるリリースで、2025年4月までサポートされる予定です。

![Deno LTS](https://docs.deno.com/runtime/fundamentals/images/deno-lts-support.png)

- [Stability and releases](https://docs.deno.com/runtime/fundamentals/stability_and_releases/)

`.wasm`のインポートに対応、`deno init --npm`を追加、`deno outdated`の追加、`deno compile`がAssetsを埋め込めるように。
`deno task`にdescriptionを表示できるように、task間の依存関係を定義できるようになるなどの変更が行われています。

---

React Router v7がリリースされました。

- [React Router v7 | Remix](https://remix.run/blog/react-router-v7)

React Router v7は、Remix v2のメジャーアップデートバージョンとなるバージョンにもなっています。
そのため、React Router v6とRemix v2からのアップデートガイドも公開されています。

- [Upgrading from v6 | React Router](https://reactrouter.com/upgrading/v6)
- [Upgrading from Remix | React Router](https://reactrouter.com/upgrading/remix)

----

{% include inline-support.html %}

----

<h1 class="site-genre">ヘッドライン</h1>

----

## Bun v1.1.35 | Bun Blog
[bun.sh/blog/bun-v1.1.35](https://bun.sh/blog/bun-v1.1.35 "Bun v1.1.35 | Bun Blog")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">Bun</span> <span class="jser-tag">ReleaseNote</span></p>

Bun v1.1.35リリース。
MuslとAlpine Linux のネイティブサポート、`bun test`の結果をJUnit XML形式で出力できるように、`Worker`のpreloadのサポートなど


----

## Meet Angular v19. In the past two years we doubled down… | by Minko Gechev | Nov, 2024 | Angular Blog
[blog.angular.dev/meet-angular-v19-7b29dfd05b84](https://blog.angular.dev/meet-angular-v19-7b29dfd05b84 "Meet Angular v19. In the past two years we doubled down… | by Minko Gechev | Nov, 2024 | Angular Blog")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">Angular</span> <span class="jser-tag">ReleaseNote</span></p>

Angular v19リリース。
Developer previewとして新しいIncremental Hydrationの仕組みを追加、ServerRouteでレンダリングモードを指定できるように、HMRのサポート。
Standalone componentがデフォルトで`true`に変更、`linkedSignal`の追加、`resource()` APIの追加など

- [Release v19.0.0 · angular/angular](https://github.com/angular/angular/releases/tag/19.0.0 "Release v19.0.0 · angular/angular")
- [Angular v19 Developer Event - YouTube](https://www.youtube.com/watch?v=JvkX2_46gUY "Angular v19 Developer Event - YouTube")

----

## Node.js — Node v23.3.0 (Current)
[nodejs.org/en/blog/release/v23.3.0](https://nodejs.org/en/blog/release/v23.3.0 "Node.js — Node v23.3.0 (Current)")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">nodejs</span> <span class="jser-tag">ReleaseNote</span></p>

Node.js v23.3.0リリース。
`util.getCallSite()`がSource Mapをサポート。
Node.jsに対する変更でSEMVER-MAJORのコミットがmainブランチに入る時のルールを厳格化など


----

## Deno 2.1: Wasm Imports and other enhancements
[deno.com/blog/v2.1](https://deno.com/blog/v2.1 "Deno 2.1: Wasm Imports and other enhancements")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">dneo</span> <span class="jser-tag">ReleaseNote</span></p>

Deno v2.1リリース。
LTSとなるリリースで、2025年4月までサポートされる。
`.wasm`のインポートに対応、`deno init --npm`を追加、`deno outdated`の追加、`deno compile`がAssetsを埋め込めるように。
`deno task`にdescriptionを表示できるように、task間の依存関係を定義できるようになるなど

- [Stability and releases](https://docs.deno.com/runtime/fundamentals/stability_and_releases/ "Stability and releases")

----

## November 20, 2024 Release – React Spectrum Releases
[react-spectrum.adobe.com/releases/2024-11-20.html](https://react-spectrum.adobe.com/releases/2024-11-20.html "November 20, 2024 Release – React Spectrum Releases")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">React</span> <span class="jser-tag">UI</span> <span class="jser-tag">library</span> <span class="jser-tag">ReleaseNote</span></p>

react-aria-components 1.5.0 リリース。
`ToggleButtonGroup`の追加、`MenuSection`ごとに設定を持たせられるように、TypeScriptの設定をStrictに変更、AccordionとDisclosureをGAに変更など


----

## Node.js 22 runtime now available in AWS Lambda | AWS Compute Blog
[aws.amazon.com/jp/blogs/compute/node-js-22-runtime-now-available-in-aws-lambda/](https://aws.amazon.com/jp/blogs/compute/node-js-22-runtime-now-available-in-aws-lambda/ "Node.js 22 runtime now available in AWS Lambda | AWS Compute Blog")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">aws</span> <span class="jser-tag">Lambda</span> <span class="jser-tag">nodejs</span> <span class="jser-tag">news</span></p>

AWS LambdaでNode.js 22をサポート


----

## React Router v7 | Remix
[remix.run/blog/react-router-v7](https://remix.run/blog/react-router-v7 "React Router v7 | Remix")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">React</span> <span class="jser-tag">Remix</span> <span class="jser-tag">ReleaseNote</span></p>

React Router v7リリース。
React Router v7はRemix v2のメジャーアップデートバージョンとなる。
React Router v6とRemix v2からのアップデートガイドも公開されている。

- [Upgrading from v6 | React Router](https://reactrouter.com/upgrading/v6 "Upgrading from v6 | React Router")
- [Upgrading from Remix | React Router](https://reactrouter.com/upgrading/remix "Upgrading from Remix | React Router")

----

## Announcing TypeScript 5.7 - TypeScript
[devblogs.microsoft.com/typescript/announcing-typescript-5-7/](https://devblogs.microsoft.com/typescript/announcing-typescript-5-7/ "Announcing TypeScript 5.7 - TypeScript")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">TypeScript</span> <span class="jser-tag">ReleaseNote</span></p>

TypeScript 5.7リリース。
初期化されてない変数のチェック、相対パスの`.ts`を出力時に`.js`へと書き換える`--rewriteRelativeImportExtensions`フラグの追加。
`--target es2024`のサポート、Node.js 22のV8 Compile Cacheをサポートして実行速度の改善など


----

## Release v1.49.0 · microsoft/playwright
[github.com/microsoft/playwright/releases/tag/v1.49.0](https://github.com/microsoft/playwright/releases/tag/v1.49.0 "Release v1.49.0 · microsoft/playwright")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">playwright</span> <span class="jser-tag">ReleaseNote</span></p>

playwright v1.49.0リリース。
Aria Snapshotの追加、古いヘッドレスモード(`chromium-headless-shell`)と新しいヘッドレスモードが両方ダウンロードされるように変更。
`--only-shell`を使うことで古いヘッドレスモードのみをダウンロードできる。新しいヘッドレスモードへ`channel: 'chromium'`で切り替えができる。

- [Changes in Chromium headless in Playwright v1.49 · Issue #33566 · microsoft/playwright](https://github.com/microsoft/playwright/issues/33566 "Changes in Chromium headless in Playwright v1.49 · Issue #33566 · microsoft/playwright")
- [Download old Headless Chrome as chrome-headless-shell  |  Blog  |  Chrome for Developers](https://developer.chrome.com/blog/chrome-headless-shell "Download old Headless Chrome as chrome-headless-shell  |  Blog  |  Chrome for Developers")

----

## State of HTML 2024
[2024.stateofhtml.com/en-US/](https://2024.stateofhtml.com/en-US/ "State of HTML 2024")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">HTML</span> <span class="jser-tag">Survey</span> <span class="jser-tag">news</span></p>

State of HTML 2024の結果が公開された


----
<h1 class="site-genre">アーティクル</h1>

----

## アクセシビリティツリーを比較する Playwright の Aria snapshots がよさそう
[azukiazusa.dev/blog/playwright-aria-snapshot/](https://azukiazusa.dev/blog/playwright-aria-snapshot/ "アクセシビリティツリーを比較する Playwright の Aria snapshots がよさそう")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">playwright</span> <span class="jser-tag">article</span> <span class="jser-tag">test</span> <span class="jser-tag">accessibility</span></p>

PlaywrightのAria snapshotsについて


----
<h1 class="site-genre">スライド、動画関係</h1>

----

## JSConf JP 2024 公開資料・Xアカウントリンクまとめ
[zenn.dev/yumemi\_inc/articles/2024-11-24-jsconf-jp-2024](https://zenn.dev/yumemi_inc/articles/2024-11-24-jsconf-jp-2024 "JSConf JP 2024 公開資料・Xアカウントリンクまとめ")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">Conference</span> <span class="jser-tag">slide</span></p>

JSConf JP 2024のスライドまとめ

- [JSConf JP](https://jsconf.jp/2024/ "JSConf JP")

----
<h1 class="site-genre">サイト、サービス、ドキュメント</h1>

----

## React Scan
[react-scan.million.dev/](https://react-scan.million.dev/ "React Scan")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">React</span> <span class="jser-tag">performance</span> <span class="jser-tag">tool</span></p>

タグを埋め込むことでReactアプリのレンダリングのプロファイルを取得したり、なぜレンダリングされているのかをみたり、レンダリング回数などの可視化をするツール。
Million Lintが開発している。

- [aidenybai/react-scan: Scan for React performance issues and eliminate slow renders in your app](https://github.com/aidenybai/react-scan "aidenybai/react-scan: Scan for React performance issues and eliminate slow renders in your app")

----
<h1 class="site-genre">ソフトウェア、ツール、ライブラリ関係</h1>

----

## ysk8hori/typescript-graph: A CLI to visualize the dependencies between files in the TypeScript codebase.
[github.com/ysk8hori/typescript-graph](https://github.com/ysk8hori/typescript-graph "ysk8hori/typescript-graph: A CLI to visualize the dependencies between files in the TypeScript codebase.")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">TypeScript</span> <span class="jser-tag">tool</span></p>

TypeScriptのコードの依存関係をMermaidでビジュアライズできるツール


----
