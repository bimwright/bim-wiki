---
title: "bim-wiki"
updated: 2026-04-20
---

<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="360" />
</p>

<p align="center">
  📖 <a href="README.md">English</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.zh-CN.md">简体中文</a> · 日本語
</p>

---

# bim-wiki

> **注記:** これは公開[bim-wiki](https://github.com/bimwright/bim-wiki)ナレッジベース（CC-BY-SA 4.0）の**ステージング**リポジトリです。ここでコンテンツを準備した後、公開リポジトリに公開します。

これらのノートは自分のために書き始めました。BEP（BIM実行計画）を作成するたびに、ISO 19650と4つのベトナム通達（QĐ 347、QĐ 348、QĐ 1057、QĐ 2500）を相互参照して、今直面しているプロジェクトに実際に適用される用語を特定する必要がありました。そしてラップトップを閉じるたびに、そのマッピングを忘れてしまいました。

これが、書き留めたそのマッピングです。

**bim-wiki**は厳選されたBIMナレッジベースです。ISO 19650パート1〜6のベトナム語ファーストの要約と、ベトナムの規制状況（上記の4つのQĐに加え、Luật 60/2024、Nghị định 111/2024および175/2024、Circulars 09/2024および24/2025）を並べて掲載しています。さらに、概念ページ（CDE、LOIN、PIM/AIM、EIRカスケード、BEPテンプレート）も含まれ、標準と現地の実務の間で相互リンクされています。

52のマークダウンページ、CC-BY-SA 4.0、ソースからパラフレーズ（逐語的ではありません）。規範的なISOテキストが必要な場合は、iso.orgから購入してください。このWikiはその代替品ではありません。

## 対象読者

- 同じ文書内でISO 19650と国内規制の両方を扱っているベトナムのBIM実務者
- QĐ 348テンプレートに基づいてBEP / pre-BEPを作成しているコーディネーター
- どの用語が何を意味するのか（LOIN vs LOD、PIM vs AIM、フェデレーション vs アグリゲーション、CDE状態 vs 改訂状態）を見失いがちな学生やエンジニア
- BIMドメインの知識基盤を必要とするAIエージェント — 各ページは人間とLLMの両方が読めるように書かれています

## 内容

- **`summary_*.md`** — ソース文書（各ISO 19650パート、各ベトナム通達）の章レベルの要約
- **概念ページ** — `cde.md`、`eir.md`、`pim.md`、`loin.md`、`bep.md`、`lod-vn.md`、および他約13ページ。各ページ1トピック、相互リンク
- **ベトナム固有の差異** — `lod-vn.md`、`bim-applicability-matrix-vn.md`、`bep-template-qd348-variants.md`：ベトナムの実務がISOと異なる点とその理由
- **`iso-19650.md`** — シリーズの親ページ
- **`index.md`** — マスターカタログ

## 読み方

完全なカタログは[`index.md`](index.md)から始めるか、探しているものがすでにわかっている場合は概念ページに直接ジャンプしてください。

### ソース帰属タグ

各ページにはタグが付いており、各記述の背後にある根拠がわかります：

- `[ISO-CORE:verified]` — 生のISOテキストと照合済み（ローカルにリファレンスコピーを保持しています。ここで表現されているのは事実のみであり、文言ではありません）
- `[ISO-CORE:structure]` — ISOの節構造に従っていますが、逐語的には検証されていません
- `[VN-BXD:verified]` — ベトナム語のソースPDFと照合済み
- `[COMMENTARY]` — bimwrightの総合または比較
- `[INFERRED]` — どのソースにも直接記載されていない論理的推論

ある主張がプロジェクトにとって重要な場合は、それを信頼する前にタグ付けされたソースまでトレースしてください。

## ライセンスと帰属

ライセンスは**CC-BY-SA 4.0**です — [`LICENSE`](LICENSE)を参照してください。

このライセンスはbimwrightの**独自の貢献**（要約、パラフレーズ、選択、構成、解説）を対象としています。基礎となるソース標準に対する権利を付与するものでは**ありません**。ソースごとのポリシーについては[`NOTICE.md`](NOTICE.md)を参照してください。どのソースがフェアユース/フェアディーリングに基づいてパラフレーズされているか、どれがベトナム政府の著作物（パブリックドメイン）か、どれが元の権利者に帰属するかが記載されています。

規範的なISOテキストが必要な場合は、iso.orgから購入してください。このWikiはその代替品ではありません。

## コントリビューション

新しいページや修正についてはIssueを開いてください。プルリクエストについては[`NOTICE.md`](NOTICE.md)を参照してください。重要なルール：**パラフレーズし、貼り付けないでください。** ライセンスされた標準からの逐語的な引用は、たとえ編集が善意に基づき内容が正しくても、却下されます。二層モデルは、公開層がクリーンな状態を保つ場合にのみ機能します。

---

Part of the [bimwright](https://github.com/bimwright) family —
[rvt-mcp](https://github.com/bimwright/rvt-mcp) · [dwg-mcp](https://github.com/bimwright/dwg-mcp) · [nwd-mcp](https://github.com/bimwright/nwd-mcp) · [ipt-mcp](https://github.com/bimwright/ipt-mcp) · bim-wiki (this repo).

---

<p align="center">
  A <a href="https://github.com/bimwright">bimwright</a> project —
  <a href="https://github.com/bimwright"><img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" height="24" align="middle" /></a>
</p>
