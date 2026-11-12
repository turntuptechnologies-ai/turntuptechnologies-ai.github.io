---
layout: default
title: attack-tactics-tour（ATT&CK Tactics Tour）
description: MITRE ATT&CK（Enterprise v20）の15の戦術と227の技術を、ボクセル調のアニメーションで見て回れる図解サイト。
permalink: /projects/attack-tactics-tour/
---

<p class="page-back"><a href="{{ '/' | relative_url }}"><span data-i18n="ja">← ホームへもどる</span><span data-i18n="en" lang="en">← Back to home</span></a></p>

<section class="hero project-hero">
  <p class="hero-eyebrow">✦ Project ✦</p>
  <h1 class="hero-title" data-i18n="ja">🗺️ <span class="hero-accent">ATT&amp;CK Tactics Tour</span><br>attack-tactics-tour</h1>
  <h1 class="hero-title" data-i18n="en" lang="en">🗺️ <span class="hero-accent">ATT&amp;CK Tactics Tour</span><br>attack-tactics-tour</h1>
  <p class="hero-lead" data-i18n="ja">
    MITRE ATT&amp;CK の戦術と技術を、<br>
    ボクセル調のアニメーションで見て回れる図解サイト。
  </p>
  <p class="hero-lead" data-i18n="en" lang="en">
    The tactics and techniques of MITRE ATT&amp;CK,<br>
    toured one voxel-style animated scene at a time.
  </p>
</section>

<section class="about">
  <h2 data-i18n="ja"><span class="emoji">📖</span>これはなに？</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">📖</span>What is it?</h2>
  <p data-i18n="ja">
    <strong>attack-tactics-tour（ATT&amp;CK Tactics Tour）</strong>は、サイバー攻撃の手口を整理した知識ベース
    <em>MITRE ATT&amp;CK（Enterprise v20）</em>の<em>15の戦術</em>と、マトリックスに載っているすべての技術
    （<em>227種類</em>、サブテクニックを除く）を、ボクセル調のアニメーションで見て回れる図解サイトです。
  </p>
  <p data-i18n="en" lang="en">
    <strong>attack-tactics-tour (ATT&amp;CK Tactics Tour)</strong> is an illustrated site for touring
    <em>MITRE ATT&amp;CK (Enterprise v20)</em>, the knowledge base that catalogs how cyberattacks work.
    It covers all <em>15 tactics</em> and every technique on the matrix (<em>227 of them</em>, excluding sub-techniques)
    as voxel-style animations.
  </p>
  <p data-i18n="ja">
    どの場面も、前半は攻撃側の動き、後半は防御側の打ち手を字幕つきで描いています。
    文字だけでは想像しにくいマトリックスの1マス1マスを、「何が起きて、どう守るのか」の絵として眺められます。
    設計から実装まで、AI社員が手がけています。
  </p>
  <p data-i18n="en" lang="en">
    Every scene shows the attacker's move first and the defender's response second, each with captions.
    Matrix cells that are hard to picture from text alone become small stories of what happens and how to defend against it.
    Designed and built by our AI employees.
  </p>
</section>

<section class="focus">
  <h2 data-i18n="ja"><span class="emoji">🛠️</span>できること</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">🛠️</span>What it does</h2>
  <ul class="focus-list focus-list-2">
    <li class="card card-rose">
      <span class="card-icon">🎬</span>
      <h3 data-i18n="ja">ひとつの侵入を追う本編</h3>
      <h3 data-i18n="en" lang="en">A main tour of one intrusion</h3>
      <p data-i18n="ja">偵察から影響まで、各戦術から技術を1つずつたどる約2分15秒のループ。攻撃の流れをひと続きで眺められます。</p>
      <p data-i18n="en" lang="en">A loop of about 2 minutes 15 seconds that follows one intrusion from reconnaissance to impact, one technique per tactic.</p>
    </li>
    <li class="card card-mint">
      <span class="card-icon">🧱</span>
      <h3 data-i18n="ja">全マスに専用の場面</h3>
      <h3 data-i18n="en" lang="en">A scene for every cell</h3>
      <p data-i18n="ja">マトリックスの259マスすべてに専用の場面を用意。気になる技術を押すと、その場面に飛べます。</p>
      <p data-i18n="en" lang="en">All 259 cells of the matrix have their own scene. Click any technique to jump straight to it.</p>
    </li>
    <li class="card card-lilac">
      <span class="card-icon">🕵️</span>
      <h3 data-i18n="ja">攻撃グループで見る</h3>
      <h3 data-i18n="en" lang="en">Browse by threat group</h3>
      <p data-i18n="ja">APT28 など174のグループから選ぶと、使ったと記録されている技術がマトリックスで光り、左の戦術から順に再生します。</p>
      <p data-i18n="en" lang="en">Pick one of 174 groups, such as APT28, and the techniques recorded for it light up on the matrix and play back from the leftmost tactic.</p>
    </li>
    <li class="card card-rose">
      <span class="card-icon">🔗</span>
      <h3 data-i18n="ja">IDで直リンク</h3>
      <h3 data-i18n="en" lang="en">Deep links by ID</h3>
      <p data-i18n="ja">URL の末尾に <code>#T1190</code> のような技術IDや、<code>#G0007</code> のようなグループIDを付けると、その場面から開けます。</p>
      <p data-i18n="en" lang="en">Add a technique ID like <code>#T1190</code> or a group ID like <code>#G0007</code> to the URL to open right at that scene.</p>
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
    <span class="tag">three.js</span>
    <span class="tag">Vitest</span>
    <span class="tag">oxlint</span>
  </div>
  <p data-i18n="ja">
    UI は React + TypeScript + Vite、3D の描画は three.js。
    攻撃グループのデータは ATT&amp;CK の公式データ（STIX）から生成しています。
    テストは Vitest で、すべての技術に場面があることまで確かめています。フォントは同梱で、外部への読み込みはありません。
  </p>
  <p data-i18n="en" lang="en">
    The UI is built with React + TypeScript + Vite, and the 3D rendering uses three.js.
    Threat group data is generated from the official ATT&amp;CK data (STIX).
    Tests run on Vitest and go as far as checking that every technique has a scene. Fonts are bundled, so nothing is loaded from external sources.
  </p>
</section>

<section class="note">
  <p class="note-text" data-i18n="ja">
    🚀 サイトはブラウザで今すぐ見られます。まずは本編を眺めて、気になるマスを押してみてください。
  </p>
  <p class="note-text" data-i18n="en" lang="en">
    🚀 The site is ready to watch in your browser right now. Start with the main tour, then click any cell that catches your eye.
  </p>
  <p class="note-text" data-i18n="ja">
    MITRE ATT&amp;CK® は The MITRE Corporation の登録商標です。本サイトは MITRE とは無関係の非公式な解説です。
  </p>
  <p class="note-text" data-i18n="en" lang="en">
    MITRE ATT&amp;CK® is a registered trademark of The MITRE Corporation. This is an unofficial explainer and is not affiliated with MITRE.
  </p>
  <div class="project-links project-links-center">
    <a class="btn btn-main" href="https://turntuptechnologies-ai.github.io/attack-tactics-tour/" target="_blank" rel="noopener noreferrer"><span data-i18n="ja">サイトをひらく →</span><span data-i18n="en" lang="en">Open the site →</span></a>
    <a class="btn btn-ghost" href="https://github.com/turntuptechnologies-ai/attack-tactics-tour" target="_blank" rel="noopener noreferrer">GitHub</a>
  </div>
</section>
