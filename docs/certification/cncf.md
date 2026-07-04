# CNCF / Kubernetes 系資格

CNCF（Cloud Native Computing Foundation）系資格の候補と検討状況。Cloud Native Phase（[roadmap.md](../roadmap.md) Phase 4）に対応。

> **注**: 受験前に CNCF / Linux Foundation の公式サイトで、試験の現行バージョン・言語（日本語対応の有無）・受験形式・有効期限・再受験ポリシーを確認すること。

## 候補一覧

| 資格 | 領域 | 形式（想定） | ステータス | 備考 |
| --- | --- | --- | --- | --- |
| KCNA (Kubernetes and Cloud Native Associate) | クラウドネイティブ全般の入門 | 選択式（想定） | 🔍 検討中 | 入門として学習コスト低。取得価値は評価軸で判断 |
| CKAD (Certified Kubernetes Application Developer) | Kubernetes 上のアプリ開発 | 実技（想定） | 🔍 検討中 | **開発者として最も実用性が高い候補**。本命 |
| CKA (Certified Kubernetes Administrator) | クラスタ管理 | 実技(想定) | 🔍 検討中 | 管理者寄り。CKAD 後に必要性を判断 |
| CKS (Certified Kubernetes Security Specialist) | Kubernetes セキュリティ | 実技（想定） | 🔍 検討中 | CKA が前提条件のはず（要公式確認） |

## 検討メモ

- 実技試験（パフォーマンスベース）のため、「学習 = ハンズオン」となり [principles.md](../principles.md) の「成果物に落とし込む」原則と相性が良い
- 順序案: KCNA（任意）→ **CKAD（本命）** → CKA / CKS（必要になったら）
- 試験言語（日本語提供の有無）は変更されることがあるため要公式確認
- 資格の有効期限（数年で失効するはず）と更新ポリシーを公式で確認し、更新コストも評価に含める
- AKS を使う場合でも、素の Kubernetes の理解は移植可能なスキルとして価値が高い

## 成果物との紐付け

- CKAD → Kubernetes（AKS）上に API をデプロイし、CI/CD と監視を接続する（[portfolio-roadmap.md](../projects/portfolio-roadmap.md)）

## 公式確認ログ

| 日付 | 資格 | 確認内容（バージョン / 言語 / 形式 / 有効期限） | 結果 |
| --- | --- | --- | --- |
| （未実施） | - | - | - |
