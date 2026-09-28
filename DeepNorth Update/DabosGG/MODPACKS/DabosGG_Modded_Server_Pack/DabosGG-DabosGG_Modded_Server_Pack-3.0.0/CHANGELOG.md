# Changelog

## [3.0.0] - Unreleased

### Changed

- Defined the Modded Server Pack as a pure aggregate package.
- The 3.0 manifest contains only the three DabosGG component packs:
  - `DabosGG-DabosGG_Vanilla_Server_Pack-3.0.0`
  - `DabosGG-DabosGG_New_Skills_Pack-3.0.0`
  - `DabosGG-DabosGG_New_Content_Pack-3.0.0`
- Individual mod dependencies are intentionally managed only by their respective component packs.

### Compatibility

- Aggregate testing should begin only after the three component packs have reached a stable 3.0 baseline.
- The Modded Server Pack inherits the client/server requirements and compatibility constraints of all three component packs.
