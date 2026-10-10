<div align="center">

# 🏁 XNFS Playlist Builder

### Your music. Your drive. Your soundtrack.

Give **Need for Speed Carbon** and **Need for Speed Most Wanted (2005)** a soundtrack built from your own music library.

![Beta 1.2](https://img.shields.io/badge/3.0-Beta%201.2-E5BB62?style=for-the-badge&labelColor=101820)
![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011-229ED9?style=for-the-badge&labelColor=101820)
![Carbon](https://img.shields.io/badge/Carbon-Public%20Beta-33BDEA?style=for-the-badge&labelColor=101820)
![Most Wanted](https://img.shields.io/badge/Most%20Wanted-In%20Development-F2A826?style=for-the-badge&labelColor=101820)

**Made by valentine** · [📥 Beta downloads (release pending)](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases) · [🚀 Getting started](docs/GETTING-STARTED.md) · [💬 Report an issue](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose)

</div>

---

> [!IMPORTANT]
> **This is a public beta, not a finished, widely tested release.** Carbon **1.2** has been tested in-game on the developer's own computer. Carbon **1.4** has only been checked offline so far. **Most Wanted remains under development**, and its automatic music switching is not finished. Results may vary on other systems, game versions and installations.

## 🎶 Make every drive sound like yours

XNFS Playlist Builder finds the songs you already own, organizes them for your game and saves playlists for the XNFS music player. You can decide where your songs belong or let the app suggest categories for you.

- **Bring your own music.** Point the builder at your music folder, scan your tracks and preview their titles, artists, genres and lengths.
- **Let the app sort things out.** Automatically suggest categories from music genres, then review or change assignments yourself.
- **Build a Carbon soundtrack that follows your car class.** Set up separate **Menu, Muscle, Tuner and Exotic** music collections.
- **Keep things fresh.** Optional shuffle playback can avoid recently heard tracks.
- **Make volume more consistent.** Optional leveling creates separate playback copies, leaving your original songs untouched.
- **Change your mind safely.** Backup and restore options help you undo supported changes.
- **Pick up where you left off.** Your selected music folder is remembered and scanned automatically when you reopen the app, if it is still available.

## 📸 Inside the app

See the **Carbon blue** and **Most Wanted gold** interfaces, along with the feature installer, audio-leveling progress and save confirmation. These pictures show the developer's local beta test, not verified behavior on every computer.

<details>
<summary><b>📷 View the application screenshot gallery</b></summary>

### Carbon soundtrack builder

![Carbon soundtrack editor showing Menu, Muscle, Tuner and Exotic song categories](screenshots/carbon-library.png)

*Blue-themed Carbon soundtrack library with car-class playlist assignments.*

| Feature settings | Audio leveling |
| :---: | :---: |
| ![Carbon player features](screenshots/carbon-features.png) | ![Preparing leveled music copies](screenshots/leveling-progress.png) |

| Save confirmation | Saved playlist files |
| :---: | :---: |
| ![Soundtrack saved summary](screenshots/save-summary.png) | ![Playlist, normalized audio and backups](screenshots/saved-files.png) |

### Most Wanted development preview

![Most Wanted gold-themed playlist builder](screenshots/most-wanted-preview.png)

*Most Wanted playlists can be prepared and exported, but automatic in-game situation switching is unfinished.*

</details>

> **Gallery upload:** The six screenshots are prepared for this folder. Image previews will appear after the image files have been uploaded.

## 🚦 What works today?

| Game | Current status | What you should know |
| --- | --- | --- |
| 🟦 **Need for Speed Carbon 1.2** | **Tested in-game on one PC** | Custom music playback, music tied to car classes, track skipping and leveled playback have been tested by the developer. Other setups still need testers. |
| 🟦 **Need for Speed Carbon 1.4** | **Not yet tested in live play** | The supported player build has been compiled and checked offline. Live gameplay testing is still required. |
| 🟨 **Need for Speed Most Wanted (2005)** | **Under development** | Playlist preparation/export is available. Fully automatic switching between Frontend, Free Roam, Race and Pursuit is not complete. |

**Please treat this as experimental software.** Keep a backup of your game installation and your existing music-player setup before experimenting.

## 🏎️ How Carbon's playlists work

| Playlist | Where it is intended to play | Music the automatic sorter tends to prefer |
| --- | --- | --- |
| **Menu** | Game menus | Your menu soundtrack choices |
| **Muscle** | Driving a Muscle-class car | Rock, Alternative, Metal |
| **Tuner** | Driving a Tuner-class car | Pop, Electronic |
| **Exotic** | Driving an Exotic-class car | Hip-Hop, Rap, Grime |

Genre suggestions are **starting points, not rules**. You can adjust assignments, and balanced placement can put tracks outside their preferred category. Songs with missing genre information may need your attention. Review the playlists before you save.

Optional Carbon features include class-aware playback, shuffling with fewer recent repeats and **F9 to skip a song** when the skip option is enabled.

## 🚀 Install and play

1. **[Download Beta 1.2](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases)** when the release asset becomes available, then unzip the download.
2. Open **`XNFS-Playlist-Builder-3.0-Beta-1.2-Setup.exe`**. You need **Windows 10 or 11, 64-bit**. No Python installation is necessary.
3. Open the builder, select **Carbon** or **Most Wanted**, and choose the folder containing your music.
4. Choose **Scan**, review your songs and their categories, and adjust anything you want.
5. For Carbon, use **Install Carbon features** if you want to add the custom player or adjust optional playback features.
6. **Close the game** and press **Build / Save changes** to save your playlist changes.

**Release upload status:** The public repository is live; the installer download has not yet been attached to a release.

**Important:** Installing the *builder app* does not install Carbon gameplay features or modify your game automatically. Those changes happen only when you select the relevant install/save actions.

For game compatibility, backups and more details, see **[Getting started](docs/GETTING-STARTED.md)**.

## 🎧 A few more useful touches

**Audio leveling:** Optional leveling prepares separate music copies with more consistent perceived loudness. Your source audio remains unchanged. Preparing a large library for the first time uses additional disk space and may take time; later builds reuse verified copies. It does **not** change the balance of engine sounds, effects or crew voices.

**Progress you can follow:** During leveling, the app shows which songs it is processing, completed-song progress and elapsed time. Near the end, one long song can make the overall bar appear to pause even while work continues.

**Now Playing:** A separate companion window can show playback information. Keep the builder running to use it. Some games running in exclusive fullscreen may cover that window.

**Undo options:** The app provides backup restoration and a fuller **Restore original game** option for changes it can track. Full restoration depends on complete records from Beta 1.2 onward; older or modified files may prevent exact restoration. [How restoring works →](docs/BACKUPS-AND-RESTORE.md)

## 🧩 Compatibility and limitations

- **Windows 10 or 11, x64** is required.
- For **Carbon**, you must already have a compatible **ASI loader** installed. Only the inspected Carbon **1.2 and 1.4** game executables are supported by this beta.
- The **Carbon 1.4** game player has not been confirmed in live play yet.
- **Most Wanted's automatic runtime playlist switching is incomplete.** Do not assume an exported playlist means that in-game transitions will work.
- A control for crew voice volume exists, but its effectiveness in live play has **not been proven**.
- The app is **unsigned**. Windows may show an unknown-publisher notice. Always download from a release you trust.
- The release contains **no games, commercial music or personal libraries**. Bring your own game installation and tracks.

## 💬 Found a problem?

Testing beyond the developer's own computer is especially valuable for this release. Visit **[Issues](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose)** and share which game and version you're using, what you tried, what you expected and what happened. Screenshots are welcome.

If Carbon music isn't playing, you can also include **`XNFSMusicPlayer.log`** from the game's `scripts/XNFSMusicPlayer` folder. **Remove usernames, private folder paths or other personal information before posting logs or screenshots.**

[📋 More help and common questions](docs/TROUBLESHOOTING.md)

## ❤️ Credits

**XNFS Playlist Builder 3.0** is developed by **valentine**. The original **XNFSMusicPlayer** is by **Lovro Pleše (xan1242)**. Third-party license notices are installed with the application.

This is an independent fan-made utility, **not affiliated with or endorsed by Electronic Arts or the Need for Speed franchise**. Game names and trademarks belong to their respective owners.

---

<div align="center"><strong>Thanks for giving this beta a spin. 🏁</strong><br><sub>Carbon: tested on one PC · Most Wanted: still being built · Feedback welcome</sub></div>