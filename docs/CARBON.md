# 🔵 Carbon (2006): Midnight Cyan

**Music for each car class, built from your own songs.** XNFS Playlist Builder 3.2 Beta 1.5.

[← Home](../README.md) · [Install](GETTING-STARTED.md) · [All photos](../screenshots/README.md)

[![Carbon Beta 1.5 music library](../screenshots/beta-1.5/carbon/01-library.png)](../screenshots/beta-1.5/carbon/01-library.png)

## The Carbon playlists

| Category | Where it plays | Genre *suggestions* |
| --- | --- | --- |
| **Menu** | Game menus | Any |
| **Muscle** | Muscle cars | Rock / Alternative |
| **Tuner** | Tuner cars | Pop / Electronic |
| **Exotic** | Exotic cars | Hip-hop / Rap / Grime |
| **Shared** | Fallback | Any |

The builder looks at metadata and balances tracks. This is **not waveform genre recognition**, and songs with missing/odd tags may go into unexpected categories. Use **Manual assignments** to choose exactly what you want. There is no artificial track-count cap.

## Playback extras

**Previously confirmed in Carbon 1.2 gameplay:**
- Music can follow the current car class.
- **F9**, when enabled/configured, skips tracks.
- Music can automatically duck while crew members speak and return afterward.

Ducking is **optional** and preserves your existing OFF setting. **Crew/speech balance is experimental**; the developer has still reported loud crew or car sounds. Music loudness leveling affects **playback copies**, not engine or voice effects.

## Canyon, pursuits and Drift: experimental

![Carbon Beta 1.5 event configuration](../screenshots/beta-1.5/carbon/18-event-music.png)

The new **Event music** page can configure original **Canyon** and **Pursuit** scoring separately; Drift can use car-class playlists, original ambience or silence. Configuration/installer combinations passed isolated tests, **not real Canyon/Pursuit/Drift gameplay**.

**Separate custom Canyon/Pursuit event song buckets have not been implemented.** When selecting custom event modes, the current runtime still uses the car-class music pools. Do not expect independent per-event custom playlists. Original scores depend on your own game audio banks; Carbon extraction remains experimental and separate from Most Wanted's in-game original soundtrack installer.

## Game version and crash notes

The installer carries matched **Carbon 1.2 and Carbon 1.4** payloads. Both passed isolated setup checks, but developer gameplay primarily used **1.2**. **Carbon 1.4 is not yet fully verified in-game**.

An **intermittent crash around “Load Complete”** remains **unresolved**. It has **not** been proven to originate in the playlist plugin. The separate Windows builder **installer-dialog animation crash** was hardened, not conclusively eliminated.

## Beta 1.5 screenshots

| Choose features | Assign songs manually |
| :---: | :---: |
| [![Carbon feature setup](../screenshots/beta-1.5/carbon/04-features.png)](../screenshots/beta-1.5/carbon/04-features.png) | [![Carbon manual assignments](../screenshots/beta-1.5/carbon/17-manual-assignments.png)](../screenshots/beta-1.5/carbon/17-manual-assignments.png) |
| [Audio / crew](../screenshots/beta-1.5/carbon/05-audio.png) | [Install / repair player](../screenshots/beta-1.5/carbon/05-installation.png) |

[Testing and limits](WHATS-NEW-BETA-1.5.md) · [Compatibility](GAMES-AND-COMPATIBILITY.md) · [Troubleshooting](TROUBLESHOOTING.md)
