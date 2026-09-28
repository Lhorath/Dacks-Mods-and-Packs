# Dack's Mods & Packs

Historical archive and active maintenance index for Valheim mods and modpacks published under the **DabosGG** and **NerdyGamerTools** namespaces.

This repository preserves complete packaged release snapshots while providing a central place to track compatibility work for modern Valheim releases.

> **Important:** A package being present here does not mean it is compatible with the current version of Valheim.
>
> Package versions such as `1.0.0` or `2.0.0` are the package's own versions. They are **not** Valheim version numbers.

## Valheim 1.0 migration

Valheim 1.0 released on **September 9, 2026**. The historical packages in this repository were created across multiple earlier Valheim releases, so compatibility is being reviewed package by package.

### Deep North / 3.0 workspace

The active compatibility work now lives in **[DeepNorth Update](DeepNorth%20Update/)**. Every maintained package has been initialized as a **3.0.0 migration candidate** with a fresh manifest, changelog, and dependency-history README.

The 3.0 manifests are starting baselines and should **not** be interpreted as tested Valheim 1.0 releases until their dependency and runtime audits are complete.

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
| [DabosGG Modded Server Pack](DabosGG/MODPACKS/DabosGG_Modded_Server_Pack/) | Main aggregate server pack | 1.5.0 | 🛠️ 3.0 migration scaffold initialized |
| [DabosGG New Content Pack](DabosGG/MODPACKS/DabosGG_New_Content_Pack/) | New creatures, equipment, systems, building/content mods | 2.0.0 | 🛠️ 3.0 migration scaffold initialized |
| [DabosGG New Skills Pack](DabosGG/MODPACKS/DabosGG_New_Skills_Pack/) | Additional skill/progression mods | 2.0.0 | 🛠️ 3.0 migration scaffold initialized |
| [DabosGG Vanilla Server Pack](DabosGG/MODPACKS/DabosGG_Vanilla_Server_Pack/) | QoL/server additions intended to stay close to vanilla | 2.0.0 | 🛠️ 3.0 migration scaffold initialized |

The Modded Server Pack historically aggregates the Vanilla, New Skills, and New Content packs plus server configuration.

### NerdyGamerTools

| Package | Purpose | Latest archived snapshot | Active/current source | Valheim 1.0 status |
| --- | --- | ---: | --- | --- |
| [NerdyGamerTools AutoBroadcaster](NerdyGamerTools/MODS/NerdyGamerTools_AutoBroadcaster/) | Dedicated-server scheduled broadcasts | 1.0.1 | [2.0.0 source](https://github.com/Lhorath/NGT-AutoBroadcaster) | 🛠️ 3.0 packaging scaffold initialized |
| [The Nerdy AzuPack](NerdyGamerTools/MODPACKS/The_Nerdy_AzuPack/) | Curated Azumatt QoL/gameplay collection | 1.0.0 | — | 🛠️ 3.0 migration scaffold initialized |

### AutoBroadcaster source repository

The maintained source for **Nerdy Gamer Tools AutoBroadcaster** lives here:

**https://github.com/Lhorath/NGT-AutoBroadcaster**

The source repository currently contains the **2.0.0 Valheim 1.0.16 rebuild**. The Deep North workspace initializes a 3.0.0 packaging target but intentionally does not relabel or copy the historical 1.0.1 DLL.

## Repository layout

```text
Dacks-Mods-and-Packs/
├── README.md
├── DeepNorth Update/       # Active 3.0.0 compatibility workspace
├── docs/
│   ├── COMPATIBILITY.md
│   ├── VALHEIM-1.0-MIGRATION.md
│   └── VERSION-HISTORY.md
├── DabosGG/                # Historical archive
└── NerdyGamerTools/        # Historical archive
```

The historical namespace folders remain immutable release history wherever practical. The **DeepNorth Update** directory is where 3.0 migration manifests, documentation, configs, and rebuilt binaries should be assembled.

## Archive policy

Historical version folders may include old manifests, configs, documentation, icons, compiled DLLs, and server snapshots. They are intentionally preserved.

Do not rewrite historical packages merely to make them look current. Current migration work belongs under **DeepNorth Update** until a validated release is ready.

## Maintainer workflow

1. Start in [DeepNorth Update](DeepNorth%20Update/).
2. Audit every baseline dependency and its maintained replacement, if needed.
3. Confirm BepInEx/Jotunn requirements.
4. Review or rebuild packaged configuration files.
5. Test game startup and world loading.
6. Test dedicated-server startup where applicable.
7. Test client/server requirements and crossplay behavior where applicable.
8. Update the 3.0 README history when dependencies are added, removed, or replaced.
9. Update changelog and manifest.
10. Mark compatibility only after testing.

## Credits

These packs depend on the work of the wider Valheim modding community. Individual manifests and historical release documentation remain the authoritative record of which creators and dependencies were included in each packaged version.

This repository exists both to preserve that history and to make future maintenance easier.
