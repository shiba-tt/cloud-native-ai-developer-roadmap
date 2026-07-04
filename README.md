# Cloud Native AI Developer Roadmap

このリポジトリは、iOSエンジニアが数年かけて **Cloud Native AI Developer** へ成長するための、学習・資格・キャリア・個人開発ロードマップを管理する場所です。

## 目的

単なる資格取得リストではなく、学んだことを小さな成果物・個人開発プロダクト・運用経験へ接続し、継続的に更新できるロードマップを作ります。

## 最終ゴール

以下を一人で設計・実装・運用できる開発者になることを目指します。

- モバイルアプリ / Webアプリ
- Azure / Cloud Native なバックエンド
- AI / RAG / Agent を組み込んだアプリケーション
- SQL / NoSQL / Vector Search を含むデータ設計
- 認証・認可・セキュリティ設計
- CI/CD、IaC、監視、運用
- 個人開発プロダクトの企画・設計・実装・改善

## Cloud Native AI Developer の定義

Cloud Native AI Developer とは、クラウドネイティブな設計・運用の考え方を土台に、AIをアプリケーション価値へ変換できる開発者です。モデルやAPIを使うだけでなく、データ、認証、セキュリティ、運用、コスト、ユーザー体験まで含めて設計します。

## 現在地

- iOSエンジニアとして Swift / SwiftUI の実務経験がある
- Azure Developer Associate（AZ-204）取得済み
- Azure AI 系資格は、日本語情報・日本語受験対応・公式情報の安定性を確認しながら検討する
- 資格は目的ではなく、実装力・設計力・キャリア形成のための手段とする

## ロードマップ概要

1. Foundation Phase: AZ-204で得たAzure開発基盤を整理する
2. Data Platform Phase: SQL / NoSQL / Cosmos DB / データモデリングを学ぶ
3. Security & Identity Phase: Entra ID、OAuth / OIDC、Managed Identity、Key Vaultを扱う
4. Cloud Native Phase: Docker、Kubernetes、IaC、Observabilityを実践する
5. AI Application Phase: Azure AI、Azure OpenAI、RAG、Agent、Evaluationを学ぶ
6. Architecture & DevOps Phase: AZ-305、AZ-400、設計、CI/CD、運用設計を深める
7. Portfolio Phase: 学んだ内容を個人開発プロダクトとして公開・改善する

詳細は [docs/roadmap.md](docs/roadmap.md) を参照します。

## 推奨学習フェーズ

- まずは **Foundation / Data / Security** を固める
- 次に **Cloud Native / DevOps / Observability** で運用できる形にする
- その上で **AI Application** を実装し、評価・改善できるようにする
- 最後に **Portfolio** として成果物を統合する

## ディレクトリ構成

```text
.
├── docs/            # ビジョン、ロードマップ、スキル、資格、学習、運用
├── career/          # キャリア目標、ロール定義、マイルストーン
├── adr/             # 重要な意思決定記録
├── templates/       # 学習・資格・プロジェクト・ADRのテンプレート
└── .github/         # Issue Template / Pull Request Template
```

## 運用方針

- 月次レビューで学習実績・成果物・課題を記録する
- 四半期レビューでロードマップと優先順位を見直す
- 資格を検討するときは、必ず個人開発の成果物と結びつける
- 重要な方針変更はADRとして記録する

## AIエージェント利用方針

- ChatGPT、Codex、Claude CodeなどのAIエージェントを、調査、設計、レビュー、テンプレート作成に活用する
- AIの出力はドラフトとして扱い、最終判断は自分で行う
- 公式情報の確認、コスト、セキュリティ、運用影響は人間が責任を持って確認する

## 公式情報確認ルール

Microsoft資格を扱う場合は、必ず公式 Microsoft Learn の試験ページで以下を確認します。

- 試験名
- 言語
- 廃止日
- 後継資格
- 更新日
- 試験範囲

ブログ記事、SNS、古い教材の情報は参考情報に留め、最新判断には使いません。
