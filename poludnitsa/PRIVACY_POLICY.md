# Privacy Policy

**Application:** `Poludnitsa` (Discord bot)
**Operator:** `Neriteria`
**Effective date:** 2026-08-18
**Last updated:** 2026-08-18

*This English text is the authoritative version of this policy. A Japanese translation
follows below for reference only; in case of any discrepancy between the two, the English
version prevails.*

---

## 1. Overview

`Poludnitsa` ("the Bot") is a Discord bot operated by `Neriteria` ("the Operator") to
support the operation of the community server for which it was commissioned.

This policy explains what data the Bot collects, why it collects it, where it is stored,
and how you can have it removed.

By adding the Bot to a Discord server, the server's administrators agree to this policy on
behalf of that server. Members of a server where the Bot is present are subject to this
policy for the data described below.

The Bot uses no artificial intelligence or machine learning. It does not sell, rent, or
share data with third parties. It does not display advertising, build user profiles, or
analyse data across servers.

## 2. Data the Bot stores

The Bot stores the following data. All of it is partitioned by Discord server (guild) ID
and is never read or combined across servers.

| Data | Purpose |
|---|---|
| Discord server IDs, user IDs, role IDs, channel IDs (numeric IDs only) | Identifying which server a setting belongs to, which member owns a point balance, and which roles/channels a rule applies to |
| Point balances (integer) | Providing the points and shop feature |
| Moderation rule definitions: trigger words, watched channel/category IDs, exempt user/role IDs, action type | Providing the moderation feature configured by server administrators |
| Custom command definitions and their attached files | Providing the custom command feature configured by server administrators |
| Custom emoji usage counts, per day (emoji ID and a count only) | Providing custom emoji usage statistics |
| Per-server runtime settings, such as the designated log channel ID | Providing configurable behaviour per server |

Point balances are created automatically when a member posts a message in a server where
the points feature is enabled. All other data listed above is created only when a server
administrator explicitly configures it.

## 3. Message content

The Bot receives the content of messages sent in servers where it is present, and uses it
to:

- compare messages against trigger words configured by server administrators (moderation);
- detect custom command invocations, i.e. a message beginning with the server's configured
  prefix;
- count occurrences of the server's custom emoji.

**Message content is not stored outside Discord.** Each message is evaluated in memory as
it arrives and is discarded immediately afterwards. Message content is never written to the
Bot's database, never included in operational logs, and never sent to any third party or
external service.

There is one exception, and it stays within Discord: when a moderation rule takes an action
on a message, the Bot posts an audit record to a log channel **inside the same Discord
server**, and that record includes the content of the message that matched. This record is
visible only to whoever can view that channel, is controlled by the server's
administrators, and is subject to Discord's own data handling rather than the Bot
operator's.

Operational logs kept by the operator deliberately exclude message content. A moderation
log entry records only the action type, the rule name, and the server, user, channel and
message IDs involved.

## 4. Data the Bot does not collect

The Bot does not collect or store:

- message content (outside the transient processing described in section 3);
- usernames, display names, avatars, or profile information;
- email addresses, real names, phone numbers, or postal addresses;
- IP addresses or device information;
- payment information (the Bot has no paid features; "points" are an in-server value with
  no monetary worth and cannot be purchased or exchanged for money);
- voice data, direct messages sent to other users, or presence/activity status.

## 5. Where data is stored

Stored data is held in Amazon Web Services (Amazon DynamoDB and Amazon S3) in the
`ap-northeast-1` (Tokyo, Japan) region, in an account controlled by the Operator. Access is
restricted to the Operator.

The account holding this infrastructure may be migrated to another account operated for the
same community server. Such a migration does not change what data is collected, why it is
collected, or who may access it.

The Bot is operated from Japan, and its users are located worldwide. If you are in the
European Economic Area or the United Kingdom, note that Japan has been recognised by the
European Commission as providing an adequate level of data protection, so the storage of
your data in Japan does not require additional safeguards.

## 6. Data sharing

Data is never sold, rented, or shared with third parties. It is not used to train
artificial intelligence or machine learning models. It is not used for advertising or
profiling.

Data may be disclosed only where required by applicable law, or where necessary to
investigate abuse of the Bot itself.

## 7. Retention, deletion and your rights

- Data is retained for as long as the Bot remains in the relevant server and the data
  remains in use.
- When the Bot is removed from a server, that server's data is deleted.
- Any user may request deletion of their own data (for example, their point balance) by
  contacting the operator using the details in section 10. Requests are handled within a
  reasonable period.
- Server administrators may delete configuration data they created (rules, custom commands
  and their attachments) at any time using the Bot's own commands.

Note that the audit records described in section 3 live in a Discord channel, not in the
Bot's storage. Deleting them is done through Discord by the server's administrators.

Wherever you are located, you may ask the operator to tell you what data is held about
you, to correct it if it is wrong, to delete it, or to stop processing it. Requests are
free of charge and can be made using the contact details in section 10. Because the Bot
identifies you only by your Discord user ID, a request must be made from the Discord
account concerned so that it can be matched to the right data.

If you are in the European Economic Area or the United Kingdom, these correspond to your
rights of access, rectification, erasure, restriction and objection, and you also have the
right to lodge a complaint with your local data protection authority.

## 8. Your choices

**Moderation.** There is no per-member opt-out from moderation, by design: a moderation
feature that the targeted member could switch off for themselves would not work. Whether a
rule applies is decided by the server's administrators, who can exempt specific users or
roles and can limit a rule to specific channels or categories. No moderation data about a
message is retained unless the message matches a rule (see section 3).

**Points.** A member who does not want a point balance to be kept for them may opt out by
contacting the operator; their balance will be deleted and no further points recorded.

**Custom commands.** These run only when a member deliberately posts a prefixed command
name.

**Emoji statistics.** These aggregate only an emoji ID and a count. Who used an emoji is
never recorded, so no user-linked data exists.

**Whole server.** A server administrator can end all data collection for their server
immediately by removing the Bot from it.

## 9. Children

The Bot is not directed at children. Use of Discord requires users to meet the minimum age
set out in the Discord Terms of Service for their country. The Bot does not knowingly
retain data belonging to anyone below that age; if such data is identified, it will be
deleted.

## 10. Contact

Questions about this policy, and requests for access to or deletion of your data, can be
raised in the community server where the Bot operates:

https://discord.gg/gfl2-exilium

Contact the server's moderators there. Enquiries are welcome in English or Japanese.

## 11. Changes to this policy

This policy may be updated. When it is, the "Last updated" date at the top of this document
is changed. Material changes will be announced in the community server where the Bot
operates. Continued use of the Bot after a change constitutes acceptance of the updated
policy.

## Revision history

| Date | Change |
|---|---|
| 2026-08-18 | Initial version. |

---
---

# プライバシーポリシー（参考訳）

**対象アプリケーション:** `Poludnitsa`（Discord bot）
**運営者:** `Neriteria`
**発効日:** 2026-08-18
**最終更新日:** 2026-08-18

*本ポリシーの正文は上記の英語版です。以下の日本語訳は参考のために提供するものであり、
両者に相違がある場合は英語版が優先します。*

## 1. 概要

`Poludnitsa`（以下「本 bot」）は、開発を委託されたコミュニティサーバーの運営を支援する
ために `Neriteria`（以下「運営者」）が運営する Discord bot です。

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
| Discord のサーバー ID・ユーザー ID・ロール ID・チャンネル ID（数値 ID のみ） | 設定がどのサーバーのものか、ポイント残高が誰のものか、ルールがどのロール／チャンネルに適用されるかの識別 |
| ポイント残高（整数） | ポイント＆ショップ機能の提供 |
| モデレーションルールの定義（トリガーワード、監視対象チャンネル／カテゴリ ID、除外ユーザー／ロール ID、動作種別） | 管理者が設定したモデレーション機能の提供 |
| カスタムコマンドの定義と添付ファイル | 管理者が設定したカスタムコマンド機能の提供 |
| カスタム絵文字の日次使用回数（絵文字 ID と回数のみ） | 絵文字使用統計の提供 |
| サーバーごとのランタイム設定（ログチャンネル ID 等） | サーバーごとの動作設定の提供 |

ポイント残高は、ポイント機能が有効なサーバーでメンバーが発言した際に自動的に作成されます。
それ以外のデータは、サーバー管理者が明示的に設定した場合にのみ作成されます。

## 3. メッセージ本文の取り扱い

本 bot は、導入されたサーバー内で送信されたメッセージの本文を受信し、以下の目的で使用します。

- サーバー管理者が設定したトリガーワードとの照合（モデレーション）
- カスタムコマンドの呼び出し判定（サーバーで設定されたプレフィックスで始まるメッセージの検出）
- そのサーバーのカスタム絵文字の使用回数の集計

**メッセージ本文を Discord 外へ保存することはありません。** 受信したメッセージはメモリ上で
評価されるのみで、評価後ただちに破棄されます。本文がデータベースへ書き込まれることはなく、
運用ログに含まれることもなく、第三者や外部サービスへ送信されることもありません。

例外は 1 点のみで、それも Discord 内で完結します。モデレーションルールが動作した際、
本 bot は**同じ Discord サーバー内**のログチャンネルへ監査記録を投稿し、その記録には
一致したメッセージの内容が含まれます。この記録は当該チャンネルを閲覧できる者のみが
参照でき、サーバー管理者の管理下にあり、運営者ではなく Discord のデータ取り扱いに従います。

運営者が保持する運用ログには、意図的にメッセージ本文を含めていません。モデレーション動作の
ログに記録されるのは、動作種別・ルール名・関係するサーバー ID・ユーザー ID・チャンネル ID・
メッセージ ID のみです。

## 4. 取得しないデータ

本 bot は以下を取得・保存しません。

- メッセージ本文（第 3 項に記載した一時的な処理を除く）
- ユーザー名、表示名、アバター、プロフィール情報
- メールアドレス、氏名、電話番号、住所
- IP アドレス、端末情報
- 決済情報（本 bot に有料機能はありません。「ポイント」はサーバー内の値であり金銭的価値を
  持たず、購入も換金もできません）
- 音声データ、他ユーザー宛の DM、プレゼンス／アクティビティ状態

## 5. データの保存場所

保存されるデータは、Amazon Web Services（Amazon DynamoDB および Amazon S3）の
`ap-northeast-1`（東京）リージョンの、運営者が管理するアカウントに保管されます。
アクセスできるのは運営者のみです。

当該インフラを保持するアカウントは、同一のコミュニティサーバーのために運用される
別のアカウントへ移管されることがあります。移管によって、取得するデータ、その目的、
アクセスできる者が変わることはありません。

本 bot は日本から運営され、利用者は世界各地に所在します。欧州経済領域または英国に
所在する利用者について、日本は欧州委員会により十分な個人データ保護の水準を確保している
と認定されているため、日本国内での保管に追加の保護措置は必要ありません。

## 6. 第三者提供

データを第三者へ販売・貸与・提供することはありません。AI・機械学習モデルの学習には
一切使用しません。広告やプロファイリングにも使用しません。

法令に基づき開示が必要な場合、および本 bot 自体への不正利用を調査する必要がある場合に
限り、開示することがあります。

## 7. 保存期間・削除・利用者の権利

- データは、本 bot が当該サーバーに在籍し、そのデータが利用されている間保持されます。
- 本 bot がサーバーから退出した場合、当該サーバーのデータを削除します。
- 利用者は、第 10 項の連絡先に連絡することで、自身のデータ（ポイント残高等）の削除を
  請求できます。請求は合理的な期間内に対応します。
- サーバー管理者は、自身が作成した設定データ（ルール、カスタムコマンドとその添付ファイル）を
  本 bot のコマンドによりいつでも削除できます。

第 3 項に記載した監査記録は本 bot のストレージではなく Discord のチャンネル上に存在します。
その削除は、サーバー管理者が Discord 上で行ってください。

所在地を問わず、利用者は運営者に対し、自身に関して保持されているデータの開示、
誤りがある場合の訂正、削除、および処理の停止を請求できます。請求は無償で、第 10 項の
連絡先から行えます。本 bot は Discord のユーザー ID のみで利用者を識別しているため、
対象データを特定できるよう、該当する Discord アカウントから請求してください。

欧州経済領域または英国に所在する利用者にとって、これらはアクセス権・訂正権・消去権・
処理制限権・異議申立権に相当します。また、所在国のデータ保護監督機関へ苦情を申し立てる
権利も有します。

## 8. 利用者の選択肢

**モデレーション:** メンバー個人によるオプトアウトは提供していません。対象となる本人が
自分だけ無効化できるモデレーション機能は機能しないためです。適用の可否を決めるのは
サーバー管理者であり、管理者は特定のユーザー・ロールを除外設定でき、ルールの適用範囲を
特定のチャンネル／カテゴリに限定できます。ルールに一致しないメッセージについては、
モデレーションに関するデータは一切残りません（第 3 項参照）。

**ポイント:** ポイント残高の保持を望まないメンバーは、運営者に連絡することでオプトアウト
できます。残高は削除され、以後ポイントは記録されません。

**カスタムコマンド:** メンバーが自らプレフィックス付きのコマンド名を投稿した場合にのみ
動作します。

**絵文字統計:** 絵文字 ID と回数のみを集計します。誰が使用したかは記録しないため、
個人に紐づくデータは存在しません。

**サーバー全体:** サーバー管理者は、本 bot を退出させることで、当該サーバーにおける
すべてのデータ取得を即座に終了できます。

## 9. 未成年の利用について

本 bot は子どもを対象としたものではありません。Discord の利用には、Discord 利用規約が
国ごとに定める最低年齢を満たす必要があります。本 bot は当該年齢未満の利用者のデータを
意図的に保持しません。該当が判明した場合は削除します。

## 10. 連絡先

本ポリシーに関する質問、およびデータの開示・削除の請求は、本 bot が稼働している
コミュニティサーバーで受け付けます。

https://discord.gg/gfl2-exilium

同サーバーのモデレーターへご連絡ください。問い合わせは英語または日本語で受け付けます。

## 11. 本ポリシーの変更

本ポリシーは更新されることがあります。更新時は冒頭の「最終更新日」を変更します。
重要な変更については、本 bot が稼働するコミュニティサーバーで告知します。
変更後も本 bot の利用を継続した場合、更新後のポリシーに同意したものとみなします。

## 変更履歴

| 日付 | 変更内容 |
|---|---|
| 2026-08-18 | 初版 |
