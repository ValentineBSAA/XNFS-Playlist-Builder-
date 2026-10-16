# 🎮 Game support and feature comparison

**XNFS Playlist Builder 3.2 Beta 1.5**, a Windows 10/11 (64-bit) experimental prerelease.

[← Home](../README.md) · [Download](../RELEASE_NOTES.md) · [Known limits](WHATS-NEW-BETA-1.5.md)

| Feature | 🟡 Most Wanted (2005) | 🔵 Carbon (2006) |
| --- | --- | --- |
| Main pools | Safe House, Free Roam, Race, Pursuit | Menu, Muscle, Tuner, Exotic |
| Fallback pool | Shared | Shared |
| Main soundtrack routing | Driving state | Car class |
| Skip key | T for ordinary/custom continuous music | Configurable F9 |
| Dynamic/default soundtrack | Original native interactive pursuit score (previous gameplay confirmation) | Original Canyon/Pursuit event choices (needs live event tests) |
| Custom event options | Library-based custom pursuit, advanced experimental mapped packs | Custom event mode currently falls back to car-class pools |
| Separate custom Canyon/Pursuit categories | Not applicable | **Not implemented** |
| Drift mode selection | Not applicable | Playlist, original ambience or silence; needs game test |
| Dialogue/music feature | EA Trax notifications | Optional crew-speech ducking; optional crew balance |
| Loudness leveling | Creates separate copies | Creates separate copies |
| Scan/assign/preview | Automated pass | Automated pass |
| Backup/original restore | Isolated pass; some native-generated files need tests | Isolated pass; pre-existing external mods complicate restore |
| Intermittent crash watch | Windows builder installer UI hardened, not all cases proven fixed | Separate **Load Complete** crash unresolved |

## Exact Carbon versions

- **Carbon 1.2:** earlier real gameplay confirmation for car-class music, F9 and crew ducking.
- **Carbon 1.4:** matched player payload present; isolated installation checks pass. **No comprehensive live-game verification yet.**

## Most Wanted verification

Earlier developer sessions confirmed music in game states, **T** skipping custom continuous music, the native in-game original pursuit soundtrack installation and playback, and custom pursuit playback. **The latest Beta 1.5 full transition/event regression is incomplete**, including original/custom overlap, long pursuits and complete restoration.

The **original native adaptive score is not T-skippable**. Most Wanted **Safe House** includes frontend menus. Police-radio ducking is a future idea, **not part of this release**.

## Supported system and safe setup

- **Windows 10/11 x64**, game and music provided separately by the player.
- **Supported game executable** required; heed application checks.
- **Compatible ASI loader** required for in-game integration. The builder guides detection/setup and does not silently replace unknown third-party loader/proxy files.
- Close the game before installing features, saving playlists or restoring.
- Back up the full game folder and any original XNFSMusicPlayer installation.
- Other game mods, sound configuration and PC hardware can affect behavior.

[Most Wanted detailed guide](MOST-WANTED.md) · [Carbon guide](CARBON.md) · [Technical notes](TECHNICAL-NOTES.md)
