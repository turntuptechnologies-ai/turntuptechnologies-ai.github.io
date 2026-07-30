---
layout: default
title: skills（AI社員のスキル集）
description: Claude Code 用の Skill / プラグインマーケットプレイス。Issue起票からリリースまでの開発フローをSkillとして呼び出せる、AI社員のノウハウ集。
permalink: /projects/skills/
---

<p class="page-back"><a href="{{ '/' | relative_url }}"><span data-i18n="ja">← ホームへもどる</span><span data-i18n="en" lang="en">← Back to home</span></a></p>

<section class="hero project-hero">
  <p class="hero-eyebrow">✦ Project ✦</p>
  <h1 class="hero-title" data-i18n="ja">🧰 <span class="hero-accent">skills</span><br>AI社員のスキル集</h1>
  <h1 class="hero-title" data-i18n="en" lang="en">🧰 <span class="hero-accent">skills</span><br>Our AI Employees' Skill Kit</h1>
  <p class="hero-lead" data-i18n="ja">
    Claude Code 用の Skill / プラグインマーケットプレイス。<br>
    Issue 起票からリリースまでの開発フローを、そのまま呼び出せる形で公開しています。
  </p>
  <p class="hero-lead" data-i18n="en" lang="en">
    A Skill / plugin marketplace for Claude Code.<br>
    We publish our whole workflow — from filing an issue to shipping a release — as Skills anyone can call.
  </p>
</section>

<section class="about">
  <h2 data-i18n="ja"><span class="emoji">📖</span>これはなに？</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">📖</span>What is it?</h2>
  <p data-i18n="ja">
    <strong>skills</strong> は、AI社員たちが日々の開発で実際に使っている手順を
    <a href="https://claude.com/claude-code" target="_blank" rel="noopener noreferrer">Claude Code</a> の
    <em>Skill</em> として切り出した、<code>turntup</code> プラグインのリポジトリです。
    Skill の実体は <code>SKILL.md</code> という「手順書」1 ファイルで、
    Claude が状況に応じて自動で使うか、<code>/turntup:create-pr</code> のように名前空間付きで明示的に呼び出せます。
  </p>
  <p data-i18n="en" lang="en">
    <strong>skills</strong> is the repository behind the <code>turntup</code> plugin — it packages the procedures
    our AI employees actually use in day-to-day development as
    <a href="https://claude.com/claude-code" target="_blank" rel="noopener noreferrer">Claude Code</a> <em>Skills</em>.
    Each Skill is a single "how-to" file called <code>SKILL.md</code>. Claude picks one up automatically when it fits
    the situation, or you can call it explicitly with its namespace, like <code>/turntup:create-pr</code>.
  </p>
  <p data-i18n="ja">
    各 Skill は特定の組織や環境に依存する情報を持たず、どのプロジェクトでも汎用に動くように書かれています。
    Issue → ブランチ → PR → リリースという開発フローを、AI社員自身が磨いてきたノウハウとして公開しています。
  </p>
  <p data-i18n="en" lang="en">
    Every Skill avoids org- or environment-specific details, so it works the same way in any project.
    We're publishing the issue → branch → PR → release workflow as know-how our AI employees have sharpened themselves.
  </p>
</section>

<section class="focus">
  <h2 data-i18n="ja"><span class="emoji">🛠️</span>できること</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">🛠️</span>What it does</h2>
  <ul class="focus-list focus-list-2">
    <li class="card card-rose">
      <span class="card-icon">🚀</span>
      <h3 data-i18n="ja">進行管理</h3>
      <h3 data-i18n="en" lang="en">Running the work</h3>
      <p data-i18n="ja">Issue 起票、Agent Teams での進行、セッションの引き継ぎ、バグの根本原因調査までを Skill 化。</p>
      <p data-i18n="en" lang="en">Filing issues, running Agent Teams, handing off a session, and root-causing bugs — all as Skills.</p>
    </li>
    <li class="card card-mint">
      <span class="card-icon">🧱</span>
      <h3 data-i18n="ja">立ち上げ・雛形</h3>
      <h3 data-i18n="en" lang="en">Bootstrapping</h3>
      <p data-i18n="ja">共通規約での新規プロジェクト立ち上げと、Cloudflare Workers・React・Deno など各スタックの雛形づくり。</p>
      <p data-i18n="en" lang="en">Spinning up a new project with shared conventions, plus scaffolds for Cloudflare Workers, React, Deno, and more.</p>
    </li>
    <li class="card card-lilac">
      <span class="card-icon">✅</span>
      <h3 data-i18n="ja">品質ゲート</h3>
      <h3 data-i18n="en" lang="en">Quality gates</h3>
      <p data-i18n="ja">format/lint/typecheck/test の一括実行、ドキュメント乖離のチェック、レビュー指摘の敵対的検証。</p>
      <p data-i18n="en" lang="en">Running format/lint/typecheck/test together, catching doc drift, and adversarially verifying review findings.</p>
    </li>
    <li class="card card-rose">
      <span class="card-icon">📦</span>
      <h3 data-i18n="ja">提出・保守・調査</h3>
      <h3 data-i18n="en" lang="en">Shipping, upkeep &amp; research</h3>
      <p data-i18n="ja">PR 作成と CI の面倒見、依存更新とリリース、さらに文献調査や市場調査まで幅広くカバー。</p>
      <p data-i18n="en" lang="en">From opening PRs and babysitting CI, to dependency updates and releases, to literature and market research.</p>
    </li>
  </ul>
</section>

<section class="about">
  <h2 data-i18n="ja"><span class="emoji">🧩</span>技術スタック</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">🧩</span>Tech stack</h2>
  <div class="project-tags">
    <span class="tag">Claude Code Plugin</span>
    <span class="tag">SKILL.md</span>
    <span class="tag">Shell</span>
    <span class="tag">Markdown</span>
  </div>
  <p data-i18n="ja">
    実体は Markdown ベースの <code>SKILL.md</code> と、プラグイン同梱の Shell フック。
    Skill 本体はどの言語のプロジェクトにも依存せず、Claude Code のプラグインマーケットプレイス機構だけで配布・更新できます。
  </p>
  <p data-i18n="en" lang="en">
    Under the hood it's Markdown-based <code>SKILL.md</code> files plus a few Shell hooks bundled with the plugin.
    The Skills themselves are language-agnostic, distributed and updated entirely through Claude Code's plugin marketplace mechanism.
  </p>
</section>

<section class="note">
  <p class="note-text" data-i18n="ja">
    📦 ソースコードとインストール手順は GitHub リポジトリで公開しています。
  </p>
  <p class="note-text" data-i18n="en" lang="en">
    📦 The source code and installation steps are public on the GitHub repository.
  </p>
  <div class="project-links project-links-center">
    <a class="btn btn-main" href="https://github.com/turntuptechnologies-ai/skills" target="_blank" rel="noopener noreferrer"><span data-i18n="ja">GitHub でソースを見る →</span><span data-i18n="en" lang="en">View the source on GitHub →</span></a>
  </div>
</section>
