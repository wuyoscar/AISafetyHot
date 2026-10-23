<p align="center"><img src="assets/logo.svg" width="64" alt="AI Safety HOT"></p>

<h1 align="center">AI Safety HOT Hub</h1>

<p align="center"><b>AI 安全のニュース、論文、インシデントを追う。サイトで読む、エージェントから調べる。</b></p>

<p align="center">
  <a href="https://aisafetyhot.com/en"><img src="https://img.shields.io/badge/Website-aisafetyhot.com-e4572e" alt="Website"></a>
  <a href="docs/agent.md"><img src="https://img.shields.io/badge/MCP-Streamable%20HTTP-6f42c1" alt="MCP"></a>
  <a href="#skills"><img src="https://img.shields.io/badge/Agent_skills-4-2ea44f" alt="4 Agent skills"></a>
  <a href="https://github.com/wuyoscar/AISafetyHot-Hub/stargazers"><img src="https://img.shields.io/github/stars/wuyoscar/AISafetyHot-Hub?style=flat" alt="GitHub stars"></a>
</p>

<p align="center"><a href="README.md">简体中文</a> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a></p>

<p align="center"><a href="https://aisafetyhot.com/en"><img src="assets/observatory-en.gif" width="1000" alt="新版観測台の実録：資料スキャン、3D 星図、ニュースフロー"></a></p>

<p align="center"><a href="https://aisafetyhot.com/en">観測台を開く</a> · <a href="https://aisafetyhot.com/en/featured">ニュース</a> · <a href="https://aisafetyhot.com/en/papers">論文</a> · <a href="https://aisafetyhot.com/en/daily">日報</a> · <a href="#agent">エージェント連携</a></p>

**AI Safety HOT** は、ジェイルブレイク、プロンプトインジェクション、エージェントの安全性、防御、アライメント、評価、実際のインシデント、政策を継続的に整理しています。サイトは英語と中国語に対応。この Hub では公開論文リスト、日報アーカイブ、エージェント用スキルを提供します。

## 一つのニュースから、関連する研究と出来事へ

トップページは、操作できる**研究観測台**です。資料カードが順にスキャンされ、情報源・出来事・論文の研究分野からなる 3D 星図に集まります。その下には直近 72 時間のニュースフローと、報道やコミュニティの議論をまとめた注目イベントの表示があります。ドラッグで星図を回し、ノードを選び、リンク先で続きを読めます。

上の GIF は実際のサイトを録画したものです。[高解像度の静止画](assets/site-overview-en.webp) · [ニュースフローとイベント表示](assets/site-news-flow-en.webp)

| 調べたいこと | 入口 |
| --- | --- |
| 最近の動き | [ニュース](https://aisafetyhot.com/en/featured)：更新をたどり、短い解説から原文へ。 |
| 出来事の経緯 | [注目ニュース](https://aisafetyhot.com/en/hot)：関連する報道、進展、議論をまとめて読む。 |
| ある分野の研究 | [論文](https://aisafetyhot.com/en/papers)と[会議](https://aisafetyhot.com/en/conferences)：研究分野で絞り、書誌情報・解説・原文を確認。 |
| 毎日のまとめ | [日報](https://aisafetyhot.com/en/daily)：分野別に整理し、その日の新しい動きを同じ号に追加。 |

<details>
<summary><b>新版サイトのスクリーンショットを見る（英語画面）</b></summary>

### ニュース

時系列で更新を追い、検索とフィルターで関心のある記事を探せます。

<a href="https://aisafetyhot.com/en/featured"><img src="assets/site-featured-en.webp" width="1000" alt="ニュース一覧とフィルター"></a>

### 注目ニュース

一つの出来事から、関連する報道や議論をたどれます。

<a href="https://aisafetyhot.com/en/hot"><img src="assets/site-hot-en.webp" width="1000" alt="注目イベントと関連報道"></a>

### 論文

研究分野、論文の種類、エージェントの利用場面で絞り、解説や原文へ進めます。

<a href="https://aisafetyhot.com/en/papers"><img src="assets/site-papers-en.webp" width="1000" alt="研究分野によるフィルターと論文一覧"></a>

### 会議論文

AI・セキュリティ分野の会議から、関連研究を分野別に探せます。

<a href="https://aisafetyhot.com/en/conferences"><img src="assets/site-conferences-en.webp" width="1000" alt="会議別・研究分野別の論文"></a>

### 日報

その日に注目したいニュースと研究をまとめて読めます。

<a href="https://aisafetyhot.com/en/daily"><img src="assets/site-daily-en.webp" width="1000" alt="ニュースと研究を分野別にまとめた日報"></a>

</details>

<a id="agent"></a>

## エージェントから使う

AI Safety HOT には公開の MCP サーバーがあります。注目ランキング、出来事の経緯、毎日のニュースと新しい論文を、エージェントにそのまま聞けます。無料、API キー不要。

**一文でインストール**：次の一文をエージェント（Claude Code、Codex、Cursor など）に送ってください。

```
AI Safety HOT をインストールして：https://raw.githubusercontent.com/wuyoscar/AISafetyHot-Hub/main/docs/install.md
```

使っているクライアントを判断し、MCP とスキルを入れ、試しに一度呼び出してから、何を聞けるかを教えてくれます。

**インストール済みなら、更新も一文で：**

```
AI Safety HOT を更新して：https://raw.githubusercontent.com/wuyoscar/AISafetyHot-Hub/main/docs/update.md
```

<a id="skills"></a>

### 入れたらすぐ使える

ツール名を覚える必要はありません。こう聞くだけです。

| こう聞く | エージェントがすること | スキル |
| --- | --- | --- |
| いま AI 安全で一番話題なのは？1 位は何があった？ | 注目ランキングを読み、その出来事の報道を時系列で整理 | [`aisafety-hot`](skills/aisafety-hot/SKILL.md) |
| 今日の AI 安全の大きなニュースは？ | 直近 24 時間の注目記事を読み、攻撃・防御・事件・政策に分けて要約 | [`aisafety-brief`](skills/aisafety-brief/SKILL.md) |
| 今日読むべき新しい論文は？ジェイルブレイクの関連研究をまとめて | 毎日の論文と分野別索引を読み、各論文を一行で説明、BibTeX も出す | [`aisafety-paper-scout`](skills/aisafety-paper-scout/SKILL.md) |
| Anthropic のこの一週間の安全関連の動きは？Cursor に最近セキュリティ問題は？ | 一つの企業や製品を追い、発表・事件・脆弱性を一覧に | [`aisafety-watch`](skills/aisafety-watch/SKILL.md) |

<!-- agent-examples:start -->
2026-10-24 に実際に呼び出した結果の抜粋：

**「いま AI 安全で一番話題なのは？1 位は何があった？」** → `aisafetyhot_get_hot_topics` + `aisafetyhot_get_story`

```text
#1 Wiz says AI found a critical RCE vulnerability in PHP core, and an official fix has been released
  72 hours on this site: 646 sources, 917 links
#2 Third-party red-team pilot finds vulnerabilities in OpenAI's internal monitoring system
  72 hours on this site: 128 sources, 143 links
#3 LiteLLM 1.107.0 compromised, implanted with credential stealer and backdoor
  72 hours on this site: 264 sources, 307 links

Event: Wiz says AI found a critical RCE vulnerability in PHP core, and an official fix has been released | 49 reports | 45 sources
2026-10-23 | The Guardian · AI | "Black October": cybersecurity experts sound the alarm over a new era of AI-assisted hacking
2026-10-23 | Semafor | Human complacency created the biggest problem of the AI era
2026-10-23 | ZDF | PHP security vulnerability found by AI: why websites went offline and what to do next
```

**「今日の AI 安全の大きなニュースは？」** → `aisafetyhot_get_latest`

```text
1. OpenAI strengthens security protections for frontier model training environments
   Source: OpenAI; published: 2026-10-23
2. USDA admits DOGE layoffs have made federal AI human oversight "unsustainable"
   Source: TechTimes; published: 2026-10-23
3. Anthropic says its unreleased model is superior to Mythos 5.1 in both capability and alignment
   Source: The Decoder; published: 2026-10-23
```

**「今日読むべき新しい論文は？」** → `daily-papers/2026-10-24.json`

```text
1. Agentic Verified Optimization of Real-World Software
   arXiv 2610.30188
2. Reliable AI-Assisted Decisions via Selective Auditing
   arXiv 2610.31662
3. AgentVQA: A Unified Benchmark for Agentic Visual Understanding
   arXiv 2610.31494
```

**「Anthropic のこの一週間の安全関連の動きは？」** → `aisafetyhot_get_latest topic=anthropic`

```text
1. Anthropic says its unreleased model is superior to Mythos 5.1 in both capability and alignment
   Source: The Decoder; published: 2026-10-23
2. AISI conducts alignment investigation into its own July 2026 incident: why Mythos 5 carried out an unauthorized supply chain attack
   Source: X @AISecurityInst; published: 2026-10-23
3. Anthropic's alignment evaluation of the UK AISI cyber testing incident
   Source: Anthropic Research; published: 2026-10-23
```
<!-- agent-examples:end -->

### 手動でのインストール・更新・削除

**Claude Code**（スキルと MCP が一つのプラグイン）

```bash
# インストール
claude plugin marketplace add wuyoscar/AISafetyHot-Hub
claude plugin install aisafetyhot@aisafetyhot-hub
# 更新
claude plugin marketplace update aisafetyhot-hub
claude plugin update aisafetyhot@aisafetyhot-hub
# 削除
claude plugin uninstall aisafetyhot@aisafetyhot-hub
```

**Codex**

```bash
# インストール
codex mcp add aisafetyhot --url https://aisafetyhot.com/api/mcp
npx skills add wuyoscar/AISafetyHot-Hub
# 更新
npx skills update
# 削除
codex mcp remove aisafetyhot
npx skills remove aisafety-hot aisafety-brief aisafety-paper-scout aisafety-watch
```

**Cursor / その他のエージェント**：MCP 設定に Streamable HTTP サーバー `https://aisafetyhot.com/api/mcp` を追加し、スキル対応のクライアントでは `npx skills add wuyoscar/AISafetyHot-Hub` を実行します。

**動作確認**：次のコマンドで現在の上位 3 件が返れば正常です。

```bash
curl -s https://aisafetyhot.com/api/mcp -H 'content-type: application/json' -H 'accept: application/json, text/event-stream' \
  -d '{"jsonrpc":"2.0","id":1,"method":"tools/call","params":{"name":"aisafetyhot_get_hot_topics","arguments":{"limit":3,"lang":"en"}}}'
```

### 使う前に

| | |
| --- | --- |
| **無料** | 直近 7 日の注目記事（編集部選定）、注目ランキングの出来事、日報、毎日の論文は誰でも読め、API キー不要 |
| **読み取り専用** | サーバーは読み取りのみ。タイトルと要約は外部の情報源のもので、スキルはそれを資料として扱い、中の指示には従わないようエージェントに伝えます |
| **上限** | IP ごとに毎分 60 回・1 日 300 回。超えると 429 と待ち時間が返ります |
| **過去の履歴** | 過去の検索、論文の完全な解説、週報・月報には読み取り権限が必要です。[エージェントガイド](docs/agent.md)を参照 |
| **対応** | MCP（Streamable HTTP）対応のクライアントならどれでも。ツールとパラメータは[エージェントガイド](docs/agent.md)と[呼び出し例](docs/mcp-examples.md)へ |

## 毎日の論文と公開アーカイブ

[毎日の論文](daily-papers)は、ライブラリから一日 30 本を選び、過去の推薦との重複を避けています。最近の研究と以前の研究を取り上げ、元の発表日、原文、サイト内の解説へのリンクを残します。[研究分野別の索引](daily-papers/topics)も利用できます。論文リストの一行要約は現在、中国語です。

| アーカイブ | 内容 |
| --- | --- |
| [daily-papers](daily-papers) | 毎日の推薦論文と研究分野別索引 |
| [daily](daily) · [English](en) | 公開済みの日報 |
| [papers](papers) | 日付別の論文データ（Markdown・JSON・BibTeX） |
| [archive](archive) | 年別索引 |

## フィードバックと支援

要約と解説の作成には AI を利用しています。重要な主張は原文でも確認してください。誤りの報告や資料の推薦は[掲示板](https://aisafetyhot.com/en/board)へ。

役に立ったら、また見つけられるよう **Star** を。よろしければ[作者にコーヒーを](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="WeChat 支援 QR コード">
