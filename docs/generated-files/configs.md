---
sidebar_position: 1
---

# config.toml

Missmojiはconfigの形式としてtomlをサポートしています。

## 初期値

### missmoji-client.toml

クライアントに生成します。

```toml title="missmoji-client.toml"
[clientConfig]
enabledEmojiPacks = []
showExternalEmojis = false
[[clientConfig.addEmojiOptions]]
alwaysDownloadExternalEmojiImage = true
```

### missmoji-server.toml

シングルプレイの場合、ワールドごとに生成します。

```toml title="missmoji-server.toml"
[serverConfig]
notifyToInstallMissmoji = true
enabledEmojiPacks = []
[[serverConfig.addEmojiOptions]]
allowGuestToCreateCache = true
# ONLY ENABLE THIS ONLY IF YOU UNDERSTAND COPYRIGHT RELATED ISSUES
dangerouslyBehaveAsCacheServer = false
```