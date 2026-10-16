# 🧪 Beta 1.5: what's new, what works and what still needs testing

**XNFS Playlist Builder 3.2 Beta 1.5 is an experimental public prerelease.** This page distinguishes a feature that exists from one verified in the latest game build.

[← Home](../README.md) · [Download Beta 1.5](../RELEASE_NOTES.md) · [Report a problem](../.github/ISSUE_TEMPLATE/bug_report.yml)

## The 1.5 redesign

- **Hybrid Performance Studio:** dark, frameless interface; **Rockport Gold** for Most Wanted, **Midnight Cyan** for Carbon; larger and more readable dialogs.
- **178-track real-library test:** compiled builder successfully scanned and switched the developer's music collection five times, with preferences copied for isolated testing.
- **Preview, search and playlists:** playback/seek/stop, category filters and order; duplicate/genre review; balanced automatic assignments.
- **Manual assignment matrix in Game configuration:** category switches per song, batch actions and explicit **Save assignments**, followed by **Build / Save** for actual export. Saving manual edits protects them by switching auto assignment OFF.
- **Install/setup manager:** selected player/components and options review; repair/status checks; replacement warnings; backup and restore choices; red errors with next-step guidance and expandable logs.
- **MW pursuit controls:** original/default and custom modes, library song selector and optional experimental mapped node editing.
- **Carbon event controls:** original Canyon/Pursuit and Drift playlist/ambience/silent configuration; actual event behavior awaits gameplay testing.
- **Runtime packaging:** compiled Windows installer includes the previously missing `uuid` dependency.
- **Crash hardening:** safer Qt timer ownership, queued worker results, dialog disposal, cancellation and persistent diagnostics. This reduces known risk, but does not prove all crashes have disappeared.

## What does each status mean?

| Label | Meaning |
| --- | --- |
| ✅ Automated pass | Logic, UI, compiled binary or isolated fixture checked. **Not** game testing |
| 🎮 Previously confirmed in game | Developer heard/saw the feature work in an earlier real gameplay session; **latest complete regression still pending** |
| 🧪 Implemented; gameplay pending | Control/configuration exists and passed isolated checks; event behavior unverified |
| ⚗️ Experimental | Optional complex feature with meaningful remaining limitations |
| 🚧 Unfinished | Do not advertise as working |
| ⚠️ Unresolved | Known issue without a confirmed full repair |

## 🟡 Most Wanted 2005

| Feature | Status | Important qualification |
| --- | --- | --- |
| Safe House (includes menus), Free Roam, Race, Pursuit and Shared pools | 🎮 Previously confirmed | Latest four-state full game retest pending |
| T-key custom/continuous song skipping | 🎮 Previously confirmed | Does not skip native original adaptive score or advanced mapped segments |
| Shuffle and multi-category playlist export | ✅ Automated pass | Small song pools repeat after exhaustion |
| Original native adaptive pursuit soundtrack | 🎮 Previously confirmed | Uses valid game's original banks/nodes and in-game extraction |
| Native install option and in-game progress/ETA | 🎮 Previously confirmed | Builder deploys/arms native ASI; **game** performs extraction |
| Custom pursuit with songs from selected library | 🎮 Previously confirmed | Long transitions, exit state and default/custom audio overlap need listening tests |
| Optional mapped segments/nodes, pack import/export | ⚗️ Experimental | Automated import/export and timing tests, not musical transition acceptance |
| Original/default vs. custom mode selection | ✅ Automated pass | Modes are exclusive and saving should not silently change modes |
| EA Trax notification support | 🎮 Previously confirmed | Historical late-notification behavior not fully resolved |
| Police-radio ducking | 🚧 Not implemented | Future possibility, not a Beta 1.5 feature |

**Beta 1.4 historical clarification:** Its public installer **did not contain the fully implemented interactive pursuit system** that had been advertised. This record remains in [the Beta 1.4 archive](WHATS-NEW-BETA-1.4.md). Beta 1.5 has further implementation and earlier gameplay confirmations, but has not passed a full new end-to-end pursuit regression. Do not merge the two status statements.

## 🔵 Carbon 2006

| Feature | Status | Important qualification |
| --- | --- | --- |
| Menu, Muscle, Tuner, Exotic and Shared music | 🎮 Previously confirmed | Earlier developer gameplay, primarily Carbon 1.2 |
| Configurable F9 skip | 🎮 Previously confirmed | Respects saved key and enabled state |
| Optional music ducking during crew speech | 🎮 Previously confirmed | Saved OFF means OFF; no silent re-enabling |
| Crew/speech balance | ⚗️ Experimental | Effects/crew balance not fully solved |
| Carbon 1.2 and 1.4 payload installation | ✅ Automated pass | 1.4 full live-game compatibility not established |
| Original Canyon/Pursuit events | 🧪 Implemented; gameplay pending | File/configuration tests are not proof of game events |
| Drift playlist / original ambience / silence | 🧪 Implemented; gameplay pending | No separate verified custom Drift bucket |
| Separate custom Canyon/Pursuit playlists | 🚧 Not implemented | Existing custom modes use car-class pools |
| Intermittent crash near **Load Complete** | ⚠️ Unresolved | Root cause is not established as player/plugin fault |

Genre preferences are **Muscle → Rock/Alternative**, **Tuner → Pop/Electronic**, **Exotic → Hip-hop/Rap/Grime**. These are suggestions, not genre recognition from the audio and not rules for manual assignment.

## Automated evidence from the final compiled build

- **Five** full 178-track scans/profile-switch cycles.
- **Ten** real UI/installer fixture install cycles with disposable Most Wanted and Carbon folders.
- **Thirty** immediate normalization cancel/close cycles, with no workers left running.
- **150** animated installation-review cycles.
- UI regression at **1280×720, 1366×768, 1920×1080 and 2560×1440**, including **100%, 125%, 150% and 200%** Qt scaling.
- Manual assignment, mode selections, playlist save/reopen, original-file tracking and rollback tests.
- Exact compiled installation/PyInstaller dependency tests show **`uuid`** packaged.

**No real installed game files were modified by these redesign/fixture checks.** The full 178-song scan proves the builder can load that collection, not that each song works in every game state.

## Still required before calling it stable

- [ ] Play through *every* latest-build Most Wanted music state and both pursuit pathways.
- [ ] Listen for dual original/custom audio, sudden volume jumps, transition glitches and return-to-menu behavior.
- [ ] Verify Carbon Canyon, Canyon Duel, Pursuit, Drift and exit transitions in supported actual game versions.
- [ ] Reproduce and root-cause the Carbon Load Complete crash.
- [ ] Test new installs, reinstalls and complete original restoration including media created by native extraction.
- [ ] Validate Carbon 1.4 against real gameplay and external mod combinations.

**Installer UI failure vs. Carbon game loading failure are separate problems.** The former was hardened after Windows identified a Qt animation-stack issue, but the exact intermittent original failure could not be reproduced reliably. The latter is still unresolved and has no confirmed plugin root cause.

## Help us test it

Use the [bug report form](../.github/ISSUE_TEMPLATE/bug_report.yml). Mention the **Beta 1.5 version**, game executable version, Windows version and scaling, selected options/pursuit modes, steps to reproduce, expected/actual result, and a screenshot or log when possible. **Remove usernames, full local paths and song metadata before posting.**

[See installation help](GETTING-STARTED.md) · [Backups and original restore](BACKUPS-AND-RESTORE.md) · [Common questions](TROUBLESHOOTING.md)
