# Bot Legal Documents

Privacy policies and terms of service for the Discord bots operated by **Neriteria**.

Each directory corresponds to one Discord application. The URLs below are the ones
registered in the Discord Developer Portal for that application.

| Bot | Status | Privacy Policy | Terms of Service |
|---|---|---|---|
| Poludnitsa | In development | [Privacy Policy](./poludnitsa/PRIVACY_POLICY.md) | [Terms of Service](./poludnitsa/TERMS_OF_SERVICE.md) |
| WoWS Utility App | Public | [Privacy Policy](./wows-utility-app/PRIVACY_POLICY.md) | [Terms of Service](./wows-utility-app/TERMS_OF_SERVICE.md) |

Enquiries about a bot are handled in a Discord server (the community or support server for
that bot); the invite link is given in the contact section of each document.

---

## Repository conventions

*(運用メモ)*

- **正文の言語は bot ごとに、利用者に合わせて決める。** 全 bot で統一しない。
  正確でなければならないのは、実際に読む人が読める側の言語。
  - Poludnitsa: 利用者はグローバルサーバーの英語話者が中心 → **英語が正文**、日本語は参考訳。
  - 私的に提供している他の bot: 利用者は日本語話者 → **日本語が正文**、英語は要約のみで足りる。
  - WoWS Utility App: 利用者は海外にもいるが、運営者が問い合わせに日本語でしか対応できない
    → **日本語が正文**、英語は全文の参考訳を付ける。
  - どちらの場合も、文書の冒頭に「どちらが正文か」「相違時はどちらが優先するか」を明記する。
    これを書いておけば、訳のズレが法的な争点にならない。
- **1 ディレクトリ = 1 Discord アプリケーション。** リポジトリ単位でも bot の表示名単位でも
  ない。Developer Portal の URL 欄はアプリごとに設定するため、そこと 1 対 1 で対応させる。
- **ディレクトリ名は一度決めたら変更しない。** URL が 404 になり、Developer Portal 側の
  設定も直す羽目になる。bot の表示名が変わってもディレクトリ名は据え置く。
- **各文書は自己完結させる。** 共通部分を別ファイルに切り出さない。審査担当も利用者も
  1 つの URL しか読まないため、リンクを辿らないと全体が分からない文書は不利になる。
  重複部分の同期は `_template/` を原本として手で反映する。
- **`_template/` はひな型であり、公開文書ではない。** Developer Portal からリンクしない。
  新しい bot を追加するときは `_template/` をコピーしてプレースホルダを埋める。
- **bot を終了してもディレクトリを削除しない。** 冒頭に終了日を追記して残す。
  削除すると過去に告知した URL が失われる。
- **公開後は force push しない／履歴を書き換えない。** 「いつ何を告知したか」の証跡が
  git 履歴そのものになる。一方、まだ push していない下書き段階の履歴は公開前に整理して
  よい。検討途中で書いた第三者名・旧連絡先などをパブリックに残さないため。
- 文書を改訂したら、冒頭の「最終更新日」と末尾の変更履歴の両方を更新する。

## URL to register in the Discord Developer Portal

```
https://github.com/Neriteria/bot-legal/blob/main/<bot>/PRIVACY_POLICY.md
https://github.com/Neriteria/bot-legal/blob/main/<bot>/TERMS_OF_SERVICE.md
```

`raw.githubusercontent.com` は `text/plain` で返り Markdown が整形されないため使わない。
コミット SHA 入りの URL も使わない（`main` を指せば改訂が自動で反映される）。

## Adding a new bot

1. `cp -r _template <bot-slug>`
2. Fill in every `<PLACEHOLDER>` and remove every HTML comment.
3. Adjust the sections marked `ADJUST` so that they match what the bot actually does —
   especially the stored-data table and the message content section.
4. Add a row to the table above.
5. Register the two URLs in the Discord Developer Portal.
