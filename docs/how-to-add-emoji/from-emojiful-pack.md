---
sidebar_position: 3
---

# Emojifulのデータパックから

Emojifulのデータパックは、以下のような構造になっています。このような形式のパックであっても、Missmojiでそのまま読み込むことができます。

```
ファイル名.zip
 ├── pack.mcmeta
 └── data/emojiful/recipes
```

このrecipesフォルダの中にJSONが入っています。

:::tip data/emojiful/recipesとは

これは一つのフォルダ名ではなく、

```
└── dataフォルダの中の
    └── emojifulフォルダの中の
        └── recipesフォルダ
```

という意味です。

:::

中身は、例えば

```json title="test.json"
{
  "category": "Kategoridesuyo",
  "name": "emojino_namae",
  "url": "https://path_to_gazou.png",
  "type": "emojiful:emoji_recipe"
}
```

のようになっています。

:::caution

この形式では当然のことながら、絵文字を何処かのサーバーにアップロードしておくことが必要となります。画像のアップロード先サーバーがダウンしている間は取得することができず、また相手方サーバーに負担をかけてしまうため非推奨です。

:::

これを手動で作成することもできますが、Discordの絵文字を導入したい場合は[Emojifulの公式Discord（Industrial Foregoing）](https://discord.gg/4tPfwjn)からBOTを使用して作成することができます。詳しいやり方は実際のチャットを参照してください。

## 次のセクション

データパックの作成が面倒であれば、コマンドから追加することもできます。コマンドから作成した場合は、リソースパックを自動で作成して適用します。