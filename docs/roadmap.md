# Roadmap — フェーズ別ロードマップ

Cloud Native AI Developer になるための大きなフェーズ定義。
フェーズは厳密な直列ではなく「重心の移動」であり、月次・四半期レビューで随時見直す。

> **注**: 各フェーズに記載した資格はあくまで「検討候補」。受験を決める前に、必ず公式ページで試験名・言語・廃止日・後継資格を確認する（[docs/certification/overview.md](certification/overview.md) 参照）。

## フェーズ一覧

| # | フェーズ | 状態 |
| --- | --- | --- |
| 1 | Foundation Phase | 🔄 進行中（AZ-204 取得済み、知識整理中） |
| 2 | Data Platform Phase | ⏳ 未着手 |
| 3 | Security & Identity Phase | ⏳ 未着手 |
| 4 | Cloud Native Phase | ⏳ 未着手 |
| 5 | AI Application Phase | ⏳ 未着手 |
| 6 | Architecture & DevOps Phase | ⏳ 未着手 |
| 7 | Portfolio Phase | ⏳ 未着手（各フェーズと並行して常時実施） |

---

## 1. Foundation Phase — Azure 開発基盤の整理

**ゴール**: AZ-204 で得た知識を「使える知識」として整理し、クラウドアプリケーション開発の基礎を固める。

- AZ-204 で学んだサービス（App Service / Functions / Storage / Cosmos DB / Service Bus など）の知識マップを作る
- 小さな API + ストレージ構成のサンプルを実際にデプロイして動かす
- Azure のコスト管理・リソース管理（リソースグループ、タグ、Cost Management）の基本を身につける
- iOS アプリから Azure バックエンドを呼び出す最小構成を作る

**成果物例**: SwiftUI アプリ + Azure Functions + Cosmos DB の最小構成サンプル

## 2. Data Platform Phase — データ設計

**ゴール**: SQL / NoSQL を適材適所で選択・設計できるようになる。

- SQL の基礎〜中級（クエリ、インデックス、正規化）
- NoSQL / Cosmos DB（パーティション設計、RU、整合性レベル）
- データモデリング（リレーショナル vs ドキュメント vs グラフ）
- Vector Search の基礎（AI Phase への布石）
- **資格検討**: DP 系資格（DP-420 など。存在・言語・廃止日は要公式確認 → [certification/data.md](certification/data.md)）

**成果物例**: Cosmos DB を使ったモバイルバックエンドのデータ設計と実装

## 3. Security & Identity Phase — 認証・認可・セキュリティ

**ゴール**: 認証・認可を「ライブラリ任せ」ではなく仕組みから理解し、安全なアプリを設計できるようになる。

- Entra ID（テナント、アプリ登録、権限）
- OAuth 2.0 / OIDC のフローの理解と実装
- Managed Identity によるシークレットレス構成
- Key Vault によるシークレット・証明書管理
- モバイルアプリの認証ベストプラクティス（MSAL 等)
- **資格検討**: SC 系資格（SC-300 など。要公式確認 → [certification/security.md](certification/security.md)）

**成果物例**: Entra ID / OAuth / OIDC を使った iOS + API の認証サンプル

## 4. Cloud Native Phase — コンテナ・IaC・Observability

**ゴール**: コンテナベースのアプリケーションを IaC でプロビジョニングし、監視まで含めて運用できるようになる。

- Docker（イメージ設計、マルチステージビルド）
- Kubernetes（Pod / Deployment / Service / Ingress、AKS）
- IaC（Terraform / Bicep）
- Observability（ログ / メトリクス / トレース、OpenTelemetry、Azure Monitor）
- **資格検討**: CNCF 系（KCNA / CKAD など → [certification/cncf.md](certification/cncf.md)）、HashiCorp 系（Terraform Associate など → [certification/hashicorp.md](certification/hashicorp.md)）

**成果物例**: Kubernetes 上にデプロイした API、Terraform による Azure リソースの IaC 化

## 5. AI Application Phase — AI / RAG / Agent

**ゴール**: AI 機能を「デモ」ではなく「運用可能なアプリケーション」として組み込めるようになる。

- Azure AI 系サービスの全体像（Azure AI Foundry / Azure OpenAI など。サービス名・構成は変化が激しいため要公式確認）
- プロンプト設計、構造化出力、ツール呼び出し
- RAG（チャンキング、埋め込み、Vector Search、ハイブリッド検索）
- Agent（ツール使用、マルチステップ、ガードレール）
- Evaluation（品質評価、回帰テスト、コスト・レイテンシ計測）
- **資格検討**: AI 系資格（変更が激しいため必ず公式確認 → [certification/ai.md](certification/ai.md)。日本語受験対応が安定してから着手する方針）

**成果物例**: 自分のデータを使った RAG アプリ、タスクを自動化する Agent アプリ

## 6. Architecture & DevOps Phase — 設計と運用

**ゴール**: システム全体の設計判断と、継続的デリバリー・運用設計ができるようになる。

- システム設計（可用性、スケーラビリティ、コスト、トレードオフの言語化）
- CI/CD（GitHub Actions、環境分離、デプロイ戦略）
- 運用設計（SLO、アラート、インシデント対応、コスト最適化）
- **資格検討**: AZ-305（Solutions Architect）、AZ-400（DevOps Engineer）（要公式確認 → [certification/azure.md](certification/azure.md)）

**成果物例**: CI/CD と監視を含むデリバリーパイプライン一式

## 7. Portfolio Phase — 個人開発プロダクト化

**ゴール**: 学んだ内容をすべて統合した個人開発プロダクトを企画・実装・リリース・運用する。

- 各フェーズの成果物を「動くサンプル」から「使われるプロダクト」へ昇華させる
- 企画 → MVP → リリース → 計測 → 改善のサイクルを回す
- 詳細は [docs/projects/portfolio-roadmap.md](projects/portfolio-roadmap.md) を参照

> Portfolio Phase は最後にまとめて行うのではなく、**各フェーズの成果物づくりとして常に並行して進める**。
