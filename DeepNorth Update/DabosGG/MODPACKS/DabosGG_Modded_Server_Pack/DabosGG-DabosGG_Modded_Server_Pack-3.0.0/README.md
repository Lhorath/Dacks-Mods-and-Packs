# DabosGG Modded Server Pack 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Aggregate package — component packs still under validation**

The **DabosGG Modded Server Pack** is the top-level bundle for the complete DabosGG modded experience.

For 3.0.0, this package intentionally contains **no individual mod dependencies**.

All individual mods belong in one of the three component packs:

1. **DabosGG Vanilla Server Pack**
2. **DabosGG New Skills Pack**
3. **DabosGG New Content Pack**

This keeps the dependency structure modular and prevents the aggregate pack from duplicating or independently managing individual mod versions.

## 3.0.0 dependencies

| Component pack | Version | Purpose |
| --- | ---: | --- |
| `DabosGG-DabosGG_Vanilla_Server_Pack` | `3.0.0` | Core QoL/server baseline |
| `DabosGG-DabosGG_New_Skills_Pack` | `3.0.0` | Skill and progression additions |
| `DabosGG-DabosGG_New_Content_Pack` | `3.0.0` | New gameplay content, equipment, creatures, building, and related systems |

## Dependency policy

The Modded Server Pack should only depend on the three DabosGG component packs.

Do **not** add individual Thunderstore mods directly to this manifest.

If a mod is added, removed, replaced, or updated:

- QoL/server mods belong in **DabosGG Vanilla Server Pack**.
- Skill/progression mods belong in **DabosGG New Skills Pack**.
- Content/gameplay-expansion mods belong in **DabosGG New Content Pack**.

The aggregate pack should only need a dependency-version change when one of those component packs changes version.

## Historical structure

The earliest `0.0.1` package directly depended on BepInEx.

Beginning with the 1.x generation, the pack was split into component packages. The 3.0 generation continues that structure and makes the separation explicit.

## 3.0 validation checklist

- [x] Restrict the manifest to the three DabosGG component packs.
- [x] Remove the need to manage individual mod dependencies at the aggregate level.
- [ ] Complete Vanilla Server Pack testing.
- [ ] Complete New Skills Pack replacement selection and testing.
- [ ] Complete New Content Pack testing.
- [ ] Install the complete aggregate pack on a clean client.
- [ ] Test dedicated-server startup.
- [ ] Test client connection with the full required mod stack.
- [ ] Review BepInEx logs for cross-pack conflicts.
- [ ] Load an existing world.
- [ ] Test a new world.
- [ ] Confirm configs from the component packs coexist correctly.
- [ ] Mark the aggregate pack release-ready only after all three component packs pass validation.

## History policy

Historical versions outside **DeepNorth Update** remain unchanged and preserve the original release structure.
