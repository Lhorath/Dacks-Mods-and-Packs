# Compatibility Matrix

Last reviewed: **2026-09-28**

This file tracks current compatibility work for the packages preserved in this repository.

## Reading this table

- **Latest archived snapshot** means the newest packaged release currently preserved in this repository.
- **Current source** is shown separately when active development happens in another repository.
- A package version does **not** imply compatibility with the same Valheim version number.
- Historical release folders are preserved as-is; current status belongs here and in package-level README files.

## Valheim 1.0 status

| Namespace | Package | Latest archived snapshot | Current source/rebuild | Status | Notes |
| --- | --- | ---: | --- | --- | --- |
| DabosGG | DabosGG Modded Server Pack | 1.5.0 | — | 🟡 Needs validation/rebuild | Aggregate pack depends on the Vanilla, Skills, and Content packs, so those dependencies should be validated first. |
| DabosGG | DabosGG New Content Pack | 2.0.0 | — | 🟡 Needs validation | April 2026 package predates Valheim 1.0 and requires dependency/config review. |
| DabosGG | DabosGG New Skills Pack | 2.0.0 | — | 🟡 Needs validation | Historical 2.0.0 package version is not evidence of Valheim 1.0 compatibility. |
| DabosGG | DabosGG Vanilla Server Pack | 2.0.0 | — | 🟡 Needs validation | QoL/server dependencies and crossplay assumptions need to be rechecked for Valheim 1.0. |
| NerdyGamerTools | The Nerdy AzuPack | 1.0.0 | — | 🟡 Needs validation | Dependency list should be audited against maintained Valheim 1.0-compatible releases. |
| NerdyGamerTools | NerdyGamerTools AutoBroadcaster | 1.0.1 | [2.0.0](https://github.com/Lhorath/NGT-AutoBroadcaster) | 🟢 Rebuilt for Valheim 1.0.16 | Active source repo contains a dedicated-server-only 2.0.0 rebuild targeting Valheim 1.0.16. Archive still stops at packaged 1.0.1. |

## Status definitions

### 🟢 Updated

A maintained rebuild exists for the stated Valheim target.

This does not automatically mean every deployment scenario has been tested. Package-specific notes should record dedicated-server, client, and crossplay testing separately where relevant.

### 🟡 Needs validation

No current compatibility conclusion should be inferred from the historical archive. Dependencies, configs, and runtime behavior still need review.

### 🛠️ Migration work

Use this when active changes are underway and a package is intentionally between historical and current states.

### 📦 Legacy archive

Use this for packages deliberately retained for history/reference and not intended for current deployment.

### ❌ Incompatible

Use only after a concrete incompatibility has been confirmed.

## AutoBroadcaster

The active source repository is:

**https://github.com/Lhorath/NGT-AutoBroadcaster**

The source repo documents **v2.0.0** as a rebuild for **Valheim 1.0.16** and retains the previous configuration model where practical.

Repository distinction:

| Location | Version currently represented |
| --- | ---: |
| Dacks-Mods-and-Packs archive | 1.0.1 |
| NGT-AutoBroadcaster source repo | 2.0.0 |

Until the 2.0.0 packaged snapshot is added to this archive, use the source repository as the current development reference.

## Validation criteria

A package should not be marked current solely because it launches once. Relevant checks include:

- dependency is still maintained and compatible;
- dependency version is correct in `manifest.json`;
- no required dependency has been renamed/replaced;
- game reaches menu without plugin load errors;
- existing world can load;
- new world can load where world-generation mods are involved;
- dedicated server boots where applicable;
- expected configuration files are accepted;
- required client mods are documented;
- vanilla-client behavior is documented;
- crossplay behavior is verified where claimed;
- representative gameplay features work;
- logs contain no recurring compatibility exceptions.

Update this file whenever one of those conclusions changes.
