# sxc-1-playbook プロジェクト

CASIO のポータブルサンプラー **SXC-1** を遊び倒すための情報をまとめ、GitHub Pages で公開する**ドキュメント中心**のリポジトリ。

- 公開サイト: GitHub Pages（`README.md` を Jekyll で自動レンダリング）
- メインコンテンツ: [README.md](README.md)

## Claude Code 使用時の重要な指示

- **回答言語**: 必ず日本語で回答すること
- **出力スタイル**: 操作の理由と内容を明確に説明する
- **事実ベース**: スペック・操作手順は公式マニュアル（`docs/` のPDF）を根拠とし、推測は明示する

## 著作権ポリシー（重要）

- `docs/` 内の CASIO 公式マニュアルPDF・収録音源・画像は **CASIO の著作物**。
- これらは **リポジトリにコミットしない**（`.gitignore` で `docs/` と `*.pdf` を除外済み）。
- 公開コンテンツでは原典への**リンク**で案内し、PDFそのものを再配布しない。

## ブランチ運用

- `main`: 公開ブランチ（GitHub Pages のソース）。PR ベースで更新
- `docs/*`: ドキュメント更新・追加
- `fix/*`: 誤記・リンク切れ修正
- `chore/*`: 設定・補助タスク

## コミット・PR 規則

- コミットメッセージ・GitHub コメントは日本語
- 形式: `[種類] 変更内容の説明`（種類: `docs` / `fix` / `chore` / `feat`）
  - 例: `[docs] MIDI実装表を追記`、`[fix] 公式リンク切れを修正`

## GitHub Pages

- ソース: `main` ブランチ / ルート（`/`）
- テーマ: `jekyll-theme-cayman`（`_config.yml`）
- `README.md` がトップページとして表示される

## よく使うコマンド

- 変更確認: `git status && git diff`
- コミット・プッシュ: `git add -A && git commit -m "[docs] 変更内容" && git push`
- Pages 状態確認: `gh api repos/:owner/:repo/pages`

## 日付の扱い

- 日付は必ず環境設定の `Today's date` を優先（ファイル名や既存日付に惑わされない）
- 形式: YYYY-MM-DD
