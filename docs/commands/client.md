---
sidebar_position: 1
---

# クライアント用コマンド

シングルプレイ、またはサーバーにMissmojiが入っていない場合はこちら。

## クライアントコマンドの挙動

`/missmoji client`で始まるコマンドは、自分のプレイ環境にのみ影響を与えます。

基本的に、ほとんどのプレイヤー（サーバーに参加する側）にとって必要な動作は、こちらのコマンドで完結します。

## コマンド一覧

### 確認用

#### `/missmoji client version`

今入っているMissmojiのバージョンを確認することができます。

#### `/missmoji client list (server/manual/datapack)`

自分が追加した絵文字の一覧を表示します。serverを選択した場合はMisskeyサーバーを、manualを選択した場合はコマンドで追加したものを、datapackを選択した場合はデータパックを表示します。指定しなかった場合はすべてを表示します。

### 絵文字を追加する

:::warning マルチプレイをする場合
マルチプレイをする際にこの操作を行うと、相手に絵文字の内容が伝わらない可能性が高まります。
:::

#### `/missmoji client <enable/disable> <絵文字名またはemojipack名>`

特定の絵文字またはemojipackの有効（enable）、無効（disable）を切り替えます。

#### `/missmoji client add <URLまたはローカルディレクトリの名前> (絵文字名)`

**自分のみ利用可能な絵文字**を追加することができます。シングルプレイに適しています。

このコマンドについては、[こちら](/docs/how-to-add-emoji/from-command#%E3%83%AD%E3%83%BC%E3%82%AB%E3%83%AB%E3%81%AB%E8%BF%BD%E5%8A%A0%E3%81%99%E3%82%8B%E5%A0%B4%E5%90%88%E3%82%B7%E3%83%B3%E3%82%B0%E3%83%AB%E3%83%97%E3%83%AC%E3%82%A4%E5%90%91%E3%81%91)をご覧ください。

#### `/missmoji client update <diff/all/single> <single -> name>`

クライアントに保存してある絵文字のアップデート作業を行います。

このコマンドについては、[こちら](/docs/how-to-add-emoji/from-misskey#%E7%B5%B5%E6%96%87%E5%AD%97%E3%81%AE%E5%86%8D%E8%AA%AD%E3%81%BF%E8%BE%BC%E3%81%BF)をご覧ください。