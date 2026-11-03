# ZoneDungeons

## Current builds / Versiones actuales — 2026-11-03 revision 2

| Side / Lado | Version | CurseForge |
|---|---|---|
| Server | 1.0.0-beta9 | [Server](https://www.curseforge.com/minecraft/mc-mods/zonedungeons/files/9427364) |
| Client | 1.0.0-beta9 | [Client](https://www.curseforge.com/minecraft/mc-mods/zonedungeons/files/9427356) |

Five private expeditions, personal room-chest/final loot and nearby connected ZParty parties. BOTH sides require LevelUp [2.0.0-beta29-r53,2.0.0-beta30). Core is needed on the server through LevelUp, not in the separated multiplayer client. / Cinco expediciones privadas con cofres/botín personal y ZParty cercano conectado; LevelUp r53+ beta29 en ambos lados, Core solo servidor.

[Release notes / Cambios e instalación](RELEASE-2026-11-03-r2.md). Beta availability depends on file approval. / Disponibilidad sujeta a aprobación del archivo.

## Earlier documentation / Documentación anterior

The version and side table above takes precedence over historical versions below. / La tabla anterior prevalece sobre versiones históricas de la documentación siguiente.

## English

Administrator-built physical dungeons and independent farming spots, ordered rooms, mob profiles, a configurable final boss, personal loot and persistent encounter state. Use /zonedungeons lista, /zonedungeons entrar <id> and /zonedungeons estado. Administrators build the arena, define a draft, mark bounds/triggers/spawns, validate and publish it. Config: config/ZONEMODS/zonedungeons/. Beta6-r1 fixes TOML room ordering. Requires the matching ZoneLevelUp side. Never install the combined laboratory singleplayer JAR with the separated distributions.

## Español

Mazmorras físicas creadas por administradores y spots independientes, salas ordenadas, perfiles de mobs, jefe final configurable, botín personal y persistencia. Usa /zonedungeons lista, entrar <id> y estado. La administración construye, configura borrador/límites/activadores/apariciones, valida y publica. Configuración: config/ZONEMODS/zonedungeons/. Beta6-r1 corrige el orden de salas TOML. Requiere ZoneLevelUp del lado correspondiente. No mezcles el JAR combinado de laboratorio con los separados.


| Side / Lado | Version | File |
|---|---|---|
| server | 1.0.0-beta6-r1 | `zonedungeons-1.0.0-beta6-r1-server-protected.jar` |
| client | 1.0.0-beta6-r1 | `zonedungeons-1.0.0-beta6-r1-client-protected.jar` |

## Dependencies / Dependencias

- **server**: zonelevelup: Required Dependency ([2.0.0-beta29-r26,2.0.0-beta30))
- **client**: zonelevelup: Required Dependency ([2.0.0-beta29-r26,2.0.0-beta30))

## Installation / Instalación

Install only the file for each side. Never mix two versions or both side distributions in one mods folder. Back up the world and preserve TOML/player data. Dedicated-server-only mods do not belong in a client modpack.

Instala solo el archivo del lado correspondiente. No mezcles versiones ni ambos JAR en una carpeta mods. Respalda mundo y conserva TOML/progreso. Los mods exclusivos de servidor no van en el modpack de cliente.

Protected public files retain features without distributing private source, mappings or production configuration/account data. File/resources/shared schemas and isolated server startup/clean save were checked; no new GUI/full-modpack or live multiplayer test was performed. File availability depends on CurseForge approval.

Los archivos públicos conservan funciones con protección, sin fuentes, mappings ni datos privados. Se verificaron archivos/esquemas y arranque/cierre local aislado; no una nueva prueba gráfica o multijugador real. Disponibilidad sujeta a aprobación de CurseForge.

## Ownership / Titularidad

Original ZONE code and artwork © Elgochogms. All Rights Reserved. Public documentation repository only; source and mappings remain private.
