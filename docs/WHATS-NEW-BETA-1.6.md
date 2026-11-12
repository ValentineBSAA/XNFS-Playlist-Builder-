# XNFS Playlist Builder 3.2 Beta 1.6: changes, tests and open issues

[← Home](../README.md) · [Release notes](../RELEASE_NOTES.md) · [Support](TROUBLESHOOTING.md)

**Status:** Windows experimental prerelease. This document distinguishes *user-heard game sessions*, *isolated/automated tests*, and *untested or unresolved behavior*. It is based on the Beta 1.6 Developer ZIP handoff and verification report.

## Changes

- Most Wanted adjustable fade-in/fade-out, finish-current-complete-song mode, improved scripted prologue and pursuit routing, native/custom pursuit separation, corrected custom T skipping and EA Trax titles, default 65% independent gain.
- Most Wanted native hook-layout matching for modified executables when **all 61 signatures match**; compatibility is not a claim of successful gameplay on every modified build.
- Carbon builds for inspected versions 1.2 and 1.4, existing class playlists and F9/ducking settings. Experimental event settings remain explicitly labeled.
- Shared manual multi-category assignment matrix, guided install/repair, target/peak loudness leveling of **copies**, improved switching performance and an in-app **Support → Save ZIP** tool.

## Most Wanted real gameplay acceptance

| Feature or scenario | Evidence recorded | Status |
| --- | --- | --- |
| Safe House complete-song fades | First three excerpts heard fading | **Passed in tested session** |
| Prologue music | Audible after independent-volume fix | **Passed in tested session** |
| Free Roam | Selected playlist played in game | **Passed in tested session** |
| Free Roam → ordinary Pursuit | Current song finished, Pursuit pool then selected | **Passed in tested session** |
| Custom interactive pursuit | Three intended library songs played; 39 logged node requests without logged errors | **Passed in tested session** |
| Custom interactive T skip | Developer confirmed track skipping in game | **Passed in tested session** |
| Custom EA Trax titles | Correct titles confirmed in game | **Passed in tested session** |
| Original adaptive pursuit music | Earlier session confirmed playback; revised exit fade subsequently heard | **Passed in tested sessions** |
| Original pursuit → Free Roam | Revised fade-out and fade-in heard; timing can feel slow | **Passed with timing caveat** |
| Music level | 65% balance accepted with engine and police radio audible | **Passed in tested session** |
| Custom pursuit → Free Roam after latest revision | Revised custom-mode handoff not separately retested | **Needs gameplay retest** |
| Incoming fade at every natural custom track boundary | BASS fixture checked endpoints, not every live transition | **Needs targeted listening** |
| First music pool after changing saves | Fresh-scene priming logic tested; no full live save-switch acceptance | **Needs gameplay retest** |
| Modified Most Wanted/PLAK gameplay | 61 music-hook signatures may match; actual game not exercised | **Unverified** |
| Reported car-body rendering issue | Observed with heavy graphics/mod stack, cause unknown | **Unresolved, not attributed to XNFS** |

The native **original** adaptive score is separate from custom library interactive music. **T does not skip original adaptive nodes**. This record proves reported sessions, not all possible tracks, save transitions, mod loads or long pursuits.

## Carbon evidence and limitations

| Feature | Evidence | Status |
| --- | --- | --- |
| 1.2 car-class pools | Earlier real gameplay confirmed class routing | **Earlier gameplay pass** |
| F9 skip, crew speech ducking | Earlier 1.2 gameplay confirmation | **Earlier gameplay pass** |
| 1.2 / 1.4 player payload installation | Version-matched payloads and isolated installation checks | **Automated pass only for 1.4** |
| Original Canyon/Pursuit, Drift choices | Configuration and fixture tests | **Needs real event playback** |
| Separate custom Canyon/Pursuit track pools | Current runtime uses existing car-class masks | **Not implemented** |
| Intermittent Load Complete game crash | Cause not established; no verified fix | **Open issue** |

## Windows app and isolated test evidence

- Clean **Inno Setup** install → installed app startup smoke test → installed documentation verification → uninstall all recorded as passed.
- Packaged smoke checks for both Most Wanted and Carbon profiles, including UI, required payloads, FFmpeg and Beta version.
- **Ten** disposable game-installation cycles alternating Most Wanted and Carbon, each checking real review/worker execution and backup verification. These used disposable folders, **not ten real game launches**.
- **17** core regression checks reported passing, plus native playlist-transition checks.
- Support button ZIP export checked after restarting Beta 1.6. One file picker produced a ZIP with `diagnostics.txt` and `diagnostics.json`; both previews and redaction were checked.
- Loudness leveling output measured at configured targets with sources unchanged; cache reuse checked. Custom music can be leveled; native original/mapped soundtrack preserves its authored levels.
- UI contrast, editable assignment matrix and improved game/tab switch behavior checked in source/automated tests. A prior local full-library switch was roughly 0.3–0.4 seconds; **not a performance guarantee**.
- Build artifacts and SHA-256 were supplied in the Developer ZIP; the Public ZIP and Setup EXE hashes were separately recalculated for publication preparation.

## Important cautions

**Do not equate an installer check with gameplay compatibility.** Carbon 1.4, actual PLAK gameplay, full save-switch sequencing, independent custom Canyon/Pursuit pools and full native-generated audio restoration are not claimed tested/completed.

**Backups:** Installing the desktop app alone does not modify your game, but installing player components, writing playlists and restoring files can. Keep an independent full copy of each modded game folder.

**Support and privacy:** the in-app report excludes raw logs, personal paths, music titles, audio and saves. It creates a local ZIP, not an automatic upload. Review any manually attached screenshots or logs separately.

**Historical releases:** [Beta 1.5](WHATS-NEW-BETA-1.5.md) and [Beta 1.4](WHATS-NEW-BETA-1.4.md) remain archived as their own release records. Beta 1.4's previously overstated interactive-pursuit claim is not retroactively corrected into a success.

[Installation](GETTING-STARTED.md) · [Most Wanted guide](MOST-WANTED.md) · [Carbon guide](CARBON.md) · [Compatibility](GAMES-AND-COMPATIBILITY.md) · [Backups](BACKUPS-AND-RESTORE.md)
