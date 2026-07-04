# Cloud Native AI Developer Roadmap

iOS エンジニアが、数年かけて **Cloud Native AI Developer** になるための学習・資格・キャリア・個人開発ロードマップを管理するリポジトリです。

このリポジトリは、ChatGPT / Codex / Claude Code などの AI エージェントと一緒に、長期的に更新しながら使うことを前提としています。

## リポジトリの目的

- Cloud Native AI Developer になるための学習・資格・個人開発の計画を一元管理する
- 資格取得を「目的」ではなく「実装力・設計力・キャリア形成の手段」として位置づける
- 学んだ技術を必ず個人開発の成果物に落とし込むサイクルを回す
- 意思決定（ADR）とレビュー（月次・四半期）を記録し、方向修正できるようにする

## 最終ゴール

以下を **一人で設計・実装・運用できる開発者** になること。

- モバイルアプリ / Web アプリ
- Azure / Cloud Native なバックエンド
- AI / RAG / Agent を組み込んだアプリケーション
- SQL / NoSQL / Vector Search を含むデータ設計
- 認証・認可・セキュリティ設計
- CI/CD、IaC、監視、運用
- 個人開発プロダクトの企画・設計・実装・改善

## Cloud Native AI Developer の定義

> クラウドネイティブな基盤（コンテナ、Kubernetes、IaC、Observability）の上に、
> AI（LLM / RAG / Agent）を組み込んだアプリケーションを、
> データ設計・セキュリティ・運用まで含めてエンドツーエンドで作れる開発者。

詳細は [docs/vision.md](docs/vision.md) と [career/role-definition.md](career/role-definition.md) を参照。

## 現在地

- iOS エンジニア（Swift / SwiftUI の実務経験あり）
- Azure Developer Associate（AZ-204）取得済み
- Azure AI 系資格には興味があるが、日本語情報・日本語受験対応が安定してから取り組む方針

## ロードマップ概要

詳細は [docs/roadmap.md](docs/roadmap.md) を参照。

| フェーズ | テーマ | 主な内容 |
| --- | --- | --- |
| 1. Foundation | Azure 開発基盤 | AZ-204 の知識整理、クラウドアプリ開発の基礎固め |
| 2. Data Platform | データ | SQL / NoSQL / Cosmos DB / データモデリング、DP 系資格の検討 |
| 3. Security & Identity | 認証・認可 | Entra ID / OAuth / OIDC / Managed Identity / Key Vault、SC 系資格の検討 |
| 4. Cloud Native | コンテナ・IaC | Docker / Kubernetes / IaC / Observability、CNCF・HashiCorp 系資格の検討 |
| 5. AI Application | AI アプリ | Azure AI / Azure OpenAI / RAG / Agent / Evaluation、AI 系資格の検討 |
| 6. Architecture & DevOps | 設計・運用 | AZ-305 / AZ-400、システム設計、CI/CD、運用設計 |
| 7. Portfolio | 成果物 | 学んだ内容を個人開発プロダクトとして形にする |

## 推奨学習フェーズ

フェーズは厳密な直列ではなく、**「基盤 → データ → セキュリティ → クラウドネイティブ → AI → 設計/運用 → ポートフォリオ」** の順に重心を移していくイメージです。各フェーズで以下を必ずセットにします。

1. 学習（書籍 / 公式ドキュメント / Microsoft Learn）
2. ハンズオン（小さな検証プロジェクト）
3. 資格（必要な場合のみ、公式情報を確認したうえで）
4. 成果物（個人開発への反映）

## ディレクトリ構成

```text
.
├── README.md                  # 入口。全体方針
├── docs/
│   ├── vision.md              # ビジョン定義
│   ├── roadmap.md             # フェーズ別ロードマップ
│   ├── skill-tree.md          # スキルツリー
│   ├── principles.md          # 判断基準・原則
│   ├── glossary.md            # 用語集
│   ├── certification/         # 資格ロードマップ（Azure / Data / Security / AI / CNCF / GitHub / HashiCorp / その他）
│   ├── learning/              # 学習リソース（書籍 / コース / ハンズオン）
│   ├── projects/              # 個人開発（ポートフォリオロードマップ / アイデア）
│   └── operations/            # 運用（月次・四半期レビュー / 意思決定ログ）
├── career/                    # キャリア（年次目標 / マイルストーン / ロール定義）
├── adr/                       # Architecture Decision Records
├── templates/                 # 各種テンプレート
└── .github/                   # Issue / PR テンプレート
```

## 運用方針

- 学習・資格・プロジェクトは **GitHub Issue** で管理する（[Issue テンプレート](.github/ISSUE_TEMPLATE/)を使用）
- 月次で [templates/monthly-review.md](templates/monthly-review.md) を使って振り返りを行い、[docs/operations/](docs/operations/) に記録する
- 大きな方針変更は **ADR** として [adr/](adr/) に記録する（[テンプレート](templates/adr-template.md)）
- ロードマップは固定ではなく、レビューのたびに見直す

## AI エージェント利用方針

- ChatGPT / Codex / Claude Code などの AI エージェントを、調査・ドキュメント更新・コードレビュー・学習支援に積極的に活用する
- ただし **最終判断は必ず自分で行う**
- AI エージェントがこのリポジトリを更新する際は、既存の構成・フォーマットに従い、断定できない情報（試験の言語・廃止日など）には「要公式確認」と明記する
- AI の出力する資格情報・試験情報は古い可能性があるため、必ず公式情報で裏取りする

## 公式情報確認ルール

Microsoft 資格については、**必ず公式 Microsoft Learn の試験ページ**で以下を確認してから計画・受験する。

- 試験名
- 言語（日本語受験の可否）
- 廃止日（Retirement date）
- 後継資格
- 更新日（試験範囲の改訂日）
- 試験範囲（Skills measured / Study guide）

CNCF / GitHub / HashiCorp などの資格も同様に、各公式サイトで最新情報を確認する。ブログ記事や古い書籍の試験情報は参考程度に留め、鵜呑みにしない。
