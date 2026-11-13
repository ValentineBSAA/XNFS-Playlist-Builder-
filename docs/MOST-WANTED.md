# 🟡 Most Wanted (2005): Rockport Gold

[← Home](../README.md) · [Setup guide](GETTING-STARTED.md) · [Beta 1.7 evidence](WHATS-NEW-BETA-1.7.md)

![Most Wanted library, existing Beta 1.5 screenshot](../screenshots/beta-1.5/most-wanted/01-library.png)

## The music categories

| Pool | Used for |
| --- | --- |
| **Safe House** | Safe House and frontend menus |
| **Free Roam** | Driving in Rockport |
| **Race** | Races |
| **Pursuit** | Police chases with ordinary music mode |
| **Shared** | Fallback |

You can add your own songs, use metadata-assisted suggestions, or manually assign tracks to one or more categories. Beta 1.7 **developer-reported gameplay passed 45 tracks in Safe House and 45 tracks in Free Roam**.

## Pursuit soundtrack modes

Under **Game configuration → Pursuit music**, choose only **one** active mode:

1. **Ordinary Pursuit playlist:** full songs from the Pursuit pool, with optional finish-current-song state transition and configurable fades.
2. **Original adaptive pursuit score:** deploy the native original installer and launch the game. The score is extracted from your own game audio by the **native in-game installer**, not by the Windows builder. **T cannot skip original adaptive nodes**.
3. **Custom interactive pursuit:** select songs from your library, with **T** skipping on supported continuous tracks. EA Trax displays custom song titles. Optional advanced node mapping remains experimental.

![Most Wanted pursuit configuration, retained Beta 1.5 screenshot](../screenshots/beta-1.5/most-wanted/11-custom-pursuit.png)

**Beta 1.7 gameplay:** the developer reported successful playback of **45 custom Pursuit songs**, including a manually added selection. They also observed live preparation percentage and successful completion of custom-song installation. Prior sessions had separately confirmed three custom interactive songs, 39 logged node requests, T skip and EA Trax titles.

## Sound balance, fades and car engine volume

The builder's independent **Music** setting defaults to **65%**; adjust it to your setup. Configurable fades and finish-current-song switching reduce sudden transitions. Earlier listening confirmed Safe House fades and the **original-score** Pursuit → Free Roam fade. That exit handoff works in the tested session but can feel slow.

> [!IMPORTANT]
> **Developer-verified sound requirement:** **car engine volume must be adjusted manually inside Most Wanted using Audio options → Car Volume.** The XNFS builder's music volume does **not** automatically change engine sound. Developer **valentine** confirmed this in gameplay. Treat the manual setting as normal configuration, **not a pending feature or test**.

Optional loudness leveling processes **copies** of your own music at the desired loudness target and peak ceiling. It does not change engine, police radio or game speech levels.

## Tests that are still limited

- The latest **custom-interactive pursuit exit fade** was not separately accepted after the final revision.
- An incoming fade at **every** natural custom-song boundary has not been game-tested.
- The first soundtrack pool after switching save files needs complete live-game acceptance.
- A modified `speed.exe` may match all **61 music-hook signatures**; **PLAK gameplay is not proven**.
- An intermittent car-body rendering problem on a heavily modified installation has no proven cause or XNFS attribution.
- **Police-radio ducking is not implemented**. Original-score extraction/media restoration is not guaranteed in every external-mod situation.

**The Beta 1.7 test handoff does not claim in-game testing of the final packaged EXE**, even though earlier and current Most Wanted gameplay scenarios were reported passed.

[Full verified matrix](WHATS-NEW-BETA-1.7.md) · [Compatibility](GAMES-AND-COMPATIBILITY.md) · [Troubleshooting](TROUBLESHOOTING.md) · [Historical Beta 1.4 disclosure](WHATS-NEW-BETA-1.4.md)
