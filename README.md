# nobinko / tobaccotaro

Cloud Infrastructure Engineer / Operations Automation  
Cloud infrastructure design, development, maintenance, and operations for enterprise systems, including financial-sector environments.  
金融系を含むエンタープライズ領域のシステム基盤について、クラウド基盤の設計・開発・保守運用を中心に関わっています。

<p>
  <a href="https://profile-site-8m6.pages.dev/">Portfolio / プロフィールサイト</a> ·
  <a href="https://x.com/nobinko">X (@nobinko)</a> ·
  <a href="https://tanktaktix.com">Play TankTaktix / 遊ぶ</a> ·
  <a href="https://github.com/nobinko/mtg-token">MTG Token Finder</a> ·
  <a href="https://github.com/nobinko/mtg-card-image-suggest">MTG Broadcast Assist Prototype</a>
</p>

I like building small systems that actually run, then improving them through real feedback.  
小さく動くものを作り、実際の反応を見ながら改善していくのが好きです。

---

## Current Focus / 最近やっていること

- Cloud infrastructure design, development, maintenance, and operations for enterprise systems, including financial-sector environments  
  金融系を含むエンタープライズ領域におけるクラウド基盤の設計・開発・保守運用
- Operations automation and reliability improvement  
  運用自動化と信頼性改善
- AI agent validation with Claude Code, Amazon Bedrock, AWS, and local LLMs  
  Claude Code、Amazon Bedrock、AWS、ローカルLLMを使ったAIエージェント検証
- Planning and running AI pilot programs and internal PoCs in enterprise environments  
  エンタープライズ領域でのAI関連パイロット・社内PoCの企画・推進
- Purchaser-side engineering judgment: estimation, architecture review, and vendor proposal validation  
  発注者側の技術判断。見積妥当性、アーキテクチャレビュー、ベンダー提案の検証
- Personal knowledge operations with Google Drive, Claude, and ChatGPT  
  Google Drive、Claude、ChatGPTを使った個人タスク・知識管理

---

## Featured Projects / 主要プロジェクト

### TankTaktix

Browser-based tactical tank game focused on readable combat, responsive controls, and map-driven strategy.

TankTaktix は、見やすい戦闘、反応のよい操作感、マップごとの戦術性を重視したブラウザ向けタンクゲームです。

**Now in Open Beta (since 2026-07-11).** One match takes about five minutes, no install needed.  
**オープンβ公開中（2026-07-11 開始）。** 1マッチ約5分、インストール不要でブラウザからすぐ遊べます。

![TankTaktix battle screen](https://profile-site-8m6.pages.dev/assets/tanktaktix-battle.svg)

**Technical highlights / 技術要素**

- TypeScript monorepo / TypeScript モノレポ
- Canvas 2D / Canvas 2D 描画
- Express + WebSocket / Express + WebSocket サーバ
- 20Hz game tick / 20Hz のゲーム進行
- Runtime geometry / 実行時ジオメトリ
- Bot players / Bot プレイヤー
- Cloud maps / クラウドマップ
- Map editor with share codes / share code で共有できる Map Editor
- Discord OAuth2 / Discord OAuth2 認証
- Supabase / Supabase 連携
- Self-hosted VPS with Caddy / 自己管理 VPS（Caddy）

**Links / リンク**

- Play / 遊ぶ: https://tanktaktix.com
- Discord: https://discord.gg/tb4sBzXjPG
- X / Twitter: https://x.com/TankTaktixGame
- Portfolio / プロフィールサイト: https://profile-site-8m6.pages.dev/
- Repo / リポジトリ: private for now / 現時点では非公開

### MTG Token Finder

Local web tool for MTG feature-match broadcast prep. Not a card search but a field prep sheet: it gathers current-format tournament decklists and lists the physical tokens, emblems, copies, and face-down helpers to pull from bulk, in an easy-to-find order.

フィーチャー卓の配信準備で、バルクのトークン束から必要な現物を抜き出すためのローカル Web ツールです。「カード検索」ではなく「現場の準備表」として、現環境の大会デッキリストからトークン・紋章・物理コピー・裏向き補助などの現物候補を探しやすい順に並べます。

**Technical / product notes / 技術・プロダクト要素**

- Format-aware decklist crawling (MTGO, MTGTop8, magic.gg, Hareruya) filtered to the current season  
  MTGO公式・MTGTop8・magic.gg・晴れる屋をフォーマット別に巡回し、現環境開始日で古いリストを除外
- Token-producer extraction with adoption counts and archetype trends  
  トークン生成カードの抽出と、採用デッキ数・アーキタイプ傾向の表示
- Japanese card names and images backfilled after the initial pass  
  日本語名・日本語画像の後追い補完
- Expansion / release-date sorting, unchecked-only filter, and print view  
  エキスパンション順・発売日順ソート、未チェックのみ表示、印刷用表示
- One-click local start via `start.bat`  
  `start.bat` ダブルクリックでローカル起動

**Link / リンク**

- Repo / リポジトリ: https://github.com/nobinko/mtg-token

Unofficial Fan Content. Card data and images belong to Wizards of the Coast.  
非公式 Fan Content です。カード画像・テキスト等の権利は Wizards of the Coast に帰属します。

### MTG Broadcast Assist Prototype

Prototype for helping MTG broadcast operators select likely card images from commentary, OCR, hand notes, and chat-derived hints.

MTGの実況・盤面OCR・ハンド公開メモ・チャット由来の情報からカード候補を出し、放送オペレーターが `Preview` と `Live` を分けて扱える補助プロトタイプです。

**Technical / product notes / 技術・プロダクト要素**

- Operator console and overlay view  
  オペレーター画面と配信用オーバーレイ表示
- Candidate evidence badges  
  候補カードごとの根拠バッジ
- Preview → Take Live workflow  
  Preview で確認してから Live に反映するワークフロー
- EN / JA / KO display language switching  
  英語・日本語・韓国語の表示切替
- OCR, speech recognition, deck-context, and manual hint inputs  
  OCR、音声認識、デッキ文脈、手入力ヒントの取り込み

**Link / リンク**

- Repo / リポジトリ: https://github.com/nobinko/mtg-card-image-suggest

---

## Work Style / 進め方

- Build small working systems and improve them through real feedback.  
  小さく動く仕組みを作り、実際の反応を見ながら改善します。
- Treat documentation, changelogs, verification notes, and gotchas as part of the product.  
  ドキュメント、変更履歴、検証メモ、落とし穴の記録もプロダクトの一部として扱います。
- Keep a clear boundary between public experiments and confidential work, especially when using AI-assisted development.  
  特にAI支援開発では、公開できる検証と業務上の機密情報を明確に分けます。

---

## Keywords / キーワード

`Cloud Infrastructure` `Enterprise Systems` `Financial-sector Environments` `Operations Automation` `AI-assisted Development` `TypeScript` `Node.js` `WebSocket` `Canvas 2D` `AWS` `Amazon Bedrock` `Supabase` `Caddy` `OCR` `Scryfall` `Broadcast Tools`
