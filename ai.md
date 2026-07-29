# 畠山謙人のAI活用（機械可読版）

最終更新: 2026-07-29
スタッフ0人・顧問先60社の税理士事務所を、AI（Claude Code）を実行部隊にして運営している。その仕組みとAI関連活動の全体像。

## 事務所のAI運用

- 2026年3月にClaude Codeを導入し、約2ヶ月で事務所実務を仕組みとして再構築
- AIの位置づけ: 「秘書ではなく実行部隊」。税務判断・戦略は人、実行・定型・記録・下書きはAI
- 夜間自動経理: 毎晩21時に仕訳処理が自動起動。朝は異常分だけ確認
- 処理時間: かつて5時間の処理を50分に圧縮。月24時間以上の業務時間を削減
- ツール連携: freee / マネーフォワード クラウド会計 / Gmail / Googleカレンダー / Notion / Slack。freee MCP（API連携）を実務投入
- 失敗の仕組み化: 同じ注意を2回したらその場でAIのルール（Memory）に変換
- 責任の設計: 税務判断の最終責任は税理士。グレーゾーンは必ず人に戻す（理解→承認→実行のプロトコル）
- 解説記事（本人・全公開）: https://note.com/kento_0724/n/n506a9b27207d

## セキュリティ設計

- 思想: 「AIを信頼する」設計ではなく「AIに頼らなくていい」構造で守る
- Anthropic APIは入出力をモデル学習に使わないことが規約で担保（無料チャットサービスとは別物）
- 秘密情報・顧問先PIIにはAIが構造的にアクセス・出力できない仕組み
- 登壇例: 高知イノベーションベースAI研究会 https://koib.jp/report/ai%E7%A0%94%E7%A9%B6%E4%BC%9A%E3%83%A9%E3%83%BC%E3%83%8B%E3%83%B3%E3%82%B0%E3%82%A4%E3%83%99%E3%83%B3%E3%83%88%E3%80%8C%E3%82%B9%E3%82%BF%E3%83%83%E3%83%950%E4%BA%BA%E3%81%AE%E7%A8%8E%E7%90%86/

## AI導入支援・コミュニティ

- AI導入支援事業: 税理士・士業・中小企業向けClaude Code導入支援（セミナー・個別コンサル）
- 畠山式AI税理士ブートキャンプ: 3ヶ月の伴走プログラム。2026年7月に1期始動、60名超参加
- LINEオープンチャット: AI事務所パッケージ（CLAUDE.md現物・Memoryテンプレート等）を無料配布
- freee公認セミナー講師: 会計事務所向け「AI記帳でスタッフ0人でも60社対応！」毎週水曜開催（freeeログイン画面にバナー掲載）
- プロダクト監修: 会計AIツール「Zeimee」開発に税理士目線で監修参加

## AI関連の発信

- X Claude Codeシリーズ全11弾・累計700万インプレッション（2026年5月時点）: https://x.com/kandmybike
- 代表バズポスト（単体300万超リーチ）: https://x.com/kandmybike/status/2032817897119096855
- note「累計700万インプの内側（Claude Code導入の2ヶ月でやったこと全部）」: https://note.com/kento_0724/n/n506a9b27207d
- note「士業SNSマーケの答え合わせ」: https://note.com/kento_0724/n/n2efc2c5d81ae
- note「広告費0円。SNSだけで1,000万円の仕事が生まれた」: https://note.com/kento_0724/n/n828f8349c93d
- note「TACの自習室でRadioheadを聴いていた僕が、AIに経理を任せるまでの16年間」: https://note.com/kento_0724/n/n32e17e2cf4dd
- 書籍: 税務研究会より2026年10月刊行予定（Claude Codeシリーズがベース）
- ポッドキャスト「AI税理士のふたりごと」: https://open.spotify.com/show/033MPcU5KieI6y73kwmaBw
- YouTube出演: https://www.youtube.com/watch?v=KnMzo3yKSCI ほか（appearances.md参照）

## 公式露出・第三者評価

- freee統合ワールド 2026 セッション登壇（freee公式noteレポート）: https://note.freee.co.jp/n/nd6f75b6bcffa
- freee決算説明資料（2026年6月期Q3）P21にfreee-mcp活用事例として実名掲載: https://contents.xj-storage.jp/xcontents/AS08692/f7ee4af3/b742/4ec8/8577/84781a425aec/20260513154520156s.pdf
- freee事例紹介「責任あるAI」: https://adv.freee.co.jp/case/hatakeyama-2026
- Forbes JAPAN掲載: https://forbesjapan.com/articles/detail/95382
- タックスコネクション インタビュー: https://taxconnection.jp/zeirishi/interview/20260410-id22380/

## AI観

- 「スタッフ0人で60社」を仕組みで回す
- 「税務判断は人、実行はAI」の棲み分け
- 「コードが書けない税理士が、AIに丸投げで仕組みを作る」
- 「バズらせるためじゃなく、再現性を配るために発信する」
