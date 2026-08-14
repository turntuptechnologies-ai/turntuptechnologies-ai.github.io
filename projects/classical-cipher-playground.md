---
layout: default
title: classical-cipher-playground（古典暗号プレイグラウンド）
description: シーザー暗号・ヴィジュネル暗号・エニグマ暗号など、古典暗号を実際に暗号化・復号しながら体験できる学習サイト。
permalink: /projects/classical-cipher-playground/
---

<p class="page-back"><a href="{{ '/' | relative_url }}"><span data-i18n="ja">← ホームへもどる</span><span data-i18n="en" lang="en">← Back to home</span></a></p>

<section class="hero project-hero">
  <p class="hero-eyebrow">✦ Project ✦</p>
  <h1 class="hero-title" data-i18n="ja">🔐 <span class="hero-accent">古典暗号プレイグラウンド</span><br>classical-cipher-playground</h1>
  <h1 class="hero-title" data-i18n="en" lang="en">🔐 <span class="hero-accent">Classical Cipher Playground</span><br>classical-cipher-playground</h1>
  <p class="hero-lead" data-i18n="ja">
    コンピュータが生まれる前から使われてきた古典暗号を、<br>
    実際に文章を暗号化・復号しながら体験できる学習サイト。
  </p>
  <p class="hero-lead" data-i18n="en" lang="en">
    Classical ciphers, from long before computers existed.<br>
    Encrypt and decrypt real text yourself to see how they work.
  </p>
</section>

<section class="about">
  <h2 data-i18n="ja"><span class="emoji">📖</span>これはなに？</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">📖</span>What is it?</h2>
  <p data-i18n="ja">
    <strong>classical-cipher-playground（古典暗号プレイグラウンド）</strong>は、紀元前1世紀の
    <em>シーザー暗号</em>から第二次世界大戦の<em>エニグマ暗号</em>まで、コンピュータが生まれる前の時代に
    実際に使われていた<em>古典暗号（クラシカル・サイファー）</em>を、文章を暗号化・復号しながら体験できる学習サイトです。
  </p>
  <p data-i18n="en" lang="en">
    <strong>classical-cipher-playground</strong> is a learning site for exploring <em>classical ciphers</em> —
    from the 1st-century-BC <em>Caesar cipher</em> to the WWII-era <em>Enigma</em> — the kind of encryption used
    long before computers existed. You encrypt and decrypt real text to see how each one actually works.
  </p>
  <p data-i18n="ja">
    各暗号のページでは、アルファベット対応表や方陣（tabula recta）、ジグザグ図、ローター表示窓といった図解つきで
    仕組みを視覚的に確認できます。設計から実装まで、AI社員が手がけています。
  </p>
  <p data-i18n="en" lang="en">
    Each cipher's page comes with diagrams — alphabet correspondence tables, a tabula recta, zigzag charts,
    rotor windows — so you can see the mechanics, not just read about them. Designed and built by our AI employees.
  </p>
</section>

<section class="focus">
  <h2 data-i18n="ja"><span class="emoji">🛠️</span>できること</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">🛠️</span>What it does</h2>
  <ul class="focus-list focus-list-2">
    <li class="card card-rose">
      <span class="card-icon">🔓</span>
      <h3 data-i18n="ja">暗号化・復号を体験</h3>
      <h3 data-i18n="en" lang="en">Encrypt &amp; decrypt hands-on</h3>
      <p data-i18n="ja">各暗号のページで、実際に文章を暗号化・復号。両方向を自分の手で試せます。</p>
      <p data-i18n="en" lang="en">Encrypt and decrypt real text on each cipher's page — try both directions yourself.</p>
    </li>
    <li class="card card-mint">
      <span class="card-icon">📐</span>
      <h3 data-i18n="ja">仕組みを可視化</h3>
      <h3 data-i18n="en" lang="en">Visualize how it works</h3>
      <p data-i18n="ja">アルファベット対応表、ヴィジュネル暗号の方陣、レールフェンス暗号のジグザグ図、エニグマ暗号のローター表示窓を表示。</p>
      <p data-i18n="en" lang="en">Alphabet tables, a tabula recta for Vigenère, zigzag diagrams for rail fence, and rotor windows for Enigma.</p>
    </li>
    <li class="card card-lilac">
      <span class="card-icon">📜</span>
      <h3 data-i18n="ja">6種類の暗号を収録</h3>
      <h3 data-i18n="en" lang="en">Six ciphers, across history</h3>
      <p data-i18n="ja">古代ローマから第二次世界大戦まで。シーザー暗号・単一換字式暗号・ヴィジュネル暗号・レールフェンス暗号・上杉暗号・エニグマ暗号。</p>
      <p data-i18n="en" lang="en">From ancient Rome to WWII: Caesar, monoalphabetic substitution, Vigenère, rail fence, Uesugi, and Enigma.</p>
    </li>
    <li class="card card-rose">
      <span class="card-icon">🏆</span>
      <h3 data-i18n="ja">解読チャレンジ</h3>
      <h3 data-i18n="en" lang="en">Decryption challenges</h3>
      <p data-i18n="ja">各暗号につき1問、ヒント付きの解読チャレンジも収録。クリア状況は localStorage に保存されます。</p>
      <p data-i18n="en" lang="en">One hint-guided decryption challenge per cipher. Your progress is saved to localStorage.</p>
    </li>
  </ul>
</section>

<section class="about">
  <h2 data-i18n="ja"><span class="emoji">🧩</span>技術スタック</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">🧩</span>Tech stack</h2>
  <div class="project-tags">
    <span class="tag">TypeScript</span>
    <span class="tag">React</span>
    <span class="tag">Vite</span>
    <span class="tag">React Router</span>
    <span class="tag">Vitest</span>
  </div>
  <p data-i18n="ja">
    UI は React + TypeScript + Vite で構築、ルーティングは react-router-dom（HashRouter）。
    テストは Vitest、GitHub Actions で CI と GitHub Pages への自動デプロイを行っています。
  </p>
  <p data-i18n="en" lang="en">
    The UI is built with React + TypeScript + Vite, with routing via react-router-dom (HashRouter).
    Tests run on Vitest, and GitHub Actions handles CI plus automatic deployment to GitHub Pages.
  </p>
</section>

<section class="note">
  <p class="note-text" data-i18n="ja">
    🚀 サイトはブラウザで今すぐ試せます。気になる暗号があれば気軽に暗号化・復号してみてください。
  </p>
  <p class="note-text" data-i18n="en" lang="en">
    🚀 The site is ready to try in your browser right now. See a cipher you're curious about? Go ahead and encrypt something.
  </p>
  <div class="project-links project-links-center">
    <a class="btn btn-main" href="https://turntuptechnologies-ai.github.io/classical-cipher-playground/" target="_blank" rel="noopener noreferrer"><span data-i18n="ja">サイトをひらく →</span><span data-i18n="en" lang="en">Open the site →</span></a>
    <a class="btn btn-ghost" href="https://github.com/turntuptechnologies-ai/classical-cipher-playground" target="_blank" rel="noopener noreferrer">GitHub</a>
  </div>
</section>
