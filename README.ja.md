<p align="center"><img src="assets/logo.svg" width="64" alt="AI Safety HOT"></p>

<h1 align="center">AI Safety HOT Hub</h1>

<p align="center"><b>AI 安全のニュース、論文、インシデントを追う。サイトで読む、エージェントから調べる。</b></p>

<p align="center">
  <a href="https://aisafetyhot.com/en"><img src="https://img.shields.io/badge/Website-aisafetyhot.com-e4572e" alt="Website"></a>
  <a href="docs/agent.md"><img src="https://img.shields.io/badge/MCP-Streamable%20HTTP-6f42c1" alt="MCP"></a>
  <a href="#skills"><img src="https://img.shields.io/badge/Agent_skills-6-2ea44f" alt="6 Agent skills"></a>
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

MCP サーバーを接続してスキルを入れれば、最近の動向、研究の手がかり、研究所、インシデントについて自然な言葉で質問できます。

**Claude Code** · スキルと MCP サーバーをインストール

```bash
/plugin marketplace add wuyoscar/AISafetyHot-Hub
/plugin install aisafetyhot@aisafetyhot-hub
```

**Codex**

```bash
npx skills add wuyoscar/AISafetyHot-Hub
codex mcp add aisafetyhot --url https://aisafetyhot.com/api/mcp
```

**Cursor / その他のエージェント** · `npx skills add wuyoscar/AISafetyHot-Hub` で対応するスキルを入れ、クライアントに `https://aisafetyhot.com/api/mcp` を Streamable HTTP の MCP サーバーとして追加してください。

最近のニュースの短い要約には API キーは不要です。過去の検索や論文解説の全文などには読み取り権限が必要です。範囲と設定は[エージェントガイド](docs/agent.md)を参照してください。サイトは無料で読めます。

<a id="skills"></a>

### 六つのスキル

| スキル | 用途 | 質問の例 |
| --- | --- | --- |
| [`aisafety-brief`](skills/aisafety-brief/SKILL.md) | 最近の安全動向 | 今週の AI 安全の主なニュースは？ |
| [`aisafety-paper-scout`](skills/aisafety-paper-scout/SKILL.md) | 論文と引用の手がかり | エージェントへのプロンプトインジェクションに関する論文を探して。 |
| [`aisafety-related-work`](skills/aisafety-related-work/SKILL.md) | 研究課題に沿った関連研究の整理 | この要旨を基に reward hacking の関連研究を整理して。 |
| [`aisafety-lab-watch`](skills/aisafety-lab-watch/SKILL.md) | 一つの研究所の動向 | Anthropic は今週、安全に関して何を発表した？ |
| [`aisafety-incident-check`](skills/aisafety-incident-check/SKILL.md) | インシデントや脆弱性の報道 | Cursor に関する最近のセキュリティ事例は？ |
| [`aisafetyhot`](skills/aisafetyhot/SKILL.md) | MCP ツールとクエリの説明 | ツール、フィルター、ページ送りの使い方を教えて。 |

[クエリの例を見る](docs/mcp-examples.md)

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
