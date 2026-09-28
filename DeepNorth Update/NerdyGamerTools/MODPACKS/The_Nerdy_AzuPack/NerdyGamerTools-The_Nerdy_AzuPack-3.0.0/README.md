# The Nerdy AzuPack 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Compatibility audit baseline — not yet release-ready**

Curated NerdyGamerTools collection of Azumatt quality-of-life and gameplay-enhancing mods plus supporting dependencies.

> The dependency versions below are an **audit starting point**, not a blanket compatibility claim. They were carried forward from the preserved 1.0.0 manifest unless otherwise noted. Each dependency should be verified and updated before this package is published.

## 3.0.0 baseline — currently included

| Dependency | Baseline version |
| --- | ---: |
| `denikson-BepInExPack_Valheim` | `5.4.2333` |
| `Azumatt-AzuExtendedPlayerInventory` | `2.4.1` |
| `Azumatt-AzuCraftyBoxes` | `1.8.14` |
| `Azumatt-AAA_Crafting` | `2.1.6` |
| `Azumatt-Recycle_N_Reclaim` | `1.4.0` |
| `Azumatt-AzuAutoStore` | `3.0.14` |
| `Azumatt-Build_Camera_Custom_Hammers_Edition` | `1.2.10` |
| `Azumatt-AzuClock` | `1.0.5` |
| `Azumatt-AzuAreaRepair` | `1.1.6` |
| `Azumatt-AzuWorkbenchTweaks` | `1.0.5` |
| `Azumatt-WardIsLove` | `3.7.2` |
| `Azumatt-AzuContainerSizes` | `1.1.4` |
| `Azumatt-AzuMiscPatches` | `1.2.8` |
| `Azumatt-AzuAntiCheat` | `4.3.11` |
| `Smoothbrain-Backpacks` | `1.3.8` |
| `Azumatt-BowsBeforeHoes` | `1.3.14` |
| `Azumatt-AzuWearNTearPatches` | `1.0.8` |
| `Azumatt-PetPantry` | `1.0.5` |
| `Azumatt-AzuHoverStats` | `1.1.9` |
| `Azumatt-FastLink` | `1.4.8` |
| `Azumatt-CurrencyPocket` | `1.0.12` |
| `Azumatt-SaveCrossbowState` | `1.0.2` |
| `Azumatt-AzuSkillTweaks` | `1.0.6` |
| `Azumatt-Where_You_At` | `1.0.11` |
| `Azumatt-SleepSkip` | `1.3.0` |
| `Azumatt-MouseTweaks` | `1.0.2` |
| `Azumatt-ChangelogEditor` | `1.0.9` |
| `Azumatt-Official_BepInEx_ConfigurationManager` | `18.4.1` |
| `Azumatt-Recipe_Description_Expansion` | `1.1.7` |

## Migration notes

Only one historical AzuPack snapshot is preserved, so there is no prior removal history yet. The complete 1.0.0 dependency set is carried into the 3.0 audit baseline for deliberate review.

## Historical mods no longer included

No package dependencies are recorded as removed in the preserved history.

## 3.0 validation checklist

- [ ] Confirm every dependency is maintained for Valheim 1.0.
- [ ] Replace obsolete or incompatible dependencies.
- [ ] Update dependency versions in `manifest.json`.
- [ ] Rebuild configuration files from current mod versions where applicable.
- [ ] Launch-test against the target Valheim 1.0 build.
- [ ] Review BepInEx log for plugin/config errors.
- [ ] Test dedicated-server behavior where applicable.
- [ ] Document client requirements and crossplay behavior.
- [ ] Update this history if a dependency is added, removed, or replaced.
- [ ] Mark the package release-ready only after the audit is complete.

## History policy

The versioned packages outside **DeepNorth Update** remain the authoritative historical snapshots. This 3.0.0 folder is the working migration package and may change until compatibility testing is complete.
