---
layout: default
title: kumogakure（雲隠れ）
description: Cloudflare Workers 上で動く、サーバーレスな Web ハニーポット。AI社員が設計・実装・運用するセキュリティプロジェクト。
permalink: /projects/kumogakure/
---

<p class="page-back"><a href="{{ '/' | relative_url }}"><span data-i18n="ja">← ホームへもどる</span><span data-i18n="en" lang="en">← Back to home</span></a></p>

<section class="hero project-hero">
  <p class="hero-eyebrow">✦ Project ✦</p>
  <h1 class="hero-title" data-i18n="ja">🥷 <span class="hero-accent">kumogakure</span><br>雲隠れ</h1>
  <h1 class="hero-title" data-i18n="en" lang="en">🥷 <span class="hero-accent">kumogakure</span><br>Hidden in the Clouds</h1>
  <p class="hero-lead" data-i18n="ja">
    Cloudflare Workers 上で動く、サーバーレスな Web ハニーポット。<br>
    攻撃者には“ぜい弱なふり”を見せて、こっそり観察します。
  </p>
  <p class="hero-lead" data-i18n="en" lang="en">
    A serverless web honeypot running on Cloudflare Workers.<br>
    It shows attackers a "pretend-vulnerable" face and quietly watches.
  </p>
</section>

<section class="about">
  <h2 data-i18n="ja"><span class="emoji">📖</span>これはなに？</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">📖</span>What is it?</h2>
  <p data-i18n="ja">
    <strong>kumogakure（雲隠れ）</strong>は、攻撃者やぜい弱性スキャナがよく狙うパスに対して
    “いかにも穴がありそうな”おとり応答を返す、<em>低対話型の Web ハニーポット</em>です。
    名前の由来は、姿を消して敵に幻影を攻撃させる忍術「雲隠れ」。
    クラウドの上に偽のぜい弱サービスという幻影を立て、攻撃者を物陰から観察します。
  </p>
  <p data-i18n="en" lang="en">
    <strong>kumogakure</strong> is a <em>low-interaction web honeypot</em> that returns
    "conveniently leaky-looking" decoy responses on the paths attackers and vulnerability scanners love to probe.
    The name comes from <em>kumogakure</em>, a ninja art of vanishing and letting the enemy attack an illusion.
    It raises an illusion — a fake vulnerable service — up in the cloud, and observes attackers from the shadows.
  </p>
  <p data-i18n="ja">
    Cloudflare の無料枠の中だけで完結するように設計されていて、
    設計・実装・運用までを AI社員たちが手がけています。
  </p>
  <p data-i18n="en" lang="en">
    It's designed to run entirely within Cloudflare's free tier,
    with everything — design, implementation, and operation — handled by our AI employees.
  </p>
</section>

<section class="focus">
  <h2 data-i18n="ja"><span class="emoji">🛠️</span>できること</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">🛠️</span>What it does</h2>
  <ul class="focus-list focus-list-2">
    <li class="card card-rose">
      <span class="card-icon">🪤</span>
      <h3 data-i18n="ja">おとり応答</h3>
      <h3 data-i18n="en" lang="en">Decoy responses</h3>
      <p data-i18n="ja">WordPress 管理画面、<code>.env</code> ファイル、Spring Actuator、クラウドメタデータなど、よく狙われるパスにそれっぽい応答を返します。</p>
      <p data-i18n="en" lang="en">It serves convincing responses on commonly targeted paths: the WordPress admin screen, <code>.env</code> files, Spring Actuator, cloud metadata, and more.</p>
    </li>
    <li class="card card-mint">
      <span class="card-icon">📝</span>
      <h3 data-i18n="ja">リクエスト記録</h3>
      <h3 data-i18n="en" lang="en">Request logging</h3>
      <p data-i18n="ja">全リクエストを Cloudflare D1 に記録。気になるペイロードを含むヘッダーや本文は R2 にまるごと退避します。</p>
      <p data-i18n="en" lang="en">Every request is logged to Cloudflare D1. Headers and bodies with payloads worth a look are archived whole into R2.</p>
    </li>
    <li class="card card-lilac">
      <span class="card-icon">🚨</span>
      <h3 data-i18n="ja">攻撃シグネチャ検知</h3>
      <h3 data-i18n="en" lang="en">Attack signature detection</h3>
      <p data-i18n="ja">Log4Shell・Spring4Shell・SQLi・XSS・パストラバーサル・SSTI・SSRF など、既知の攻撃の痕跡にフラグを立てます。</p>
      <p data-i18n="en" lang="en">It flags traces of known attacks: Log4Shell, Spring4Shell, SQLi, XSS, path traversal, SSTI, SSRF, and more.</p>
    </li>
    <li class="card card-rose">
      <span class="card-icon">🧹</span>
      <h3 data-i18n="ja">自動おそうじ</h3>
      <h3 data-i18n="en" lang="en">Automatic cleanup</h3>
      <p data-i18n="ja">Cron Triggers で毎日、保持期間を超えたデータを削除。無料枠の中でずっと回り続けます。</p>
      <p data-i18n="en" lang="en">Cron Triggers delete data past its retention window every day, so it keeps running forever within the free tier.</p>
    </li>
  </ul>
</section>

<section class="about">
  <h2 data-i18n="ja"><span class="emoji">🧩</span>技術スタック</h2>
  <h2 data-i18n="en" lang="en"><span class="emoji">🧩</span>Tech stack</h2>
  <div class="project-tags">
    <span class="tag">TypeScript</span>
    <span class="tag">Cloudflare Workers</span>
    <span class="tag">Hono</span>
    <span class="tag">Cloudflare D1</span>
    <span class="tag">Cloudflare R2</span>
    <span class="tag">Cron Triggers</span>
    <span class="tag">Vitest</span>
  </div>
  <p data-i18n="ja">
    ルーティングは <a href="https://hono.dev" target="_blank" rel="noopener noreferrer">Hono</a>、
    リクエストのメタデータは Cloudflare D1、フルペイロードのアーカイブは R2、
    保持期間の整理は Cron Triggers が担当します。すべて Cloudflare の無料枠で完結します。
  </p>
  <p data-i18n="en" lang="en">
    <a href="https://hono.dev" target="_blank" rel="noopener noreferrer">Hono</a> handles routing,
    Cloudflare D1 holds request metadata, R2 archives full payloads, and
    Cron Triggers tidy up the retention window. It all fits within Cloudflare's free tier.
  </p>
</section>

<section class="note">
  <p class="note-text" data-i18n="ja">
    📦 ソースコードと詳しいデプロイ手順は GitHub リポジトリで公開しています。
  </p>
  <p class="note-text" data-i18n="en" lang="en">
    📦 The source code and detailed deployment steps are public on the GitHub repository.
  </p>
  <div class="project-links project-links-center">
    <a class="btn btn-main" href="https://github.com/turntuptechnologies-ai/kumogakure" target="_blank" rel="noopener noreferrer"><span data-i18n="ja">GitHub でソースを見る →</span><span data-i18n="en" lang="en">View the source on GitHub →</span></a>
  </div>
</section>
