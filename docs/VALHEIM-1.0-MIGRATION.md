# Valheim 1.0 Migration Tracker

This is the working checklist for bringing the historical DabosGG and NerdyGamerTools packages forward after Valheim 1.0.

The historical release folders are intentionally preserved. Migration work should produce new releases rather than rewriting old snapshots.

## Recommended order

The DabosGG packs have dependencies between them, so the safest order is:

1. **DabosGG Vanilla Server Pack**
2. **DabosGG New Skills Pack**
3. **DabosGG New Content Pack**
4. **DabosGG Modded Server Pack**
5. **The Nerdy AzuPack**
6. **AutoBroadcaster archive synchronization**

The Modded Server Pack should be rebuilt last because it aggregates the three DabosGG component packs.

## Common checklist

Use this checklist for every package:

- [ ] Record the intended Valheim 1.0.x target.
- [ ] Audit every `manifest.json` dependency.
- [ ] Confirm dependency project is still maintained.
- [ ] Replace abandoned/incompatible dependencies where appropriate.
- [ ] Confirm BepInEx requirement.
- [ ] Confirm Jotunn requirement where applicable.
- [ ] Review bundled `BepInEx/config` files for renamed/removed keys.
- [ ] Remove obsolete generated/runtime files from the **new** release package.
- [ ] Launch-test locally.
- [ ] Check BepInEx log for exceptions.
- [ ] Load an existing world.
- [ ] Test a new world where generation/content mods require it.
- [ ] Start dedicated server where applicable.
- [ ] Verify required client-side installation behavior.
- [ ] Verify vanilla-client compatibility where claimed.
- [ ] Verify crossplay behavior where claimed.
- [ ] Update README.
- [ ] Update CHANGELOG.
- [ ] Update `manifest.json`.
- [ ] Build a new version folder.
- [ ] Update [COMPATIBILITY.md](COMPATIBILITY.md).
- [ ] Update [VERSION-HISTORY.md](VERSION-HISTORY.md).

## DabosGG Vanilla Server Pack

Latest archived snapshot: **2.0.0**

Primary goal: re-establish the baseline QoL/server package before other DabosGG packs depend on it.

### Dependency review

Historical 2.0.0 includes projects such as BepInExPack Valheim, Jotunn, PlantEasily, PlantEverything, ComfyMods building/QoL mods, AzuAutoStore, AzuCraftyBoxes, ItemDrawers, NoStamCosts, StumpsRegrow, and WardIsLove.

- [ ] Check every historical dependency for a maintained Valheim 1.0-compatible release.
- [ ] Confirm storage/crafting mods do not overlap incompatibly.
- [ ] Re-evaluate the historical "vanilla/crossplay-friendly" description against the rebuilt dependency set.
- [ ] Re-test server-side vs client-required behavior.
- [ ] Rebuild forced/default configs from current mod versions rather than blindly carrying old configs forward.

## DabosGG New Skills Pack

Latest archived snapshot: **2.0.0**

Historical package is centered on Smoothbrain skill mods.

- [ ] Verify each historical skill mod has a Valheim 1.0-compatible release.
- [ ] Confirm skill identifiers/config keys have not changed.
- [ ] Re-check the historical Farming exclusion/compatibility note.
- [ ] Test skill gain, persistence, death penalties, and multiplayer sync.
- [ ] Refresh the changelog; the archived 2.0.0 snapshot contains an older changelog header.

## DabosGG New Content Pack

Latest archived snapshot: **2.0.0**

This is the highest-risk pack because it combines content, creatures, weapons, building pieces, inventory changes, map/server systems, and marketplace/NPC tooling.

- [ ] Audit all content dependencies.
- [ ] Pay special attention to mods touching prefabs, world content, networking, inventory, and NPC systems.
- [ ] Verify Deep North-related mods against Valheim 1.0's official Deep North content.
- [ ] Check for obsolete pre-1.0 biome/content replacements.
- [ ] Test existing worlds before recommending upgrade-in-place.
- [ ] Test progression and crafting unlocks.
- [ ] Validate marketplace/NPC configs.
- [ ] Validate server-side map behavior.
- [ ] Refresh package credits from the final dependency set.

## DabosGG Modded Server Pack

Latest archived snapshot: **1.5.0**

This aggregate pack historically references the Vanilla, New Skills, and New Content packs.

Do not rebuild this first.

- [ ] Finish or establish target versions for all three component packs.
- [ ] Update aggregate dependency versions.
- [ ] Rebuild forced server configuration.
- [ ] Review compatibility blacklist.
- [ ] Run full dedicated-server smoke test.
- [ ] Join with a correctly modded client.
- [ ] Test crossplay/vanilla clients only if the final dependency model claims to support them.
- [ ] Update package README version text.
- [ ] Create a new release snapshot rather than modifying 1.5.0.

## The Nerdy AzuPack

Latest archived snapshot: **1.0.0**

The historical package is a curated set of Azumatt mods plus related dependencies.

- [ ] Audit every Azumatt dependency for current package names/versions.
- [ ] Remove duplicates or superseded utilities.
- [ ] Review configuration interactions among inventory, crafting, storage, ward, and UI/QoL mods.
- [ ] Write full package documentation; the archived README is intentionally minimal.
- [ ] Add a changelog for the next release.

## NerdyGamerTools AutoBroadcaster

Latest archived snapshot here: **1.0.1**

Active source repository:

**https://github.com/Lhorath/NGT-AutoBroadcaster**

Current source version: **2.0.0**

Target documented by the source repository: **Valheim 1.0.16**

Completed in the source repository:

- [x] Rebuilt plugin source for Valheim 1.0.16.
- [x] Preserved minute-of-hour scheduling behavior.
- [x] Preserved legacy config keys where practical.
- [x] Kept the mod dedicated-server only.
- [x] Avoided a custom client network handshake.
- [x] Added per-message enable switches.
- [x] Added debug logging configuration.
- [x] Documented source build process and migration from 1.0.1.

Archive follow-up:

- [ ] Add the final 2.0.0 packaged snapshot to this repository when ready.
- [ ] Include its README, changelog, manifest, icon, and release DLL/package contents as appropriate.
- [ ] Update [VERSION-HISTORY.md](VERSION-HISTORY.md) after the archive snapshot is added.

## Definition of done

A migrated package is ready to be marked **Updated** when:

1. dependency audit is complete;
2. configs are based on current dependency versions;
3. local runtime test passes;
4. applicable dedicated-server test passes;
5. client requirements are documented;
6. crossplay claim, if any, is actually verified;
7. a new immutable release snapshot is created;
8. README/changelog/manifest describe that new release accurately.
