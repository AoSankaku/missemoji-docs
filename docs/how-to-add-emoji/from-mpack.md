---
sidebar_position: 2
---

# emojipackから

このMODは、`emojipacks`というフォルダを新規に生成します。ここに追加することで、手動で追加することができます。

:::tip
emojipacksは、`/missmoji client add`実行時に自動で生成しますが、手動で追加することもできます。
:::

## 前提知識：名前空間

マイクラには「名前空間」というものが存在します。これは、例えば`minecraft:stone`の`minecraft:`、`namae:orijinaru_aitemu`の`namae:`が名前空間を表しています。

ところで、この概念をそのまま絵文字MODに持ち込み、「:」で挟むとこうなってしまいます。

```
:namae:emojinonamae:
```

こうなってしまうことを防ぐために、emojipack経由の絵文字は

```
:emojinonamae@namae.minecraft:
```

に変換されます。名前空間の部分が@の右に来て、その右には`.minecraft`が来ます。こうすることで、例えば`:kiss:`の絵文字が複数あったとしても、衝突することなく正常に処理することができます💋

## emojipackの作成

emojipackのツリー構造は、例えばこのようになっています。

```
(パックの名前)
├── misskey_servers.json
├── pack.json
└── custom_emojis
   ├── category_name
   │    ├── test_emoji1.png
   │    └── test_emoji2.apng
   └── cavegory_name_2
         ├── alias.json
         ├── test_emoji3.gif
         └── test_emoji4.png
```

適切なディレクトリに画像を入れれば、それだけで問題なく動作します。

:::tip
emojipackはリソースパックと同様、zip圧縮してあってもそのままフォルダーになっていても動作します。
:::

### 適用方法

作成したemojipackは、適用が必要です。

## 次のセクション

このMODはEmojifulそのものとは互換性がありませんが、Emojiful用の絵文字データパックとは互換性があります。導入方法についてもお伝えします。
