# Deep North / Valheim 1.0 — 3.0 Workspace

This directory contains the active **3.0 generation** of the DabosGG and NerdyGamerTools packages for the Valheim 1.0 / Deep North era.

The dependency-selection/reset pass is now complete for the current package structure. A 3.0 folder being present does **not** mean that package has completed runtime validation.

## Current package state

| Namespace | Package | Current 3.0 state | Dependency state |
| --- | --- | --- | --- |
| DabosGG | [Vanilla Server Pack](DabosGG/MODPACKS/DabosGG_Vanilla_Server_Pack/DabosGG-DabosGG_Vanilla_Server_Pack-3.0.0/) | Runtime/client testing | 6 selected dependencies |
| DabosGG | [New Skills Pack](DabosGG/MODPACKS/DabosGG_New_Skills_Pack/DabosGG-DabosGG_New_Skills_Pack-3.0.0/) | Replacement search | BepInEx only |
| DabosGG | [New Content Pack](DabosGG/MODPACKS/DabosGG_New_Content_Pack/DabosGG-DabosGG_New_Content_Pack-3.0.0/) | Runtime/client/world testing | 17 selected dependencies |
| DabosGG | [Modded Server Pack](DabosGG/MODPACKS/DabosGG_Modded_Server_Pack/DabosGG-DabosGG_Modded_Server_Pack-3.0.0/) | Waiting on component packs | Aggregate of the three DabosGG component packs only |
| NerdyGamerTools | [The Nerdy AzuPack](NerdyGamerTools/MODPACKS/The_Nerdy_AzuPack/NerdyGamerTools-The_Nerdy_AzuPack-3.0.0/) | Rebuild/source migration | BepInEx only |
| NerdyGamerTools | [AutoBroadcaster](NerdyGamerTools/MODS/NerdyGamerTools_AutoBroadcaster/NerdyGamerTools-NerdyGamerTools_AutoBroadcaster-3.0.0/) | Packaging/source synchronization | Package scaffold pending matching current build |

## DabosGG dependency model

```text
DabosGG Modded Server Pack 3.0.0
├── DabosGG Vanilla Server Pack 3.0.0
├── DabosGG New Skills Pack 3.0.0
└── DabosGG New Content Pack 3.0.0
```

The aggregate pack does not directly manage individual mods.

## Migration rules

- Historical package folders outside this workspace remain unchanged.
- Do not copy old DLLs into a 3.0 package unless that exact binary has been deliberately validated.
- Do not preserve a stale dependency merely because it existed in an older package.
- Removed dependencies can return when maintained updates or replacements are available.
- Build configs against the actual current mod version rather than blindly copying old config files.
- Keep each package README and CHANGELOG synchronized with manifest changes.
- Mark a package release-ready only after its applicable runtime tests pass.

## Recommended testing order

1. DabosGG Vanilla Server Pack
2. DabosGG New Skills Pack after replacement mods are selected
3. DabosGG New Content Pack
4. DabosGG Modded Server Pack
5. The Nerdy AzuPack after maintained sources/replacements are selected
6. AutoBroadcaster packaging/source synchronization

Repository-wide status:

- [Compatibility Matrix](../docs/COMPATIBILITY.md)
- [Migration Tracker](../docs/VALHEIM-1.0-MIGRATION.md)
- [Version History](../docs/VERSION-HISTORY.md)
- [Repository Changelog](../CHANGELOG.md)
