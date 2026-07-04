# Glossary — 用語集

このロードマップで頻出する用語の定義。新しい用語が出てきたら随時追記する。

## ロードマップ運用

| 用語 | 定義 |
| --- | --- |
| ADR | Architecture Decision Record。重要な意思決定を記録する文書。[adr/](../adr/) に保存 |
| SSOT | Single Source of Truth。唯一の正とする情報源。本リポジトリでは GitHub がロードマップの SSOT |
| 要公式確認 | 公式ページでの確認が済んでいない情報に付けるマーク。確認後に更新する |
| フェーズ | [roadmap.md](roadmap.md) で定義した学習の重心期間 |
| 成果物 | 学習の結果として作る、動くもの（リポジトリ / デプロイ / アプリ / 記事） |

## クラウド / Azure

| 用語 | 定義 |
| --- | --- |
| Entra ID | Microsoft の ID 管理サービス（旧 Azure AD） |
| Managed Identity | Azure リソースに自動付与される ID。シークレットなしで他リソースへ認証できる |
| Key Vault | シークレット・鍵・証明書を管理する Azure サービス |
| RU | Request Unit。Cosmos DB のスループット単位 |
| IaC | Infrastructure as Code。インフラをコードで定義・管理する手法（Terraform / Bicep など） |
| AKS | Azure Kubernetes Service |

## 認証・認可

| 用語 | 定義 |
| --- | --- |
| OAuth 2.0 | 認可のためのフレームワーク |
| OIDC | OpenID Connect。OAuth 2.0 上に構築された認証レイヤー |
| MSAL | Microsoft Authentication Library。Entra ID 認証用の公式ライブラリ |

## AI

| 用語 | 定義 |
| --- | --- |
| LLM | Large Language Model。大規模言語モデル |
| RAG | Retrieval-Augmented Generation。検索で取得した情報を LLM の生成に組み込む手法 |
| Agent | LLM がツールを使いながら複数ステップでタスクを遂行する仕組み |
| Embedding | テキスト等をベクトルに変換したもの。類似検索に使う |
| Vector Search | ベクトルの類似度に基づく検索 |
| Evaluation | AI 機能の品質を計測・評価すること（正確性、コスト、レイテンシ等） |

## Cloud Native / DevOps

| 用語 | 定義 |
| --- | --- |
| CNCF | Cloud Native Computing Foundation。Kubernetes 等をホストする財団 |
| Observability | ログ・メトリクス・トレースによりシステム内部状態を観測可能にすること |
| OpenTelemetry | Observability のためのオープンな計装標準 |
| SLO | Service Level Objective。サービスレベル目標 |
| CI/CD | 継続的インテグレーション / 継続的デリバリー |
