# DabosGG New Skills Pack 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Compatibility audit baseline — not yet release-ready**

DabosGG skill/progression collection, historically centered on Smoothbrain skill mods.

> The dependency versions below are an **audit starting point**, not a blanket compatibility claim. They were carried forward from the historical 2.0.0 manifest unless otherwise noted. Each dependency should be verified and updated before this package is published.

## 3.0.0 baseline — currently included

| Dependency | Baseline version |
| --- | ---: |
| `Smoothbrain-Blacksmithing` | `1.3.3` |
| `Smoothbrain-Cooking` | `1.2.2` |
| `Smoothbrain-DualWield` | `1.0.10` |
| `Smoothbrain-Foraging` | `1.0.10` |
| `Smoothbrain-Ranching` | `1.1.6` |
| `Smoothbrain-Mining` | `1.1.6` |
| `Smoothbrain-Lumberjacking` | `1.0.6` |
| `Smoothbrain-PackHorse` | `1.0.4` |
| `Smoothbrain-Evasion` | `1.0.4` |
| `Smoothbrain-Tenacity` | `1.0.4` |
| `Smoothbrain-Exploration` | `1.0.4` |

## Migration notes

The historical Farming skill was removed after 1.0.0 because of documented compatibility issues with the other DabosGG packs. It is not automatically restored for 3.0.

## Historical mods no longer included

| Dependency | Last included | Historical note |
| --- | --- | --- |
| `Smoothbrain-Farming` | 1.0.0 | Removed in 1.0.1; historical documentation records compatibility issues with other DabosGG packs. |

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
