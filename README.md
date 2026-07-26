# Victus Engine — prebuilt server jars

GPL-3.0. Source: https://github.com/Gravatar123A/victus-engine
Run on Java 25: `java -XX:+UseZGC -XX:+ZGenerational -jar victus-server.jar --nogui`

## Current build

- Minecraft/Paper base: `26.2`
- Victus Engine source: `02ae25c2e5fa093ff85de0dd48d0719586d74c8c`
- Size: `64,363,656` bytes
- SHA-256: `db285d9d66e7ac76976c6ee2be2462982b916c9a9342a1367551c0c0bae0cf7e`
- Validated with Java 25, including 40 console commands across startup with zero command exceptions.

## Pterodactyl

Import [`egg-victus-engine.json`](egg-victus-engine.json) into a Pterodactyl Minecraft nest and use its Java 25 image. The egg installs a commit-pinned, validated Victus Engine build and can optionally install ViaVersion and ViaBackwards for older Java client protocol support.

Victus Engine is currently built against Minecraft/Paper 26.2. One server JAR cannot safely run every historical Minecraft server version. ViaVersion and ViaBackwards provide supported client protocol compatibility (currently advertised upstream as 1.8–26.2); separate engine builds must be published for genuinely different server versions. Geyser and Floodgate may be added for Bedrock/mobile clients.