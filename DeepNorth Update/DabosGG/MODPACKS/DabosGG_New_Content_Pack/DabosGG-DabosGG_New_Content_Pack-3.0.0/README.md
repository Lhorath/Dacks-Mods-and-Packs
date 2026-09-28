# DabosGG New Content Pack 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Dependency list established — runtime/client testing still required**

The New Content Pack is the main gameplay-expansion layer of the DabosGG modded stack. For 3.0, the package has been reduced to the maintained content and framework dependencies selected for the Valheim 1.0 / Deep North generation.

The dependency list below is the current 3.0 package target. Runtime compatibility, client requirements, configuration, world behavior, and multiplayer behavior still need to be tested before release.

## 3.0.0 — currently included

| Dependency | Version | 3.0 status |
| --- | ---: | --- |
| `denikson-BepInExPack_Valheim` | `5.4.2351` | New 3.0 framework dependency |
| `KGvalheim-MoreMapPins` | `1.1.0` | New in 3.0 |
| `Sakey-SakeysCozyPixelMapIcons` | `1.1.2` | New in 3.0 |
| `ValheimModding-Jotunn` | `2.30.2` | New 3.0 framework dependency |
| `Akuichi-ReforgedPotential` | `2.0.6` | New in 3.0 |
| `ValheimModding-YamlDotNet` | `16.3.1` | New in 3.0 |
| `Vapok-AdventureBackpacks` | `2.2.1` | Retained / updated |
| `Therzie-Warfare` | `1.9.4` | Retained / updated |
| `Therzie-Monstrum` | `1.6.0` | Retained / updated |
| `Therzie-Armory` | `1.4.2` | Retained / updated |
| `Therzie-Wizardry` | `1.2.2` | New in 3.0 |
| `ishid4-BetterArchery` | `2.0.2` | Retained / updated |
| `OdinPlus-OdinArchitect` | `1.7.6` | Retained / updated |
| `OdinPlus-OdinHorse` | `1.7.4` | Retained / updated |
| `OdinPlus-OdinsSteelworks` | `0.4.1` | Retained / updated |
| `OdinPlus-OdinsFoodBarrels` | `1.3.4` | Retained / updated |
| `Mydayyy-ServerSideMap` | `1.3.14` | Retained / updated |

## Carried forward from 2.0

The following dependencies remain part of the New Content Pack and have been advanced to newer versions for the 3.0 generation:

| Dependency | 2.0 version | 3.0 version |
| --- | ---: | ---: |
| `Vapok-AdventureBackpacks` | `1.9.13` | `2.2.1` |
| `Therzie-Warfare` | `1.8.9` | `1.9.4` |
| `Therzie-Monstrum` | `1.5.1` | `1.6.0` |
| `Therzie-Armory` | `1.3.1` | `1.4.2` |
| `ishid4-BetterArchery` | `1.9.82` | `2.0.2` |
| `OdinPlus-OdinArchitect` | `1.6.5` | `1.7.6` |
| `OdinPlus-OdinHorse` | `1.6.1` | `1.7.4` |
| `OdinPlus-OdinsSteelworks` | `0.3.4` | `0.4.1` |
| `OdinPlus-OdinsFoodBarrels` | `1.2.2` | `1.3.4` |
| `Mydayyy-ServerSideMap` | `1.3.13` | `1.3.14` |

## New to the 3.0 dependency set

These dependencies were not in the historical 2.0.0 manifest and are now part of the 3.0 package target:

- `denikson-BepInExPack_Valheim-5.4.2351`
- `KGvalheim-MoreMapPins-1.1.0`
- `Sakey-SakeysCozyPixelMapIcons-1.1.2`
- `ValheimModding-Jotunn-2.30.2`
- `Akuichi-ReforgedPotential-2.0.6`
- `ValheimModding-YamlDotNet-16.3.1`
- `Therzie-Wizardry-1.2.2`

## Removed from the 3.0 baseline

The following dependencies were included in the historical 2.0.0 package but are not part of the current 3.0 dependency set.

They may be reconsidered later if they are updated, replaced, or become useful again.

| Dependency | 2.0 version | 3.0 status |
| --- | ---: | --- |
| `Smoothbrain-HildirsQuest` | `1.0.2` | Removed from current baseline |
| `TheOllix-PixelMapIcons` | `1.4.5` | Removed from current baseline |
| `OdinPlus-BoomStick` | `0.1.0` | Removed from current baseline |
| `Marlthon-Cats` | `0.3.2` | Removed from current baseline |
| `Marlthon-Dogs` | `0.2.1` | Removed from current baseline |
| `RandyKnapp-EpicLoot` | `0.12.11` | Removed from current baseline |
| `Azumatt-AzuExtendedPlayerInventory` | `2.4.1` | Removed from current baseline |
| `Therzie-MonstrumDeepNorth` | `2.0.6` | Removed from current baseline |
| `Therzie-WarfareFireAndIce` | `2.0.8` | Removed from current baseline |
| `Nextek-SpeedyPaths` | `1.0.9` | Removed from current baseline |
| `OdinPlus-BetterLanterns` | `1.1.1` | Removed from current baseline |
| `KGvalheim-Marketplace_And_Server_NPCs_Revamped` | `9.7.6` | Removed from current baseline |
| `KGvalheim-Marketplace_NPC_Models` | `1.1.0` | Removed from current baseline |
| `MathiasDecrock-PlanBuild` | `0.18.4` | Removed from current baseline |

## Older historical removals

These dependencies had already left the pack before the 2.0 generation:

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

- [x] Establish the initial Valheim 1.0 dependency set.
- [x] Remove dependencies that are not being carried into the 3.0 baseline.
- [x] Update retained dependency version strings.
- [x] Add newly selected 3.0 dependencies.
- [ ] Determine client-side installation requirements for each dependency.
- [ ] Rebuild configuration files from the current mod versions.
- [ ] Launch-test the complete pack against the target Valheim 1.0 build.
- [ ] Review BepInEx log for plugin/config errors.
- [ ] Test existing-world loading and progression.
- [ ] Test new-world loading.
- [ ] Test creature, item, crafting, building, backpack, map, and server-side map functionality.
- [ ] Test multiplayer with all required client mods installed.
- [ ] Document known incompatibilities.
- [ ] Mark the package release-ready only after runtime testing is complete.

## Credits

See [CREDITS.md](CREDITS.md) for attribution to the authors/projects whose work is represented by this modpack.

## History policy

The versioned packages outside **DeepNorth Update** remain the authoritative historical snapshots. This 3.0.0 folder is the working migration package and may change until compatibility testing is complete.
