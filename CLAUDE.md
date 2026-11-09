# SeedCrackerX — Dylan's 1.21.11 copy

This is a local copy of SeedCrackerX (Fabric mod, MIT license) by 19MisterX98, checked out at the last
upstream commit for **Minecraft 1.21.11** (commit 4551964, mod version 2.15.6). Upstream `master` has
moved on to 26.x, so do not merge or pull from upstream master.

## About the user
- Dylan doesn't code himself: explain changes in plain language and keep steps simple.
- He is on Windows. Use `gradlew.bat` (or `.\gradlew` in PowerShell).
- Keep the LICENSE file and the original copyright notice (MIT requirement).

## Setup / build
- Needs **Java 21 (JDK)**. Check with `java -version`; if missing, tell Dylan to install
  Eclipse Temurin 21 (https://adoptium.net) before building.
- Build: `.\gradlew build` — the first build downloads Minecraft, Fabric and Gradle and takes a while.
- The finished mod is `build\libs\seedcrackerX-<version>.jar` (not the `-sources` jar).
- Test in game: put the jar in a 1.21.11 Fabric profile's `mods` folder together with Fabric API
  (and Cloth Config / Mod Menu if wanted).
- `.\gradlew runClient` starts a dev Minecraft client for quick testing.

## Git (set up 2026-11-09)
- Branch `1.21.11`, history starts fresh with the commit
  "Import SeedCrackerX 1.21.11 (upstream 19MisterX98/SeedcrackerX @ 4551964)".
- `origin` is Dylan's fork https://github.com/dylanvod/SeedcrackerX; `1.21.11` tracks `origin/1.21.11`.
- Upstream's `.github/workflows/build.yml` was left out; it is not needed to build locally.
- Commit after each working change.

## Codex
- Codex (background) has no internet: it can edit Java files but cannot run Gradle builds.
  Let Codex write code changes; Claude runs the builds and tests.
