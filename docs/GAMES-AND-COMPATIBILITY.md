# 🎮 Game support and compatibility: Beta 1.6

[← Home](../README.md) · [Full test record](WHATS-NEW-BETA-1.6.md) · [Installation](GETTING-STARTED.md)

| Feature | Most Wanted (2005) | Carbon (2006) |
| --- | --- | --- |
| Core categories | Safe House, Free Roam, Race, Pursuit, Shared | Menu, Muscle, Tuner, Exotic, Shared |
| Routing | Driving state | Menu and car class |
| Skip key | **T** for ordinary/custom continuous audio | Optional/configurable **F9** |
| Original dynamic music | Native adaptive pursuit score; earlier and revised fade gameplay confirmed | Original Canyon/Pursuit and Drift controls **unverified in event gameplay** |
| Custom music | Ordinary pursuit pool or custom interactive selected songs | Class pools; **no independent custom Canyon/Pursuit pools** |
| Leveling | Source-preserving audio copies and adjustable target/peak | Source-preserving audio copies and adjustable target/peak |
| Dialogue options | Independent mix, EA Trax titles; **no police radio ducking** | Crew speech ducking and balance (partly experimental) |
| Installation | Existing ASI loader and accepted hook signatures needed | Version-matched player for inspected 1.2 and 1.4 |
| Live verification | Numerous **specific Beta 1.6 MW sessions** accepted | Earlier **Carbon 1.2** class/F9/ducking gameplay only |
| Known issues | Save switching, some custom fades, modified-game compatibility, heavily modded rendering report | Event playback, 1.4 game test and unresolved Load Complete crash |

## Executable and compatibility boundaries

**Most Wanted:** modified executables can pass installer checking **if all 61 native music-hook signatures match**. Modified or PLAK gameplay has **not** been accepted merely by matching signatures. Scripted prologue and standard pursuit routing were heard in the tested installation; other installs/mod combinations may differ.

**Carbon 1.2:** earlier gameplay confirmed core car-class playback, F9 and crew ducking. **Carbon 1.4:** its inspected payload and fixture installation pass but real gameplay remains unverified. Other region/version builds are not automatically declared compatible.

**Windows:** 10/11 x64, game/music provided by the user, compatible existing ASI loader. The installer must not silently overwrite unrecognized third-party proxy loaders or assume an unknown mod stack is safe.

**Safe changes:** Close the game, back up its whole folder, inspect options and use **Check setup** after any uncertain interruption. Install/restore operations can modify game files, while uninstalling the desktop app does not revert those changes.

[Most Wanted guide](MOST-WANTED.md) · [Carbon guide](CARBON.md) · [Troubleshooting](TROUBLESHOOTING.md)
