# Valheim 1.0 Migration Tracker

This is the working checklist for bringing the historical DabosGG and NerdyGamerTools packages forward after Valheim 1.0.

The historical release folders are intentionally preserved. Migration work should produce new releases rather than rewriting old snapshots.

## Deep North 3.0 initialization

The **[DeepNorth Update](../DeepNorth%20Update/)** workspace is now initialized. All six maintained packages have a 3.0.0 migration folder with fresh metadata and dependency-history documentation. Historical package folders remain unchanged.

## Recommended order

The DabosGG packs have dependencies between them, so the safest order is:

1. **DabosGG Vanilla Server Pack**
2. **DabosGG New Skills Pack**
3. **DabosGG New Content Pack**
4. **DabosGG Modded Server Pack**
5. **The Nerdy AzuPack**
6. **AutoBroadcaster 3.0 packaging/source synchronization**

The Modded Server Pack should be rebuilt last because it aggregates the three DabosGG component packs.

## Common checklist

Use this checklist for every package:

- [x] Create the 3.0.0 migration scaffold.
- [x] Add a README showing currently included and historically removed dependencies.
- [ ] Record the final intended Valheim 1.0.x target.
- [ ] Audit every `manifest.json` dependency.
- [ ] Confirm dependency project is still maintained.
- [ ] Replace abandoned/incompatible dependencies where appropriate.
- [ ] Confirm BepInEx requirement.
- [ ] Confirm Jotunn requirement where applicable.
- [ ] Review bundled `BepInEx/config` files for renamed/removed keys.
- [ ] Build fresh configs/binaries where applicable; do not relabel historical binaries.
- [ ] Launch-test locally.
- [ ] Check BepInEx log for exceptions.
- [ ] Load an existing world.
- [ ] Test a new world where generation/content mods require it.
- [ ] Start dedicated server where applicable.
- [ ] Verify required client-side installation behavior.
- [ ] Verify vanilla-client compatibility where claimed.
- [ ] Verify crossplay behavior where claimed.
- [ ] Finalize README.
- [ ] Finalize CHANGELOG.
- [ ] Finalize `manifest.json`.
- [ ] Update [COMPATIBILITY.md](COMPATIBILITY.md).
- [ ] Update [VERSION-HISTORY.md](VERSION-HISTORY.md).

## Package workspaces

- [DabosGG Vanilla Server Pack 3.0.0](../DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_Vanilla_Server_Pack/DabosGG-DabosGG_Vanilla_Server_Pack-3.0.0/)
- [DabosGG New Skills Pack 3.0.0](../DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_New_Skills_Pack/DabosGG-DabosGG_New_Skills_Pack-3.0.0/)
- [DabosGG New Content Pack 3.0.0](../DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_New_Content_Pack/DabosGG-DabosGG_New_Content_Pack-3.0.0/)
- [DabosGG Modded Server Pack 3.0.0](../DeepNorth%20Update/DabosGG/MODPACKS/DabosGG_Modded_Server_Pack/DabosGG-DabosGG_Modded_Server_Pack-3.0.0/)
- [The Nerdy AzuPack 3.0.0](../DeepNorth%20Update/NerdyGamerTools/MODPACKS/The_Nerdy_AzuPack/NerdyGamerTools-The_Nerdy_AzuPack-3.0.0/)
- [AutoBroadcaster 3.0.0](../DeepNorth%20Update/NerdyGamerTools/MODS/NerdyGamerTools_AutoBroadcaster/NerdyGamerTools-NerdyGamerTools_AutoBroadcaster-3.0.0/)

## Package-specific priorities

### DabosGG Vanilla Server Pack

The dependency-selection pass is complete for the initial 3.0 baseline.

Currently retained:

- `denikson-BepInExPack_Valheim-5.4.2351`
- `ValheimModding-Jotunn-2.30.2`
- `Advize-PlantEasily-2.2.2`
- `Advize-PlantEverything-1.21.3`
- `ValheimModding-HookGenPatcher-0.0.4`
- `Searica-AdvancedTerrainModifiers-1.5.4`

The pack is now intentionally **QoL-focused rather than vanilla-client/crossplay-focused**. Some dependencies may require installation on clients. The next pass is runtime testing, client/server requirement verification, and rebuilding configs.

Removed 2.0 dependencies remain candidates for reintroduction if they receive Valheim 1.0 updates or a maintained replacement is selected.

### DabosGG New Skills Pack

Audit every Smoothbrain skill mod and keep Farming excluded unless compatibility is deliberately re-established.

### DabosGG New Content Pack

Highest-risk audit. Review Deep North/biome content, prefabs, world systems, inventory, networking, NPC/marketplace systems, and upgrade safety for existing worlds.

### DabosGG Modded Server Pack

Test after the three component packs are stable. Its 3.0.0 manifest already points to the 3.0.0 component candidates.

### The Nerdy AzuPack

Audit every dependency for current package name/version and review interactions among inventory, crafting, storage, ward, and UI/QoL mods.

### NerdyGamerTools AutoBroadcaster

Maintained source: **https://github.com/Lhorath/NGT-AutoBroadcaster**

The source repo already documents a 2.0.0 Valheim 1.0.16 rebuild. The 3.0 scaffold must receive a matching rebuilt DLL/source version before it is publishable.

## Definition of done

A 3.0 package is ready to be marked **Updated** when:

1. dependency audit is complete;
2. configs are based on current dependency versions;
3. required binaries are rebuilt rather than copied from incompatible history;
4. local runtime test passes;
5. applicable dedicated-server test passes;
6. client and crossplay requirements are documented and tested where claimed;
7. README/changelog/manifest describe the final package accurately.
