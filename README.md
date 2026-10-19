# ZhanchengSync

Closed-source Fabric 1.20.1 mod for server-driven resource pack and mod synchronization.

This repository is **not** the source repository. It only hosts:

- `mods/packsync.jar` — the client/server mod download
- `resourcepack/` — resource packs served through GitHub Raw
- GitHub Issues — bug reports and support

## Download

Use the stable file:

```
https://raw.githubusercontent.com/WBlackTL/ZhanchengSync/main/mods/packsync.jar
```

Put it into the `mods/` folder on both the server and client. Fabric Loader 0.15+,
Fabric API 0.92.x for 1.20.1, and Java 17 are required.

## Server URL example

```json
{
  "contentBaseUrl": "https://raw.githubusercontent.com/WBlackTL/ZhanchengSync/main/",
  "urlPacks": ["resourcepack/ZhanchengSync-Demo.zip"],
  "urlMods": ["/mods/packsync.jar"]
}
```

The mod itself is updated through the same `urlMods` entry. Resource packs are
hot-reloaded; mod updates are staged and applied by the updater after the game
exits or at the next pre-launch update.

## Reporting bugs

Open an issue and include:

- Minecraft version, Fabric Loader version, PackSync version
- Server and client logs
- Steps to reproduce
- Relevant `config/packsync-server.json` with secrets removed

The source code is proprietary and is not distributed in this repository.

## License

All rights reserved. Redistribution of modified builds is not permitted.
