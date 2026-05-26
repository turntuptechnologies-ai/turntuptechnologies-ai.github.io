---
layout: default
title: terminarai（Linux CLI 見習い道場）
description: ブラウザだけで Linux の基本コマンドを練習できる学習サイト。AI社員が設計・実装する CLI 学習プロジェクト。
permalink: /projects/terminarai/
---

<p class="page-back"><a href="{{ '/' | relative_url }}">← ホームへもどる</a></p>

<section class="hero project-hero">
  <p class="hero-eyebrow">✦ Project ✦</p>
  <h1 class="hero-title">🖥️ <span class="hero-accent">terminarai</span><br>Linux CLI 見習い道場</h1>
  <p class="hero-lead">
    ブラウザだけで、Linux の基本コマンドを練習できる学習サイト。<br>
    仮想シェルで安全に手を動かしながら、CLI の基礎を身につけます。
  </p>
</section>

<section class="about">
  <h2><span class="emoji">📖</span>これはなに？</h2>
  <p>
    <strong>terminarai（ターミナライ）</strong>は、CLI をこれから学ぶ人のためのブラウザ完結の練習サイトです。
    名前は <code>terminal</code> と <em>見習い (minarai)</em> の合成語。
    実際の Linux 環境ではなく、ブラウザ上でエミュレートされた<em>仮想シェル</em>でコマンドを叩けるので、
    どんなに失敗しても安全です。
  </p>
  <p>
    チュートリアル形式で順序立てて基本を学び、自習問題で力試しができる構成を目指しています。
    バックエンドを持たない純粋な SPA として作られていて、設計から実装まで AI社員たちが手がけています。
  </p>
</section>

<section class="focus">
  <h2><span class="emoji">🛠️</span>できること</h2>
  <ul class="focus-list focus-list-2">
    <li class="card card-rose">
      <span class="card-icon">🎓</span>
      <h3>チュートリアル学習</h3>
      <p>第1〜2章、計10レッスンで基本コマンドを順番に学べます。進めるごとに少しずつ難しくなる構成です。</p>
    </li>
    <li class="card card-mint">
      <span class="card-icon">🧪</span>
      <h3>仮想シェル</h3>
      <p>ブラウザ上でファイルシステムとシェルをエミュレート。実環境を壊す心配ゼロで自由に試せます。</p>
    </li>
    <li class="card card-lilac">
      <span class="card-icon">⌨️</span>
      <h3>主要コマンド対応</h3>
      <p><code>pwd</code> <code>ls</code> <code>cd</code> <code>mkdir</code> <code>touch</code> <code>cat</code> <code>echo</code> <code>rm</code> <code>cp</code> <code>mv</code>、リダイレクト (<code>></code> <code>>></code>) も。Tab 補完つき。</p>
    </li>
    <li class="card card-rose">
      <span class="card-icon">💾</span>
      <h3>進捗ローカル保存</h3>
      <p>レッスンの進捗は localStorage に保存。バックエンド不要、ログイン不要で、続きからすぐ再開できます。</p>
    </li>
  </ul>
</section>

<section class="about">
  <h2><span class="emoji">🧩</span>技術スタック</h2>
  <div class="project-tags">
    <span class="tag">TypeScript</span>
    <span class="tag">React 19</span>
    <span class="tag">Vite</span>
    <span class="tag">Tailwind CSS v4</span>
    <span class="tag">React Router v7</span>
    <span class="tag">Vitest</span>
    <span class="tag">Biome</span>
  </div>
  <p>
    UI は React 19 + Tailwind CSS v4、ルーティングは React Router v7、テストは Vitest + Testing Library、
    リント・フォーマットは Biome。GitHub Pages へ GitHub Actions から自動デプロイしています。
  </p>
</section>

<section class="note">
  <p class="note-text">
    🚀 サイトはブラウザで今すぐ試せます。気になるコマンドがあれば気軽に叩いてみてください。
  </p>
  <div class="project-links project-links-center">
    <a class="btn btn-main" href="https://turntuptechnologies-ai.github.io/terminarai/" target="_blank" rel="noopener noreferrer">サイトをひらく →</a>
    <a class="btn btn-ghost" href="https://github.com/turntuptechnologies-ai/terminarai" target="_blank" rel="noopener noreferrer">GitHub</a>
  </div>
</section>
