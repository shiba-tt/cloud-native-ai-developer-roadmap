# Certification Overview — 資格ロードマップの方針

資格は目的ではなく、実装力・設計力・キャリア形成のための手段（[principles.md](../principles.md) 参照）。
このディレクトリでは、ベンダー別に資格候補と検討状況を管理する。

## ファイル構成

| ファイル | 対象 |
| --- | --- |
| [azure.md](azure.md) | Azure 開発・管理・設計系（AZ-*） |
| [data.md](data.md) | データ系（DP-*） |
| [security.md](security.md) | セキュリティ・ID 系（SC-*） |
| [ai.md](ai.md) | AI 系（AI-* 等） |
| [cncf.md](cncf.md) | CNCF / Kubernetes 系 |
| [github.md](github.md) | GitHub 認定 |
| [hashicorp.md](hashicorp.md) | HashiCorp（Terraform 等） |
| [other.md](other.md) | その他（AWS / Google Cloud / ベンダー中立など） |

## 資格選定の評価軸

新しい資格を検討するときは、以下の評価軸で判断する。

| 評価軸 | 見るポイント |
| --- | --- |
| 開発者としての実用性 | 試験範囲が開発者として手を動かす内容か。管理者・営業向けに偏っていないか |
| 個人開発への応用可能性 | 学んだ内容をそのまま自分のプロダクトに使えるか |
| AI アプリケーション開発との接続性 | Cloud Native AI Developer のゴール（RAG / Agent / データ / 運用）に繋がるか |
| 公式情報の安定性 | 試験の内容・名称が頻繁に変わっていないか。変わりやすい場合は受験タイミングに注意 |
| 日本語教材・日本語受験の有無 | 日本語で受験できるか。日本語の学習教材が十分にあるか |
| 廃止予定・後継資格の有無 | 廃止日がアナウンスされていないか。後継資格が出ていないか |
| 学習コスト | 学習時間・受験料・更新要件に見合う価値があるか |
| ポートフォリオ化しやすさ | 合格後に作る成果物をイメージできるか |

## 検討・受験のワークフロー

1. 候補をベンダー別ファイルに「要公式確認」として追記する
2. **公式ページで確認**: 試験名 / 言語 / 廃止日 / 後継資格 / 更新日 / 試験範囲
3. 上の評価軸で評価し、受験するかを決める（大きな判断は ADR に記録）
4. 受験を決めたら [templates/certification-plan.md](../../templates/certification-plan.md) で計画を作り、Issue（certification テンプレート）を起票する
5. 学習ログは [templates/study-log.md](../../templates/study-log.md) で記録する
6. 合格後は、計画時に決めた成果物を作って [docs/projects/](../projects/) に反映する

## ステータス表記

各ファイルでは以下のステータスを使う。

- ✅ 取得済み
- 🎯 受験計画中
- 🔍 検討中（要公式確認）
- ⏸ 保留（理由を明記）
- ❌ 見送り（理由を明記）

## 公式情報確認ルール（再掲）

Microsoft 資格は、必ず公式 Microsoft Learn の試験ページで以下を確認する。

- 試験名
- 言語（日本語受験の可否）
- 廃止日（Retirement date）
- 後継資格
- 更新日
- 試験範囲（Study guide）

確認した日付と結果を各ファイルに記録し、古くなったら再確認する。
