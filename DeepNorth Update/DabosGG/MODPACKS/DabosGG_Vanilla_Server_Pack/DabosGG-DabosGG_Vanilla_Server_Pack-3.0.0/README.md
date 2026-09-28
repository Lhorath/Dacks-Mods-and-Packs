# DabosGG Vanilla Server Pack 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Dependency list established — runtime/client testing still required**

The 3.0 generation of the Vanilla Server Pack is being rebuilt as a **quality-of-life focused baseline for Valheim 1.0**.

Unlike older versions of this pack, **3.0 is no longer being designed around vanilla-client or crossplay compatibility**. Some included mods may need to be installed client-side for the intended experience. Exact client/server requirements still need to be confirmed during testing.

## 3.0.0 — currently included

These are the dependencies currently being retained because they are the maintained Valheim 1.0 options selected for the 3.0 migration.

| Dependency | 3.0 version | Status |
| --- | ---: | --- |
| `denikson-BepInExPack_Valheim` | `5.4.2351` | Retained / updated |
| `ValheimModding-Jotunn` | `2.30.2` | Retained / updated |
| `Advize-PlantEasily` | `2.2.2` | Retained / updated |
| `Advize-PlantEverything` | `1.21.3` | Retained / updated |
| `ValheimModding-HookGenPatcher` | `0.0.4` | Retained |
| `Searica-AdvancedTerrainModifiers` | `1.5.4` | Retained / updated |

## Removed from the 3.0 baseline

The following dependencies were present in the historical **2.0.0** pack but are **not currently included in 3.0.0**.

Their removal is not necessarily permanent. They may be restored if they are updated for Valheim 1.0, or replaced if a maintained alternative is found.

| Dependency | Last pack version included | 3.0 status |
| --- | --- | --- |
| `ComfyMods-PotteryBarn` | 2.0.0 | Removed pending update or replacement |
| `ComfyMods-SearsCatalog` | 2.0.0 | Removed pending update or replacement |
| `ComfyMods-ComfyAutoRepair` | 2.0.0 | Removed pending update or replacement |
| `Azumatt-AzuAutoStore` | 2.0.0 | Removed pending update or replacement |
| `Azumatt-AzuCraftyBoxes` | 2.0.0 | Removed pending update or replacement |
| `makail-ItemDrawers` | 2.0.0 | Removed pending update or replacement |
| `BasilPanda-NoStamCosts` | 2.0.0 | Removed pending update or replacement |
| `Advize-StumpsRegrow` | 2.0.0 | Removed pending update or replacement |
| `Azumatt-WardIsLove` | 2.0.0 | Removed pending update or replacement |

## Earlier historical removals and replacements

These dependencies had already left the pack before the 3.0 migration.

| Dependency | Last included | History |
| --- | --- | --- |
| `bbepis-BepInExPack` | 1.0.1 | Replaced by `denikson-BepInExPack_Valheim` beginning with 1.0.2. |
| `Goldenrevolver-Quick_Stack_Store_Sort_Trash_Restock` | 1.0.1 | Removed in 1.0.2 because of documented compatibility issues. |
| `Tekla-AutoRepair` | 1.5.0 | Replaced in the 2.0 generation by `ComfyMods-ComfyAutoRepair`, which is itself currently removed from 3.0 pending maintenance/replacement. |

## Pack direction

The historic name **Vanilla Server Pack** is being retained for continuity, but the design goal for 3.0 is:

- preserve a mostly vanilla-style progression;
- add practical quality-of-life improvements;
- avoid abandoned dependencies;
- use actively maintained Valheim 1.0 mods;
- accept client-side requirements where a QoL mod needs them;
- **do not promise vanilla-client or crossplay compatibility**;
- reintroduce removed features when maintained replacements or updates become available.

## 3.0 validation checklist

- [x] Identify dependencies currently maintained for the Valheim 1.0 migration.
- [x] Remove unmaintained dependencies from the 3.0 manifest.
- [x] Update retained dependency version strings.
- [ ] Determine client-side installation requirements for each dependency.
- [ ] Rebuild configuration files from the current mod versions.
- [ ] Launch-test the complete pack against the target Valheim 1.0 build.
- [ ] Review BepInEx log for plugin/config errors.
- [ ] Test existing-world loading.
- [ ] Test new-world loading.
- [ ] Test multiplayer with all required client mods installed.
- [ ] Test dedicated-server startup where applicable.
- [ ] Document known incompatibilities.
- [ ] Evaluate replacements for removed QoL features.
- [ ] Mark the package release-ready only after runtime testing is complete.

## Credits

See [CREDITS.md](CREDITS.md) for attribution to the authors/projects whose work is represented by this modpack.

## History policy

The versioned packages outside **DeepNorth Update** remain the authoritative historical snapshots. This 3.0.0 folder is the working migration package and may change until compatibility testing is complete.
