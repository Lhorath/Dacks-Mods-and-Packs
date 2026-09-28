# DabosGG New Skills Pack 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Rebuild / replacement-search phase**

The New Skills Pack is being rebuilt for Valheim 1.0.

All historical **Smoothbrain** skill dependencies have been removed from the 3.0 baseline because they have not yet been updated for Valheim 1.0 compatibility.

For now, this package contains only **BepInExPack Valheim 5.4.2351** as its base dependency while new or updated skill-related mods are evaluated.

## 3.0.0 — currently included

| Dependency | Version | Purpose |
| --- | ---: | --- |
| `denikson-BepInExPack_Valheim` | `5.4.2351` | Core mod framework dependency |

## Looking for new skill mods

The goal of the 3.0 New Skills Pack remains the same: provide additional character progression and skill systems without compromising Valheim 1.0 compatibility.

We are currently looking for maintained mods that can fill areas such as:

- blacksmithing / crafting progression;
- cooking progression;
- dual-wield or weapon specialization;
- foraging;
- ranching;
- mining;
- lumberjacking;
- carry-weight / pack-horse style progression;
- evasion;
- tenacity / survivability;
- exploration;
- other well-maintained skill systems that fit the pack.

New dependencies should only be added after confirming that they are maintained for Valheim 1.0 and work cleanly with the rest of the DabosGG 3.0 stack.

## Removed from the 3.0 baseline

The following historical Smoothbrain dependencies are **not included in 3.0.0** at this time:

| Dependency | Last historical version used | 3.0 status |
| --- | ---: | --- |
| `Smoothbrain-Blacksmithing` | `1.3.3` | Removed pending Valheim 1.0 update or replacement |
| `Smoothbrain-Cooking` | `1.2.2` | Removed pending Valheim 1.0 update or replacement |
| `Smoothbrain-DualWield` | `1.0.10` | Removed pending Valheim 1.0 update or replacement |
| `Smoothbrain-Foraging` | `1.0.10` | Removed pending Valheim 1.0 update or replacement |
| `Smoothbrain-Ranching` | `1.1.6` | Removed pending Valheim 1.0 update or replacement |
| `Smoothbrain-Mining` | `1.1.6` | Removed pending Valheim 1.0 update or replacement |
| `Smoothbrain-Lumberjacking` | `1.0.6` | Removed pending Valheim 1.0 update or replacement |
| `Smoothbrain-PackHorse` | `1.0.4` | Removed pending Valheim 1.0 update or replacement |
| `Smoothbrain-Evasion` | `1.0.4` | Removed pending Valheim 1.0 update or replacement |
| `Smoothbrain-Tenacity` | `1.0.4` | Removed pending Valheim 1.0 update or replacement |
| `Smoothbrain-Exploration` | `1.0.4` | Removed pending Valheim 1.0 update or replacement |
| `Smoothbrain-Farming` | `2.1.12` in pack 1.0.0 | Had already been removed in pack 1.0.1 because of historical compatibility issues; remains excluded |

## Pack direction

For 3.0, this package should:

- prioritize actively maintained Valheim 1.0 skill mods;
- avoid carrying forward abandoned or unverified dependencies;
- preserve the idea of expanded character progression;
- document every replacement when an old Smoothbrain feature is restored through another mod;
- stay modular so dependencies can be added or removed without disturbing the rest of the DabosGG stack.

## 3.0 validation checklist

- [x] Remove unverified Smoothbrain dependencies from the 3.0 manifest.
- [x] Add BepInExPack Valheim 5.4.2351 as the base dependency.
- [ ] Identify maintained Valheim 1.0 skill mods.
- [ ] Evaluate replacements for the historical skill categories.
- [ ] Confirm client/server requirements for each new dependency.
- [ ] Test skill progression, persistence, multiplayer sync, and death penalties where applicable.
- [ ] Update the manifest as replacement mods are selected.
- [ ] Update this README history whenever a skill dependency is added or replaced.
- [ ] Mark the pack release-ready only after the replacement set is tested.

## History policy

The versioned packages outside **DeepNorth Update** remain the authoritative historical snapshots. This 3.0.0 folder is the working migration package and may change until compatibility testing is complete.
