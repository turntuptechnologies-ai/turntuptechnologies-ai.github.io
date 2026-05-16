---
layout: default
title: kumogakure（雲隠れ）
description: Cloudflare Workers 上で動く、サーバーレスな Web ハニーポット。AI社員が設計・実装・運用するセキュリティプロジェクト。
permalink: /projects/kumogakure/
---

<p class="page-back"><a href="{{ '/' | relative_url }}">← ホームへもどる</a></p>

<section class="hero project-hero">
  <p class="hero-eyebrow">✦ Project ✦</p>
  <h1 class="hero-title">🥷 <span class="hero-accent">kumogakure</span><br>雲隠れ</h1>
  <p class="hero-lead">
    Cloudflare Workers 上で動く、サーバーレスな Web ハニーポット。<br>
    攻撃者には“ぜい弱なふり”を見せて、こっそり観察します。
  </p>
</section>

<section class="about">
  <h2><span class="emoji">📖</span>これはなに？</h2>
  <p>
    <strong>kumogakure（雲隠れ）</strong>は、攻撃者やぜい弱性スキャナがよく狙うパスに対して
    “いかにも穴がありそうな”おとり応答を返す、<em>低対話型の Web ハニーポット</em>です。
    名前の由来は、姿を消して敵に幻影を攻撃させる忍術「雲隠れ」。
    クラウドの上に偽のぜい弱サービスという幻影を立て、攻撃者を物陰から観察します。
  </p>
  <p>
    Cloudflare の無料枠の中だけで完結するように設計されていて、
    設計・実装・運用までを AI社員たちが手がけています。
  </p>
</section>

<section class="focus">
  <h2><span class="emoji">🛠️</span>できること</h2>
  <ul class="focus-list focus-list-2">
    <li class="card card-rose">
      <span class="card-icon">🪤</span>
      <h3>おとり応答</h3>
      <p>WordPress 管理画面、<code>.env</code> ファイル、Spring Actuator、クラウドメタデータなど、よく狙われるパスにそれっぽい応答を返します。</p>
    </li>
    <li class="card card-mint">
      <span class="card-icon">📝</span>
      <h3>リクエスト記録</h3>
      <p>全リクエストを Cloudflare D1 に記録。気になるペイロードを含むヘッダーや本文は R2 にまるごと退避します。</p>
    </li>
    <li class="card card-lilac">
      <span class="card-icon">🚨</span>
      <h3>攻撃シグネチャ検知</h3>
      <p>Log4Shell・Spring4Shell・SQLi・XSS・パストラバーサル・SSTI・SSRF など、既知の攻撃の痕跡にフラグを立てます。</p>
    </li>
    <li class="card card-rose">
      <span class="card-icon">🧹</span>
      <h3>自動おそうじ</h3>
      <p>Cron Triggers で毎日、保持期間を超えたデータを削除。無料枠の中でずっと回り続けます。</p>
    </li>
  </ul>
</section>

<section class="about">
  <h2><span class="emoji">🧩</span>技術スタック</h2>
  <div class="project-tags">
    <span class="tag">TypeScript</span>
    <span class="tag">Cloudflare Workers</span>
    <span class="tag">Hono</span>
    <span class="tag">Cloudflare D1</span>
    <span class="tag">Cloudflare R2</span>
    <span class="tag">Cron Triggers</span>
    <span class="tag">Vitest</span>
  </div>
  <p>
    ルーティングは <a href="https://hono.dev" target="_blank" rel="noopener noreferrer">Hono</a>、
    リクエストのメタデータは Cloudflare D1、フルペイロードのアーカイブは R2、
    保持期間の整理は Cron Triggers が担当します。すべて Cloudflare の無料枠で完結します。
  </p>
</section>

<section class="note">
  <p class="note-text">
    📦 ソースコードと詳しいデプロイ手順は GitHub リポジトリで公開しています。
  </p>
  <div class="project-links project-links-center">
    <a class="btn btn-main" href="https://github.com/turntuptechnologies-ai/kumogakure" target="_blank" rel="noopener noreferrer">GitHub でソースを見る →</a>
  </div>
</section>
