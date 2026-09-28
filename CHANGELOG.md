# Repository Changelog

This changelog tracks repository-level maintenance and the active **3.0 Valheim 1.0 / Deep North migration**.

Historical package changelogs inside old version folders remain unchanged.

## [3.0.0 migration] - 2026-09-28

### Repository

- Formalized namespace responsibilities:
  - **DabosGG** for Dabos.GG game-server-specific curated mods/modpacks/configuration packages.
  - **NerdyGamerTools** for original mods/tools developed and released by NerdyGamerTools/Lhorath.
- Documented **The_Nerdy_AzuPack** as a legacy namespace exception.
- Added package-specific `CREDITS.md` files to every active 3.0 modpack.
- Added repository-wide namespace and attribution policy documentation.

- Added the **DeepNorth Update** workspace for current Valheim 1.0 migration work.
- Initialized 3.0.0 folders for all maintained DabosGG and NerdyGamerTools packages.
- Removed all temporary `crumb.txt` placeholder files.
- Added current compatibility, migration, version-history, and dependency-history documentation.
- Preserved all historical version folders unchanged.

### DabosGG Vanilla Server Pack

- Established the 3.0 Vanilla Server Pack baseline with seven dependencies:
  - `denikson-BepInExPack_Valheim-5.4.2351`
  - `ValheimModding-Jotunn-2.30.2`
  - `Advize-PlantEasily-2.2.2`
  - `Advize-PlantEverything-1.21.3`
  - `ValheimModding-HookGenPatcher-0.0.4`
  - `Searica-AdvancedTerrainModifiers-1.5.4`
  - `NerdyGamerTools-NerdyGamerTools_AutoBroadcaster-3.0.0`
- Added **NerdyGamerTools AutoBroadcaster** to the Vanilla Server Pack so scheduled server broadcasts are part of the baseline Dabos.GG server stack.
- Reframed the pack as a **quality-of-life** package rather than a crossplay-first package.
- Documented that some dependencies may require client installation.
- Preserved removed 2.0 dependencies as possible future restoration/replacement candidates.

### DabosGG New Skills Pack

- Removed all historical Smoothbrain dependencies from the active 3.0 manifest.
- Added `denikson-BepInExPack_Valheim-5.4.2351` as the sole current dependency.
- Moved the pack into a **replacement-search phase** for maintained Valheim 1.0 skill/progression mods.

### DabosGG New Content Pack

- Rebuilt the dependency list around a 17-dependency Valheim 1.0 baseline.
- Updated ten carried-forward dependencies.
- Added seven new 3.0 dependencies.
- Removed fourteen dependencies from the historical 2.0 baseline.
- Preserved all removed dependency history in the 3.0 README.

### DabosGG Modded Server Pack

- Finalized the pack as a **pure aggregate**.
- The manifest now depends only on:
  - `DabosGG-DabosGG_Vanilla_Server_Pack-3.0.0`
  - `DabosGG-DabosGG_New_Skills_Pack-3.0.0`
  - `DabosGG-DabosGG_New_Content_Pack-3.0.0`
- Individual mods are managed only in the component packs.

### The Nerdy AzuPack

- Audited the historical dependency set for the Valheim 1.0 migration.
- Removed the legacy mod dependency collection from the active 3.0 manifest.
- Updated the sole current dependency to `denikson-BepInExPack_Valheim-5.4.2351`.
- Documented which historical mods received 1.0-era fixes and which still lack a maintained upstream 1.0 path.
- Moved the pack into a **maintained-source / replacement rebuild phase**.

### NerdyGamerTools AutoBroadcaster

- Added the 3.0 package scaffold to the Deep North workspace.
- Kept the historical packaged archive unchanged through 1.0.1.
- Linked the maintained source repository:
  - https://github.com/Lhorath/NGT-AutoBroadcaster
- Did not copy or relabel the historical 1.0.1 DLL as a 3.0 build.

### Remaining work

- Runtime-test the Vanilla Server Pack.
- Identify replacements/new mods for the New Skills Pack.
- Runtime/world/client-test the New Content Pack.
- Test the complete Modded Server Pack after its three component packs stabilize.
- Rebuild the AzuPack from maintained current sources/replacements.
- Produce/package a matching current AutoBroadcaster build for the 3.0 package.
