# 卒研支援システム — SPP × ZIF-67 空気電池カソード触媒

芝浦工業大学 石﨑研究室 卒業研究(担当: AC23087 馬場智久)を、Claude Code 上の
分業エージェント体制で支援するためのリポジトリです。

## 構成

- `CLAUDE.md` — 研究の要点と分業体制の使い方(このリポジトリを開くと自動で読み込まれます)
- `docs/research-integrated-record.html` — これまでの検討・結果・設計の統合記録(一次情報源)
- `.claude/agents/` — 役割別サブエージェント定義
  - `idea-generator` — アイデア出し・新規実験ルートのブレインストーミング
  - `method-reviewer` — 実験手順の批判的レビュー・改正提案
  - `lit-data-analyst` — 既存データの解析支援・文献整合性チェック
- `ideas/` — アイデア出しの記録
- `experiments/` — 実験計画書

## 使い方

Claude Code でこのリポジトリを開いて相談してください。
専門的な視点が欲しいときは、Agent ツールで上記のサブエージェントを指定して呼び出せます。

例:
- 「idea-generator に、Fe導入以外で二機能化する新しいアイデアを出してほしい」
- 「method-reviewer に、低温温度シリーズの実験計画をレビューしてほしい」
- 「lit-data-analyst に、Run15のXPSデータの解釈を確認してほしい」

## 更新の仕方

新しい実験結果や意思決定があったら、`CLAUDE.md`(要点サマリ)と
`docs/research-integrated-record.html`(全記録)の両方を最新化してください。
これにより、どのエージェントに聞いても最新の研究状況を前提に回答できます。
