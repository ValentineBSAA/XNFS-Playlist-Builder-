<div align="center">

# 🏁 XNFS Playlist Builder
### Your music. Your drive. Your soundtrack.

**Personal soundtrack studio for Need for Speed: Most Wanted (2005) and Carbon (2006)**

**Windows 10 / 11 x64 · 3.2 Beta 1.7 · Public beta / prerelease**

[**⬇️ DOWNLOAD FROM RELEASES**](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases) · [**Getting started**](docs/GETTING-STARTED.md) · [**Test record**](docs/WHATS-NEW-BETA-1.7.md) · [**Screenshots**](screenshots/README.md)

</div>

> [!IMPORTANT]
> **Beta 1.7 is published.** Developer **valentine** subsequently confirmed successful hands-on use of Beta 1.7 on a **Windows 11 PC running Most Wanted (2005) Black Edition 1.3** (November 13, 2026). Every feature exercised in that session worked as expected. Earlier 45-song category tests are documented separately; other executables, Carbon modes and independent user environments have not received equivalent confirmation. Read the [PC validation record](docs/PC-VALIDATION-BETA-1.7.md) and [full test matrix](docs/WHATS-NEW-BETA-1.7.md).

## Build the soundtrack you want

Select your own music folders, scan and preview songs, organize tracks by game state or car class, choose manual assignments, and deploy the game-side player where compatible. The app provides guided installation, status checks, recovery options and local diagnostic export. **No Python installation is required.**

| **🟡 Most Wanted: Rockport Gold** | **🔵 Carbon: Midnight Cyan** |
| :---: | :---: |
| [![Most Wanted studio from the unchanged Beta 1.5 gallery](screenshots/beta-1.5/most-wanted/01-library.png)](screenshots/beta-1.5/most-wanted/01-library.png) | [![Carbon studio from the unchanged Beta 1.5 gallery](screenshots/beta-1.5/carbon/01-library.png)](screenshots/beta-1.5/carbon/01-library.png) |
| [Most Wanted guide](docs/MOST-WANTED.md) | [Carbon guide](docs/CARBON.md) |

*The existing Beta 1.5 screenshot gallery remains representative. Beta 1.7 does not require new screenshots.*

## ✨ What's new in Beta 1.7

- **Live audio-preparation progress:** per-song analysis / leveling percentage, completed-song count, installation stages and ETA when enough timing data is available.
- **Clear finish:** installation completion summary closes with **OK**, returning to the main workspace.
- **Windows polish:** embedded application icon, consistent taskbar identity and shortcut artwork.
- **Installation reliability:** avoids duplicate reads of the same custom pursuit audio, checks generated files and reports restore / cleanup / player-install phases after the final song. Versioned runtime dependency layout addresses a previously reproduced Shiboken DLL upgrade failure.
- **Developer gameplay confirmation:** **45 custom interactive Pursuit tracks**, **45 Safe House tracks** and **45 Free Roam tracks** played successfully in the reported test sessions. The custom pursuit run included a manually added song; on-screen preparation progress completed.
- **Existing audio controls preserved:** selectable Most Wanted fades, finish-current-song switching, **T** skipping for ordinary/custom songs and EA Trax titles; optional loudness leveling creates playback copies without editing originals.

## 🎮 Games and soundtrack routing

| | **Most Wanted (2005)** | **Carbon (2006)** |
| --- | --- | --- |
| Categories | Safe House (also frontend menus), Free Roam, Race, Pursuit, Shared | Menu, Muscle, Tuner, Exotic, Shared |
| Music switches | Driving state; optional finish-current-song; selected pursuit mode | Menu and car class |
| Skip control | **T** skips ordinary/custom continuous tracks, **not** the original adaptive score | Optional/configurable **F9** |
| Special audio | Original adaptive pursuit score or custom interactive library music; EA Trax titles | Optional crew-speech ducking; experimental original Canyon/Pursuit and Drift choices |
| Important limits | Some custom fade boundaries, save-switch first track and modified-EXE gameplay still need targeted tests | **No independent custom Canyon/Pursuit buckets**; Carbon 1.4 and event playback not yet game-verified |

### 🎚️ Developer-verified engine-volume setting

**Car engine volume must be adjusted manually in the game's own Audio options.** The builder's independent music volume does not control the car engine sound level. Developer **valentine** verified this during gameplay testing. In **Most Wanted**, use the **Car Volume** setting in the game's Audio options to balance the engine against the soundtrack; treat the builder's **65% music mix** as a starting point, not a universal preset. **This is an expected manual adjustment, not a failed feature or an outstanding test.**

[Complete audio guidance](docs/MOST-WANTED.md) · [Testing evidence](docs/WHATS-NEW-BETA-1.7.md).

## 🚀 Installation

1. When published, download **`XNFS-Playlist-Builder-3.2-Beta-1.7-Public.zip`** from [GitHub Releases](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases). Do not use GitHub's automatic Source code ZIP.
2. Extract it and run **`XNFS-Playlist-Builder-3.2-Beta-1.7-Setup.exe`** on Windows 10/11 x64. The installer is unsigned.
3. Select **Most Wanted** or **Carbon**, identify your game folder and own music library, scan and edit assignments.
4. **Close the game**, check setup under **Game configuration → Installation**, review the options and install selected features. An existing compatible **ASI loader** is required.
5. After installation, review the completion summary and select **OK** to return to the workspace. Use **Build / Save**, then launch your game.

**Back up the complete game folder first.** Desktop Setup alone does not alter the game, but the player's install and playlist build operations can. Uninstalling the desktop app does not undo game-side changes.

[Detailed start guide](docs/GETTING-STARTED.md) · [Backup and restore](docs/BACKUPS-AND-RESTORE.md).

## 🧪 Verified, limited and unresolved

**Most Wanted, reported actual gameplay:** 45 custom interactive Pursuit, 45 Safe House and 45 Free Roam tracks; earlier acceptance of prologue audio, T skip, EA Trax titles, state-based song routing and original-score exit fade. **New November 13 hardware verification:** all features exercised in Beta 1.7 on **Windows 11 + Most Wanted Black Edition 1.3 (PC)** worked correctly, according to the developer. The original-score fade can feel slow.

**Automated / packaged checks:** clean Windows setup and upgrade repair evidence, 10 completion-review-and-return cycles, underlying installer/backup fixtures and checks on both packaged game profiles. The **original Developer ZIP** recorded no gameplay on the final packaged EXE **at handoff**. The developer later verified Beta 1.7 in real PC gameplay; an exact hash proving that the later-tested EXE matches the published installer was not provided. See the [dated validation record](docs/PC-VALIDATION-BETA-1.7.md).

**Still unverified / unresolved outside the new PC confirmation:** Carbon 1.4 gameplay and Canyon/Pursuit/Drift playback; separate custom Carbon Canyon/Pursuit pools (not implemented); PLAK gameplay; independently isolated tests of every save-switch or custom fade boundary; the intermittent Carbon Load Complete crash; and a rendering issue on a heavily modded Most Wanted installation. These are **scope limits**, not problems observed in the developer's latest Black Edition 1.3 test.

[See the detailed Beta 1.7 test matrix](docs/WHATS-NEW-BETA-1.7.md).

## 📚 Support, verification and credits

Use **Support** in the app to preview Plain English or JSON diagnostics and export a local ZIP containing both files. Nothing is uploaded automatically. Review manually added screenshots and logs for private data.

[Report a problem](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose) · [Join discussions](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/discussions) · [Help center](docs/README.md) · [SHA-256](docs/SHA256-OF-BETA-1.7.txt) · [Licenses and credits](docs/LICENSING-AND-CREDITS.md) · [Release notes](RELEASE_NOTES.md).

> [!NOTE]
> GitHub's automatic **Source code (zip/tar.gz)** archives contain the public documentation and screenshot repository, **not the Windows installer or editable builder source**. The Developer ZIP remains separate from the Public ZIP.

---

<div align="center">

Developed by **valentine**. Original **XNFSMusicPlayer** and native in-game soundtrack installer by **Lovro Pleše (xan1242)**.

<sub>Independent fan-made utility, not affiliated with or endorsed by Electronic Arts. Does not distribute commercial game or music assets.</sub>

</div>
