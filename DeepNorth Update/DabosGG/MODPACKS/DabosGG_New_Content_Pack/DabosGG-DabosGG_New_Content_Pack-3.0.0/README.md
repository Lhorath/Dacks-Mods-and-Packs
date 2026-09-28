# DabosGG New Content Pack 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Compatibility audit baseline — not yet release-ready**

Content-heavy DabosGG package containing creatures, equipment, building pieces, map/server systems, NPC systems, and other gameplay additions.

> The dependency versions below are an **audit starting point**, not a blanket compatibility claim. They were carried forward from the historical 2.0.0 manifest unless otherwise noted. Each dependency should be verified and updated before this package is published.

## 3.0.0 baseline — currently included

| Dependency | Baseline version |
| --- | ---: |
| `Smoothbrain-HildirsQuest` | `1.0.2` |
| `TheOllix-PixelMapIcons` | `1.4.5` |
| `Vapok-AdventureBackpacks` | `1.9.13` |
| `Therzie-Armory` | `1.3.1` |
| `ishid4-BetterArchery` | `1.9.82` |
| `OdinPlus-BoomStick` | `0.1.0` |
| `Marlthon-Cats` | `0.3.2` |
| `Marlthon-Dogs` | `0.2.1` |
| `RandyKnapp-EpicLoot` | `0.12.11` |
| `Azumatt-AzuExtendedPlayerInventory` | `2.4.1` |
| `Therzie-Monstrum` | `1.5.1` |
| `Therzie-MonstrumDeepNorth` | `2.0.6` |
| `OdinPlus-OdinArchitect` | `1.6.5` |
| `OdinPlus-OdinHorse` | `1.6.1` |
| `OdinPlus-OdinsSteelworks` | `0.3.4` |
| `Therzie-Warfare` | `1.8.9` |
| `Therzie-WarfareFireAndIce` | `2.0.8` |
| `Nextek-SpeedyPaths` | `1.0.9` |
| `OdinPlus-OdinsFoodBarrels` | `1.2.2` |
| `OdinPlus-BetterLanterns` | `1.1.1` |
| `Mydayyy-ServerSideMap` | `1.3.13` |
| `KGvalheim-Marketplace_And_Server_NPCs_Revamped` | `9.7.6` |
| `KGvalheim-Marketplace_NPC_Models` | `1.1.0` |
| `MathiasDecrock-PlanBuild` | `0.18.4` |

## Migration notes

The preserved **1.5.0** manifest is an unusual outlier containing only `OdinPlus-ShrinkMe-1.0.3`. The newer **2.0.0** manifest is therefore used as the 3.0 audit baseline. Deep North-specific historical mods deserve special scrutiny now that Deep North is official Valheim content.

## Historical mods no longer included

| Dependency | Last included | Historical note |
| --- | --- | --- |
| `Smoothbrain-Jewelcrafting` | 1.0.0 | Removed in 1.1.0; the historical changelog records incompatibility with EpicLoot. |
| `Rolo-ExploreTogether` | 1.1.2 | Present in 1.1.0–1.1.2; absent from later preserved baselines. |
| `Azumatt-AzuMapDetails` | 1.3.0 | Present in 1.1.3–1.3.0; absent from 2.0.0. |
| `OdinPlus-Clutter` | 1.3.0 | Present through 1.3.0; absent from 2.0.0. |
| `RandyKnapp-EquipmentAndQuickSlots` | 1.3.0 | Present through 1.3.0; absent from 2.0.0. |
| `Therzie-MonstrumAshlands` | 1.3.0 | Present through 1.3.0; absent from 2.0.0. |
| `OdinPlus-ShrinkMe` | 1.5.0 | Introduced in 1.1.2; absent from the 2.0.0 baseline. |
| `JewelHeim-Marketplace_Configs` | 1.3.0 | Present in 1.2.0–1.3.0; absent from 2.0.0. |

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
