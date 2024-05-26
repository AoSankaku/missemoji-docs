---
sidebar_position: 1
---

# config.toml

Missmojiはconfigの形式としてtomlをサポートしています。

## 初期値

### missmoji-client.toml

クライアントに生成します。

```toml title=missmoji-client.toml

```

### missmoji-server.toml

シングルプレイの場合、ワールドごとに生成します。

```toml title=missmoji-server.toml
notify-to-install-missmoji = true
auto-installed-misskey-server = []
```