# Dack's Mods & Packs

Historical archive and active Valheim 1.0 migration workspace for mods and modpacks published under the **DabosGG** and **NerdyGamerTools** namespaces.

The repository now has two distinct purposes:

- preserve the original historical release snapshots exactly as they were packaged;
- build and document the new **3.0 generation** for Valheim 1.0 / Deep North.

> Package versions such as `1.0.0`, `2.0.0`, and `3.0.0` are package versions. They are not Valheim game-version numbers.

## Current 3.0 work

Active migration work lives in **[DeepNorth Update](DeepNorth%20Update/)**.

The dependency-selection/reset pass has now been completed for the current 3.0 package structure. Runtime testing, replacement selection, source migration, configuration work, and packaging still remain where noted.

| Namespace | Package | 3.0 state | Current dependency direction |
| --- | --- | --- | --- |
| DabosGG | [Vanilla Server Pack](DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_Vanilla_Server_Pack/DabosGG-DabosGG_Vanilla_Server_Pack-3.0.0/) | Runtime/client testing | 6 maintained Valheim 1.0 dependencies; QoL-focused; no vanilla-client/crossplay guarantee |
| DabosGG | [New Skills Pack](DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_New_Skills_Pack/DabosGG-DabosGG_New_Skills_Pack-3.0.0/) | Replacement search | BepInEx only while maintained skill/progression mods are identified |
| DabosGG | [New Content Pack](DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_New_Content_Pack/DabosGG-DabosGG_New_Content_Pack-3.0.0/) | Runtime/client/world testing | 17-dependency Valheim 1.0 content baseline |
| DabosGG | [Modded Server Pack](DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_Modded_Server_Pack/DabosGG-DabosGG_Modded_Server_Pack-3.0.0/) | Waiting on component packs | Aggregate only: Vanilla + New Skills + New Content |
| NerdyGamerTools | [The Nerdy AzuPack](DeepNorth%20Update/NerdyGamerTools/MODPACKS/The_Nerdy_AzuPack/NerdyGamerTools-The_Nerdy_AzuPack-3.0.0/) | Rebuild/source migration | BepInEx only while maintained sources/replacements are selected |
| NerdyGamerTools | [AutoBroadcaster](DeepNorth%20Update/NerdyGamerTools/MODS/NerdyGamerTools_AutoBroadcaster/NerdyGamerTools-NerdyGamerTools_AutoBroadcaster-3.0.0/) | Packaging/source synchronization | 3.0 package scaffold; maintained source currently documents the 2.0.0 Valheim 1.0.16 rebuild |

## DabosGG 3.0 structure

The full DabosGG modded stack is deliberately modular:

```text
DabosGG Modded Server Pack 3.0.0
├── DabosGG Vanilla Server Pack 3.0.0
├── DabosGG New Skills Pack 3.0.0
└── DabosGG New Content Pack 3.0.0
```

The aggregate **Modded Server Pack should never directly list individual mods**. Individual dependencies belong only in the appropriate component pack.

### Vanilla Server Pack

The 3.0 pack is now a maintained **quality-of-life** baseline rather than a crossplay-first package.

Current manifest:

- `denikson-BepInExPack_Valheim-5.4.2351`
- `ValheimModding-Jotunn-2.30.2`
- `Advize-PlantEasily-2.2.2`
- `Advize-PlantEverything-1.21.3`
- `ValheimModding-HookGenPatcher-0.0.4`
- `Searica-AdvancedTerrainModifiers-1.5.4`

Removed historical QoL dependencies remain candidates for reintroduction if maintained updates or replacements become available.

### New Skills Pack

All historical Smoothbrain skill dependencies have been removed from the active 3.0 manifest because they have not yet been brought forward for the intended Valheim 1.0 stack.

Current manifest:

- `denikson-BepInExPack_Valheim-5.4.2351`

The package remains active, but is now explicitly looking for maintained skill/progression mods.

### New Content Pack

The 3.0 dependency-selection pass established a new 17-dependency content baseline containing updated historical mods plus new Valheim 1.0-era dependencies.

See the [3.0 package README](DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_New_Content_Pack/DabosGG-DabosGG_New_Content_Pack-3.0.0/) for the complete current list and removal history.

### Modded Server Pack

The 3.0 aggregate contains only:

- `DabosGG-DabosGG_Vanilla_Server_Pack-3.0.0`
- `DabosGG-DabosGG_New_Skills_Pack-3.0.0`
- `DabosGG-DabosGG_New_Content_Pack-3.0.0`

## NerdyGamerTools 3.0

### The Nerdy AzuPack

The old 1.0.0 dependency collection has been cleared from the active 3.0 manifest.

Current manifest:

- `denikson-BepInExPack_Valheim-5.4.2351`

Several historical Azumatt mods did receive Valheim 1.0 fixes, but the old Thunderstore package lines are not being used as the basis of the new pack. The AzuPack is now in a **maintained-source / replacement rebuild phase**.

### AutoBroadcaster

Maintained source repository:

**https://github.com/Lhorath/NGT-AutoBroadcaster**

The source repository currently documents **AutoBroadcaster 2.0.0** as rebuilt for **Valheim 1.0.16**.

The Deep North workspace contains a **3.0.0 package scaffold**, but no historical DLL has been relabeled as 3.0. A matching current build should be packaged before that candidate is treated as releasable.

## Documentation

- [Repository Changelog](CHANGELOG.md)
- [Deep North / 3.0 Workspace](DeepNorth%20Update/)
- [Compatibility Matrix](docs/COMPATIBILITY.md)
- [Valheim 1.0 Migration Tracker](docs/VALHEIM-1.0-MIGRATION.md)
- [Repository Version History](docs/VERSION-HISTORY.md)

## Repository layout

```text
Dacks-Mods-and-Packs/
├── README.md
├── CHANGELOG.md
├── DeepNorth Update/       # Active 3.0 migration packages
├── docs/                   # Current compatibility/migration documentation
├── DabosGG/                # Historical DabosGG archive
└── NerdyGamerTools/        # Historical NerdyGamerTools archive
```

## Archive policy

Historical version-numbered folders are release snapshots. They may contain old manifests, configs, README files, changelogs, icons, DLLs, or server files.

Those historical files are intentionally preserved, even when their text or dependency versions are now outdated.

Current information belongs in:

- package-level README files;
- the **DeepNorth Update** workspace;
- repository-wide documentation.

## 3.0 release policy

A 3.0 package should only be treated as ready when its dependency set is finalized **and** the relevant runtime tests have passed.

Depending on the package, that includes:

- clean game startup;
- BepInEx/Jotunn load validation;
- existing-world and new-world loading;
- dedicated-server startup;
- client installation requirements;
- multiplayer behavior;
- configuration compatibility;
- cross-pack conflict testing;
- representative gameplay testing.

## Credits

These packs depend on the work of the wider Valheim modding community. Historical manifests remain the authoritative record of exactly which third-party projects were included in each archived release.
