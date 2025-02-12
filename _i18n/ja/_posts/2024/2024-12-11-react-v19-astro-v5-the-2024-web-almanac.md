---
title: "2024-12-11のJS: React v19、Astro v5、The 2024 Web Almanac"
author: "azu"
layout: post
date: 2024-12-11T02:51:36.980Z
category: JSer
tags:
- React
- TypeScript
- Chrome
- document
- performance

---

JSer.info #718 - React v19がリリースされました。

- [React v19 – React](https://react.dev/blog/2024/12/05/react-19)
- [Release 19.0.0 (December 5, 2024) · facebook/react](https://github.com/facebook/react/releases/tag/v19.0.0)

2年半ぶりのメジャーリリースとなります。
非同期遷移を扱うアクションの概念の追加と`useActionState`/`useFormStatus`/`useOptimistic`/`use` APIの追加が行わなわれています。
また、react-domにprerender APIの追加、Server ComponentとServer Actionの追加が行われています。

そのほかの改善として、`ref`をpropsとして渡す際に`forwardRef`は不要に、Hydration Errorの改善、`ref` callbackがcleanup関数を返せるようになりました。
`<title>`/`<meta>`/`<link>`などのメタタグをサポート、`<link rel=stylesheet>`や`<script async={true} src=...>`のサポートも追加されています。
また、リソースのpreload APIのサポート、Custom Elementをサポートなども行われています。

Next.jsは15.1でReact v19のStableをサポートしています。

- [Next.js 15.1 | Next.js](https://nextjs.org/blog/next-15-1)

---

Astro 5.0がリリースされました。

- [Astro 5.0 | Astro](https://astro.build/blog/astro-5/)
- [astro/packages/astro/CHANGELOG.md at main · withastro/astro](https://github.com/withastro/astro/blob/main/packages/astro/CHANGELOG.md#500)

Content Layerの改善、Server Islands/astro:envをStableに、Vite 6へアップデートなどが行われています。

---

HTTP Archiveのデータを元にしたウェブのステータスをまとめたレポートであるThe 2024 Web Almanacがリリースされました。

- [The 2024 Web Almanac](https://almanac.httparchive.org/en/2024/)

HTML/CSS/JavaScript/Performance/Accessibility/SEO/Securityなど幅広い項目にわたって調査されたレポートがまとめられています。

----

{% include inline-support.html %}

----

<h1 class="site-genre">ヘッドライン</h1>

----

## React v19 – React
[react.dev/blog/2024/12/05/react-19](https://react.dev/blog/2024/12/05/react-19 "React v19 – React")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">React</span> <span class="jser-tag">ReleaseNote</span></p>

React 19リリース。
非同期遷移を扱うアクションの概念の追加と`useActionState`/`useFormStatus`/`useOptimistic`/`use` APIの追加。
react-domにprerender APIの追加、Server ComponentとServer Actionの追加。
`ref`をpropsとして渡す際に`forwardRef`は不要に、Hydration Errorの改善、`ref` callbackがcleanup関数を返せるように。
`<title>`/`<meta>`/`<link>`などのメタタグをサポート、`<link rel=stylesheet>`や`<script async={true} src=...>`をサポート。
リソースのpreload APIのサポート、Custom Elementをサポートなど

- [Release 19.0.0 (December 5, 2024) · facebook/react](https://github.com/facebook/react/releases/tag/v19.0.0 "Release 19.0.0 (December 5, 2024) · facebook/react")
- [Release v15.0.4 · vercel/next.js](https://github.com/vercel/next.js/releases/tag/v15.0.4 "Release v15.0.4 · vercel/next.js")

----

## ECMAScript proposal updates @ 2024-12 | ECMAScript Daily
[ecmascript-daily.github.io/ecmascript/2024/12/08/ecmascript-proposal-update](https://ecmascript-daily.github.io/ecmascript/2024/12/08/ecmascript-proposal-update "ECMAScript proposal updates @ 2024-12 | ECMAScript Daily")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">ECMAScript</span> <span class="jser-tag">news</span></p>

2024年12月のTC39ミーティングでのECMAScript Proposalのステータス変更のまとめ。
Sync Importsの追加、`Error.isError`がStage 3に、`Intl.DurationFormat`がStage 4となるなど


----

## Astro 5.0 | Astro
[astro.build/blog/astro-5/](https://astro.build/blog/astro-5/ "Astro 5.0 | Astro")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">astro</span> <span class="jser-tag">ReleaseNote</span></p>

Astro 5.0リリース。
Content Layerの改善、Server Islands/astro:envをStableに、Vite 6へアップデートなど

- [astro/packages/astro/CHANGELOG.md at main · withastro/astro](https://github.com/withastro/astro/blob/main/packages/astro/CHANGELOG.md#500 "astro/packages/astro/CHANGELOG.md at main · withastro/astro")

----

## Next.js 15.1 | Next.js
[nextjs.org/blog/next-15-1](https://nextjs.org/blog/next-15-1 "Next.js 15.1 | Next.js")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">Next.js</span> <span class="jser-tag">ReleaseNote</span></p>

Next.js 15.1リリース。
React 19 Stableに対応、Source Mapsの改善、エラースタックトレースの改善。
実験的な機能として`forbidden()`と`unauthorized()`を追加、`<link>`と`<style>`のインライン化の対応。


----
<h1 class="site-genre">アーティクル</h1>

----

## 改めて学ぶ satisfies 演算子
[zenn.dev/okkun/articles/ed6f146e03c60a](https://zenn.dev/okkun/articles/ed6f146e03c60a "改めて学ぶ satisfies 演算子")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">TypeScript</span> <span class="jser-tag">article</span></p>

TypeScriptの`satisfies`演算子の使い方について


----

## ニコニコ生放送のアプリケーションにRspackを導入している話
[zenn.dev/thiry/articles/0f671d086b2fb0](https://zenn.dev/thiry/articles/0f671d086b2fb0 "ニコニコ生放送のアプリケーションにRspackを導入している話")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">webpack</span> <span class="jser-tag">rspack</span> <span class="jser-tag">article</span></p>

webpackからrspackへの移行について。
css modules周りのいくつかの動作の問題があるが、ほとんどの部分でwebpackと互換性がある状態でbundleのパフォーマンスが改善できたという話


----

## Introducing Nuxt Icon v1 · Nuxt Blog
[nuxt.com/blog/nuxt-icon-v1-0](https://nuxt.com/blog/nuxt-icon-v1-0 "Introducing Nuxt Icon v1 · Nuxt Blog")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">Nuxt</span> <span class="jser-tag">article</span></p>

Nuxt Icon v1.0リリース。
アイコンロードの方法の比較とNuxt Iconでの実装について。
imgタグ/Webフォント/インラインSVG/動的なAPI/コンポーネント/CSSアイコンのアプローチの比較。
Nuxt Iconで時はCSSモードとSVGモードを両方サポートし、アイコンごとに切り替えられる。


----

## What&#039;s new in DevTools, Chrome 132  |  Blog  |  Chrome for Developers
[developer.chrome.com/blog/new-in-devtools-132?hl&#x3D;en](https://developer.chrome.com/blog/new-in-devtools-132?hl=en "What&#039;s new in DevTools, Chrome 132  |  Blog  |  Chrome for Developers")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">Chrome</span> <span class="jser-tag">article</span></p>

Chrome 132でのChrome DevToolsの変更点について。
AI assistanceの改善、パフォーマンスタブのNetworkパネルにそのリソースがレンダリングブロックしてるかを表示、`scheduler.postTask`の可視化など


----

## How To Improve INP: Yield Patterns | Jacob &#039;Kurt&#039; Groß
[kurtextrem.de/posts/improve-inp](https://kurtextrem.de/posts/improve-inp "How To Improve INP: Yield Patterns | Jacob &#039;Kurt&#039; Groß")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">React</span> <span class="jser-tag">performance</span> <span class="jser-tag">article</span></p>

ReactアプリケーションでInteraction-to-Next-Paint(INP)を改善するアプローチについての連載記事


----

## State of JavaScript 2024
[survey.devographics.com/survey/state-of-js/2024](https://survey.devographics.com/survey/state-of-js/2024 "State of JavaScript 2024")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">Survey</span></p>

JavaScriptについての開発者アンケートであるState of JavaScript 2024の募集が開始された


----

## A leap in the evolution of Airtable’s codebase: Scaling TypeScript to thousands of projects | by Michael Mitchell | The Airtable Engineering Blog | Dec, 2024 | Medium
[medium.com/airtable-eng/a-leap-in-the-evolution-of-airtables-codebase-scaling-typescript-to-thousands-of-projects-734326c3a553](https://medium.com/airtable-eng/a-leap-in-the-evolution-of-airtables-codebase-scaling-typescript-to-thousands-of-projects-734326c3a553 "A leap in the evolution of Airtable’s codebase: Scaling TypeScript to thousands of projects | by Michael Mitchell | The Airtable Engineering Blog | Dec, 2024 | Medium")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">TypeScript</span> <span class="jser-tag">article</span> <span class="jser-tag">performance</span></p>

Bazelを使ったTypeScriptの並列ビルドを最適化する話。
TypeScriptのプロジェクト同士が循環参照していたのをCopilotを使ってインターフェースの分離、Isolated Declarationsを使った並列ビルドができるような明示的な型付けなど


----
<h1 class="site-genre">サイト、サービス、ドキュメント</h1>

----

## CSS Wrapped 2024
[chrome.dev/css-wrapped-2024/](https://chrome.dev/css-wrapped-2024/ "CSS Wrapped 2024")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">browser</span> <span class="jser-tag">css </span> <span class="jser-tag">document</span> <span class="jser-tag">example</span> <span class="jser-tag">Chrome</span></p>

2024年にChromeへ追加されたCSSの機能を体験できるサイト。


----

## onlook-dev/onlook: The open source, local-first Figma for React. Design directly in your live React app and publish your changes to code.
[github.com/onlook-dev/onlook](https://github.com/onlook-dev/onlook "onlook-dev/onlook: The open source, local-first Figma for React. Design directly in your live React app and publish your changes to code.")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">React</span> <span class="jser-tag">figma</span> <span class="jser-tag">editor</span> <span class="jser-tag">software</span></p>

FigmaライクなUIでReactアプリケーションを編集できるエディタアプリ


----

## The 2024 Web Almanac
[almanac.httparchive.org/en/2024/](https://almanac.httparchive.org/en/2024/ "The 2024 Web Almanac")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">document</span> <span class="jser-tag">HTTP</span></p>

Web Almanacの2024年版が公開された。
HTTP Archiveのデータを元にしたウェブのステータスをまとめたレポート。


----
