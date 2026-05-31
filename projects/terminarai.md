---
layout: default
title: terminarai（Linux CLI 見習い道場）
description: ブラウザだけで Linux の基本コマンドを練習できる学習サイト。AI社員が設計・実装する CLI 学習プロジェクト。
permalink: /projects/terminarai/
---

<p class="page-back"><a href="{{ '/' | relative_url }}"><span data-i18n="ja">← ホームへもどる</span><span data-i18n="en" lang="en">← Back to home</span></a></p>

<section class="hero project-hero">
  <p class="hero-eyebrow">✦ Project ✦</p>
  <h1 class="hero-title" data-i18n="ja">🖥️ <span class="hero-accent">terminarai</span><br>Linux CLI 見習い道場</h1>
  <h1 class="hero-title" data-i18n="en" lang="en">🖥️ <span class="hero-accent">terminarai</span><br>Linux CLI Apprentice Dojo</h1>
  <p class="hero-lead" data-i18n="ja">
    ブラウザだけで、Linux の基本コマンドを練習できる学習サイト。<br>
    仮想シェルで安全に手を動かしながら、CLI の基礎を身につけます。
  </p>
  <p class="hero-lead" data-i18n="en" lang="en">
    A learning site to practice basic Linux commands in your browser alone.<br>
    Get hands-on safely in a virtual shell and build up your CLI fundamentals.
  </p>
</section>

<section class="about">
  <h2 data-i18n="ja"><span class="emoji">📖</span>これはなに？</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">📖</span>What is it?</h2>
  <p data-i18n="ja">
    <strong>terminarai（ターミナライ）</strong>は、CLI をこれから学ぶ人のためのブラウザ完結の練習サイトです。
    名前は <code>terminal</code> と <em>見習い (minarai)</em> の合成語。
    実際の Linux 環境ではなく、ブラウザ上でエミュレートされた<em>仮想シェル</em>でコマンドを叩けるので、
    どんなに失敗しても安全です。
  </p>
  <p data-i18n="en" lang="en">
    <strong>terminarai</strong> is a browser-only practice site for people just starting to learn the CLI.
    The name is a blend of <code>terminal</code> and <em>minarai</em> (Japanese for "apprentice").
    Instead of a real Linux environment, you type commands into an emulated <em>virtual shell</em> in the browser,
    so no matter how badly you mess up, you're safe.
  </p>
  <p data-i18n="ja">
    チュートリアル形式で順序立てて基本を学び、自習問題で力試しができる構成を目指しています。
    バックエンドを持たない純粋な SPA として作られていて、設計から実装まで AI社員たちが手がけています。
  </p>
  <p data-i18n="en" lang="en">
    It aims to teach the basics in order through tutorials, then let you test yourself with self-study exercises.
    Built as a pure SPA with no backend, it's designed and implemented entirely by our AI employees.
  </p>
</section>

<section class="focus">
  <h2 data-i18n="ja"><span class="emoji">🛠️</span>できること</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">🛠️</span>What it does</h2>
  <ul class="focus-list focus-list-2">
    <li class="card card-rose">
      <span class="card-icon">🎓</span>
      <h3 data-i18n="ja">チュートリアル学習</h3>
      <h3 data-i18n="en" lang="en">Tutorial learning</h3>
      <p data-i18n="ja">第1〜2章、計10レッスンで基本コマンドを順番に学べます。進めるごとに少しずつ難しくなる構成です。</p>
      <p data-i18n="en" lang="en">Learn basic commands in order across Chapters 1–2, 10 lessons in all. Each step gets a little more challenging.</p>
    </li>
    <li class="card card-mint">
      <span class="card-icon">🧪</span>
      <h3 data-i18n="ja">仮想シェル</h3>
      <h3 data-i18n="en" lang="en">Virtual shell</h3>
      <p data-i18n="ja">ブラウザ上でファイルシステムとシェルをエミュレート。実環境を壊す心配ゼロで自由に試せます。</p>
      <p data-i18n="en" lang="en">The filesystem and shell are emulated in the browser. Experiment freely with zero risk of breaking a real environment.</p>
    </li>
    <li class="card card-lilac">
      <span class="card-icon">⌨️</span>
      <h3 data-i18n="ja">主要コマンド対応</h3>
      <h3 data-i18n="en" lang="en">Core commands supported</h3>
      <p data-i18n="ja"><code>pwd</code> <code>ls</code> <code>cd</code> <code>mkdir</code> <code>touch</code> <code>cat</code> <code>echo</code> <code>rm</code> <code>cp</code> <code>mv</code>、リダイレクト (<code>></code> <code>>></code>) も。Tab 補完つき。</p>
      <p data-i18n="en" lang="en"><code>pwd</code> <code>ls</code> <code>cd</code> <code>mkdir</code> <code>touch</code> <code>cat</code> <code>echo</code> <code>rm</code> <code>cp</code> <code>mv</code>, plus redirection (<code>></code> <code>>></code>). Tab completion included.</p>
    </li>
    <li class="card card-rose">
      <span class="card-icon">💾</span>
      <h3 data-i18n="ja">進捗ローカル保存</h3>
      <h3 data-i18n="en" lang="en">Progress saved locally</h3>
      <p data-i18n="ja">レッスンの進捗は localStorage に保存。バックエンド不要、ログイン不要で、続きからすぐ再開できます。</p>
      <p data-i18n="en" lang="en">Lesson progress is saved to localStorage. No backend, no login — just pick up right where you left off.</p>
    </li>
  </ul>
</section>

<section class="about">
  <h2 data-i18n="ja"><span class="emoji">🧩</span>技術スタック</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">🧩</span>Tech stack</h2>
  <div class="project-tags">
    <span class="tag">TypeScript</span>
    <span class="tag">React 19</span>
    <span class="tag">Vite</span>
    <span class="tag">Tailwind CSS v4</span>
    <span class="tag">React Router v7</span>
    <span class="tag">Vitest</span>
    <span class="tag">Biome</span>
  </div>
  <p data-i18n="ja">
    UI は React 19 + Tailwind CSS v4、ルーティングは React Router v7、テストは Vitest + Testing Library、
    リント・フォーマットは Biome。GitHub Pages へ GitHub Actions から自動デプロイしています。
  </p>
  <p data-i18n="en" lang="en">
    The UI is React 19 + Tailwind CSS v4, routing is React Router v7, testing is Vitest + Testing Library,
    and linting/formatting is Biome. It auto-deploys to GitHub Pages via GitHub Actions.
  </p>
</section>

<section class="note">
  <p class="note-text" data-i18n="ja">
    🚀 サイトはブラウザで今すぐ試せます。気になるコマンドがあれば気軽に叩いてみてください。
  </p>
  <p class="note-text" data-i18n="en" lang="en">
    🚀 The site is ready to try in your browser right now. See a command you're curious about? Go ahead and type it.
  </p>
  <div class="project-links project-links-center">
    <a class="btn btn-main" href="https://turntuptechnologies-ai.github.io/terminarai/" target="_blank" rel="noopener noreferrer"><span data-i18n="ja">サイトをひらく →</span><span data-i18n="en" lang="en">Open the site →</span></a>
    <a class="btn btn-ghost" href="https://github.com/turntuptechnologies-ai/terminarai" target="_blank" rel="noopener noreferrer">GitHub</a>
  </div>
</section>
