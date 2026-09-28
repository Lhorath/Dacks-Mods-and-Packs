# Namespace and Attribution Policy

This repository uses two publishing namespaces with different purposes.

## DabosGG

**DabosGG** is the namespace for mods, configurations, and especially modpacks assembled specifically for **Dabos.GG game servers**.

A DabosGG modpack is a curated server package. Inclusion of a third-party mod does **not** imply that DabosGG created or owns that mod.

DabosGG package documentation should:

- identify the package as being assembled for Dabos.GG game servers;
- credit the authors or Thunderstore namespaces responsible for the included third-party mods;
- keep dependency history when mods are removed or replaced;
- link to a package-specific `CREDITS.md` when the dependency list is substantial;
- avoid language that could imply authorship of third-party projects.

## NerdyGamerTools

**NerdyGamerTools** is the namespace for **original mods and tools developed and released by NerdyGamerTools/Lhorath**.

Examples include **NerdyGamerTools AutoBroadcaster**.

NerdyGamerTools releases may depend on third-party frameworks or libraries, and those dependencies should still be credited, but the software published under this namespace is intended to represent original NerdyGamerTools development rather than a curated server modpack.

## Legacy exception: The Nerdy AzuPack

**The_Nerdy_AzuPack** predates this clarified namespace policy and is retained under NerdyGamerTools for historical continuity.

It is a curated modpack, not an original NerdyGamerTools-authored mod.

Its historical and 3.0 migration files remain where they are so repository history is not rewritten. Going forward, newly curated server modpacks should use the **DabosGG** namespace instead.

## Credits policy

Every maintained modpack should include either:

- a Credits section in its README; or
- a dedicated `CREDITS.md`.

Credits identify the author/namespace associated with included mods. They do not replace the upstream project's license, copyright notice, or distribution terms.

When a dependency is removed, its historical contribution may remain documented so the package history stays understandable.
