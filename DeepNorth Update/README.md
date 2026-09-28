# Deep North / Valheim 1.0 — 3.0 Migration Workspace

This directory is the working area for establishing **Valheim 1.0 / Deep North compatibility** across the DabosGG and NerdyGamerTools packages.

All packages in this workspace are initialized as **3.0.0**.

> **3.0.0 currently means migration candidate, not compatibility certification.**
>
> Historical dependency versions are carried forward as audit baselines so each dependency can be checked, replaced, updated, or removed deliberately.

## Packages

| Namespace | Package | Type | 3.0 workspace |
| --- | --- | --- | --- |
| DabosGG | DabosGG Vanilla Server Pack | Modpack | [3.0.0](DabosGG/MODPACKS/DabosGG_Vanilla_Server_Pack/DabosGG-DabosGG_Vanilla_Server_Pack-3.0.0/) |
| DabosGG | DabosGG New Skills Pack | Modpack | [3.0.0](DabosGG/MODPACKS/DabosGG_New_Skills_Pack/DabosGG-DabosGG_New_Skills_Pack-3.0.0/) |
| DabosGG | DabosGG New Content Pack | Modpack | [3.0.0](DabosGG/MODPACKS/DabosGG_New_Content_Pack/DabosGG-DabosGG_New_Content_Pack-3.0.0/) |
| DabosGG | DabosGG Modded Server Pack | Aggregate modpack | [3.0.0](DabosGG/MODPACKS/DabosGG_Modded_Server_Pack/DabosGG-DabosGG_Modded_Server_Pack-3.0.0/) |
| NerdyGamerTools | The Nerdy AzuPack | Modpack | [3.0.0](NerdyGamerTools/MODPACKS/The_Nerdy_AzuPack/NerdyGamerTools-The_Nerdy_AzuPack-3.0.0/) |
| NerdyGamerTools | AutoBroadcaster | Server mod | [3.0.0](NerdyGamerTools/MODS/NerdyGamerTools_AutoBroadcaster/NerdyGamerTools-NerdyGamerTools_AutoBroadcaster-3.0.0/) |

## Migration order

1. DabosGG Vanilla Server Pack
2. DabosGG New Skills Pack
3. DabosGG New Content Pack
4. DabosGG Modded Server Pack
5. The Nerdy AzuPack
6. AutoBroadcaster 3.0 packaging/source synchronization

## Rules for this workspace

- Historical packages outside this directory remain untouched.
- Do not assume an old dependency version works with Valheim 1.0.
- Update manifests only after checking the actual maintained package/version.
- Do not copy historical DLLs into 3.0 unless they have been explicitly validated.
- Rebuild configs from current mod versions when config schemas have changed.
- Every 3.0 README keeps a record of dependencies that are still included and dependencies that were removed from earlier package history.
- Once a package passes validation, its README and the repository compatibility matrix should be updated together.
