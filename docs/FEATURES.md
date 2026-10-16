# 🎛️ Features: plain-English guide to Beta 1.5

[← Home](../README.md) · [New screens](../screenshots/README.md) · [Testing matrix](WHATS-NEW-BETA-1.5.md)

## Build a soundtrack from your music

**Scan songs** in a folder and view track name, artist, length and available genre information. The builder remembers folders. The **final compiled build** completed five real-library scans/profile switches with **178 tracks** during automated/isolated acceptance.

**Preview songs**, pause/stop/seek, filter by category, search, inspect possible duplicate tracks and choose playback ordering. Preview playback is separate from in-game playback.

**Auto assignment** uses song metadata and balancing, not waveform-based genre recognition. It may place songs outside ideal genre categories. Songs without reliable genre tags deserve a manual review. There is **no artificial per-playlist song cap**.

**Manual assignment** is under **Game configuration → Manual assignments**. Assign a track to more than one driving pool when helpful; **Shared** is a fallback, not an extra music state. Carbon Menu and Shared are exclusive choices. **Save assignments** saves the manual matrix; **Build / Save** separately writes playlists for your game. Manual edits disable auto-assignment until you choose to turn it back on.

## Music in game

| | Most Wanted | Carbon |
| --- | --- | --- |
| Music groups | Safe House (menus too), Free Roam, Race, Pursuit, Shared | Menu, Muscle, Tuner, Exotic, Shared |
| Skip control | **T** for custom/continuous tracks; not native adaptive score | Configurable optional **F9** |
| Special music | Original/default native score or custom pursuit; experimental advanced mapping | Car-class routing; optional crew-dialogue ducking |
| Experimental | Custom pursuit transitions and node mapping require extensive listening tests | Original Canyon/Pursuit and Drift modes require event testing; no separate custom Canyon/Pursuit buckets |

**Shuffle** can reduce early repeats until a pool is exhausted. Songs in multiple pools may be heard in multiple contexts.

**EA Trax notifications** exist for Most Wanted and have earlier user confirmation, but historical late-notification issues have not been comprehensively retested.

## Audio leveling and mixing

Optional loudness leveling prepares **separate playback copies**; originals are preserved. It may take time and disk space. It does not magically lower engines, police-radio voices or other sound effects.

Carbon's music ducking during crew speech was confirmed in earlier gameplay. Crew/speech balance sliders remain experimental; **do not silently turn ducking back ON** when the saved setting is OFF.

## Install, restore and diagnose

**Install selected features** makes the game-file changes requested in Game configuration; **Build / Save** writes playlists. The redesigned installation screen shows status, available setup/repair actions, component review, replacement warnings, expandable errors and **Open troubleshooting logs**.

**Restore backup** returns to a tracked saved player/playlist setup. **Restore original game** attempts to recover the recorded original baseline; both require valid records. Native-generated original soundtrack files need more complete restoration testing. See [backup warnings](BACKUPS-AND-RESTORE.md).

**Important:** successful file checks, configuration tests, and fixture installations are **not** proof of real gameplay. [See exactly what is and isn't tested](WHATS-NEW-BETA-1.5.md).
