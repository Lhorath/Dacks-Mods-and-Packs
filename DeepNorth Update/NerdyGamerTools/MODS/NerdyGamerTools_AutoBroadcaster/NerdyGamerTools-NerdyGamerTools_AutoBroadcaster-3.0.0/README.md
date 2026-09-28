# NerdyGamerTools AutoBroadcaster 3.0.0

**Migration workspace:** Valheim 1.0 / Deep North  
**Package version:** `3.0.0`  
**State:** **Packaging/source synchronization — not yet packaged**

AutoBroadcaster is a dedicated-server scheduled broadcast mod for Valheim.

The maintained source repository currently documents **AutoBroadcaster 2.0.0** as rebuilt for **Valheim 1.0.16**:

**https://github.com/Lhorath/NGT-AutoBroadcaster**

This 3.0.0 folder is the Deep North package-generation workspace. It exists to prepare the next packaged release without modifying or relabeling the historical 1.0.x binaries.

## Current 3.0 package metadata

| Dependency | Version | Source |
| --- | ---: | --- |
| `denikson-BepInExPack_Valheim` | `5.4.2202` | Current AutoBroadcaster 2.0.0 source metadata |

The dependency string is inherited from the maintained source repository's current package metadata. It should only change when the matching AutoBroadcaster source/package is intentionally updated.

## Source state

The maintained source already documents the major Valheim 1.0 migration work, including:

- rebuild for Valheim 1.0.16;
- dedicated-server-only operation;
- vanilla-client compatibility without a custom client handshake;
- minute-of-hour scheduling;
- Alert, Chat, or Both delivery modes;
- live configuration reload;
- per-message enable switches;
- debug logging controls;
- removal of the old Steam_0 log-suppression workaround;
- build documentation for the current source.

## Packaging rule

**Do not copy the archived 1.0.1 DLL into this 3.0 folder and relabel it.**

A matching current build must be produced from the maintained source before this package is considered releasable.

## Historical packaged versions

The archive outside **DeepNorth Update** currently preserves:

- 1.0.0
- 1.0.1

The maintained source repository is newer than those packaged snapshots.

## 3.0 checklist

- [x] Create a 3.0 package scaffold.
- [x] Link the maintained source repository.
- [x] Preserve the source package dependency metadata.
- [x] Keep historical binaries out of the new package.
- [ ] Produce the matching current DLL/build for the 3.0 package generation.
- [ ] Confirm the final package manifest against the source release.
- [ ] Dedicated-server smoke test the packaged build.
- [ ] Verify Alert mode.
- [ ] Verify Chat mode.
- [ ] Verify Both mode.
- [ ] Verify live config reload.
- [ ] Verify vanilla-client behavior.
- [ ] Finalize package README/changelog and archive the completed release.

## History policy

Historical release folders remain unchanged. Current source development belongs in the AutoBroadcaster source repository; this workspace tracks packaging for the Dacks-Mods-and-Packs archive.
