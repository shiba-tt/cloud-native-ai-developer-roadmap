# CLAUDE.md — AI エージェント向け作業規約

このリポジトリは、iOS エンジニアが Cloud Native AI Developer になるための学習・資格・キャリア・個人開発ロードマップを管理する。AI エージェント（Claude Code / ChatGPT / Codex 等）が更新作業を行う際は、以下の規約に従うこと。

## 最重要ルール

1. **文章は日本語で書く**（コード・コマンド・固有名詞は除く）
2. **資格・試験情報を断定しない**: 試験の存在・名称・言語・廃止日・後継資格・試験範囲は、公式ページで確認していない限り必ず「要公式確認」と明記する。ブログ・古い書籍・自身の学習データの情報を事実として書かない
3. **公式確認した情報には確認日を残す**: 各 certification ファイル末尾の「公式確認ログ」表に日付・確認内容・結果を追記する
4. **空ファイルを作らない**: 新規ファイルには必ず意味のある初期内容を書く
5. **大きな方針変更は ADR にする**: フェーズ構成・技術選定・運用方式の変更は `adr/` に ADR を追加してから該当ファイルを更新する（[テンプレート](templates/adr-template.md)、連番 4 桁）

## ファイル配置ルール

| 追加したいもの | 置き場所 |
| --- | --- |
| 資格の候補・検討メモ | `docs/certification/<ベンダー>.md` に追記 |
| 記入済み資格取得計画 | `docs/certification/plans/<試験番号>.md` |
| 学習リソース | `docs/learning/books.md` / `courses.md` / `hands-on.md` |
| 記入済み学習ログ | `docs/learning/logs/YYYY/YYYY-MM-DD.md` |
| プロダクトアイデア | `docs/projects/ideas.md` に追記 |
| 記入済みプロジェクト計画 | `docs/projects/plans/<プロジェクト名>.md` |
| レビュー結果 | `docs/operations/monthly-review.md` / `quarterly-review.md`（新しい期間を上に追記） |
| 軽い意思決定 | `docs/operations/decision-log.md`（大きな決定は ADR へ） |
| 意思決定（重要） | `adr/NNNN-タイトル.md` + `adr/README.md` の一覧を更新 |

## 表記の統一

- ステータス絵文字（資格）: ✅ 取得済み / 🎯 受験計画中 / 🔍 検討中 / ⏸ 保留 / ❌ 見送り
- ステータス絵文字（タスク・成果物）: ✅ 完了 / 🔄 進行中 / 📋 予定 / ⏳ 未着手
- スキルレベル: Lv1 知っている / Lv2 使える / Lv3 設計できる / Lv4 教えられる・運用できる
- 見出しは `#` 階層を飛ばさない。表を優先し、長い箇条書きを避ける

## リンクのルール

- **Markdown ファイル間**: 相対パスで書く（例: `[roadmap.md](../roadmap.md)`）
- **Issue テンプレート（`.github/ISSUE_TEMPLATE/*.yml`）内**: 相対パスは Issue 作成画面で壊れるため、`https://github.com/shiba-tt/cloud-native-ai-developer-roadmap/blob/main/...` の絶対 URL で書く
- ファイルを移動・改名したら、参照元をすべて更新する（CI のリンクチェックが検出する）

## 整合性の維持

以下は内容が連動しているため、片方だけ更新しない。

- `docs/roadmap.md` のフェーズ状態 ⇔ `docs/projects/portfolio-roadmap.md` の成果物状態 ⇔ `career/milestones.md`
- 資格のステータス変更 ⇔ 該当 `docs/certification/*.md` と `portfolio-roadmap.md`
- ディレクトリ構成の変更 ⇔ `README.md` のツリーと各 overview のファイル構成表
- ラベルの追加・変更 ⇔ `.github/labels.yml`（GitHub UI で直接作らない）

## やってはいけないこと

- 受験判断・キャリア判断・技術選定を勝手に確定させること（提案は Issue や ADR の Proposed として出す）
- 「要公式確認」の注記を、公式確認なしに削除すること
- 既存の記録（レビュー結果・公式確認ログ・決定ログ）を書き換えること（追記のみ）
- このファイルと `README.md` の方針に矛盾する変更を、ADR なしで入れること
