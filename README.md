# Server Pinger Fixer (NeoForge)

Unofficial NeoForge port of [Server Pinger Fixer](https://modrinth.com/mod/serverpingerfixer) by JustAlittleWolf.
Please don't report issues to JustAlittleWolf, use this repo's issue tracker.

Improves how servers in the multiplayer list are pinged. In vanilla the list can get stuck on "Pinging..."
after pressing refresh a few times, or when some servers in the list don't answer. With this mod the other
servers still load.

It uses more threads for pinging servers and clears them out when they pile up.

Client-side only, no dependencies, fine to put in modpacks.

| Minecraft | NeoForge | Java |
|---|---|---|
| 1.20.4 | 20.4.253 or newer | 17 |
| 1.21 | 21.0.167 or newer | 21 |
| 1.21.1 | 21.1.252 or newer | 21 |
| 1.21.4 | 21.4.161 or newer | 21 |
| 1.21.5 | 21.5.101 or newer | 21 |
| 1.21.8 | 21.8.57 or newer | 21 |
| 1.21.10 | 21.10.64 or newer | 21 |
| 1.21.11 | 21.11.48 or newer | 21 |
| 26.1.2 | 26.1.2.122 or newer | 25 |
| 26.2 | 26.2.0.93 or newer | 25 |
| 26.3 | 26.3.0.94 or newer | 25 |

## Install
Put the jar for your Minecraft version in the `mods` folder of a NeoForge instance. Servers do not need it.

## Build
Each Minecraft version is its own Gradle project under `versions/`.

```
cd versions/26.3
./gradlew build
```

The jar lands in `versions/<version>/build/libs/`.

## Licence
MIT, same as the original. See [LICENSE](LICENSE).
