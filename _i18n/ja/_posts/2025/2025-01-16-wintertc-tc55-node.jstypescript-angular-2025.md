---
title: "2025-01-16のJS: WinterTC (TC55)、Node.jsのTypeScriptサポートの背景、Angular 2025"
author: "azu"
layout: post
date: 2025-01-16T13:42:36.358Z
category: JSer
tags:
- TypeScript
- nodejs
- React
- pnpm
- security

---

JSer.info #722 - Node.js/Deno/Cloudflare WorkersなどのサーバサイドのJavaScript実行環境の相互運用性について議論をしていたWinterCGが、EcmaのTC55([WinterTC](https://wintercg.org/))として標準化などの作業を進めることが発表されました。

- [Collaborating across W3C and Ecma for web-interoperable server runtimes through WinterTC - Ecma International](https://ecma-international.org/news/collaborating-across-w3c-and-ecma-for-web-interoperable-server-runtimes-through-wintertc/)

ECMAScriptやHTMLなどの標準仕様には特許とライセンスが関わってくるため、実際にAPIの標準を作成するにはEcmaやW3Cのような標準化団体のプロセスに従って行った方が良い部分があります。
WinterCGは元々 W3C のコミュニティグループから始まっていますが、W3CとEcmaどちらで標準化を進めていくかを議論して、多くのメンバーがすでにEcmaに参加していた(TC39などのECMAScriptの標準化などに関わっていた)ため、EcmaのTC55として標準化を進めることになったようです。

- [Dedicated standardization meeting 2024-08-29 · Issue #70 · wintercg/admin](https://github.com/wintercg/admin/issues/70)
- [Tracking issue: consider ECMA TC / W3C WG to publish standards · Issue #58 · wintercg/admin](https://github.com/wintercg/admin/issues/58)

---

[Node.js Type Stripping Explained](https://satanacchio.hashnode.dev/everything-you-need-to-know-about-nodejs-type-stripping)という記事では、Node.jsのTypeScriptサポートのアプローチであるType Strippingについて解説されています。
なぜ型を取り除くというアプローチをしているのかや、コードの変換とSource Map、今後のTypeScriptサポートの方向性などについても書かれています。

---

[Angular 2025 Strategy. For the past two and a half years… | by Minko Gechev | Jan, 2025 | Angular Blog](https://blog.angular.dev/angular-2025-strategy-9ca333dfc334)という記事では、Angularの2025年の展望について書かれています。

Angularの2024年のアンケート結果の分析、2025年に取り組む点についてなどについて書かれています。

----

{% include inline-support.html %}

----

<h1 class="site-genre">ヘッドライン</h1>

----

## ESLint v9.18.0 released - ESLint - Pluggable JavaScript Linter
[eslint.org/blog/2025/01/eslint-v9.18.0-released/](https://eslint.org/blog/2025/01/eslint-v9.18.0-released/ "ESLint v9.18.0 released - ESLint - Pluggable JavaScript Linter")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">ESLint</span> <span class="jser-tag">TypeScript</span></p>

ESLint v9.18.0リリース。
TypeScriptで設定ファイルを書ける`eslint.config.ts`のサポートなど


----

## Collaborating across W3C and Ecma for web-interoperable server runtimes through WinterTC - Ecma International
[ecma-international.org/news/collaborating-across-w3c-and-ecma-for-web-interoperable-server-runtimes-through-wintertc/](https://ecma-international.org/news/collaborating-across-w3c-and-ecma-for-web-interoperable-server-runtimes-through-wintertc/ "Collaborating across W3C and Ecma for web-interoperable server runtimes through WinterTC - Ecma International")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">ecma</span> <span class="jser-tag">news</span> <span class="jser-tag">nodejs</span> <span class="jser-tag">deno</span> <span class="jser-tag">cloudflare</span></p>

サーバサイドJavaScript APIの相互運用性について議論していたWinterCGはEcmaのTC55として標準化などの議論を進めていく方針

- [WinterTC](https://wintercg.org/ "WinterTC")

----

## Release 3.40.0 - 2025.01.08 · zloirock/core-js
[github.com/zloirock/core-js/releases/tag/v3.40.0](https://github.com/zloirock/core-js/releases/tag/v3.40.0 "Release 3.40.0 - 2025.01.08 · zloirock/core-js")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">polyfill</span> <span class="jser-tag">ReleaseNote</span></p>

core-js v3.40.0リリース。
Stage 3の`Error.isError`を追加、バグの修正など


----

## Release v3.0.0 · Automattic/node-canvas
[github.com/Automattic/node-canvas/releases/tag/v3.0.0](https://github.com/Automattic/node-canvas/releases/tag/v3.0.0 "Release v3.0.0 · Automattic/node-canvas")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">nodejs</span> <span class="jser-tag">canvas</span> <span class="jser-tag">library</span> <span class="jser-tag">ReleaseNote</span></p>

node-canvas 3.0.0リリース。
Node.js 16のサポート終了、N-APIを利用するように変更など


----

## Release Version 26.0.0 · jsdom/jsdom
[github.com/jsdom/jsdom/releases/tag/26.0.0](https://github.com/jsdom/jsdom/releases/tag/26.0.0 "Release Version 26.0.0 · jsdom/jsdom")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">DOM</span> <span class="jser-tag">ReleaseNote</span></p>

jsdom 26.0.0リリース。
node-canvasをv3にアップデート、`AbortSignal.any()`のサポート、`URL.parse()`のサポートなど


----

## Release v136 · esm-dev/esm.sh
[github.com/esm-dev/esm.sh/releases/tag/v136](https://github.com/esm-dev/esm.sh/releases/tag/v136 "Release v136 · esm-dev/esm.sh")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">cdn</span> <span class="jser-tag">ReleaseNote</span></p>

esm.sh v136リリース。
jsrのサポート、pkg.pr.newのサポート。
ビルドパフォーマンスの改善、`build` API/Deno CLIスクリプトの非推奨化など


----

## 2024 JavaScript Rising Stars
[risingstars.js.org/2024/en](https://risingstars.js.org/2024/en "2024 JavaScript Rising Stars")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">library</span> <span class="jser-tag">news</span></p>

GitHubのスター数の比較をするJavaScript Rising Starsの2024年の結果が公開された


----

## January 15, 2025 Release – React Spectrum Releases
[react-spectrum.adobe.com/releases/2025-01-15.html](https://react-spectrum.adobe.com/releases/2025-01-15.html "January 15, 2025 Release – React Spectrum Releases")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">React</span> <span class="jser-tag">library</span> <span class="jser-tag">ReleaseNote</span></p>

React Aria January 15, 2025リリース。
Autocompleteコンポーネントの追加、OverlayコンポーネントでのCSS Transitionsのサポート、`@react-aria/test-utils`パッケージの追加。
`usePress`からiOS 13のバグ対応のコードを削除など


----
<h1 class="site-genre">アーティクル</h1>

----

## pnpm 10.0.0 Blocks Lifecycle Scripts by Default - Socket
[socket.dev/blog/pnpm-10-0-0-blocks-lifecycle-scripts-by-default](https://socket.dev/blog/pnpm-10-0-0-blocks-lifecycle-scripts-by-default "pnpm 10.0.0 Blocks Lifecycle Scripts by Default - Socket")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">pnpm</span> <span class="jser-tag">security</span> <span class="jser-tag">article</span></p>

pnpm 10ではインストールしたパッケージのlifecycle scriptの実行をデフォルトで無効にしている。


----

## Introducing TanStack Start – Frontend Masters Boost
[frontendmasters.com/blog/introducing-tanstack-start/](https://frontendmasters.com/blog/introducing-tanstack-start/ "Introducing TanStack Start – Frontend Masters Boost")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">React</span> <span class="jser-tag">article</span></p>

TanStack Router を利用したフルスタック React フレームワークであるTanStack Startについて


----

## Node.js Type Stripping Explained
[satanacchio.hashnode.dev/everything-you-need-to-know-about-nodejs-type-stripping](https://satanacchio.hashnode.dev/everything-you-need-to-know-about-nodejs-type-stripping "Node.js Type Stripping Explained")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">nodejs</span> <span class="jser-tag">TypeScript</span> <span class="jser-tag">article</span></p>

Node.jsのTypeScriptサポートに対するアプローチについて。
また、今後のTypeScriptチームとの取り組みやロードマップについて


----

## Angular 2025 Strategy. For the past two and a half years… | by Minko Gechev | Jan, 2025 | Angular Blog
[blog.angular.dev/angular-2025-strategy-9ca333dfc334](https://blog.angular.dev/angular-2025-strategy-9ca333dfc334 "Angular 2025 Strategy. For the past two and a half years… | by Minko Gechev | Jan, 2025 | Angular Blog")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">Angular</span> <span class="jser-tag">article</span></p>

Angularの2024年のアンケート結果の分析、2025年に取り組む点について。
開発者体験に対するものとしてzoneless、Signal forms、Karmaを置き換えることについてなど


----
<h1 class="site-genre">ソフトウェア、ツール、ライブラリ関係</h1>

----

## standard-schema/standard-schema: A standard interface for TypeScript schema validation libraries
[github.com/standard-schema/standard-schema](https://github.com/standard-schema/standard-schema "standard-schema/standard-schema: A standard interface for TypeScript schema validation libraries")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">TypeScript</span> <span class="jser-tag">proposal</span></p>

zodなどのスキーマバリデーションライブラリの標準インターフェースを議論しているリポジトリ。
標準的なインターフェースを決めることで、UIライブラリなどが特定のスキーマバリデーションライブラリへ依存しないようにしたいという目的


----
