# Decision Log — 意思決定ログ

日々の小さな意思決定を時系列で記録する軽量ログ。
アーキテクチャや方針に関わる大きな決定は [adr/](../../adr/) に ADR として記録し、ここからリンクする。

## 使い分け

| 記録先 | 対象 | 例 |
| --- | --- | --- |
| このファイル | 軽量な判断・選択 | 「教材 A ではなく B を使う」「今月は Phase 2 を優先」 |
| ADR | 長期に影響する決定 | 「IaC は Terraform を採用」「AI 資格は日本語対応まで保留」 |

## フォーマット

```markdown
### YYYY-MM-DD: 決定のタイトル
- **決定**: 何を決めたか
- **理由**: なぜそうしたか
- **関連**: Issue / ADR / ファイルへのリンク
```

---

## ログ

### 2026-07: リポジトリ初期構成を作成

- **決定**: GitHub をロードマップ管理の Single Source of Truth とし、docs / career / adr / templates / .github の初期構成で運用を開始する
- **理由**: [ADR-0001](../../adr/0001-use-github-as-roadmap-source-of-truth.md) 参照
- **関連**: ADR-0001
