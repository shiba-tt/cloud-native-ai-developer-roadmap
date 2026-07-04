# ADR 0001: GitHubをロードマップ管理のSingle Source of Truthにする

## Status

Accepted

## Context

Cloud Native AI Developerを目指す学習は、資格、個人開発、キャリア、設計判断、振り返りが長期にわたって変化します。AIエージェントと共同で更新するためには、変更履歴、レビュー、Issue管理、テンプレートが使える場所が必要です。

## Decision

このリポジトリをロードマップ管理のSingle Source of Truthとします。学習計画、資格候補、プロジェクト案、ADR、レビューはGitHub上のMarkdown、Issue、Pull Requestで管理します。

## Consequences

- 変更履歴がGitで追跡できる
- AIエージェントがファイルを読み書きしやすい
- IssueとPRで学習タスクを運用できる
- 一方で、継続的な整理を怠るとドキュメントが古くなるため、月次・四半期レビューが必要になる

## Alternatives considered

- Notion: 柔軟だが、Git履歴やAIエージェントとのコードベース連携が弱い
- スプレッドシート: 一覧性は高いが、設計判断や長文ドキュメントに向かない
- ローカルメモ: 手軽だが、継続運用とレビューが難しい
