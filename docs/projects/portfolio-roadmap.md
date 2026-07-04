# Portfolio Roadmap — 資格・学習と成果物の対応

「学んだこと・取得した資格」を「作る成果物」に紐付けるロードマップ。
資格は検討候補の段階でも、対応する成果物は資格の有無に関係なく作る。

> 資格名はすべて「要公式確認」の候補（[docs/certification/](../certification/)) 参照）。

## 対応表

| 資格 / 学習領域 | 成果物 | フェーズ | ステータス |
| --- | --- | --- | --- |
| AZ-204（取得済み） | SwiftUI アプリ + Azure Functions + Cosmos DB の最小構成サンプル | 1. Foundation | 📋 予定 |
| DP-420（候補） / データ設計 | Cosmos DB を使ったモバイルバックエンド（パーティション設計ドキュメント付き） | 2. Data Platform | 📋 予定 |
| SC-300（候補） / 認証認可 | Entra ID / OAuth / OIDC を使った iOS + API の認証サンプル（MSAL、Managed Identity、Key Vault） | 3. Security & Identity | 📋 予定 |
| CKAD（候補） / Kubernetes | Kubernetes（AKS）上に API をデプロイ（Helm チャート、Ingress、オートスケール） | 4. Cloud Native | 📋 予定 |
| Terraform Associate（候補） / IaC | 上記の Azure リソース一式を Terraform で IaC 化（環境分離付き） | 4. Cloud Native | 📋 予定 |
| AI 系資格（候補） / RAG・Agent | 自分のデータを使った RAG アプリ + タスク自動化 Agent（Evaluation 付き） | 5. AI Application | 📋 予定 |
| AZ-400（候補） / DevOps | CI/CD と監視を含むデリバリーパイプライン（GitHub Actions、OpenTelemetry、アラート） | 6. Architecture & DevOps | 📋 予定 |
| AZ-305（候補） / 設計 | 個人開発プロダクトのアーキテクチャ設計書 + ADR 一式 | 6. Architecture & DevOps | 📋 予定 |

## 統合プロダクト（最終形）

各成果物は独立させず、**1 つの個人開発プロダクトに段階的に統合していく**ことを目指す。

```text
iOS アプリ (SwiftUI)
   │
   ├─ 認証: Entra ID / OIDC (Phase 3)
   ▼
API (コンテナ / AKS or Container Apps)  ← CI/CD (Phase 6)
   │                                     ← IaC: Terraform (Phase 4)
   ├─ データ: Cosmos DB + Vector Search (Phase 2)
   ├─ AI: RAG / Agent (Phase 5)
   └─ 監視: OpenTelemetry + Azure Monitor (Phase 4, 6)
```

具体的なプロダクト案は [ideas.md](ideas.md) で管理し、Foundation Phase の間に 1 つ選定する。

## 成果物の完了条件（共通）

- [ ] リポジトリに README（目的・アーキテクチャ図・使用技術）がある
- [ ] 再現可能（IaC またはセットアップ手順）である
- [ ] シークレットがコードに含まれていない
- [ ] コスト上限が設定されている
- [ ] 学びが月次レビューに記録されている
