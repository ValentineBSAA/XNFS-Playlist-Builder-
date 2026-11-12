# 🏁 XNFS Playlist Builder 3.2 Beta 1.6

**Experimental Windows prerelease for Most Wanted (2005) and Carbon (2006)**

> Beta 1.6 expands the amount of **real Most Wanted gameplay confirmation**. It is not a blanket claim of compatibility or bug-free gameplay. Publish this as a **prerelease** with tag `v3.2-beta.1.6`.

## Download and installation

On the [Releases page](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases), choose `XNFS-Playlist-Builder-3.2-Beta-1.6-Public.zip` once posted. Extract it and run `XNFS-Playlist-Builder-3.2-Beta-1.6-Setup.exe`. Requires Windows 10/11 x64, a legal copy of either game, your own music and a compatible existing ASI loader for the game. The Windows installer is **unsigned**. Close the game and independently back up its folder before modifying files.

**Release attachment:** Public ZIP, including Setup EXE, user guide, changelog and third-party notices. The Developer ZIP is **not** the public download. GitHub's automatic Source code links contain only the repository's docs and screenshots.

## What's new

### Most Wanted

- Configurable fade-in and fade-out, plus an option to **finish the current complete song** before switching playlists.
- Better scripted prologue and pursuit routing; **original adaptive**, **custom interactive** and **ordinary pursuit playlist** are separate modes.
- Pursuit-to-Free-Roam fade-out/fade-in improved. The **original-score exit** passed listening acceptance, although its timing can still feel slow.
- Custom interactive library music supports **T skipping** and correctly displayed **EA Trax** song titles. T does **not** skip the game's original adaptive score.
- Default independent music level is **65%**. Optional loudness leveling accepts a target and peak ceiling, using playback copies rather than changing originals.
- Modified `speed.exe` can be accepted when all **61 native music-hook signatures** match. **Actual PLAK gameplay is not verified.**

### Carbon

- Menu, Muscle, Tuner, Exotic and Shared pools, optional F9 skipping, crew balance and ducking controls.
- Matching player payloads for the inspected **Carbon 1.2 and 1.4** executables. **Earlier 1.2 gameplay** confirmed class routing; **1.4 live gameplay is not yet verified**.
- Original Canyon and Pursuit and Drift audio options remain **experimental**; distinct custom Canyon/Pursuit pools are not implemented. The intermittent **Load Complete** crash remains unresolved.

### Builder and support

- Guided per-game installation/review, manual multi-category assignments, backup and original-restoration tools, and improved interface responsiveness.
- The new **Support** button previews a plain-English or JSON report and exports one local ZIP containing both formats. Users decide whether and where to share it; it excludes raw logs, personal paths, song titles, music files and saves.
- No screenshots have been changed for Beta 1.6; the Beta 1.5 gallery remains available.

## What was actually tested

**Reported in actual Most Wanted gameplay:** first three Safe House song fades; prologue audibility; Free Roam track playback; complete-song Free Roam → ordinary Pursuit switching; custom interactive pursuit playing all three selected songs (39 node requests logged without playback errors); T skip; corrected EA Trax titles; 65% mix with car and police radio; and the revised **original** pursuit-score exit fade.

**Build and isolated verification (not game sessions):** clean Windows Setup install, installed-app smoke test and uninstall; both game-mode packaged smoke checks; **10** disposable install/backup/restore review cycles split between the games; **17** core regressions; diagnostics TXT/JSON ZIP export; and native playlist-transition tests. The supplied handoff also records real-output loudness tests and compiled 61-signature hook matching. These findings are taken from the supplied developer verification records; they are not all independently rerun here.

**Still outstanding:** revised **custom** pursuit-mode exit-fade retest; incoming fade at every natural custom-song boundary; first music pool after switching save files; extended regression of all pursuit and mod combinations; PLAK gameplay; Carbon 1.4 and event-mode playback; Carbon Load Complete crash investigation; and a rendering issue seen with a heavily modded Most Wanted installation. Full restoration of all audio generated later by the native extractor is not guaranteed.

## Safety and compatibility

The desktop Setup installer does not automatically alter the game. **Install selected features**, **Build / Save**, and restoration commands can affect game files. Review replacement warnings and backups, particularly on modded installations. A successful file check is not proof of in-game playback. For the original Most Wanted score, extraction runs **inside the game** after the native component is installed, not independently in the Windows builder.

## Checksums

```text
8bf8d69cfaeef2d8759ff172694747fbaebef39661088f1b99bc46110fc3cfd8  XNFS-Playlist-Builder-3.2-Beta-1.6-Public.zip
334ee6a3c55e65e4531bfd8f15036d003a33c20ed71f16133e838c15cdf70511  XNFS-Playlist-Builder-3.2-Beta-1.6-Setup.exe
```

Checksums checked against the supplied Public ZIP and extracted installer, and match the Developer ZIP's manifest.

## Read more

[First-time setup](docs/GETTING-STARTED.md) · [Most Wanted](docs/MOST-WANTED.md) · [Carbon](docs/CARBON.md) · [Complete Beta 1.6 testing matrix](docs/WHATS-NEW-BETA-1.6.md) · [Troubleshooting](docs/TROUBLESHOOTING.md) · [Licensing and credits](docs/LICENSING-AND-CREDITS.md) · [Screenshot gallery](screenshots/README.md).

Historical Beta 1.4 and Beta 1.5 notes are retained. In particular, Beta 1.4's advertised complete interactive pursuit system was not delivered in that earlier build; this note does not retroactively change that history.

---

Built by **valentine**, incorporating original XNFSMusicPlayer and native installer work by **Lovro Pleše (xan1242)**. Independent fan-made tool. No Electronic Arts affiliation or bundled commercial game/music assets.
