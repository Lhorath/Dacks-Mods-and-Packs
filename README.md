# Dack's Mods & Packs

Historical archive and active maintenance index for Valheim mods and modpacks published under the **DabosGG** and **NerdyGamerTools** namespaces.

This repository preserves complete packaged release snapshots while providing a central place to track compatibility work for modern Valheim releases.

> **Important:** A package being present here does not mean it is compatible with the current version of Valheim.
>
> Package versions such as `1.0.0` or `2.0.0` are the package's own versions. They are **not** Valheim version numbers.

## Valheim 1.0 migration

Valheim 1.0 released on **September 9, 2026**. The historical packages in this repository were created across multiple earlier Valheim releases, so compatibility is being reviewed package by package.

See:

- [Compatibility Matrix](docs/COMPATIBILITY.md)
- [Valheim 1.0 Migration Tracker](docs/VALHEIM-1.0-MIGRATION.md)
- [Repository Version History](docs/VERSION-HISTORY.md)

### Status legend

| Status | Meaning |
| --- | --- |
| 🟢 **Updated** | A current rebuild exists for the stated Valheim target. |
| 🟡 **Needs validation** | Historical package has not completed Valheim 1.0 compatibility review. |
| 🛠️ **Migration work** | Package is being rebuilt, reconfigured, or dependency-audited. |
| 📦 **Legacy archive** | Preserved for historical/reference use rather than current deployment. |
| ❌ **Incompatible** | Confirmed incompatible with the stated Valheim target. |

## Package index

### DabosGG

| Package | Purpose | Latest archived snapshot | Valheim 1.0 status |
| --- | --- | ---: | --- |
| [DabosGG Modded Server Pack](DabosGG/MODPACKS/DabosGG_Modded_Server_Pack/) | Main aggregate server pack | 1.5.0 | 🟡 Needs validation/rebuild |
| [DabosGG New Content Pack](DabosGG/MODPACKS/DabosGG_New_Content_Pack/) | New creatures, equipment, systems, building/content mods | 2.0.0 | 🟡 Needs validation |
| [DabosGG New Skills Pack](DabosGG/MODPACKS/DabosGG_New_Skills_Pack/) | Additional skill/progression mods | 2.0.0 | 🟡 Needs validation |
| [DabosGG Vanilla Server Pack](DabosGG/MODPACKS/DabosGG_Vanilla_Server_Pack/) | QoL/server additions intended to stay close to vanilla | 2.0.0 | 🟡 Needs validation |

The Modded Server Pack historically aggregates the Vanilla, New Skills, and New Content packs plus server configuration.

### NerdyGamerTools

| Package | Purpose | Latest archived snapshot | Active/current source | Valheim 1.0 status |
| --- | --- | ---: | ---: | --- |
| [NerdyGamerTools AutoBroadcaster](NerdyGamerTools/MODS/NerdyGamerTools_AutoBroadcaster/) | Dedicated-server scheduled broadcasts | 1.0.1 | [2.0.0 source](https://github.com/Lhorath/NGT-AutoBroadcaster) | 🟢 Rebuilt for Valheim 1.0.16 |
| [The Nerdy AzuPack](NerdyGamerTools/MODPACKS/The_Nerdy_AzuPack/) | Curated Azumatt QoL/gameplay collection | 1.0.0 | — | 🟡 Needs validation |

### AutoBroadcaster source repository

The maintained source for **Nerdy Gamer Tools AutoBroadcaster** lives here:

**https://github.com/Lhorath/NGT-AutoBroadcaster**

The source repository currently contains the **2.0.0 Valheim 1.0.16 rebuild**. This archive currently preserves packaged versions through **1.0.1**, so the two version numbers are intentionally shown separately until the newer packaged release is added here.

## Repository layout

```text
Dacks-Mods-and-Packs/
├── README.md
├── docs/
│   ├── COMPATIBILITY.md
│   ├── VALHEIM-1.0-MIGRATION.md
│   └── VERSION-HISTORY.md
├── DabosGG/
│   └── MODPACKS/
│       ├── DabosGG_Modded_Server_Pack/
│       ├── DabosGG_New_Content_Pack/
│       ├── DabosGG_New_Skills_Pack/
│       └── DabosGG_Vanilla_Server_Pack/
└── NerdyGamerTools/
    ├── MODS/
    │   └── NerdyGamerTools_AutoBroadcaster/
    └── MODPACKS/
        └── The_Nerdy_AzuPack/
```

Each package directory contains historical release folders. For example:

```text
DabosGG_New_Content_Pack/
├── README.md
├── DabosGG-DabosGG_New_Content_Pack-1.0.0/
├── ...
└── DabosGG-DabosGG_New_Content_Pack-2.0.0/
```

The package-level `README.md` is the navigation/current-status page. Version-numbered folders are preserved release snapshots.

## Archive policy

The version folders in this repository are intentionally historical.

They may include:

- historical `manifest.json` dependency lists;
- configuration files from that release;
- original README/changelog text;
- package icons;
- compiled mod binaries;
- server configuration snapshots.

Old snapshots should generally remain unchanged, even if their documentation later becomes stale. Corrections and current compatibility information belong in the package-level README and repository-wide documentation.

When a new package is released, prefer adding a new version folder rather than replacing an older snapshot.

## Versioning

Packages generally use semantic-style versioning:

```text
MAJOR.MINOR.PATCH
```

These numbers describe the **package release**, not Valheim itself.

Always check [COMPATIBILITY.md](docs/COMPATIBILITY.md) before using an archived release on a current server.

## Maintainer workflow

For a Valheim 1.0 migration or new package release:

1. Audit every dependency and its maintained replacement, if needed.
2. Confirm BepInEx/Jotunn requirements.
3. Review packaged configuration files.
4. Test game startup and world loading.
5. Test dedicated-server startup where applicable.
6. Test client/server requirements and crossplay behavior where applicable.
7. Update package documentation and changelog for the new release.
8. Create a new immutable version folder.
9. Update the repository compatibility matrix and migration tracker.
10. Publish the package.

## Credits

These packs depend on the work of the wider Valheim modding community. Individual manifests and historical release documentation remain the authoritative record of which creators and dependencies were included in each packaged version.

This repository exists both to preserve that history and to make future maintenance easier.
