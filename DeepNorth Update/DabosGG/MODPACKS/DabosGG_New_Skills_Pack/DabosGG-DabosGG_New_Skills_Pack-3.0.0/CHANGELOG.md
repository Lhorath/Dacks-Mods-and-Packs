# Changelog

## [3.0.0] - Unreleased

### Added

- Added `denikson-BepInExPack_Valheim-5.4.2351` as the base dependency for the rebuilt New Skills Pack.
- Added documentation explaining that the pack is actively looking for maintained Valheim 1.0 skill-related mods and replacements.

### Removed from the 3.0 baseline

Removed all historical Smoothbrain dependencies because they have not yet been updated for confirmed Valheim 1.0 compatibility:

- `Smoothbrain-Blacksmithing`
- `Smoothbrain-Cooking`
- `Smoothbrain-DualWield`
- `Smoothbrain-Foraging`
- `Smoothbrain-Ranching`
- `Smoothbrain-Mining`
- `Smoothbrain-Lumberjacking`
- `Smoothbrain-PackHorse`
- `Smoothbrain-Evasion`
- `Smoothbrain-Tenacity`
- `Smoothbrain-Exploration`

`Smoothbrain-Farming` was already absent from later historical versions and remains excluded.

### Compatibility

- The New Skills Pack is now in a **rebuild / replacement-search phase**.
- No historical Smoothbrain skill mod is being treated as Valheim 1.0 compatible by default.
- Removed skill categories may return through future Smoothbrain updates or maintained replacement mods.
