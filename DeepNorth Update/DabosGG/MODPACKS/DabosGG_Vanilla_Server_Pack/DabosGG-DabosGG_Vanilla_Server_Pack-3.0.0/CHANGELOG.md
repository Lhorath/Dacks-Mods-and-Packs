# Changelog

## [3.0.0] - Unreleased

### Added

- Initialized the Valheim 1.0 / Deep North generation of the DabosGG Vanilla Server Pack.
- Defined the 3.0 pack direction as a maintained **quality-of-life** package rather than a vanilla-client/crossplay-oriented package.
- Added explicit dependency-history documentation for retained, temporarily removed, and historically replaced mods.

### Updated

- `denikson-BepInExPack_Valheim`: `5.4.2333` → `5.4.2351`
- `ValheimModding-Jotunn`: `2.29.0` → `2.30.2`
- `Advize-PlantEasily`: `2.1.1` → `2.2.2`
- `Advize-PlantEverything`: `1.20.0` → `1.21.3`
- `Searica-AdvancedTerrainModifiers`: `1.4.1` → `1.5.4`
- Retained `ValheimModding-HookGenPatcher-0.0.4`.

### Removed from the 3.0 baseline

These dependencies were present in 2.0.0 but are not currently being carried into 3.0:

- `ComfyMods-PotteryBarn`
- `ComfyMods-SearsCatalog`
- `ComfyMods-ComfyAutoRepair`
- `Azumatt-AzuAutoStore`
- `Azumatt-AzuCraftyBoxes`
- `makail-ItemDrawers`
- `BasilPanda-NoStamCosts`
- `Advize-StumpsRegrow`
- `Azumatt-WardIsLove`

They may be restored if updated for Valheim 1.0 or replaced by maintained alternatives.

### Compatibility

- The retained dependency list has been selected for the Valheim 1.0 migration.
- Runtime compatibility testing is still required before 3.0.0 is considered release-ready.
- Some mods may require client-side installation.
- The 3.0 pack **does not promise vanilla-client or crossplay compatibility**.
