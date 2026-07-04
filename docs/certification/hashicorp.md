# HashiCorp 系資格

HashiCorp 認定資格の候補と検討状況。Cloud Native Phase の IaC 領域（[roadmap.md](../roadmap.md) Phase 4）に対応。

> **注**: 受験前に HashiCorp 公式の認定資格ページで、試験の現行バージョン・言語（日本語対応の有無）・有効期限・前提条件を確認すること。Terraform はライセンス変更や OpenTofu の登場など周辺状況の変化もあるため、エコシステムの動向も合わせて確認する。

## 候補一覧

| 資格 | 領域 | ステータス | 備考 |
| --- | --- | --- | --- |
| Terraform Associate | Terraform の基礎〜実務 | 🔍 検討中 | IaC 学習の体系化として有力候補。試験バージョン（003 等）は要公式確認 |
| Terraform Authoring and Operations Professional | Terraform の上級（実技想定） | 🔍 検討中 | Associate 後に検討。前提条件・形式を要公式確認 |
| Vault Associate | シークレット管理 | 🔍 検討中 | Azure Key Vault を基本とするため優先度低。必要になったら評価 |

## 検討メモ

- Azure では Bicep という選択肢もあるため、**Terraform と Bicep の使い分け方針を先に ADR で決める**（マルチクラウド可搬性 vs Azure 統合）
- 資格の有効期限（2 年のはず。要公式確認）と更新コストを評価に含める
- 学習はこのリポジトリの成果物（Azure リソースの IaC 化）を教材にする

## 成果物との紐付け

- Terraform Associate → 個人開発プロダクトの Azure リソースを Terraform で IaC 化（[portfolio-roadmap.md](../projects/portfolio-roadmap.md)）

## 公式確認ログ

| 日付 | 資格 | 確認内容（バージョン / 言語 / 有効期限） | 結果 |
| --- | --- | --- | --- |
| （未実施） | - | - | - |
