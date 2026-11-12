# 🎛️ Features and limitations | Beta 1.6

[← Home](../README.md) · [Test evidence](WHATS-NEW-BETA-1.6.md) · [Screenshots](../screenshots/README.md)

## Music library and organization

Select local music folders, scan audio, inspect available metadata, preview/pause/seek and search. Browse categories, identify possible duplicate tracks, adjust song order or shuffle with early-repeat avoidance. The builder does **not** recognize music genres by listening to waveforms; it uses song tags and balancing, so review imperfect tags. There is **no artificial playlist track cap**.

**Game configuration → Manual assignments** offers a per-track multi-category matrix with bulk controls. Assign songs to more than one relevant driving pool if desired. **Shared** is fallback, not an extra driving state. For Carbon, Menu/Shared rules apply as described in the Carbon guide. **Save assignments** saves your choices; **Build / Save** later writes game playlists. Manual choices should not be silently replaced by automatic assignment.

## Game-specific music

| | Most Wanted (2005) | Carbon (2006) |
| --- | --- | --- |
| Categories | Safe House / menus, Free Roam, Race, Pursuit, Shared | Menu, Muscle, Tuner, Exotic, Shared |
| Skip | **T** on ordinary/custom continuous songs | Configurable **F9** |
| Original music | Native adaptive pursuit score (not T-skippable) | Canyon/Pursuit original music choices experimental |
| Custom dynamic music | Custom interactive pursuit from user's library; advanced node/segment editing experimental | Class pools confirmed earlier on 1.2; custom Canyon/Pursuit-specific buckets not implemented |
| Mixing | Independent music gain defaults to 65%; fades, finish-current-song option | Crew speech ducking and balance settings (partly experimental) |

**Most Wanted testing improved in Beta 1.6:** prologue audio, Safe House fades, Free Roam, ordinary Pursuit routing, custom pursuit tracks, T skipping, EA Trax titles and original score exit fade have live-session confirmations. They do not establish general compatibility for all mods and saves.

**Carbon testing remains limited:** earlier gameplay confirmed class music, F9 and crew ducking on 1.2. The 1.4 player passed isolated packaging/installer checks, **not** live-game acceptance. Original Canyon/Pursuit and Drift mode controls remain experimental.

## Sound and loudness

Configurable song fade-in/fade-out and complete-song state transitions are part of the Most Wanted path. The original score has its own authored timing; custom continuous song skipping is a different feature.

Optional loudness leveling uses FFmpeg to create **playback copies** at a selected target and peak ceiling. It does not overwrite your library or change the volume of car engines, police radio or other game sound effects. Native original/mapped score components preserve their authored levels.

## Install, backup and diagnose

Use **Game configuration → Installation** to check player components, review editable options, install/repair a compatible player and examine restoration actions. The Windows Setup EXE only installs the builder. **Install selected features**, **Build / Save**, and restore actions can change your game files.

The **Support** button lets you preview either Plain English or JSON diagnostics and save both formats into one local ZIP; it never submits it automatically. The report omits raw logs, paths, song names, media and game saves. Independent screenshots and manually attached logs still require privacy review.

[Installation guide](GETTING-STARTED.md) · [Backups](BACKUPS-AND-RESTORE.md) · [Detailed acceptance matrix](WHATS-NEW-BETA-1.6.md)
