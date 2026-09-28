# NerdyGamerTools AutoBroadcaster 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Compatibility audit baseline — not yet release-ready**

Dedicated-server scheduled broadcast mod. The maintained source repository already contains a 2.0.0 rebuild documented for Valheim 1.0.16; this 3.0.0 folder initializes the Deep North package-generation track.

> The dependency versions below are an **audit starting point**, not a blanket compatibility claim. They were carried forward from the current 2.0.0 source metadata unless otherwise noted. Each dependency should be verified and updated before this package is published.

## 3.0.0 baseline — currently included

| Dependency | Baseline version |
| --- | ---: |
| `denikson-BepInExPack_Valheim` | `5.4.2202` |

## Migration notes

**No DLL is copied into this 3.0.0 scaffold.** The old 1.0.1 binary must not be relabeled as 3.0.0. Build/package the matching 3.0 source before this folder is treated as publishable.

## Historical mods no longer included

No package dependencies are recorded as removed in the preserved history.

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

## Source / upstream

Maintained source repository: **https://github.com/Lhorath/NGT-AutoBroadcaster**

## History policy

The versioned packages outside **DeepNorth Update** remain the authoritative historical snapshots. This 3.0.0 folder is the working migration package and may change until compatibility testing is complete.
