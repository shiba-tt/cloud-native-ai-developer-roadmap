# Certification Plans — 資格取得計画の保存先

[templates/certification-plan.md](../../../templates/certification-plan.md) をコピーして記入した資格取得計画を、このディレクトリに保存する。

## 命名規則

```text
docs/certification/plans/<試験番号など小文字>.md

例:
docs/certification/plans/az-305.md
docs/certification/plans/ckad.md
docs/certification/plans/terraform-associate.md
```

## 運用ルール

- 計画を作成したら、対応するベンダー別ファイル（[azure.md](../azure.md) 等）のステータスを 🎯 受験計画中 に更新し、この計画へリンクする
- 受験用 Issue（certification テンプレート）からもこの計画にリンクする
- 合格・見送り後もファイルは削除せず、記録セクションに結果を残す
