# ZoneDungeons — Configuration / Configuración (2026-11-08)

| Side / Lado | Version / Versión |
|---|---|
| Server / Servidor | 1.0.0-beta10 |
| Client / Cliente | 1.0.0-beta10 |

## Server files / Archivos del servidor

`config/ZONEMODS/zonedungeons/MasmorrasZ/general.toml` and `nivel_20.toml`, `nivel_40.toml`, `nivel_60.toml`, `nivel_80.toml`, `nivel_100.toml`, `nivel_120.toml`, `nivel_150.toml`. Files are generated only when absent. General ZoneDungeons limits remain in `config/ZONEMODS/zonedungeons/general.toml`. / Los archivos solo se crean si faltan; se conservan los valores existentes.

| Per-tier key / Clave por nivel | Default / Inicial | Meaning / Uso |
|---|---:|---|
| `max_jugadores` |5| Capacity / Aforo |
| `espera_segundos` |300| Entry queue / Espera de entrada |
| `duracion_segundos` |1800| Combat duration / Duración combate |
| `botin_segundos` |60| Post-victory loot;0 exits immediately / Botín tras victoria;0 salida inmediata |
| `recarga_segundos` |7200| Cooldown / Recarga |
| `premio_godiecoins` |100| Virtual coins per member / Monedas virtuales por miembro |
| `premio_xp` |500| Exact LevelUp XP per member / XP exactos por miembro |
| `moneda_probabilidad_por_1000` |50|5% mob coin drop chance / Probabilidad5% |
| `monedas_por_drop` |5| Physical coins / Monedas físicas |
| `max_cofres` |8| Chest cap / Límite de cofres |
| `objetos_por_cofre` |3| Rolls per chest / Tiradas por cofre |

General defaults: `ganadores_semanales=1`, `premio_semanal_godiecoins=500`, `item_moneda="zonecrates:gochocoin"`. Weekly close uses real time Monday 00:00UTC; waiting/combat/cooldown use server game time. / Cierre semanal por tiempo real; esperas/combate/recarga por tiempo de juego.

## Loot and guardians / Botín y guardianes

Default chests roll from installed item registrations except excluded administration items and create*/mekanism* namespaces. The selection can include powerful modded items. Set `objetos_permitidos_loot` or `objetos_excluidos_loot` and `mods_excluidos_loot` to control balance. Chests are shared, not personal; each new run replaces their inventory. / El botín amplio puede contener objetos poderosos. Configura listas para equilibrarlo; cofres compartidos y contenido reemplazado en la siguiente partida.

Tier guardian health defaults:500/900/1500/2200/3000/4000/5000; armor 6/10/14/18/22/26/30. `jefe_vida` accepts 1–5000, `jefe_armadura`0–30. Effective guardian health, including modifiers, is capped at 5000 without raising every mob's global attribute cap. / Vida y armadura configurables con límite efectivo 5000 solo para guardián.

`jefe_resistencia_melee_porcentaje` and `jefe_resistencia_magia_porcentaje` accept 0–100 and apply after armor. 25 reduces remaining 100 damage to 75; 100 blocks that category. Magic recognizes supported magic tags/types including Iron's Spellbooks; arbitrary external damage needs compatible tags. / Resistencias tras armadura; 25 reduce 100 a 75 y 100 impide esa categoría. Ataques externos requieren etiquetas compatibles.

`jefe_regeneracion_vida=20.0` every `jefe_regeneracion_segundos=10` heals10 hearts per cycle. Zero disables healing; unloaded/offline time does not accumulate healing. `jefe_efectos_negativos`, duration/amplifier control harmful on-hit effects; amplifier0 is levelI. / Regeneración por tiempo de juego, sin acumular tiempo descargado; amplificador0 es nivelI.

Empty `mobs=[]` chooses installed compatible humanoid hostiles or a zombie fallback. Explicit IDs must exist and physically fit the rooms. `jefe="automatico"` selects the guardian; configured external attacks may not use generic.attack_damage. / IDs explícitos deben existir y caber; no todos los ataques externos usan atributo de ataque.

## Administration and data / Administración y datos

```text
/masmorrasz lista
/masmorrasz entrar nivel_20
/masmorrasz top
/zsalir
/masmorrasz recargar
/masmorrasz reiniciar nivel_20
```

Reload/reset require OP level 2; entry uses `zonelevelup.use`. Do not reload with active sessions or structure preparation. `/zonedungeons admin recargar` also reloads MasmorrasZ. Reset expels members and applies cooldown without victory rewards. / Recarga/reinicio requieren OP 2; entrar permiso de uso. Reiniciar expulsa y aplica recarga sin victoria.

Preserve `<world>/data/zonedungeons.dat` and player data for sessions, leaderboard, receipts and pending rewards. A LevelUp cap below 150 prevents reaching all default dungeon levels: administrators may choose `max_level=150` or higher in LevelUp `general.toml`, but the update never forces this change. / Conserva datos. Un límite LevelUp menor 150 impide los niveles máximos predeterminados; el administrador decide cambiar max_level, no se impone.

[Current release / Entrega actual](RELEASE-2026-11-08.md) · [README](README.md).
