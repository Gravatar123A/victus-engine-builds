# Victus Engine — prebuilt server jars

GPL-3.0. Source: https://github.com/Gravatar123A/victus-engine
Run on Java 25: `java -XX:+UseZGC -XX:+ZGenerational -jar victus-server.jar --nogui`

## Pterodactyl

Import [`egg-victus-engine.json`](egg-victus-engine.json) into a Pterodactyl Minecraft nest and use its Java 25 image. The egg installs a commit-pinned, validated Victus Engine build and can optionally install ViaVersion and ViaBackwards for older Java client protocol support.

Victus Engine is currently built against Minecraft/Paper 26.2. One server JAR cannot safely run every historical Minecraft server version. ViaVersion and ViaBackwards provide supported client protocol compatibility (currently advertised upstream as 1.8–26.2); separate engine builds must be published for genuinely different server versions. Geyser and Floodgate may be added for Bedrock/mobile clients.