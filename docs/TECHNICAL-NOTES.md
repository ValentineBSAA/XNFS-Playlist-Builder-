# 🔧 Technical notes | Beta 1.5

[← Home](../README.md) · [Beginner guide](GETTING-STARTED.md) · [Current evidence](WHATS-NEW-BETA-1.5.md)

## Supported environment

- **Windows 10/11 x64** compiled application; no user-side Python required.
- Original locally installed **Most Wanted (2005)** or **Carbon (2006)** with an executable accepted by the game's setup manager.
- Compatible **ASI loader** for in-game integration; the manager **does not silently replace an existing third-party loader/proxy**.
- Music library files provided by user; no commercial music or game audio distributed.
- Version-matched **Carbon 1.2 / 1.4** installer payloads passed isolated checks. 1.4 gameplay remains unverified.

## Packaging and install differences

The Beta 1.5 **public Windows ZIP** contains the Setup EXE, first-run help in TXT/HTML, CHANGELOG.md, VERIFICATION.md, and real before/after screenshots. Its ZIP SHA-256 is published in [SHA256-OF-BETA-1.5.txt](SHA256-OF-BETA-1.5.txt).

**Beta 1.4's `No module named 'uuid'` error:** the final Beta 1.5 PyInstaller payload packages the module and `_uuid.pyd`; the last compiled test executable and ten install fixtures passed. Other failures may still exist.

**Public repository:** user-facing docs and screenshots only. GitHub's automatically offered **Source code** zip/tar.gz files contain only the repository snapshot. **The user's editable application source is not included in this public distribution.**

## Most Wanted original soundtrack

Installing **Original interactive music** in the builder deploys/arms the **native XNFS ASI** and supporting files. **Extraction occurs within the game process**, using the original user's audio banks and mappings; a standalone Windows-builder extractor/verification pass must not be substituted. The in-game installer reports progress and approximate per-stage ETA. Game exits/relaunch may be required after native extraction.

The original adaptive score is **not T-skippable**. Custom-library interactive songs and advanced mapped segments are separate modes; mixing original and custom output is not intended. Playback correctness for all recent transitions, sustained pursuit and mode switches still needs a full gameplay regression.

## Carbon event modes

Current Carbon player masks/pools remain **Menu/Muscle/Tuner/Exotic**. Beta 1.5 has tested configuration for original Canyon/Pursuit plus Drift playlist/ambience/silence, and isolated installers for versions 1.2 and 1.4. **Separate custom Canyon/Pursuit runtime context selection is not implemented**. No standalone custom event buckets should be documented as functioning.

Carbon original-score extraction is **experimental** and **must not be equated with Most Wanted's previously accepted native install**.

## What the automated tests demonstrate

Final build: five 178-track full scans/profile switches; ten compiled installer UI/worker cycles against disposable folders; thirty normalization cancel/close cycles; 150 animated review cycles. Tests cover UI operations, playlist output, native mode configuration and rollback fixture behavior. **They are not a fresh full-game compatibility or game-soundtrack acceptance run.**

## Crash diagnostics and rollback

Beta 1.5 replaces transient Qt animation objects with longer-lived timers, queues background installer progress through GUI receivers, disposes completed dialogs/workers and exposes persistent operation, Python and Qt logs. Windows native process faults are still diagnosed using Windows Error Reporting; **Python exception logs cannot capture every native crash**. The intermittent Qt installer failure was hardened but not conclusively reproduced/fixed. Carbon's game-side **Load Complete** failure is a separate unresolved problem.

Installation can complete before a GUI fault, so **reopen → Check setup before reinstallation**. Original restoration depends on tracked baselines; native-extractor-generated audio requires fuller end-to-end restoration tests.

## Disclosures and bug reports

For reproducibility, report Beta 1.5, game executable version, Windows build/scaling, installed loader/other mods, selected options, clear steps, and redacted logs/screenshots. Do not publicly share full personal paths, library metadata or private network details.

[Download checksum](SHA256-OF-BETA-1.5.txt) · [Backups guide](BACKUPS-AND-RESTORE.md) · [File a report](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose)
