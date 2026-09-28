# The Nerdy AzuPack 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Rebuild / maintained-package search**

The Nerdy AzuPack is being rebuilt for Valheim 1.0.

The historical 1.0.0 pack was a large collection of Azumatt quality-of-life mods plus Smoothbrain Backpacks. That dependency set is **not being carried forward directly into the 3.0 Thunderstore manifest**.

A review performed on **2026-09-28** found two different situations:

1. several historical Azumatt mods **did receive Valheim 1.0 fixes**, but their Thunderstore packages are now marked **Deprecated** and are not a good long-term basis for a newly rebuilt Thunderstore pack;
2. several other dependencies have **no current upstream Valheim 1.0 release** and should not be carried forward without a maintained replacement or compatibility plan.

For now, the 3.0 package contains only the current BepInExPack dependency while the AzuPack is rebuilt around maintained package sources.

## 3.0.0 — currently included

| Dependency | Version | Purpose |
| --- | ---: | --- |
| `denikson-BepInExPack_Valheim` | `5.4.2351` | Core Valheim mod framework |

## Historical dependencies that received Valheim 1.0 fixes but are not retained

These historical AzuPack mods did receive 1.0-era fixes or rebuilds, but their Thunderstore packages are now deprecated or otherwise unsuitable as the long-term 3.0 dependency source.

| Historical dependency | Historical AzuPack version | 1.0-era status |
| --- | ---: | --- |
| `Azumatt-AzuExtendedPlayerInventory` | `2.4.1` | Later 2.4.x releases include a Valheim 1.0 update |
| `Azumatt-AzuCraftyBoxes` | `1.8.14` | Later 1.8.x releases include Valheim 1.0 fixes |
| `Azumatt-AAA_Crafting` | `2.1.6` | Later 2.1.x release includes Valheim 1.0 fixes |
| `Azumatt-Recycle_N_Reclaim` | `1.4.0` | Later 1.4.x release includes Valheim 1.0 fixes |
| `Azumatt-AzuAutoStore` | `3.0.14` | Later 3.1.x releases include Valheim 1.0 fixes |
| `Azumatt-Build_Camera_Custom_Hammers_Edition` | `1.2.10` | Later 1.3.x release includes a 1.0 update |
| `Azumatt-AzuClock` | `1.0.5` | Later 1.1.x release was published after Valheim 1.0 |
| `Azumatt-AzuAreaRepair` | `1.1.6` | Later 1.1.x release explicitly fixes Valheim 1.0 |
| `Azumatt-AzuWorkbenchTweaks` | `1.0.5` | Later 1.0.x releases include 1.0 fixes |
| `Azumatt-AzuContainerSizes` | `1.1.4` | Thunderstore changelog records a 1.0 fix in the later release line |
| `Azumatt-AzuWearNTearPatches` | `1.0.8` | Later 1.0.x release includes Valheim 1.0 fixes |
| `Azumatt-PetPantry` | `1.0.5` | Later 1.0.6 release explicitly contains 1.0 updates/fixes |
| `Azumatt-AzuHoverStats` | `1.1.9` | Later 1.1.10 release explicitly updates for 1.0 |
| `Azumatt-CurrencyPocket` | `1.0.12` | Later 1.0.13 release fixes Valheim 1.0 UI changes |
| `Azumatt-Where_You_At` | `1.0.11` | Later 1.0.12 release was published after Valheim 1.0 |
| `Azumatt-MouseTweaks` | `1.0.2` | Later 1.0.4 release contains Valheim 1.0 fixes |

These are documented here so that “removed from 3.0” is not confused with “never updated.”

## Historical dependencies without a maintained upstream 1.0 path in this Thunderstore pack

The following dependencies are not being carried forward because no suitable maintained upstream Valheim 1.0 dependency was identified for the 3.0 Thunderstore package during this review:

| Historical dependency | Historical version | 3.0 status |
| --- | ---: | --- |
| `Azumatt-AzuMiscPatches` | `1.2.8` | Removed pending maintained 1.0 source/replacement |
| `Azumatt-AzuAntiCheat` | `4.3.11` | Removed pending maintained 1.0 source/replacement |
| `Smoothbrain-Backpacks` | `1.3.8` | Upstream has no native 1.0 release; third-party compatibility shim exists |
| `Azumatt-BowsBeforeHoes` | `1.3.14` | Removed pending maintained 1.0 source/replacement |
| `Azumatt-FastLink` | `1.4.8` | Removed pending maintained 1.0 source/replacement |
| `Azumatt-SaveCrossbowState` | `1.0.2` | Deprecated; removed |
| `Azumatt-AzuSkillTweaks` | `1.0.6` | Pre-1.0 build; known to target changed APIs |
| `Azumatt-SleepSkip` | `1.3.0` | Pre-1.0 upstream build; unofficial compatibility fork exists |
| `Azumatt-ChangelogEditor` | `1.0.9` | Removed pending maintained 1.0 source/replacement |
| `Azumatt-Official_BepInEx_ConfigurationManager` | `18.4.1` | Removed pending maintained 1.0 source/replacement |
| `Azumatt-Recipe_Description_Expansion` | `1.1.7` | Removed pending maintained 1.0 source/replacement |
| `Azumatt-WardIsLove` | `3.7.2` | Removed pending maintained 1.0 source/replacement |

## Pack direction

The 3.0 AzuPack should not simply freeze old Thunderstore dependency strings.

The rebuild should instead:

- prefer packages that are actively maintained for Valheim 1.0;
- evaluate the current maintained source for Azumatt mods rather than depending on deprecated Thunderstore snapshots;
- use replacements where an older feature is no longer maintained;
- avoid compatibility shims unless there is a deliberate reason to accept the maintenance risk;
- document client/server requirements for every selected mod;
- preserve this history so removed features can be restored deliberately later.

## 3.0 validation checklist

- [x] Audit the historical 1.0.0 dependency set.
- [x] Remove the legacy mod dependency set from the 3.0 Thunderstore manifest.
- [x] Update BepInExPack Valheim to `5.4.2351`.
- [ ] Identify the maintained current package source for desired Azumatt mods.
- [ ] Decide whether the 3.0 AzuPack remains Thunderstore-only or supports a mixed package-manager workflow.
- [ ] Select maintained replacements for abandoned/deprecated features.
- [ ] Rebuild the final dependency manifest.
- [ ] Verify client/server requirements.
- [ ] Test the final dependency set on Valheim 1.0.
- [ ] Update this README when each feature is restored or replaced.

## Credits

See [CREDITS.md](CREDITS.md) for attribution to the authors/projects whose work is represented by this modpack.

## History policy

The historical 1.0.0 snapshot outside **DeepNorth Update** remains unchanged and is the authoritative record of the original AzuPack dependency set.
