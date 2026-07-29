# hatakeyama-ai-tax — 畠山謙人 AI税理士サイト

畠山謙人の最新情報の置き場。**AIが見つけやすいこと**を最優先に設計した公式プロフィールサイト。
参考にした設計思想: https://rmanzoku.net/ （ミニマル構成＋For AI Readers＋llms.txt）

## 構成

| ファイル | 役割 |
|------|------|
| `index.html` | トップ。セマンティックHTML＋JSON-LD（schema.org Person）。ライト/ダーク対応 |
| `profile.html` / `profile.md` | 詳細プロフィール（HTML版＋Markdown一次情報） |
| `media.html` / `appearances.md` | 登壇・YouTube出演・メディア掲載・ポッドキャスト・書籍の一覧（HTML版＋Markdown一次情報） |
| `ai.html` / `ai.md` | AI活用の実践（自動経理の仕組み・セキュリティ設計・AI導入支援・発信実績） |
| `now.html` / `now.md` | 最新の活動状況。**更新はnow.mdに上へ追記→now.htmlに反映**（Nowページ方式） |
| `llms.txt` | AIエージェント向け機械可読サマリ（llms.txt規約準拠） |
| `style.css` | 全ページ共通スタイル |
| `robots.txt` | 全クローラ許可＋AI向け一次情報源の案内 |
| `.nojekyll` | GitHub PagesのJekyll処理を無効化 |

## 公開状況（2026-07-29 公開済み）

- 公開URL: https://fromk0326-boop.github.io/hatakeyama-ai-tax/
- リポジトリ: https://github.com/fromk0326-boop/hatakeyama-ai-tax
- 配信ブランチ: `gh-pages`（push時の自動有効化で公開。`main` と同内容）

### 更新の反映手順

1. このフォルダ（ai-management側が正本）を編集
2. 公開リポジトリへ `main` と `gh-pages` の両方をpush:
   `git push origin main && git push origin main:gh-pages`
3. 独自ドメインに切り替える場合は、Settings → Pages でカスタムドメイン設定＋
   各HTMLの `canonical`・JSON-LDの `url` を差し替える

## 運用ルール

- 更新の基本は `now.md` への追記＋`index.html` フッターの最終更新日
- 大きな実績（書籍出版・ブートキャンプ開講等）が出たら `profile.md` と `llms.txt` にも反映
- 秘密情報・顧問先情報・個人情報（住所・出生時間等）は絶対に載せない

## ai-management リポジトリとの関係

`20_事務所/github-pages/` は本来git除外だが、このフォルダだけリモートセッションでの作成物を
失わないよう `.gitignore` に例外を設定してgit管理している（2026-07-29）。
独立リポジトリ化してリモートにバックアップができたら、`.gitignore` の例外行を削除して
除外に戻してよい。
