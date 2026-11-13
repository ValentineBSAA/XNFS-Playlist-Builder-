# XNFS Playlist Builder | Changelog

[← Home](README.md) · [Current release notes](RELEASE_NOTES.md) · [Complete test matrix](docs/WHATS-NEW-BETA-1.7.md)

## 3.2 Beta 1.7 · Public beta / prerelease

**Post-release verification, November 13, 2026:** developer valentine reports a successful hands-on Beta 1.7 gameplay test on **Windows 11 / Need for Speed: Most Wanted (2005) Black Edition 1.3 (PC)**. Every feature exercised in that session worked as expected. See [dated PC test record](docs/PC-VALIDATION-BETA-1.7.md). Other systems/games are not implied.

- Added per-song loudness level/progress, completed-song counters, named installer stages and ETA when timing is available.
- Completion-review **OK** now returns to the workspace.
- Embedded Windows app icon and consistent taskbar/shortcut identity.
- Hardened custom-pursuit installation to avoid duplicate source reads, verify outputs and display post-audio restore/cleanup/player-install phases.
- Retained repair for older runtime DLL / Shiboken errors during upgrades.
- Reported **45-song real Most Wanted** custom Pursuit, Safe House and Free Roam gameplay passes; custom Pursuit progress completed.
- **Developer valentine confirmed:** Most Wanted car engine sound volume is **manually** adjusted with the in-game **Car Volume** control; independent builder music gain does not automatically adjust it.
- Packaged installation and views passed reported checks. The **original Developer ZIP** marked final compiled EXE gameplay as not performed **at the time of that report**; developer PC gameplay verification was subsequently reported on November 13, with no tested EXE hash supplied.
- Outstanding: Carbon 1.4 and event gameplay, PLAK, several custom fades, first track after save-switch, unresolved Carbon Load Complete crash.

## 3.2 Beta 1.6 · Documentation and previous test baseline

- Most Wanted custom/ordinary pursuit paths, fades, EA Trax titles, 65% mix, T skip and earlier sessions documented.
- Support ZIP export and independent test matrix, updated licensing notices and GitHub documentation validation.
- See the [archived Beta 1.6 notes](docs/WHATS-NEW-BETA-1.6.md) and [historical release notes](.github/RELEASE-NOTES-BETA-1.6-FOR-GITHUB.md).

## 3.2 Beta 1.5 / 1.4 · Historical releases

- [Beta 1.5 record](docs/WHATS-NEW-BETA-1.5.md) · [Beta 1.4 disclosure](docs/WHATS-NEW-BETA-1.4.md).
- Historical version claims remain anchored to the releases in which they appeared. In particular, Beta 1.4's complete original interactive pursuit feature was not delivered as originally advertised.
