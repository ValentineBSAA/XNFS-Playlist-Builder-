<div align="center">

# 🏁 XNFS Playlist Builder
### Your music. Your drive. Your soundtrack.

**A personal soundtrack studio for Need for Speed: Most Wanted (2005) and Carbon (2006)**

**Windows 10 / 11 (64-bit) · Version 3.2 · Beta 1.5 · Experimental prerelease**

[**⬇️ DOWNLOAD BETA 1.5 FOR WINDOWS**](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/Beta-1.5/XNFS-Playlist-Builder-3.2-Beta-1.5-Public.zip)

[**Quick start**](docs/GETTING-STARTED.md) · [**New screenshots**](screenshots/README.md) · [**Release notes**](RELEASE_NOTES.md) · [**Help**](docs/TROUBLESHOOTING.md)

</div>

---

> [!IMPORTANT]
> **Beta 1.5 is public, but is NOT a fully gameplay-verified stable release.** Earlier sessions confirmed important Most Wanted and Carbon features. Automated checks passed on the new build, but a full in-game retest after the redesign remains outstanding. Read [what is tested and what still needs work](docs/WHATS-NEW-BETA-1.5.md).

## Meet your music studio

Choose a folder of your own songs, scan your library, build playlists for the game you play, and optionally install the compatible in-game player features. **No coding or Python installation is needed.** The refreshed **Hybrid Performance Studio** has a frameless dark interface, **Rockport Gold** for Most Wanted and **Midnight Cyan** for Carbon.

| **🟡 Most Wanted: Rockport Gold** | **🔵 Carbon: Midnight Cyan** |
| :---: | :---: |
| [![Most Wanted Beta 1.5 music library](screenshots/beta-1.5/most-wanted/01-library.png)](screenshots/beta-1.5/most-wanted/01-library.png) | [![Carbon Beta 1.5 music library](screenshots/beta-1.5/carbon/01-library.png)](screenshots/beta-1.5/carbon/01-library.png) |
| [Most Wanted details](docs/MOST-WANTED.md) | [Carbon details](docs/CARBON.md) |

**See the [complete Beta 1.5 screenshot gallery](screenshots/README.md)** for library, configuration, player installation, manual assignments, audio, restoration and experimental editing screens.

## 🎵 What can I do?

- **Scan your own music:** remember folders, search songs, preview playback and seek, find possible duplicates and review metadata.
- **Organize soundtracks:** genre-assisted automatic distribution or precise manual per-track assignments, including multiple driving categories. There is **no artificial playlist track cap**.
- **Choose the playback order:** inspect category membership and optional shuffle with early-repeat avoidance.
- **Make music loudness more consistent:** optionally level *separate playback copies*. Original audio files stay untouched.
- **Set up and recover:** review selected components before installing; examine status, troubleshooting logs, backup and original-restore choices.
- **Customize per game:** each game remembers its own settings and uses its own configuration tools.

Automatic genre placement is an aid, not magic: it uses metadata and balancing, not audio waveform recognition. Review songs without accurate tags.

## 🎮 Pick your game

| | **Most Wanted (2005)** | **Carbon (2006)** |
| --- | --- | --- |
| **Soundtrack categories** | Safe House, Free Roam, Race, Pursuit, Shared | Menu, Muscle, Tuner, Exotic, Shared |
| **How music changes** | Driving state and selected pursuit mode | Car class and menu |
| **Skip button** | **T** for continuous/custom tracks while driving | Optional/configurable **F9** |
| **Extras** | Original/default or custom pursuit options, EA Trax notifications | Optional crew-speech ducking, crew balance controls, experimental event modes |
| **Important limit** | Original adaptive score is **not T-skippable**; custom pursuit transitions/overlap need focused retesting | Separate custom Canyon/Pursuit buckets are **not implemented**; event behavior needs live testing |

**Most Wanted:** The **Safe House** pool also covers frontend menus. The game supports distinct pursuit-mode configuration. Earlier user gameplay confirmed original interactive pursuit playback and custom pursuit music. This is **not** a claim that all Beta 1.5 pursuit transitions, authored segments or overlap behavior have passed a complete new regression. [Learn about Most Wanted](docs/MOST-WANTED.md).

**Carbon:** Car-class playlists, optional F9 skipping and crew-dialogue ducking were confirmed in earlier gameplay, primarily on **Carbon 1.2**. A Carbon 1.4 player payload exists and passed isolated tests, but has **not** been fully live verified. Canyon/Pursuit original-score options and Drift choices need real-event testing. [Learn about Carbon](docs/CARBON.md).

## 🚀 First-time setup (five steps)

1. **[Download the public Beta 1.5 ZIP](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/Beta-1.5/XNFS-Playlist-Builder-3.2-Beta-1.5-Public.zip)** and use Windows **Extract All**.
2. Run **`XNFS-Playlist-Builder-3.2-Beta-1.5-Setup.exe`**. The app installer is unsigned; confirm you are using this repository's release.
3. Select **Most Wanted** or **Carbon**, then choose the game folder and your music folder.
4. **Scan** your songs, review the playlists, and choose any player components under **Game configuration → Installation**. **Close the game before making game-file changes.**
5. Review the feature-installation prompts and use **Build / Save** to write the playlists. Launch the game and test.

You need your **own legally obtained game and music**. In-game player integration requires a supported game executable and a **compatible existing ASI loader**. The setup manager guides checks, but does not silently overwrite an unknown third-party loader. Back up your game folder first.

**[Full illustrated beginner guide →](docs/GETTING-STARTED.md)**

## 🧪 Beta 1.5: know before you install

| **Status** | **What it means** |
| --- | --- |
| ✅ Automated checks | Compiled app, 178-track scans, playlist/configuration logic, UI, installer fixtures, cancellation and logging were exercised |
| 🎮 Earlier gameplay confirmation | Most Wanted driving pools, T skipping, native original score and custom pursuit; Carbon 1.2 car classes, F9 and optional speech ducking |
| 🧪 Needs fresh gameplay | Full Beta 1.5 MW pursuit transitions/overlap, Carbon original event modes, Carbon 1.4 |
| ⚠️ Known unresolved | Intermittent Carbon **Load Complete** crash; native installer UI crash was hardened but not proven eliminated; some original-media restoration edge cases |
| 🚧 Not implemented | Separate custom Carbon Canyon/Pursuit event buckets; Most Wanted police-radio ducking |

**A successfully installed file is not proof of successful in-game playback.** All known limitations and tests are documented in [Beta 1.5 status](docs/WHATS-NEW-BETA-1.5.md) and [release notes](RELEASE_NOTES.md). The old [Beta 1.4 pursuit disclosure](docs/WHATS-NEW-BETA-1.4.md) is retained as historical documentation, not the status of this new build.

## 🛡️ Backups, crashes and support

Before installing game features, **make your own copy of the game folder**. **Restore backup** attempts to return to a saved setup; **Restore original game** attempts to undo tracked changes. Either requires complete, valid backup records. Full restoration of media created later by the native in-game extractor still needs an end-to-end test. Uninstalling the Windows app does not automatically restore the game.

If the builder closes unexpectedly, reopen it, go to **Game configuration → Installation → Check setup**, then use **Open troubleshooting logs**. Review logs for private paths and song names before sharing.

**[Report a bug](.github/ISSUE_TEMPLATE/bug_report.yml)** · [Open an issue](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose) · [Ask the community](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/discussions) · [Restoration guide](docs/BACKUPS-AND-RESTORE.md)

## 📚 Documentation

| Start here | Go deeper |
| --- | --- |
| [Installation and first playlist](docs/GETTING-STARTED.md) | [All supported features and limits](docs/FEATURES.md) |
| [Most Wanted guide](docs/MOST-WANTED.md) | [Most Wanted vs Carbon comparison](docs/GAMES-AND-COMPATIBILITY.md) |
| [Carbon guide](docs/CARBON.md) | [Technical notes and compatibility](docs/TECHNICAL-NOTES.md) |
| [Screenshot gallery](screenshots/README.md) | [Troubleshooting](docs/TROUBLESHOOTING.md) |
| [Beta 1.5 change and testing status](docs/WHATS-NEW-BETA-1.5.md) | [Release checksum](docs/SHA256-OF-BETA-1.5.txt) |

> [!NOTE]
> The release page also shows automatic GitHub **“Source code (zip/tar.gz)”** links. Those contain this *documentation repository snapshot*, **not the Windows application** and **not its editable development source**. For Windows, download **`XNFS-Playlist-Builder-3.2-Beta-1.5-Public.zip`**.

---

<div align="center">

Created by **valentine**. Based on original **XNFSMusicPlayer** and in-game installer work by **Lovro Pleše (xan1242)**.

<sub>Independent fan-made utility. Not affiliated with or endorsed by Electronic Arts. No game assets or commercial music included.</sub>

</div>
