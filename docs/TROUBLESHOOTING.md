# 🛟 Troubleshooting Beta 1.6

[← Home](../README.md) · [Getting started](GETTING-STARTED.md) · [Known test status](WHATS-NEW-BETA-1.6.md)

## I can't find the Windows installer

Visit [Releases](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases). Once published, download **`XNFS-Playlist-Builder-3.2-Beta-1.6-Public.zip`**, extract it, and run **`XNFS-Playlist-Builder-3.2-Beta-1.6-Setup.exe`**. GitHub's automatically created Source code ZIP is **not** the installer. The public package does not ship new screenshots.

## Unknown publisher / security prompt

The Setup EXE is **unsigned**. Confirm the file came from this repository and compare the [SHA-256 checksum](SHA256-OF-BETA-1.6.txt). A matching checksum detects alteration but does not certify the program's security.

## No music in game

1. Confirm your game and selected executable, correct game/music folders, and that library Scan found songs.
2. Review **Game configuration → Manual assignments** and save changes if needed.
3. Close the game. Use **Game configuration → Installation → Check setup** to confirm required player components.
4. Make sure a compatible **ASI loader** is already installed and working. Do not casually overwrite other proxy loaders.
5. Use **Build / Save**, then test a simple music state in game. File checks alone do not prove in-game audio.
6. Use **Support** to generate a ZIP for a bug report if the issue persists.

## Which Most Wanted pursuit option should I choose?

- **Ordinary Pursuit playlist:** complete songs from the Pursuit pool, with configurable fades/finish-current-song behavior.
- **Original interactive:** your game's native adaptive score, extracted **inside the game** after the original installer feature is enabled. **T cannot skip native score nodes**.
- **Custom interactive:** your own library songs; **T skip and EA Trax titles** were confirmed in Beta 1.6 gameplay. Advanced authored mapping stays experimental.

Do not select original and custom output together. Beta 1.6 confirms the **original-mode** pursuit-to-Free-Roam fade but its timing can feel slow. **Custom-mode exit fade after the latest revision is not separately confirmed**.

## A first track or fade behaves strangely

The first selected pool after switching saves still needs a full gameplay retest. Likewise, the incoming fade at **every** natural custom-interactive song boundary is not yet confirmed. Capture game mode, settings and expected versus actual behavior. Do not report these as universally fixed.

## Carbon Canyon/Pursuit playlists are missing

That is expected: independent **custom** Canyon/Pursuit song buckets are **not implemented**. Existing custom event paths still reuse car-class pools. Original Canyon/Pursuit and Drift audio configuration has not passed real event-mode acceptance. Carbon **1.4 gameplay is unverified** even though version-matched binaries were packaged.

## Carbon freezes around Load Complete

The intermittent **Load Complete** crash remains open. There is no verified root cause or complete fix. Report the Carbon executable (1.2/1.4), other mods/loader, stage of failure and whether it also occurs without the new player components. Do not delete backups.

## The Windows builder closed during or just after installation

The operation may have already completed. Reopen it and use **Game configuration → Installation → Check setup** before retrying. Inspect any local troubleshooting logs privately. Beta 1.6's clean Setup and disposable installation verification does not guarantee all intermittent UI/runtime faults are resolved.

## Most Wanted car rendering is broken

One heavily modded installation showed a disappearing or incorrectly rendered body. A limited read-only check did **not** establish the cause. It is **not proven** to be related to the music player. This release did not change graphics or LAA flags to address it.

## How do I share useful diagnostics?

Open **Support**, preview **Plain English** or **JSON**, and choose **Save ZIP**. It creates a local archive with **`diagnostics.txt`** and **`diagnostics.json`**; attach it yourself to an issue. The reports exclude raw logs, personal paths, track names, audio files and saves. Scrub **any additional** screenshots/logs you choose to post for private information.

For accurate reproduction, include Beta 1.6, the exact game executable, Windows version, your selected music mode, other mods, steps and expected/actual results.

## Restoration safety

A full native-generated audio rollback is not completely accepted, and pre-existing external mods can complicate restoration. Keep a known-good copy of your complete game folder. Uninstalling the Windows builder does not restore game files.

[Backup guide](BACKUPS-AND-RESTORE.md) · [Create an issue](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose) · [Discussion](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/discussions)
