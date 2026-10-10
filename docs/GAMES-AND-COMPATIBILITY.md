# 🎮 Carbon and Most Wanted: what's supported?

**Both games work with XNFS Playlist Builder.** They now share a stronger set of playlist-building and playback options, but still have different game-specific features.

[← Home](../README.md) · [How to get started](GETTING-STARTED.md)

## 🟡 Most Wanted (2005)

**Four soundtrack groups:**
- **Safe House:** game menus and safe house. These now use one playlist, not two.
- **Free Roam:** driving around Rockport.
- **Race:** active racing.
- **Pursuit:** police chases.

Automatic driving playlist routing is implemented. State playback and **T skipping while driving** were tested by the developer in earlier Beta 1.4 sessions. **The latest change merging menu and safe-house routing has not yet received a new in-game acceptance test.**

Extras include repeat-aware shuffle, optional music loudness leveling, and EA Trax song notifications. Most Wanted doesn't use Carbon's F9 skip shortcut. **Automatic music ducking for police radio is not in this release.**

## 🔵 Carbon (2006)

- **Menu:** menus and browsing.
- **Muscle:** rock and guitar-focused genres are suggested.
- **Tuner:** pop and electronic genres are suggested.
- **Exotic:** hip-hop, rap and grime are suggested.

Optional **F9 skipping**, shuffle, leveling, and music ducking while crew members speak are available.

**Carbon 1.2:** In-game playback, car-class routing, skipping and leveling have been tested by the developer.

**Carbon 1.4:** Version-matched player prepared and checked offline. More live gameplay testing is required.

## Shared library features

| What you can do | Carbon | Most Wanted |
| --- | --- | --- |
| Add music from your computer | ✅ | ✅ |
| Organize tracks automatically or manually | ✅ | ✅ |
| Four game-specific playlist categories | ✅ | ✅ |
| Automatic selection in-game | Car class | Game situation |
| Shuffle without early repeats | ✅ | ✅ |
| Optional consistent-volume music copies | ✅ | ✅ |
| Skip songs | F9, if enabled | T while driving |
| Backup and restore supported changes | ✅ | ✅ |

**The genre sorter uses saved music metadata, not online services or audio recognition.** Automatic balancing can place tracks outside their typical genre group. There is no hard track-count cap.

## Game setup matters

A compatible **ASI loader**, supported executable and correct folders are required for game integration. Existing mods and different game installations can affect behavior. The installer performs compatibility checks before applying changes.

Never override a compatibility warning to force unsupported game files.

[Questions about installation?](TROUBLESHOOTING.md) · [Backups and restoring](BACKUPS-AND-RESTORE.md)
