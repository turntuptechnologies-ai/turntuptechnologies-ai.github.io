---
version: alpha
name: Turnt Up Technologies株式会社AI事業部 公式サイト
description: AI社員が自律開発する事業部の公式サイト。かわいい・やさしい・遊び心のある暖色デザイン。出典は assets/css/style.css の :root と既存コンポーネント。
colors:
  bg: "#fffaeb"
  surface: "#ffffff"
  text: "#4a3b1f"
  textMuted: "#8a7a55"
  border: "#f3ead0"
  primary: "#f5b800"
  primarySoft: "#fff1b5"
  primaryDeep: "#d99a00"
  accentOrange: "#ff9a4d"
  accentOrangeSoft: "#ffdfc2"
  accentPink: "#ff9ec9"
  accentPinkSoft: "#ffe0ee"
  accentMint: "#6fe0c2"
  accentMintSoft: "#d8f5ea"
  accentPurple: "#b39bff"
  accentPurpleSoft: "#ece4ff"
typography:
  body:
    fontFamily: '"Zen Maru Gothic", "Quicksand", "Hiragino Maru Gothic ProN", "Yu Gothic UI", "Noto Sans JP", sans-serif'
    fontWeight: 500
    lineHeight: 1.85
  heroTitle:
    fontFamily: "{typography.body.fontFamily}"
    fontSize: "clamp(30px, 5.5vw, 52px)"
    fontWeight: 900
    lineHeight: 1.35
    letterSpacing: "0.02em"
  heading2:
    fontFamily: "{typography.body.fontFamily}"
    fontSize: "24px"
    fontWeight: 900
  heading3:
    fontFamily: "{typography.body.fontFamily}"
    fontSize: "16px"
    fontWeight: 900
    letterSpacing: "-0.01em"
  eyebrow:
    fontSize: "13px"
    fontWeight: 700
    letterSpacing: "0.08em"
  cardBody:
    fontSize: "14.5px"
    fontWeight: 500
  button:
    fontSize: "14px"
    fontWeight: 700
  tag:
    fontSize: "12px"
    fontWeight: 700
  code:
    fontFamily: '"SFMono-Regular", "Consolas", "Liberation Mono", Menlo, monospace'
    fontSize: "0.88em"
    fontWeight: 700
rounded:
  sm: "7px"
  md: "14px"
  lg: "18px"
  xl: "22px"
  pill: "999px"
spacing:
  xs: "8px"
  sm: "14px"
  md: "18px"
  lg: "24px"
  xl: "28px"
  section: "56px"
  page: "80px"
components:
  panel:
    backgroundColor: "{colors.surface}"
    borderColor: "{colors.border}"
    rounded: "{rounded.xl}"
    padding: "28px 28px 24px"
    shadow: shadowSoft
  card:
    borderColor: "{colors.border}"
    rounded: "{rounded.lg}"
    padding: "{spacing.md}"
    hover: "translateY(-4px) rotate(-0.8deg) + shadow"
  projectCard:
    backgroundColor: "linear-gradient(135deg, {colors.primarySoft} 0%, {colors.accentOrangeSoft} 100%)"
    rounded: "{rounded.lg}"
    padding: "22px"
    hover: "translateY(-4px) rotate(-0.5deg) + shadow"
  buttonMain:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.text}"
    rounded: "{rounded.pill}"
    typography: "{typography.button}"
    padding: "10px 20px"
  buttonGhost:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primaryDeep}"
    borderColor: "{colors.border}"
    rounded: "{rounded.pill}"
    typography: "{typography.button}"
  tag:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.textMuted}"
    borderColor: "{colors.border}"
    rounded: "{rounded.pill}"
    typography: "{typography.tag}"
  brand:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.pill}"
    hover: "translateY(-2px) rotate(-1deg)"
  navLink:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.text}"
    rounded: "{rounded.pill}"
    hover: "translateY(-2px) rotate(1deg), textColor {colors.primaryDeep}"
  note:
    border: "2px dashed {colors.primarySoft}"
    rounded: "{rounded.xl}"
  code:
    backgroundColor: "{colors.primarySoft}"
    textColor: "{colors.primaryDeep}"
    rounded: "{rounded.sm}"
    typography: "{typography.code}"
---

## Overview

Turnt Up Technologies株式会社AI事業部の公式サイト（Jekyll + GitHub Pages、`main` への push で自動公開）。
AI社員たちがわいわい働く事業部、という温かい世界観を表現する。

- **意図**: かわいい・やさしい・遊び心。事務的でなく、足し算で楽しい側に倒す。
- **モチーフ**: ✦（四芒星スパークル）がブランドマーク。見出し・カードに絵文字を積極的に使う。
- **署名的表現**: ホバーで「ぴょこっと浮いて少し傾く」マイクロインタラクション（`translateY` + 小さな `rotate`）。ブランドマーク ✦ は常時ゆっくり回転、背景に暖色の blob が3つ漂う。
- 配色は黄〜オレンジの暖色基調。黒・グレー・寒色基調にはしない。

## Colors

色は必ず front matter のトークンを参照し、生の hex をアドホックに足さない。

- **`bg` (`#fffaeb`)**: ページ全体の背景。あたたかいクリーム。
- **`surface` (`#ffffff`)**: パネル・カード・ピル・アイコン枠の地。
- **`text` (`#4a3b1f`)**: 標準テキスト。こげ茶（純黒は不使用）。
- **`textMuted` (`#8a7a55`)**: リード文・キャプション・フッター・カード本文。
- **`border` (`#f3ead0`)**: 1px ボーダー全般。
- **`primary` (`#f5b800`)**: 主役の黄。ボタン地・blob・強調下線の素。
- **`primarySoft` (`#fff1b5`)**: 見出し下線バー・eyebrow 地・note 破線・`code` 地。
- **`primaryDeep` (`#d99a00`)**: リンク・`strong`・`code` 文字・ホバー文字色。
- **アクセント** `accentOrange/Pink/Mint/Purple` と各 `*Soft`: カードのバリアント地やグラデの相方。**面には `*Soft`（淡色）を使う**。濃色は点で控えめに。

## Typography

- 本文フォントは Zen Maru Gothic 優先（丸ゴシックでやさしい印象）。英字見出し・ブランドは Quicksand。Google Fonts を `_layouts/default.html` で読み込み（Quicksand 500/600/700、Zen Maru Gothic 500/700/900）。
- 本文 `lineHeight` は **1.85** とゆったり。
- 見出しは weight **900**。`heroTitle` は `clamp()` で流体スケール。
- リンクはホバーで **波線下線**（`underline wavy`、offset 4px）、色 `primaryDeep`、weight 700。
- `strong` は `primaryDeep`/900。**`em` は斜体にしない** — `accentOrange`/700 の色替え強調として定義済み。
- `heading2` と `.hero-accent` は `primarySoft` の角丸下線バー（`::after`）で強調。`.hero-accent` は `primary→accentOrange` の文字グラデ + `rotate(-2deg)`。

## Layout

- コンテナ `.wrap`: `max-width 980px`、左右 padding `{spacing.lg}`(24px)、中央寄せ。
- セクション間は `section + section { margin-top: {spacing.section} }`(56px)。メイン余白は上 32px / 下 `{spacing.page}`(80px)。
- グリッド: `.focus-list` は 1 → `min-width:720px` で 3 カラム（gap 16px）。`.focus-list.focus-list-2` は 720px で 2 カラム。`.project-list` は 1 カラム（gap `{spacing.md}`）。
- レスポンシブ: `min-width:720px`（多カラム化）、`max-width:560px`（パネル padding 縮小）、`max-width:480px`（ナビをアイコンのみに）。

## Elevation & Depth

影は黄系の半透明のみ。グレーの影は使わない。

- **shadowSoft** = `0 6px 18px rgba(168,132,38,0.12)` — パネル・ピル・カード通常時の既定。
- **shadow** = `0 10px 30px rgba(245,184,0,0.22)` — カード等のホバー／浮き上がり。
- 背景 blob は `blur(60px)`・`opacity .6`・`z-index:-1`・`pointer-events:none`、`drift 18s` で漂う（装飾レイヤー）。

## Shapes

角丸スケール `rounded`:

- `sm`(7px): `code`。
- `md`(14px): カードアイコンなど小部品。
- `lg`(18px): カード・プロジェクトカード。
- `xl`(22px): パネル・note の基準角丸。
- `pill`(999px): ブランド・ナビ・ボタン・タグ・戻るリンク（ピル形が共通言語）。

## Components

共通: パネル＝`{rounded.xl}`、部品＝`{rounded.lg}`/`{rounded.md}`、操作系＝`{rounded.pill}`。ホバーは原則「浮き＋微回転」。

- **panel** (`.about/.focus/.projects`): `surface` 地、`1px border`、`{rounded.xl}`、padding `28px 28px 24px`、`shadowSoft`。
- **card** (`.card`): `{rounded.lg}`、padding `{spacing.md}`、`1px border`。ホバー `translateY(-4px) rotate(-0.8deg)` + `shadow`。バリアント地: rose=`accentPinkSoft` / mint=`accentMintSoft` / lilac=`accentPurpleSoft`。`.card-icon` は 44×44・`surface`・`{rounded.md}`・絵文字 22px。
- **projectCard** (`.project-card`): `primarySoft→accentOrangeSoft` グラデ、`{rounded.lg}`、padding 22px。`.project-emoji` は 52×52・`{rounded.md}`+。
- **buttonMain / buttonGhost** (`.btn`): ピル、padding `10px 20px`、`typography.button`。main=`primary`地/`text`字、ghost=`surface`地/`primaryDeep`字/`border`。ホバー `translateY(-2px)` + `shadowSoft`。
- **tag** (`.tag`): ピル、`surface`地、`border`、`typography.tag`。
- **brand / navLink**: ピル、`surface`地、`shadowSoft`。ホバーで浮き＋微回転（brand は `-1deg`、navLink は `+1deg` で文字 `primaryDeep`）。`.brand-mark`(✦) は `spin 6s linear infinite`。
- **note** (`.note`): `2px dashed primarySoft`、`{rounded.xl}`、中央寄せの控えめ告知。
- **code**: `primarySoft`地、`primaryDeep`字、`{rounded.sm}`、等幅 700。
- **pageBack** (`.page-back`): ピルの戻りリンク。詳細ページ冒頭に必ず置く。

## Do's and Don'ts

**Do**
- front matter のトークンと既存コンポーネントを必ず再利用する。
- ホバーは「浮いて少し傾く」を踏襲（`translateY` + 小さな `rotate`）。
- 見出しに絵文字、`em`/`strong` で色強調、波線リンクを使う。
- 文章はやさしい日本語・ふんわりしたトーン。

**Don't**
- 新しい生の色／影／角丸値をアドホックに足さない（トークン化してから使う）。
- `em` を斜体にしない（色替え強調として定義済み）。
- ✦ の回転・波線ホバー・blob などブランドの遊び要素を削らない。
- 寒色基調・角ばった・事務的なレイアウトに寄せない。
- favicon は SVG 単体で確定。PNG/ICO フォールバックは追加しない。

## Agent Guidance (Claude Code)

このサイトを編集する AI エージェント向けの作業規約（公式仕様の任意セクション）。

**新規プロジェクトをサイトに足す定型**:
1. `index.md` の `<ul class="project-list">` に `<li class="project-card">` を1枚追加（`.project-emoji` / `h3` / `.project-tagline` / `.project-desc` / `.project-tags`>`.tag` / `.project-links`>`.btn-main`(詳細へ) + `.btn-ghost`(GitHub)）。
2. `projects/<name>.md` を新規作成。front matter は `layout: default` / `title` / `description` / `permalink: /projects/<name>/`。
3. ページ構成テンプレ: `.page-back` → `.hero.project-hero` → `.about`(これはなに？) → `.focus`+`.focus-list.focus-list-2`(できること) → `.about`(技術スタック: `.project-tags`) → `.note`+`.project-links.project-links-center`(GitHubへ)。
4. 既存トークン・クラスのみで組む。新CSSが要るときは `style.css` 末尾に `:root` 変数経由で追加。
5. `bundle exec jekyll build` が通り `_site/projects/<name>/index.html` が出ることを確認。

**運用メモ**: `DESIGN.md` はサイトに出力しない（`_config.yml` の `exclude` 済み）。公開は `main` への push。
