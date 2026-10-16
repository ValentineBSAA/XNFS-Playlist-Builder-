# 🏁 XNFS Playlist Builder 3.2 | Beta 1.5 (experimental prerelease)

**Your music. Your drive. Your soundtrack.**

A significantly redesigned Windows music-playlist studio for **Need for Speed Most Wanted (2005)** and **Need for Speed Carbon (2006)**.

> **This is a public experimental beta, not a stable or completely gameplay-regression-tested release.** Please read the confirmed/experimental distinctions below before downloading.

## ⬇️ Download and install

**[Get XNFS Playlist Builder 3.2 Beta 1.5 for Windows](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/Beta-1.5/XNFS-Playlist-Builder-3.2-Beta-1.5-Public.zip)**

**Download:** `XNFS-Playlist-Builder-3.2-Beta-1.5-Public.zip` (about 100 MB). Extract it and run **`XNFS-Playlist-Builder-3.2-Beta-1.5-Setup.exe`**.

Requires **Windows 10/11 x64**, your own music, your own compatible copy of the game and a suitable **ASI loader** for game integration. Python is not needed. This unsigned installer may show a Windows unknown-publisher warning. **Back up your game folder and close the game before installing features.**

The public ZIP contains the installer, README, changelog, verification notes, and before/after application screenshots. GitHub's automatic **Source code** archives are documentation snapshots, **not** the Windows app or editable application code.

## ✨ What's new in Beta 1.5

- **Hybrid Performance Studio:** redesigned frameless dark interface, **Rockport Gold** Most Wanted theme, **Midnight Cyan** Carbon theme, more readable configuration and installation screens.
- **Full music library workflow:** scan remembered folders; preview/pause/seek; search, category filters and ordering; genre review and duplicate checking.
- **Manual assignments inside Game configuration:** per-song category switches, bulk tools and explicit **Save assignments**. **Build / Save** remains the separate action that writes game playlists.
- **Improved setup manager:** pre-install component/settings review, guided repair/status checks, backup warnings, errors with next steps and expandable diagnostics.
- **Optional playback-copy loudness leveling:** source music remains unchanged. Hardened cancellation/close handling.
- **Most Wanted pursuit settings:** separate original/default, custom interactive and continuous pursuit-playlist choices; experimental node mapping/segment editing and packs.
- **Carbon event configuration:** original Canyon/Pursuit mode choices and Drift playlist/original ambience/silent options. The underlying event behavior still needs in-game verification.
- **Packaging fix for Beta 1.4's missing `uuid` runtime:** dependency verified in the final compiled build and fixture installer.
- **Installation crash hardening:** persistent Qt timer ownership, queued GUI updates and safer cleanup. **Not a confirmed complete fix for every intermittent crash.**
- **Updated real-application screenshots**, new help pages and clearer user-facing status labels.

## 🟡 Most Wanted: what currently works, and the limits

**Soundtrack pools:** **Safe House** (includes menus), **Free Roam**, **Race**, **Pursuit**, plus **Shared** fallback.

**Earlier developer gameplay confirmed** state-based music, **T** skipping for ordinary/custom continuous tracks, EA Trax notifications, the original native interactive pursuit score and custom-library pursuit playback.

**Original interactive soundtrack setup:** select **Game configuration → Installation → Install original interactive music → Install selected features**, then launch the game and use the **native in-game XNFS installation/extraction flow**. The game extracts from your own game audio banks and shows percent/progress and stage ETA. **The builder does not independently extract the original score.** A valid game-audio and node baseline is required.

**Choose one original/default or custom pursuit mode at a time.** The **T** key does **not** skip the original native adaptive score or advanced mapped segments. Saved custom-song selections should survive mode changes.

**Still needs focused gameplay tests:** extended pursuits, custom authored transitions, start/exit events, playlist save/reopen, and overlap between original and custom audio. **Police-radio ducking is not implemented.** Do not treat short playback confirmation as proof of a complete new regression.

## 🔵 Carbon: what currently works, and the limits

**Soundtrack pools:** **Menu, Muscle, Tuner, Exotic**, plus **Shared**. The builder uses metadata/genre preferences, not waveform classification; automatic balancing can place a song outside its preferred genre.

**Earlier gameplay confirmed** car-class routing on Carbon 1.2, optional/configurable **F9** skipping and music lowering during crew dialogue. Do not silently re-enable ducking when a user's saved setting is OFF.

**Carbon 1.2 and 1.4 installation payloads** passed isolated checks. **Carbon 1.4 has not received a complete live-game verification.** Crew/speech balance remains experimental.

**Experimental event controls:** original Canyon and Pursuit scores; Drift playlist, original ambience or silence. Actual event transitions need gameplay tests. **There are no independent custom Canyon/Pursuit track buckets yet**: existing custom modes use car-class pools.

**Known issue:** an intermittent crash near **Load Complete** remains unresolved. Its root cause is not proven to be the playlist plugin.

## 🧪 What was actually tested?

**Automated / isolated checks, not gameplay:**
- Final compiled executable: five 178-track library scans/profile switches.
- Ten installer/UI fixture cycles across Most Wanted and Carbon; backups, dialogs and installer worker paths exercised against disposable folders.
- Configuration, playlist output, manual assignment, save/reload, mode combinations and restore/rollback fixtures.
- 30 rapid normalization cancel/close cycles with no remaining workers; 150 animated review cycles.
- UI checks across 1280×720 to 2560×1440 and 100–200% scaling.
- Compiled packaging inspection confirms the missing `uuid` module is included.

**Not completed:** comprehensive new in-game regressions for either game; fresh extraction/reinstall/original restoration that includes all native-generated media; Carbon Load Complete crash reproduction and root-cause fix; full custom pursuit overlap/transition listening; live Carbon 1.4 and event-mode verification.

## 🛡️ Install and restoration safety

Installing the Windows app **does not itself modify game files**. **Install selected features** and **Build / Save** can. Read replacement prompts and preserve original game files and tracked backups.

**Restore backup** recovers a compatible saved player setup; **Restore original game** aims to undo tracked changes. Neither is guaranteed when the baseline is missing or files were edited externally. Original soundtrack files generated later by the native in-game installer require additional end-to-end restore testing.

If the application closes while installing, **reopen → Game configuration → Installation → Check setup** before reinstalling. **Open troubleshooting logs** and include a *redacted* log in a bug report when possible.

## 🔗 Guide and help

[First-time installation](docs/GETTING-STARTED.md) · [Most Wanted](docs/MOST-WANTED.md) · [Carbon](docs/CARBON.md) · [Beta 1.5 full status](docs/WHATS-NEW-BETA-1.5.md) · [Screenshots](screenshots/README.md) · [Known issues](docs/TROUBLESHOOTING.md) · [Report a bug](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose)

**The historical Beta 1.4 notice remains true for Beta 1.4:** its advertised complete interactive pursuit feature was not actually implemented. **Beta 1.5 is a different experimental build** with new implementation and additional outstanding verification. We will not retroactively label Beta 1.4 as working.

---

Created by **valentine**. Original XNFSMusicPlayer and native in-game soundtrack installer work by **Lovro Pleše (xan1242)**. Independent fan tool, not affiliated with Electronic Arts. Commercial game/audio assets are not included.
