# 🛟 Troubleshooting XNFS Playlist Builder Beta 1.7

[← Home](../README.md) · [First-time guide](GETTING-STARTED.md) · [Exact test status](WHATS-NEW-BETA-1.7.md)

## Where is the installer?

The public release asset is **`XNFS-Playlist-Builder-3.2-Beta-1.7-Public.zip`**, to be posted on [Releases](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases). Extract it and run **`XNFS-Playlist-Builder-3.2-Beta-1.7-Setup.exe`**. GitHub's automatic Source code archives are **not installers**. The Setup EXE is unsigned; compare the [SHA-256](SHA256-OF-BETA-1.7.txt) and only run software you trust.

## Music works, but the engine is too loud or too quiet

**Developer-verified resolution:** In **Most Wanted**, **car engine sound volume must be changed manually inside the game** under **Audio options → Car Volume**. The XNFS builder's independent music volume controls music and **does not change engine volume**. The builder's **65% default** is a suggested starting mix, not a universal fixed balance.

**Status:** this is expected configuration confirmed by developer **valentine**; **it is not a missing feature, open problem or unperformed test**.

## Custom music or song changes don't play

1. Confirm the correct game folder/executable, selected music library and successful scan.
2. Open **Game configuration → Manual assignments**, review category membership and **Save assignments**.
3. With the game closed, open **Game configuration → Installation → Check setup**. Verify player and ASI loader compatibility.
4. Run **Build / Save**, then launch the game.
5. In Most Wanted, try ordinary music before testing advanced pursuit modes. In Carbon, use known class pools for initial verification.

**Gameplay evidence:** the developer reported 45 tracks successfully playing in each of **Most Wanted custom Pursuit, Safe House and Free Roam** during Beta 1.7 tests. **On November 13, the developer also confirmed that all personally exercised features worked on a Windows 11 PC with Most Wanted Black Edition 1.3.** A successful file check or test on one machine does not prove every other game/mod configuration works. [Exact PC record](PC-VALIDATION-BETA-1.7.md).

## Which Most Wanted pursuit mode?

- **Ordinary Pursuit playlist:** full custom songs with chosen fade and finish-current-song options.
- **Original adaptive score:** native soundtrack extracted **inside the game** from your game files. **T does not skip original adaptive nodes**.
- **Custom interactive:** your own selected library tracks, with supported **T** skipping and EA Trax title display. Advanced authored segments remain experimental.

Choose **one** active pursuit mode. Earlier listening accepted the revised **original-score Pursuit → Free Roam** fade, but its timing can feel slow. The newest **custom-mode exit fade**, all natural-song incoming fades and first track after switching saves still require targeted game tests.

## The installer looks stuck at the final audio file

Beta 1.7 adds **post-audio restore, cleanup and player-install stages**, avoids redundant source-audio reads and shows completion counts/ETA when known. Watch the named stage as well as audio percentage. The developer observed the full preparation/installation flow with 45 custom pursuit songs.

If an operation closes unexpectedly, **reopen → Game configuration → Installation → Check setup** before starting installation again. Previous files may have already been written.

## A Shiboken DLL error appears after upgrading the app

An earlier in-place upgrade could leave older runtime DLLs alongside the new application. The Beta 1.7 handoff reports a **versioned runtime** repair and a successful **in-place upgrade** on the affected installation. Close the old error and run the current Beta 1.7 Setup EXE over the existing installed app. This does **not** fix unrelated Carbon game crashes.

## Carbon 1.4 or experimental Canyon/Pursuit/Drift music

The Carbon 1.4 player payload passed isolated installer checks but **not comprehensive live gameplay**. Event mode controls are still experimental; separate custom Canyon/Pursuit buckets are **not implemented**. Carbon's intermittent **Load Complete** crash remains unresolved, and no reliable cause has been established.

## PLAK or heavily modded Most Wanted has problems

Matching all **61 music-hook signatures** can allow installation of a modified executable but **does not verify actual PLAK gameplay**. An observed heavily modded car-body rendering issue remains of uncertain origin; it is not proven to be caused by this audio tool. Do not alter unrelated graphics settings on the assumption XNFS caused it.

## Support ZIP, privacy and restoring files

Choose **Support**, preview Plain English or JSON, and save one local ZIP containing `diagnostics.txt` and `diagnostics.json`. You attach it to GitHub yourself. Generated diagnostics exclude raw logs, private paths, song titles, audio and saves. Manually attached images or logs need separate privacy review.

**Restore backup** uses tracked previous setup records; **Restore original game** attempts to return to recorded originals. Externally edited files and audio generated by the native in-game original-score installer may not be fully recoverable. Keep an independent backup. Uninstalling the desktop app does not reverse game modifications.

**Report useful context:** Beta 1.7, game/executable version, Windows version, selected options, ASI loader, other mods, reproduction steps and the difference between expected and actual playback.

[Report a bug](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose) · [Discussions](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/discussions) · [Backups](BACKUPS-AND-RESTORE.md)
