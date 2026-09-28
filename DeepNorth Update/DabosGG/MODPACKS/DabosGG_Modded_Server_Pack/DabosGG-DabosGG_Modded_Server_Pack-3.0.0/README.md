# DabosGG Modded Server Pack 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Compatibility audit baseline — not yet release-ready**

The aggregate DabosGG server package. For 3.0.0 it points at the three new 3.0.0 component-pack candidates so compatibility work remains modular.

> The dependency versions below are an **audit starting point**, not a blanket compatibility claim. They were carried forward from the historical 1.5.0 aggregate structure unless otherwise noted. Each dependency should be verified and updated before this package is published.

## 3.0.0 baseline — currently included

| Dependency | Baseline version |
| --- | ---: |
| `DabosGG-DabosGG_Vanilla_Server_Pack` | `3.0.0` |
| `DabosGG-DabosGG_New_Skills_Pack` | `3.0.0` |
| `DabosGG-DabosGG_New_Content_Pack` | `3.0.0` |

## Migration notes

Unlike the component packs, the 3.0.0 aggregate manifest intentionally advances its three DabosGG dependencies to **3.0.0**. Validate the Vanilla, Skills, and Content packs before testing this aggregate.

## Historical mods no longer included

| Dependency | Last included | Historical note |
| --- | --- | --- |
| `bbepis-BepInExPack` | 0.0.1 | Direct dependency in the original monolithic package; removed when the pack was split into the three DabosGG component packs in 1.0.0. |

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
