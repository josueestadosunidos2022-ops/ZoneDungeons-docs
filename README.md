# ZoneDungeons

[CurseForge](https://www.curseforge.com/minecraft/mc-mods/zonedungeons) · [Wiki](https://github.com/josueestadosunidos2022-ops/ZoneDungeons-docs/wiki) · [Issues](https://github.com/josueestadosunidos2022-ops/ZoneDungeons-docs/issues)

## English

Physical, administrator-built dungeons for Minecraft Java 1.20.1 / Forge 47.4.x / Java 17. Configure ordered rooms, proximity-triggered encounters, waves, personal loot, cooldowns and farming spots in TOML. This mod does not generate buildings or create parallel dungeon instances.

**Requires ZoneLevelUp beta29-r26 or later within beta29**; the current companion release is **beta29-r28**. Install ZoneDungeons **1.0.0-beta2** Server on the dedicated server and matching Client on players. For singleplayer use only Client, which includes integrated-server logic. Do not install both side JARs together. Dedicated ZoneLevelUp requires ZoneCore server-side; Core is not forced on multiplayer clients.

Administrators configure `config/ZONEMODS/zonedungeons/`: general settings, mobs, loot, dungeons and spots. Players enter using `/zonedungeons entrar <id>` according to configured IDs, requirements and server rules. Encounter mobs are marked so unrelated kills do not advance a room. Rewards are personal; inventory-full claims remain pending. Existing saved data is preserved.

The beta2 resource packaging fix includes valid `pack.mcmeta` format 15, with no gameplay, network or save-data changes. Protected public builds exclude private server data and sources. Archive/shared-schema and isolated server startup checks do not certify real multiplayer or graphical gameplay.

## Español

Mazmorras físicas construidas por la administración para Minecraft Java 1.20.1 / Forge 47.4.x / Java 17. Configura salas ordenadas, encuentros por proximidad, oleadas, botín personal, esperas y spots de farmeo mediante TOML. No genera edificios ni crea instancias paralelas.

**Requiere ZoneLevelUp beta29-r26 o superior dentro de beta29**; la versión acompañante actual es **beta29-r28**. Instala ZoneDungeons **1.0.0-beta2** Server en el dedicado y Client en cada jugador. En mundo individual usa solo Client, que incluye servidor integrado. No mezcles los dos JAR en una carpeta. ZoneLevelUp dedicado necesita ZoneCore solo en el servidor.

La configuración está en `config/ZONEMODS/zonedungeons/`: ajustes generales, mobs, botines, mazmorras y spots. Los jugadores usan `/zonedungeons entrar <id>` con los identificadores y requisitos definidos por el servidor. Las marcas de encuentro evitan contar muertes ajenas a una sala; las recompensas son personales y quedan pendientes si no hay espacio. Se conservan los datos existentes.

La corrección de recursos beta2 incluye `pack.mcmeta` formato 15 sin cambiar lógica, red ni datos guardados. Compilación pública protegida sin fuentes ni datos privados. Las verificaciones locales no certifican cliente gráfico ni multijugador real.

## Release files / Archivos de esta publicación

Minecraft **1.20.1** · Forge **47.4.x** · Java **17**. Check the approval status on CurseForge before downloading. / Comprueba la aprobación en CurseForge antes de descargar.

| Side / Lado | Version / Versión | CurseForge file / Archivo |
|---|---|---|
| server | 1.0.0-beta2 | [9303276](https://www.curseforge.com/minecraft/mc-mods/zonedungeons/files/9303276) |
| client | 1.0.0-beta2 | [9303281](https://www.curseforge.com/minecraft/mc-mods/zonedungeons/files/9303281) |

## Installation checklist / Lista de instalación

1. Back up your world and existing TOML files. / Respalda tu mundo y los TOML existentes.
2. Stop the game or server before replacing JAR files. / Cierra el juego o servidor antes de sustituir JAR.
3. Keep one matching version for each installation side. / Mantén una versión correspondiente a cada lado.
4. Preserve player progress and configuration; remove the previous JAR only from the active mods folder. / Conserva progreso y configuración; retira el JAR anterior de la carpeta mods activa.

## Player commands / Comandos de jugadores

| Command / Comando | Use / Uso |
|---|---|
| `/zonedungeons lista` | Available dungeons / Mazmorras disponibles |
| `/zonedungeons entrar <id>` | Join at its configured entrance / Unirse desde la entrada configurada |
| `/zonedungeons estado` | Session status / Estado de partida |
| `/zonedungeons salir` | Leave the session / Salir de la partida |

Administration requires operator level 2. Build rooms in the world, define their regions and encounters, validate the draft, then publish it. Do not reload definitions during active sessions. / La administración requiere operador nivel 2. Construye las salas, define regiones y encuentros, valida el borrador y publícalo. No recargues definiciones durante partidas activas.

## Support / Soporte

Open an Issue with the exact mod version, Minecraft/Forge version, installation side, steps to reproduce, and a sanitized log excerpt. Remove credentials, private addresses and player data. / Abre un Issue con versión exacta del mod, Minecraft/Forge, lado de instalación, pasos y un fragmento de log sin datos privados. Elimina credenciales, direcciones privadas y datos de jugadores.

## Ownership / Titularidad

Documentation and original ZONE assets © Elgochogms. All rights reserved. This repository distributes public documentation only; it contains no mod source code, private mappings, secrets, player accounts or production configuration. / Documentación y recursos originales ZONE © Elgochogms. Todos los derechos reservados. Este repositorio contiene documentación pública; no distribuye fuentes del mod, mapas privados, secretos, cuentas ni configuración de producción.
