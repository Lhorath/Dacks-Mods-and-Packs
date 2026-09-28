# Compatibility Matrix

Last reviewed: **2026-09-28**

This file tracks current compatibility work for the packages preserved in this repository and the new **Deep North 3.0** migration workspace.

## Valheim 1.0 status

| Namespace | Package | Latest historical snapshot | 3.0 migration package | Status | Notes |
| --- | --- | ---: | --- | --- | --- |
| DabosGG | DabosGG Vanilla Server Pack | 2.0.0 | [3.0.0](../DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_Vanilla_Server_Pack/DabosGG-DabosGG_Vanilla_Server_Pack-3.0.0/) | 🛠️ Runtime/client testing | Dependency list narrowed to six maintained Valheim 1.0 migration dependencies. 3.0 is QoL-focused and no longer promises vanilla-client/crossplay compatibility. |
| DabosGG | DabosGG New Skills Pack | 2.0.0 | [3.0.0](../DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_New_Skills_Pack/DabosGG-DabosGG_New_Skills_Pack-3.0.0/) | 🛠️ Replacement search | All Smoothbrain dependencies removed from the 3.0 baseline. Only BepInExPack Valheim 5.4.2351 remains while maintained Valheim 1.0 skill mods are identified. |
| DabosGG | DabosGG New Content Pack | 2.0.0 | [3.0.0](../DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_New_Content_Pack/DabosGG-DabosGG_New_Content_Pack-3.0.0/) | 🛠️ Runtime/client/world testing | 17-dependency Valheim 1.0 content baseline established: 10 historical dependencies updated, 7 new dependencies added, and 14 former 2.0 dependencies removed from the current baseline. |
| DabosGG | DabosGG Modded Server Pack | 1.5.0 | [3.0.0](../DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_Modded_Server_Pack/DabosGG-DabosGG_Modded_Server_Pack-3.0.0/) | 🛠️ Waiting on component packs | Pure aggregate package. Manifest contains only the Vanilla, New Skills, and New Content 3.0 packs; individual mods are managed exclusively in those component packs. |
| NerdyGamerTools | The Nerdy AzuPack | 1.0.0 | [3.0.0](../DeepNorth%20Update/NerdyGamerTools/MODPACKS/The_Nerdy_AzuPack/NerdyGamerTools-The_Nerdy_AzuPack-3.0.0/) | 🛠️ Rebuild / source migration | Legacy mod dependencies removed from the active 3.0 manifest. Several received 1.0 fixes but their Thunderstore lines are now deprecated; others never received a maintained native 1.0 upstream update. BepInExPack 5.4.2351 remains as the sole baseline dependency. |
| NerdyGamerTools | AutoBroadcaster | 1.0.1 | [3.0.0 scaffold](../DeepNorth%20Update/NerdyGamerTools/MODS/NerdyGamerTools_AutoBroadcaster/NerdyGamerTools-NerdyGamerTools_AutoBroadcaster-3.0.0/) | 🛠️ Packaging/source sync | Maintained [source repo](https://github.com/Lhorath/NGT-AutoBroadcaster) has a 2.0.0 rebuild documented for Valheim 1.0.16; no old DLL was copied into 3.0. |

## Status definitions

### 🟢 Updated

A maintained rebuild exists and has passed the stated compatibility checks.

### 🟡 Needs validation

No active migration work has established compatibility yet.

### 🛠️ Migration work

A 3.0 candidate exists, but dependencies/configs/runtime behavior are still being audited or tested.

### 📦 Legacy archive

Historical/reference package, not intended as a current deployment.

### ❌ Incompatible

A concrete incompatibility has been confirmed.

## 3.0 rule

A `3.0.0` version number means **Deep North migration generation**, not “verified compatible.” The package README and this matrix remain authoritative for validation state.

## AutoBroadcaster

Active source repository:

**https://github.com/Lhorath/NGT-AutoBroadcaster**

The source repository documents **v2.0.0** as a rebuild for **Valheim 1.0.16**. The 3.0 package scaffold in this repository intentionally contains metadata/documentation only until a matching 3.0 build is produced.

## Validation criteria

Before changing a package to **Updated**, verify as applicable:

- dependency is maintained and Valheim 1.0 compatible;
- manifest version is the intended maintained version;
- renamed/replaced projects are handled explicitly;
- game reaches menu without plugin load errors;
- existing and new worlds load as appropriate;
- dedicated server boots;
- configs are accepted by current mod versions;
- client installation requirements are documented;
- vanilla-client and crossplay behavior are actually tested when claimed;
- representative gameplay features work;
- logs contain no recurring compatibility exceptions.
