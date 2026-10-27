# プライバシーポリシー

**対象アプリケーション:** `WoWS Utility App`（Discord bot）
**運営者:** `Neriteria`
**発効日:** 2026-10-28
**最終更新日:** 2026-10-28

*本ポリシーの正文は日本語版です。下部の英語訳は参考のために提供するものであり、両者に
相違がある場合は日本語版が優先します。*

*(The Japanese text is authoritative. An English translation follows below for reference
only; in case of any discrepancy, the Japanese version prevails.)*

---

## 1. 概要

`WoWS Utility App`（以下「本 bot」）は、World of Warships のプレイヤー向けに、リプレイ
ファイルからタイムラプス動画を生成する機能などを提供する Discord bot です。個人である
`Neriteria`（以下「運営者」）が運営しています。

本ポリシーは、本 bot が取得するデータ、その目的、保存場所、保存期間、および削除方法に
ついて説明します。

本 bot をサーバーに導入した時点で、当該サーバーの管理者はサーバーを代表して本ポリシーに
同意したものとみなします。本 bot の機能を利用した利用者は、以下に記載する範囲で本ポリシーの
対象となります。

本 bot は AI・機械学習を一切使用しません。取得したデータを第三者へ販売・提供することは
なく、広告表示・プロファイリング・サーバーをまたいだ分析も行いません。

## 2. 取得・保存するデータ

本 bot は、利用者がコマンドを実行したときにのみデータを取得します。取得するデータは
以下のとおりです。

| データ | 目的 | 保存期間 |
|---|---|---|
| 利用者がコマンドに添付したリプレイファイル（`.wowsreplay`） | タイムラプス動画およびビルドカード画像の生成、本 bot の機能改善および不具合の調査・修正（下記参照） | 30 日後に自動削除 |
| 生成したタイムラプス動画およびビルドカード画像 | 生成結果の送信、および生成後にビルドカードを表示するため | 30 日後に自動削除 |
| プリセット（Discord ユーザー ID、プリセット名、描画オプションの設定値、更新日時、既定プリセットの設定） | 利用者が保存した描画設定の再利用 | 利用者が削除するまで |
| 運用ログ（下記参照） | 障害の調査、不正利用への対処、問い合わせへの対応 | 30 日後に自動削除 |

運用ログには、コマンドが実行されるたびに以下の項目が記録されます。

- コマンド名、実行日時
- 実行者の Discord ユーザー ID およびユーザー名
- 実行場所のサーバー ID・サーバー名・チャンネル ID
- 処理ごとに割り当てる識別番号（ジョブ ID）、処理結果、エラー情報

プリセットは、利用者が自らプリセットを保存した場合にのみ作成されます。

### リプレイファイルの機能改善・不具合修正への利用

送信されたリプレイファイルは、動画の生成に加えて、本 bot の機能改善および不具合の
調査・修正に利用することがあります。たとえば、描画に失敗したリプレイの原因調査や、
修正後の動作確認に使用します。

この目的のために、運営者が保存期間内のリプレイファイルを複製することがあります。
複製は運営者が管理する環境でのみ保管し、目的を達成した時点で削除します。複製した
リプレイファイルを公開したり、第三者へ提供したりすることはありません。

## 3. リプレイファイルに含まれる他のプレイヤーの情報

World of Warships のリプレイファイルには、録画した本人だけでなく、同じ試合に参加した
すべてのプレイヤーのゲーム内の名前、艦艇、装備構成、ゲーム内チャットが記録されています。
これらの情報は、第 2 項に記載した目的（動画とビルドカード画像の生成、機能改善および不具合の
調査・修正）にのみ使用し、それ以外の目的では利用・集計しません。

生成されるものには、以下のとおり他のプレイヤーの情報が含まれることがあります。

- **タイムラプス動画:** 描画オプションの設定によっては、プレイヤー名およびゲーム内チャットが
  映ります。動画は**コマンドを実行したチャンネルへ投稿**され、そのチャンネルを閲覧できる
  すべての人が見ることができます。プレイヤー名やチャットを映すかどうかは、実行者が描画
  オプションで選択できます。
- **ビルドカード画像:** プレイヤー名と装備構成が含まれます。動画を生成した実行者が選択した
  場合に限り、実行者本人にのみ見えるメッセージとして表示されます。

## 4. メッセージ本文

本 bot は、サーバー内で送信されたメッセージの本文を読み取りません。処理するのは、
スラッシュコマンドの入力内容と、コマンドに添付されたリプレイファイルのみです。

## 5. 取得しないデータ

本 bot は以下を取得・保存しません。

- メッセージ本文（第 4 項参照）
- アバター、プロフィール情報、サーバーのメンバー一覧
- メールアドレス、氏名、電話番号、住所
- IP アドレス、端末情報
- 決済情報（本 bot に有料機能はありません）
- 音声データ、他ユーザー宛の DM、プレゼンス／アクティビティ状態

## 6. データの保存場所

データは、Amazon Web Services（AWS）の `ap-northeast-1`（東京）リージョンにある、
運営者が管理するアカウントに保管・処理されます。プリセットは Amazon DynamoDB に、
リプレイファイルと生成物は Amazon S3 に、運用ログは Amazon CloudWatch Logs に
保存されます。動画の生成は AWS Lambda 上で行います。アクセスできるのは運営者のみです。

本 bot は日本から運営されています。日本は欧州委員会により十分な個人データ保護の水準を
確保していると認定されています。このため、欧州経済領域または英国に所在する利用者の
データを日本国内で保管するにあたり、追加の保護措置は必要ありません。

## 7. 第三者提供

データを第三者へ販売・貸与・提供することはありません。AI・機械学習モデルの学習には
一切使用しません。広告やプロファイリングにも使用しません。

法令に基づき開示が必要な場合、および本 bot 自体への不正利用を調査する必要がある場合に
限り、開示することがあります。

## 8. 保存期間・削除・利用者の権利

- **リプレイファイルと生成物**は、保存から 30 日後に自動的に削除されます。削除後は、
  過去の動画に付いているビルドカードの選択メニューも利用できなくなります。
- 機能改善・不具合修正のために運営者が**複製したリプレイファイル**は、目的を達成した時点で
  削除します（第 2 項参照）。
- **プリセット**は、利用者が `/timelapse preset delete` コマンドでいつでも削除できます。
  プリセットはサーバーではなく利用者に紐づくため、本 bot がサーバーから退出しても
  削除されません。
- **運用ログ**は、記録から 30 日後に自動的に削除されます。
- チャンネルに投稿された動画は Discord 上のメッセージであり、運営者の保存領域ではなく
  Discord に保存されています。削除は、当該サーバーの管理者が Discord 上で行ってください。

所在地を問わず、利用者は運営者に対し、自身に関して保持されているデータの開示、
誤りがある場合の訂正、削除、および処理の停止を請求できます。請求は無償で、第 11 項の
連絡先から行えます。本 bot は Discord のユーザー ID で利用者を識別しているため、
対象データを特定できるよう、該当する Discord アカウントから請求してください。
請求は合理的な期間内に対応します。

欧州経済領域または英国に所在する利用者にとって、これらはアクセス権・訂正権・消去権・
処理制限権・異議申立権に相当します。また、所在国のデータ保護監督機関へ苦情を申し立てる
権利も有します。

## 9. 利用者の選択肢

**機能の利用:** 本 bot は、利用者が自らコマンドを実行した場合にのみ動作します。
コマンドを実行しない限り、その利用者に関するデータは取得されません。

**動画の内容:** プレイヤー名やゲーム内チャットを動画に映すかどうかは、描画オプションで
選択できます。

**プリセット:** プリセットの保存は任意です。保存しなくても動画の生成は利用できます。

**サーバー全体:** サーバー管理者は、Discord のサーバー設定（連携サービス）で本 bot の
コマンドを使えるメンバーやチャンネルを制限できます。また、本 bot を退出させることで、
当該サーバーでの利用を即座に終了できます。

## 10. 未成年の利用について

本 bot は子どもを対象としたものではありません。Discord の利用には、Discord 利用規約が
国ごとに定める最低年齢を満たす必要があります。本 bot は当該年齢未満の利用者のデータを
意図的に保持しません。該当が判明した場合は削除します。

## 11. 連絡先

本ポリシーに関する質問、およびデータの開示・削除の請求は、以下のサポートサーバーで
受け付けます。

https://discord.gg/sWzGnFygJK

問い合わせは日本語で受け付けます。

## 12. 本ポリシーの変更

本ポリシーは更新されることがあります。更新時は冒頭の「最終更新日」を変更します。
重要な変更については、第 11 項のサポートサーバーで告知します。変更後も本 bot の利用を
継続した場合、更新後のポリシーに同意したものとみなします。

## 変更履歴

| 日付 | 変更内容 |
|---|---|
| 2026-10-28 | 初版 |

---
---

# Privacy Policy (reference translation)

**Application:** `WoWS Utility App` (Discord bot)
**Operator:** `Neriteria`
**Effective date:** 2026-10-28
**Last updated:** 2026-10-28

*This English text is a translation provided for reference only. The Japanese version above
is authoritative; in case of any discrepancy between the two, the Japanese version
prevails.*

## 1. Overview

`WoWS Utility App` ("the Bot") is a Discord bot that provides utilities for World of
Warships players, such as generating time-lapse videos from replay files. It is operated by
an individual, `Neriteria` ("the Operator").

This policy explains what data the Bot collects, why it collects it, where it is stored,
how long it is kept, and how you can have it removed.

By adding the Bot to a Discord server, the server's administrators agree to this policy on
behalf of that server. Users who use the Bot's features are subject to this policy for the
data described below.

The Bot uses no artificial intelligence or machine learning. It does not sell, rent, or
share data with third parties. It does not display advertising, build user profiles, or
analyse data across servers.

## 2. Data the Bot collects and stores

The Bot collects data only when a user runs one of its commands. The data it collects is:

| Data | Purpose | Retention |
|---|---|---|
| Replay files (`.wowsreplay`) attached to a command by the user | Generating time-lapse videos and build card images; improving the Bot and investigating and fixing defects (see below) | Deleted automatically after 30 days |
| Generated time-lapse videos and build card images | Delivering the result, and showing build cards after generation | Deleted automatically after 30 days |
| Presets (Discord user ID, preset name, rendering option values, last-updated time, default-preset setting) | Letting users reuse rendering settings they saved | Until the user deletes them |
| Operational logs (see below) | Investigating failures, dealing with abuse, and answering enquiries | Deleted automatically after 30 days |

Each time a command is run, the operational logs record:

- the command name and the time it was run;
- the Discord user ID and username of the user who ran it;
- the server ID, server name and channel ID where it was run;
- an identifier assigned to each job, the result, and any error information.

Presets are created only when a user chooses to save one.

### Use of replay files to improve the Bot and fix defects

In addition to generating videos, submitted replay files may be used to improve the Bot and
to investigate and fix defects — for example, to find out why a replay failed to render, or
to confirm that a fix works.

For this purpose, the Operator may make a copy of a replay file while it is within its
retention period. Such copies are kept only in an environment controlled by the Operator and
are deleted once the purpose has been achieved. Copied replay files are never published or
shared with third parties.

## 3. Information about other players contained in replay files

A World of Warships replay file records not only the player who recorded it, but also the
in-game names, ships, loadouts and in-game chat of every player in that match. This
information is used only for the purposes described in section 2 (generating videos and
build card images, and improving the Bot and investigating and fixing defects), and is not
used or aggregated for any other purpose.

The generated output may contain information about other players, as follows:

- **Time-lapse videos:** depending on the rendering options, player names and in-game chat
  may appear in the video. The video is **posted to the channel where the command was run**
  and can be seen by everyone who can view that channel. The user who runs the command
  chooses, through the rendering options, whether player names and chat are shown.
- **Build card images:** these contain player names and loadouts. They are shown only when
  the user who generated the video selects one, as a message visible only to that user.

## 4. Message content

The Bot does not read the content of messages sent in servers. It processes only the input
to its slash commands and the replay files attached to them.

## 5. Data the Bot does not collect

The Bot does not collect or store:

- message content (see section 4);
- avatars, profile information, or server member lists;
- email addresses, real names, phone numbers, or postal addresses;
- IP addresses or device information;
- payment information (the Bot has no paid features);
- voice data, direct messages sent to other users, or presence/activity status.

## 6. Where data is stored

Data is stored and processed in Amazon Web Services (AWS), in the `ap-northeast-1` (Tokyo,
Japan) region, in an account controlled by the Operator. Presets are stored in Amazon
DynamoDB, replay files and generated output in Amazon S3, and operational logs in Amazon
CloudWatch Logs. Videos are generated on AWS Lambda. Access is restricted to the Operator.

The Bot is operated from Japan. Japan has been recognised by the European Commission as
providing an adequate level of data protection, so storing the data of users in the
European Economic Area or the United Kingdom in Japan does not require additional
safeguards.

## 7. Data sharing

Data is never sold, rented, or shared with third parties. It is not used to train
artificial intelligence or machine learning models. It is not used for advertising or
profiling.

Data may be disclosed only where required by applicable law, or where necessary to
investigate abuse of the Bot itself.

## 8. Retention, deletion and your rights

- **Replay files and generated output** are deleted automatically 30 days after they are
  stored. After that, the build card menu attached to an older video stops working.
- **Copies of replay files** made by the Operator to improve the Bot or fix defects are
  deleted once the purpose has been achieved (see section 2).
- **Presets** can be deleted by the user at any time with the `/timelapse preset delete`
  command. Presets belong to the user rather than to a server, so they are not deleted when
  the Bot leaves a server.
- **Operational logs** are deleted automatically 30 days after they are recorded.
- A video posted to a channel is a Discord message, stored by Discord rather than in the
  Operator's storage. Deleting it is done through Discord by the server's administrators.

Wherever you are located, you may ask the Operator to tell you what data is held about you,
to correct it if it is wrong, to delete it, or to stop processing it. Requests are free of
charge and can be made using the contact details in section 11. Because the Bot identifies
you by your Discord user ID, a request must be made from the Discord account concerned so
that it can be matched to the right data. Requests are handled within a reasonable period.

If you are in the European Economic Area or the United Kingdom, these correspond to your
rights of access, rectification, erasure, restriction and objection, and you also have the
right to lodge a complaint with your local data protection authority.

## 9. Your choices

**Using the features.** The Bot acts only when a user deliberately runs a command. No data
about a user is collected unless that user runs a command.

**Video content.** Whether player names and in-game chat appear in a video can be chosen in
the rendering options.

**Presets.** Saving a preset is optional. Videos can be generated without one.

**Whole server.** A server administrator can restrict which members and channels can use
the Bot's commands in Discord's server settings (Integrations), and can end the Bot's use in
their server immediately by removing it.

## 10. Children

The Bot is not directed at children. Use of Discord requires users to meet the minimum age
set out in the Discord Terms of Service for their country. The Bot does not knowingly
retain data belonging to anyone below that age; if such data is identified, it will be
deleted.

## 11. Contact

Questions about this policy, and requests for access to or deletion of your data, can be
raised in the support server:

https://discord.gg/sWzGnFygJK

Enquiries are handled in Japanese.

## 12. Changes to this policy

This policy may be updated. When it is, the "Last updated" date at the top of this document
is changed. Material changes will be announced in the support server given in section 11.
Continued use of the Bot after a change constitutes acceptance of the updated policy.

## Revision history

| Date | Change |
|---|---|
| 2026-10-28 | Initial version. |
