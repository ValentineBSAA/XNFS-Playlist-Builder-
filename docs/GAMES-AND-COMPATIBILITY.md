# 🎮 Games and compatibility | Beta 1.7

[← Home](../README.md) · [Verified test matrix](WHATS-NEW-BETA-1.7.md) · [Setup](GETTING-STARTED.md)

| Area | Most Wanted (2005) | Carbon (2006) |
| --- | --- | --- |
| Core pools | Safe House, Free Roam, Race, Pursuit, Shared | Menu, Muscle, Tuner, Exotic, Shared |
| Routing | In-game driving state | Menu / active vehicle class |
| Skip button | **T** ordinary/custom continuous; not native adaptive score | Optional/configurable **F9** |
| Dynamic music | Original native adaptive or custom interactive pursuit | Original Canyon/Pursuit and Drift modes experimental |
| Unique custom event pools | Custom interactive Pursuit exists | **No separate custom Canyon/Pursuit pools** |
| Audio controls | Independent Music gain defaults 65%; car engine level adjusted **manually in game** | Crew ducking and audio balance controls |
| Player builds | Accepts inspected hook layouts with 61 matching signatures | Inspected 1.2 and 1.4 version-matched player files |
| Real gameplay test | **45-track** custom Pursuit, Safe House, Free Roam developer confirmations | Earlier **1.2** class/F9/ducking confirmations |
| Outstanding | Save-switch first track, custom fade paths, PLAK, modded rendering report | 1.4 game test, event-music test, intermittent Load Complete crash |

### Most Wanted testing distinction

The developer reported successfully playing **45 tracks in each of three contexts** in Beta 1.7. Earlier sessions confirmed prologue audio, T skipping, EA Trax titles and the original pursuit-score exit fade. These results do not establish compatibility with all saves or modified executables. **Matching 61 music-hook signatures is an installation check, not a PLAK game test.**

**Manual sound balance verified by valentine:** use Most Wanted's **Audio options → Car Volume** for engine sound. The builder's Music level is independent. This is a required manual adjustment, **not an unresolved test**.

### Carbon testing distinction

Carbon 1.2 class music, F9 skip and crew ducking have earlier live-session confirmation; 1.4 installer checks are isolated. Original event soundtrack and Drift choices still need in-game listening. Separate custom Canyon/Pursuit pools remain unimplemented. No root cause has been proven for the intermittent Load Complete crash.

### Safe setup

Requires **Windows 10/11 x64**, user-supplied supported game/music and compatible existing **ASI loader**. Close the game before installation/playlist writes. The builder must not silently replace unfamiliar loader/proxy files. Back up your entire game installation, particularly when using additional mods.

The Beta 1.7 Developer ZIP reports packaged app checks but `gameplay_on_final_exe: false`. See [the exact evidence](WHATS-NEW-BETA-1.7.md).

[Most Wanted guide](MOST-WANTED.md) · [Carbon guide](CARBON.md) · [Technical notes](TECHNICAL-NOTES.md)
