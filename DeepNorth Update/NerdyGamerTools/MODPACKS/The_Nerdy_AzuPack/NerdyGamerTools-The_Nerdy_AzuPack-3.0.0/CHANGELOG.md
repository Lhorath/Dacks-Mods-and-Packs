# Changelog

## [3.0.0] - Unreleased

### Changed

- Reset The Nerdy AzuPack dependency list for the Valheim 1.0 / Deep North rebuild.
- Updated the base framework dependency to `denikson-BepInExPack_Valheim-5.4.2351`.
- Removed the historical mod dependency set from the active 3.0 Thunderstore manifest.

### Dependency audit

- Confirmed that several historical Azumatt mods did receive Valheim 1.0 fixes.
- Those old Thunderstore package lines are now deprecated and are not being used as the long-term 3.0 dependency source.
- Other historical dependencies have no maintained native Valheim 1.0 upstream release and remain removed.
- Smoothbrain Backpacks currently requires a third-party compatibility shim for Valheim 1.0 and is therefore not retained directly.
- AzuSkillTweaks and the original SleepSkip build remain excluded because their pre-1.0 API usage requires updates or replacement paths.

### Next steps

- Identify maintained current package sources for desired Azumatt functionality.
- Select replacements where appropriate.
- Rebuild the AzuPack around only maintained Valheim 1.0 dependencies.
