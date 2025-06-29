# foxloader-mmc-modrinth

This is the ready instance provided by [FoxLoader](https://github.com/Fox2Code/FoxLoader) repository, but patched to support [Modrinth](https://modrinth.com/).

## Patch description

Several changes are made to make this work:
- File `patches/net.minecraft.json`: changed version from `no-op` to `b1.7.3`, so the modrinth could properly fetch minecraft version.
- New file `patches/net.fabricmc.fabric-loader.json`: a stab with `uid` of fabric present, so the launcher could treat this instance as "fake" fabric.
- File `mmc-pack.json`: added same changes, but to cached data.