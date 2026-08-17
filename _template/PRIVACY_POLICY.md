<!--
  TEMPLATE — do not link to this file from a Discord Developer Portal.
  Copy this file to <bot-slug>/PRIVACY_POLICY.md and fill in every <PLACEHOLDER>.
  Sections marked "ADJUST" describe features and must match what the bot actually does.
  Delete every HTML comment before publishing.

  LANGUAGE: decide which language is authoritative from the bot's actual users, not from
  a repo-wide default. Put the authoritative language first, label the other as a
  reference translation, and state which one prevails on a discrepancy. A bot serving a
  Japanese community should be Japanese-authoritative; one serving a global server should
  be English-authoritative.
-->

# Privacy Policy

**Application:** `<BOT_NAME>` (Discord bot)
**Operator:** `<OPERATOR_NAME>`
**Effective date:** `<YYYY-MM-DD>`
**Last updated:** `<YYYY-MM-DD>`

*(日本語版は下部にあります / A Japanese version follows below.)*

---

## 1. Overview

`<BOT_NAME>` ("the Bot") is a Discord bot operated by an individual for the purpose of
`<PURPOSE — e.g. supporting the operation of a gaming community>`. This policy explains
what data the Bot collects, why it collects it, where it is stored, and how you can have it
removed.

By adding the Bot to a Discord server, the server's administrators agree to this policy on
behalf of that server. Members of a server where the Bot is present are subject to this
policy for the data described below.

The Bot uses no artificial intelligence or machine learning. It does not sell, rent, or
share data with third parties. It does not display advertising, build user profiles, or
analyse data across servers.

<!-- If the bot DOES use AI, or does share data, delete the paragraph above and state the
     truth instead. Never leave a claim here that the implementation contradicts. -->

## 2. Data the Bot stores

<!-- ADJUST: one row per kind of stored data. Keep it exhaustive — this table is what a
     Discord reviewer compares against the intent application answers. -->

The Bot stores the following data. All of it is partitioned by Discord server (guild) ID
and is never read or combined across servers.

| Data | Purpose |
|---|---|
| Discord server IDs, user IDs, role IDs, channel IDs (numeric IDs only) | `<PURPOSE>` |
| `<DATA>` | `<PURPOSE>` |

`<Describe which data is created automatically and which is created only when a server
administrator explicitly configures something.>`

## 3. Message content

<!-- ADJUST or DELETE this whole section if the bot does not use the Message Content
     Intent. If it does, this section is the most closely read part of the document. -->

The Bot receives the content of messages sent in servers where it is present, and uses it
to:

- `<USE 1>`;
- `<USE 2>`.

**Message content is not stored outside Discord.** Each message is evaluated in memory as
it arrives and is discarded immediately afterwards. Message content is never written to the
Bot's database, never included in operational logs, and never sent to any third party or
external service.

<!-- If the bot posts message content anywhere that persists, disclose it here, as in the
     audit-record example below. Delete the paragraph if it does not apply. -->

There is one exception, and it stays within Discord: `<DESCRIBE — e.g. when a moderation
rule takes an action on a message, the Bot posts an audit record to a log channel inside
the same Discord server, and that record includes the content of the message that
matched>`. This record is visible only to whoever can view that channel, is controlled by
the server's administrators, and is subject to Discord's own data handling rather than the
Bot operator's.

Operational logs kept by the operator deliberately exclude message content. `<Describe what
a log entry does contain — e.g. only the action type, the rule name, and the server, user,
channel and message IDs involved.>`

## 4. Data the Bot does not collect

The Bot does not collect or store:

- message content (outside the transient processing described in section 3);
- usernames, display names, avatars, or profile information;
- email addresses, real names, phone numbers, or postal addresses;
- IP addresses or device information;
- payment information;
- voice data, direct messages sent to other users, or presence/activity status.

<!-- ADJUST: remove any line the bot actually does collect, and move it to section 2.
     A false negative here is worse than an omission. -->

## 5. Where data is stored

Stored data is held in `<PROVIDER AND SERVICES — e.g. Amazon Web Services (Amazon DynamoDB
and Amazon S3)>` in the `<REGION — e.g. ap-northeast-1 (Tokyo, Japan)>` region. Access is
restricted to the operator.

## 6. Data sharing

Data is never sold, rented, or shared with third parties. It is not used to train
artificial intelligence or machine learning models. It is not used for advertising or
profiling.

Data may be disclosed only where required by applicable law, or where necessary to
investigate abuse of the Bot itself.

## 7. Retention and deletion

- Data is retained for as long as the Bot remains in the relevant server and the data
  remains in use.
- When the Bot is removed from a server, that server's data is deleted.
- Any user may request deletion of their own data by contacting the operator using the
  details in section 10. Requests are handled within a reasonable period.
- Server administrators may delete configuration data they created at any time using the
  Bot's own commands.

## 8. Your choices

<!-- ADJUST: state per feature whether a user can opt out, and where they cannot, say so
     plainly and give the reason. A candid "no opt-out, because X" reads better to a
     reviewer than a vague claim that everything is optional. -->

**`<FEATURE>`.** `<Whether opt-out is possible, how, or why it is not.>`

**Whole server.** A server administrator can end all data collection for their server
immediately by removing the Bot from it.

## 9. Children

The Bot is not directed at children. Use of Discord requires users to meet the minimum age
set out in the Discord Terms of Service for their country. The Bot does not knowingly
retain data belonging to anyone below that age; if such data is identified, it will be
deleted.

## 10. Contact

<!-- Give at least one route that actually works and will keep working. A permanent
     (non-expiring) invite to the community server is enough, provided requests can be
     raised there. Bear in mind that a user who has left or been banned from the server
     cannot use an invite-only route; if that matters for this bot, add an email address
     as well. -->

Questions about this policy, and requests for access to or deletion of your data, can be
sent to:

`<CONTACT ROUTE — e.g. a permanent Discord invite, and/or an email address>`

## 11. Changes to this policy

This policy may be updated. When it is, the "Last updated" date at the top of this document
is changed. Material changes will be announced in the community server where the Bot
operates. Continued use of the Bot after a change constitutes acceptance of the updated
policy.

## Revision history

| Date | Change |
|---|---|
| `<YYYY-MM-DD>` | Initial version. |

---
---

# プライバシーポリシー

**対象アプリケーション:** `<BOT_NAME>`（Discord bot）
**運営者:** `<OPERATOR_NAME>`
**発効日:** `<YYYY-MM-DD>`
**最終更新日:** `<YYYY-MM-DD>`

## 1. 概要

`<BOT_NAME>`（以下「本 bot」）は、`<目的>`を目的として個人が運営している Discord bot です。
本ポリシーは、本 bot が取得するデータ、その目的、保存場所、および削除方法について
説明します。

本 bot をサーバーに導入した時点で、当該サーバーの管理者はサーバーを代表して本ポリシーに
同意したものとみなします。本 bot が導入されたサーバーのメンバーは、以下に記載する範囲で
本ポリシーの対象となります。

本 bot は AI・機械学習を一切使用しません。取得したデータを第三者へ販売・提供することは
なく、広告表示・プロファイリング・サーバーをまたいだ分析も行いません。

## 2. 保存するデータ

本 bot は以下のデータを保存します。すべて Discord サーバー（ギルド）ID で分離されており、
サーバーをまたいで参照・結合することはありません。

| データ | 目的 |
|---|---|
| Discord のサーバー ID・ユーザー ID・ロール ID・チャンネル ID（数値 ID のみ） | `<目的>` |
| `<データ>` | `<目的>` |

`<自動的に作成されるデータと、管理者が明示的に設定した場合にのみ作成されるデータを区別して
記載する。>`

## 3. メッセージ本文の取り扱い

本 bot は、導入されたサーバー内で送信されたメッセージの本文を受信し、以下の目的で
使用します。

- `<用途 1>`
- `<用途 2>`

**メッセージ本文を Discord 外へ保存することはありません。** 受信したメッセージはメモリ上で
評価されるのみで、評価後ただちに破棄されます。本文がデータベースへ書き込まれることはなく、
運用ログに含まれることもなく、第三者や外部サービスへ送信されることもありません。

例外は 1 点のみで、それも Discord 内で完結します。`<説明>`。この記録は当該チャンネルを
閲覧できる者のみが参照でき、サーバー管理者の管理下にあり、運営者ではなく Discord の
データ取り扱いに従います。

運営者が保持する運用ログには、意図的にメッセージ本文を含めていません。`<ログに記録される
項目を記載する。>`

## 4. 取得しないデータ

本 bot は以下を取得・保存しません。

- メッセージ本文（第 3 項に記載した一時的な処理を除く）
- ユーザー名、表示名、アバター、プロフィール情報
- メールアドレス、氏名、電話番号、住所
- IP アドレス、端末情報
- 決済情報
- 音声データ、他ユーザー宛の DM、プレゼンス／アクティビティ状態

## 5. データの保存場所

保存されるデータは、`<事業者およびサービス名>`の `<リージョン>` に保管されます。
アクセスできるのは運営者のみです。

## 6. 第三者提供

データを第三者へ販売・貸与・提供することはありません。AI・機械学習モデルの学習には
一切使用しません。広告やプロファイリングにも使用しません。

法令に基づき開示が必要な場合、および本 bot 自体への不正利用を調査する必要がある場合に
限り、開示することがあります。

## 7. 保存期間と削除

- データは、本 bot が当該サーバーに在籍し、そのデータが利用されている間保持されます。
- 本 bot がサーバーから退出した場合、当該サーバーのデータを削除します。
- 利用者は、第 10 項の連絡先に連絡することで、自身のデータの削除を請求できます。
  請求は合理的な期間内に対応します。
- サーバー管理者は、自身が作成した設定データを本 bot のコマンドによりいつでも削除できます。

## 8. 利用者の選択肢

**`<機能名>`:** `<オプトアウトの可否、方法、または不可である理由を記載する。>`

**サーバー全体:** サーバー管理者は、本 bot を退出させることで、当該サーバーにおける
すべてのデータ取得を即座に終了できます。

## 9. 未成年の利用について

本 bot は子どもを対象としたものではありません。Discord の利用には、Discord 利用規約が
国ごとに定める最低年齢を満たす必要があります。本 bot は当該年齢未満の利用者のデータを
意図的に保持しません。該当が判明した場合は削除します。

## 10. 連絡先

本ポリシーに関する質問、およびデータの開示・削除の請求は以下へご連絡ください。

`<連絡手段 — 例: 無期限の Discord 招待リンク、またはメールアドレス>`

## 11. 本ポリシーの変更

本ポリシーは更新されることがあります。更新時は冒頭の「最終更新日」を変更します。
重要な変更については、本 bot が稼働するコミュニティサーバーで告知します。
変更後も本 bot の利用を継続した場合、更新後のポリシーに同意したものとみなします。

## 変更履歴

| 日付 | 変更内容 |
|---|---|
| `<YYYY-MM-DD>` | 初版 |
