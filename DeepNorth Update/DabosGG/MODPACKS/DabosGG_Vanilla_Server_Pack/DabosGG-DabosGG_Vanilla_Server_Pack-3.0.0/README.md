# DabosGG Vanilla Server Pack 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Compatibility audit baseline — not yet release-ready**

Baseline DabosGG QoL/server package. This should be audited first because the full Modded Server Pack depends on it.

> The dependency versions below are an **audit starting point**, not a blanket compatibility claim. They were carried forward from the historical 2.0.0 manifest unless otherwise noted. Each dependency should be verified and updated before this package is published.

## 3.0.0 baseline — currently included

| Dependency | Baseline version |
| --- | ---: |
| `denikson-BepInExPack_Valheim` | `5.4.2333` |
| `ValheimModding-Jotunn` | `2.29.0` |
| `Advize-PlantEasily` | `2.1.1` |
| `Advize-PlantEverything` | `1.20.0` |
| `ComfyMods-PotteryBarn` | `1.20.0` |
| `ComfyMods-SearsCatalog` | `1.8.0` |
| `ComfyMods-ComfyAutoRepair` | `1.0.0` |
| `ValheimModding-HookGenPatcher` | `0.0.4` |
| `Searica-AdvancedTerrainModifiers` | `1.4.1` |
| `Azumatt-AzuAutoStore` | `3.0.14` |
| `Azumatt-AzuCraftyBoxes` | `1.8.14` |
| `makail-ItemDrawers` | `0.5.8` |
| `BasilPanda-NoStamCosts` | `0.1.2` |
| `Advize-StumpsRegrow` | `1.0.5` |
| `Azumatt-WardIsLove` | `3.7.2` |

## Migration notes

The historical package described itself as vanilla/crossplay-friendly. That claim must be re-tested against the final 3.0 dependency set rather than carried forward automatically.

## Historical mods no longer included

| Dependency | Last included | Historical note |
| --- | --- | --- |
| `bbepis-BepInExPack` | 1.0.1 | Replaced by denikson-BepInExPack_Valheim beginning with 1.0.2. |
| `Goldenrevolver-Quick_Stack_Store_Sort_Trash_Restock` | 1.0.1 | Removed in 1.0.2; the historical changelog records compatibility issues. |
| `Tekla-AutoRepair` | 1.5.0 | Absent from 2.0.0; the 2.0.0 baseline uses ComfyMods-ComfyAutoRepair. |

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
