# Fast Logic

[![Latest release](https://img.shields.io/github/v/release/andrewmaiorov2010-source/Fast-Logic?display_name=tag)](https://github.com/andrewmaiorov2010-source/Fast-Logic/releases/latest)
![Mindustry 160.7](https://img.shields.io/badge/Mindustry-160.7-orange)
![Java 17](https://img.shields.io/badge/Java-17-blue)

[Русская версия](docs/README.ru.md) · [Releases](https://github.com/andrewmaiorov2010-source/Fast-Logic/releases) · [Issues](https://github.com/andrewmaiorov2010-source/Fast-Logic/issues)

**Fast Logic** is a Java plugin for Mindustry 160.7. It changes the instruction rate of the vanilla Micro, Logic, and Hyper Processors.

## Features

- Independent enable switches and integer multipliers from **1× to 15×** for each processor.
- One master switch controls all three processor types.
- Settings are saved by Mindustry and survive mod updates.
- English and Russian setting labels.
- The wait instruction duration and game time are unchanged.

The default multipliers are 5×. Vanilla instruction rates are 2, 8, and 25 instructions per tick for Micro, Logic, and Hyper Processors.

## Install

### In-game Mod Browser

Once the automatic catalog includes the repository, open **Mods → Mod Browser** and search for **Fast Logic** or **логика**. The catalog refreshes automatically every few hours; until it appears there, use the release download below.

### JAR

1. Open [Releases](https://github.com/andrewmaiorov2010-source/Fast-Logic/releases/latest) and download `Fast-Logic-1.3.1.jar`.
2. In Mindustry, choose **Mods → Import mod → Import file**, select the JAR, and restart the game.
3. Open **Settings → Fast Logic** (Russian: **Настройки → Fast Logic — настройки процессоров**).

When replacing the previous LogicSpeedFive JAR manually, remove or replace only that old JAR before importing this one. Mindustry preference keys and the plugin's `logicspeedfive.*` setting keys remain unchanged, so your saved multipliers and switches are retained.

## Settings

| Setting | Default | Effect |
| --- | --- | --- |
| Master acceleration | On | Enables or disables all processor acceleration |
| Micro Processor toggle and speed | On, 5× | 1×–15×; vanilla rate: 2 instructions/tick |
| Logic Processor toggle and speed | On, 5× | 1×–15×; vanilla rate: 8 instructions/tick |
| Hyper Processor toggle and speed | On, 5× | 1×–15×; vanilla rate: 25 instructions/tick |

Turning off either the master switch or a processor's own switch restores that processor to its vanilla rate. A multiplier of 1× is also the vanilla rate.

## Compatibility and checks

- Target: **Mindustry 160.7**, Java 17.
- The plugin keeps its original internal ID (`logic-speed-five`), Java package, class name, and saved preference keys to avoid creating a separate mod identity.
- The release workflow compiles against the official Mindustry 160.7 desktop JAR and runs a standalone rate-policy check. It does not launch Mindustry. This release has not received an in-game test by the publisher.
- No multiplayer compatibility claim is made.

## Build from source

Install JDK 17 and obtain the official Mindustry 160.7 desktop JAR. Run PowerShell:

```powershell
.\build.ps1 -MindustryJar 'C:\path\to\Mindustry.jar'
```

The script creates `build/Fast-Logic-1.3.1.jar`. It does not launch Mindustry or bundle the game libraries.

## Versions

- **v1.3.1 — Fast Logic:** catalog metadata and project branding; keeps the original internal mod ID and settings.
- **v1.3.0 — LogicSpeedFive:** adds documented rate and setting behavior.

## License

No license file is present for this project. The code is not licensed for reuse or redistribution by this repository; ask the owner before using it. The Mindustry API JAR is used only as a compile dependency and is not included in the mod.

[Source](https://github.com/andrewmaiorov2010-source/Fast-Logic/tree/main) · [Issues](https://github.com/andrewmaiorov2010-source/Fast-Logic/issues) · [Releases](https://github.com/andrewmaiorov2010-source/Fast-Logic/releases)
