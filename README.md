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

## 公開手順（未実施）

1. GitHubで公開リポジトリ `hatakeyama-ai-tax` を新規作成（個人アカウント側）
2. このフォルダの中身をそのままpush
3. Settings → Pages → Branch: `main` / root で公開
4. 公開URLが確定したら `index.html` の `canonical`・OGP・JSON-LDの `url` を実URLに差し替える
   （現状は `https://fromk0326-boop.github.io/hatakeyama-ai-tax/` を仮置き。独自ドメインにするならここを変更）

## 運用ルール

- 更新の基本は `now.md` への追記＋`index.html` フッターの最終更新日
- 大きな実績（書籍出版・ブートキャンプ開講等）が出たら `profile.md` と `llms.txt` にも反映
- 秘密情報・顧問先情報・個人情報（住所・出生時間等）は絶対に載せない

## ai-management リポジトリとの関係

`20_事務所/github-pages/` は本来git除外だが、このフォルダだけリモートセッションでの作成物を
失わないよう `.gitignore` に例外を設定してgit管理している（2026-07-29）。
独立リポジトリ化してリモートにバックアップができたら、`.gitignore` の例外行を削除して
除外に戻してよい。
