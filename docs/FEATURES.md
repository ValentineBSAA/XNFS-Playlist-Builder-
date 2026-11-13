# 🎛️ Features | XNFS Playlist Builder 3.2 Beta 1.7

[← Home](../README.md) · [Test evidence](WHATS-NEW-BETA-1.7.md) · [Existing screenshots](../screenshots/README.md)

## Build playlists from your own library

Scan local music, preview/pause/seek, inspect artist and genre metadata, search and filter tracks, review duplicates, and choose playback ordering and shuffle. The automatic category suggestions use **tags and balancing**, not audio waveform classification. There is **no artificial per-playlist track cap**.

**Game configuration → Manual assignments** offers per-song multi-category choices and bulk controls. **Save assignments** records the choices, while **Build / Save** writes the game playlists. **Shared** is fallback, not another driving state.

## Live gameplay music

| Feature | Most Wanted | Carbon |
| --- | --- | --- |
| Main pools | Safe House (includes menus), Free Roam, Race, Pursuit, Shared | Menu, Muscle, Tuner, Exotic, Shared |
| State switching | Driving state, configurable fades and optional finish-current-song | Class and menu |
| Skipping | **T** for ordinary/custom continuous songs | Configurable **F9** |
| Interactive / event audio | Native original adaptive pursuit or custom interactive library songs | Experimental original Canyon/Pursuit/Drift modes |
| Notifications / voices | EA Trax titles; no automatic police radio ducking | Optional crew-dialogue ducking and balance controls |

**Most Wanted gameplay:** developer-reported **45-track passes** in custom Pursuit, Safe House and Free Roam during Beta 1.7 testing. Earlier sessions confirmed scripted prologue audio, T skipping, EA Trax names and the revised original-score exit fade. See the [detailed table](WHATS-NEW-BETA-1.7.md) for the specific distinction between earlier and newer tests.

**Carbon:** previous 1.2 gameplay passed class routing, F9 and ducking. The inspected 1.4 player package passed isolated checks, not full live gameplay. **Separate custom Canyon/Pursuit track buckets are not implemented**.

## 🎚️ Music gain, engine audio and loudness leveling

**Developer valentine verified:** for Most Wanted, **car engine volume is adjusted manually through the game's Audio options → Car Volume**. The builder's Music volume controls music independently; it does not set the engine volume. The **65% music default** is a starting point; manual game-audio balancing is expected and is **not an unfinished feature**.

Adjustable music fades and the option to finish a song before switching pools help avoid abrupt transitions. Optional loudness leveling accepts a target and peak ceiling and prepares **copies** of your music. Original files remain unchanged. Native original/mapped score components retain their authored gain.

## Installation and progress in Beta 1.7

The builder's installation manager checks the game folder, reports installed features, allows review/repair/restore and displays validation diagnostics. Beta 1.7 adds **live per-song leveling/analysis percentage**, a completed-item counter, installation stages and ETA after sufficient timing data. Post-audio restore, cleanup and player-install tasks appear instead of leaving progress apparently stuck at the final song.

The **OK** button on completion returns to the main workspace; **10 packaged UI cycles** reportedly passed. A compatible existing ASI loader is required for game integration; installation of the builder by itself does not change your game.

The **Support** button can preview Plain English or JSON and export both in one local ZIP. It never uploads reports automatically; review any additional screenshots/raw logs before sharing.

[Getting started](GETTING-STARTED.md) · [Restoring files](BACKUPS-AND-RESTORE.md) · [All evidence and limits](WHATS-NEW-BETA-1.7.md)
