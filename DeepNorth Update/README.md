# Deep North / Valheim 1.0 — 3.0 Workspace

This directory contains the active **3.0 generation** for the Valheim 1.0 / Deep North era.

## Namespace distinction

The two namespaces intentionally mean different things:

| Namespace | Purpose |
| --- | --- |
| **DabosGG** | Mods, configurations, and modpacks assembled specifically for **Dabos.GG game servers** |
| **NerdyGamerTools** | **Original mods and tools** developed and released by NerdyGamerTools/Lhorath |

**The_Nerdy_AzuPack** is a legacy curated modpack that predates this distinction. It remains under NerdyGamerTools to preserve history, but newly curated server modpacks should use DabosGG.

See [Namespace and Attribution Policy](../docs/NAMESPACE-POLICY.md).

## Current package state

| Namespace | Package | Current 3.0 state | Dependency state |
| --- | --- | --- | --- |
| DabosGG | [Vanilla Server Pack](DabosGG/MODPACKS/DabosGG_Vanilla_Server_Pack/DabosGG-DabosGG_Vanilla_Server_Pack-3.0.0/) | Runtime/client testing | 7 dependencies, including AutoBroadcaster |
| DabosGG | [New Skills Pack](DabosGG/MODPACKS/DabosGG_New_Skills_Pack/DabosGG-DabosGG_New_Skills_Pack-3.0.0/) | Replacement search | BepInEx only |
| DabosGG | [New Content Pack](DabosGG/MODPACKS/DabosGG_New_Content_Pack/DabosGG-DabosGG_New_Content_Pack-3.0.0/) | Runtime/client/world testing | 17 selected dependencies |
| DabosGG | [Modded Server Pack](DabosGG/MODPACKS/DabosGG_Modded_Server_Pack/DabosGG-DabosGG_Modded_Server_Pack-3.0.0/) | Waiting on component packs | Aggregate of three DabosGG component packs |
| NerdyGamerTools | [The Nerdy AzuPack](NerdyGamerTools/MODPACKS/The_Nerdy_AzuPack/NerdyGamerTools-The_Nerdy_AzuPack-3.0.0/) | Legacy modpack rebuild/source migration | BepInEx only |
| NerdyGamerTools | [AutoBroadcaster](NerdyGamerTools/MODS/NerdyGamerTools_AutoBroadcaster/NerdyGamerTools-NerdyGamerTools_AutoBroadcaster-3.0.0/) | Original mod; packaging/source synchronization | Package scaffold pending matching current build |

## Credit rule

Every maintained modpack in this workspace has a package-specific `CREDITS.md`.

DabosGG packages are curated server packages. Their third-party dependencies remain the work of the credited authors/projects.

## DabosGG dependency model

```text
DabosGG Modded Server Pack 3.0.0
├── DabosGG Vanilla Server Pack 3.0.0
├── DabosGG New Skills Pack 3.0.0
└── DabosGG New Content Pack 3.0.0
```

## Migration rules

- Historical package folders outside this workspace remain unchanged.
- Do not copy old DLLs into a 3.0 package unless that exact binary has been deliberately validated.
- Do not preserve a stale dependency merely because it existed in an older package.
- Removed dependencies can return when maintained updates or replacements are available.
- Keep README, CHANGELOG, manifest, and CREDITS synchronized when dependencies change.
- Mark a package release-ready only after its applicable runtime tests pass.

Repository-wide status:

- [Compatibility Matrix](../docs/COMPATIBILITY.md)
- [Migration Tracker](../docs/VALHEIM-1.0-MIGRATION.md)
- [Version History](../docs/VERSION-HISTORY.md)
- [Repository Changelog](../CHANGELOG.md)
