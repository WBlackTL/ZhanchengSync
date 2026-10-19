# Resource packs

This directory is served through GitHub Raw.

Current demo pack:

```
https://raw.githubusercontent.com/WBlackTL/ZhanchengSync/main/resourcepack/ZhanchengSync-Demo.zip
```

Replace `ZhanchengSync-Demo.zip` with your real 1.20.1 resource pack and update
`urlPacks` in `config/packsync-server.json`.

The zip must have `pack.mcmeta` at its root with `pack_format: 15`, or be a
GitHub repository archive containing one pack directory, which the client will
normalize automatically.

Served files should stay below GitHub's 100 MB raw-file limit. Large packs
should be hosted as release assets or on a normal file server.
