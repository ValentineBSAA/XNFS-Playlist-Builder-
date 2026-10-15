<div align="center">

# 🏁 XNFS Playlist Builder

**Your music. Your drive. Your soundtrack.**

Make your own soundtracks for **Need for Speed Carbon (2006)** and **Need for Speed Most Wanted (2005)**.

**Both games are supported by the builder**, but some in-game features are still incomplete or require more testing. In particular, the full interactive pursuit-music system for Most Wanted was **not fully implemented in Beta 1.4** (details below).

**Windows 10 / 11 · 64-bit · Public Beta 3.2 / 1.4**

### [⬇️ Download XNFS Playlist Builder for Windows](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/v3.2-beta.1.4/XNFS-Playlist-Builder-3.2-Beta-1.4-Clean-Public.zip)

[**First-time setup guide**](docs/GETTING-STARTED.md) · [**Browse screenshots**](screenshots/README.md) · [**Help & questions**](docs/TROUBLESHOOTING.md)

</div>

---

## ⚠️ Beta 1.4 known issue: Most Wanted interactive pursuit music

**The complete interactive pursuit-music system was never fully implemented in public 3.2 Beta 1.4.** The builder includes a **Pursuit** playlist for organizing tracks and some underlying playback groundwork, but that is **not the same as a complete, functioning interactive pursuit-music system**. This was an **incomplete feature**, not a finished feature that later broke. Please do not install Beta 1.4 expecting fully functional interactive pursuit music.

Completing the interactive pursuit-music implementation is being addressed for **Beta 1.5**. **Beta 1.5 is still in development and is not ready for release.** See the [Beta 1.4 status and testing notes](docs/WHATS-NEW-BETA-1.4.md#known-issue-interactive-pursuit-music).

**A note from the developer:** I'm sorry I described interactive pursuit music in a way that suggested it was already implemented and working in Beta 1.4. That was inaccurate. I'm the sole developer of XNFS Playlist Builder, and while I test as much as I can, I cannot personally verify every game state, feature, PC configuration, or mod combination. That limitation doesn't excuse presenting an incomplete feature as finished. I should have made the distinction clear before release. Thank you to Kronos and everyone helping identify and report problems.

---

## 🎶 What does it actually do?

Choose a folder of songs on your computer. The builder scans them, helps you sort them into playlists, and saves a custom soundtrack for your game. You can **organize music yourself** or ask the app to suggest categories based on genres.

You don't need programming knowledge or Python. You do need your own game installation, your own music, and a compatible game setup for in-game playback.

## 🎮 Pick your game

### 🔵 Need for Speed Carbon: music that follows your car

[![XNFS Playlist Builder Carbon music library](screenshots/carbon/library.png)](screenshots/carbon/library.png)

Carbon has four soundtrack groups:

| Menu | Muscle | Tuner | Exotic |
| --- | --- | --- | --- |
| Menus and browsing | Muscle-class cars | Tuner-class cars | Exotic-class cars |

**What makes Carbon different?** Music can follow your current car class, **F9** can skip tracks when enabled, and an optional feature lowers music during crew dialogue.

[**Explore Carbon's features and pictures →**](docs/CARBON.md)

<sub>Carbon image: earlier Beta 1.2 interface. The core playlists are still applicable to Beta 1.4.</sub>

### 🟡 Need for Speed Most Wanted: music that follows the action

[![XNFS Playlist Builder Most Wanted Beta 1.4 music library with Safe House, Free Roam, Race and Pursuit](screenshots/most-wanted/library.png)](screenshots/most-wanted/library.png)

Most Wanted has four soundtrack groups:

| Safe House | Free Roam | Race | Pursuit |
| --- | --- | --- | --- |
| Menus and safe house | Driving around Rockport | Racing | Playlist for police chases; **full interactive system not implemented in Beta 1.4** |

**What makes Most Wanted different?** It offers playlists for different driving situations, **T** can skip songs while driving, and **EA Trax notifications** can display song information. **Full interactive Pursuit playback was not implemented** in Beta 1.4.

[**Explore Most Wanted's features and four new screenshots →**](docs/MOST-WANTED.md)

<sub>Most Wanted image: new 3.2 Beta 1.4 interface.</sub>

## ✅ What both games share

- **Your own songs:** scan a local music folder and inspect tracks.
- **Easy playlist editing:** automatic genre suggestions, manual assignments and playlist ordering.
- **Four game-specific music groups:** different categories suited to each game.
- **In-game playback options:** automatic playlist selection and optional shuffle with fewer recent repeats.
- **More consistent loudness:** optional leveling makes separate playback copies instead of changing your original songs.
- **Clearer setup:** checks for game-player components and installation status.
- **Recovery options:** backed-up setups and original-game restoration when valid records exist.

Want the detailed comparison? [**Carbon vs. Most Wanted feature table →**](docs/GAMES-AND-COMPATIBILITY.md)

## 🚀 Get started without the guesswork

1. **[Download the actual Windows installer ZIP](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/v3.2-beta.1.4/XNFS-Playlist-Builder-3.2-Beta-1.4-Clean-Public.zip)**, not the GitHub “Source code” ZIP.
2. In Windows, choose **Extract All**, then run **XNFS-Playlist-Builder-3.2-Beta-1.4-Setup.exe**.
3. Open the builder and choose **Carbon** or **Most Wanted**.
4. Select your game folder and music folder, then click **Scan**.
5. Review your playlists. **Close the game**, choose the game features you want, and click **Build / Save**.

**First time modding a game?** Start with the [step-by-step installation guide](docs/GETTING-STARTED.md). It explains folders, backups, and what an ASI loader is in everyday language.

## 🆕 What's different in Beta 1.4?

**Most Wanted has had the biggest upgrade.** Its Safe House, Free Roam, Race, and Pursuit playlist categories, T-key skipping, shuffle, leveling, EA Trax notifications, and install/restore controls bring it much closer to Carbon's overall experience. **However, the full interactive pursuit-music system was not completed or released in Beta 1.4** and is being addressed in the unreleased Beta 1.5.

Carbon retains its car-class soundtrack system and optional crew-dialogue ducking.

[**Read the Beta 1.4 changes →**](docs/WHATS-NEW-BETA-1.4.md)

## 🛡️ Before changing your game

> **This is a public beta.** Keep a backup of your game folder, especially if you have other mods. A compatible ASI loader and supported game executable are needed for in-game music features. The installer is unsigned, so Windows may display an unknown-publisher warning.
>
> Carbon 1.2 has been tested in-game on the developer's PC; Carbon 1.4 still needs live-game testing. Earlier Most Wanted playback behavior and T-key skipping were tested, but **full interactive pursuit music was never fully implemented in Beta 1.4**; the newest combined menu/Safe House adjustment also needs another live test. Other PCs and mod combinations need community testing.

Installing the Windows builder alone doesn't automatically alter your game. Installing game features or saving playlists **can** change game files.

## 📚 Need something specific?

| I want to... | Go here |
| --- | --- |
| Install this for the first time | [Simple setup guide](docs/GETTING-STARTED.md) |
| Understand Carbon | [Carbon guide](docs/CARBON.md) |
| Understand Most Wanted | [Most Wanted guide](docs/MOST-WANTED.md) |
| Compare their features | [Game comparison](docs/GAMES-AND-COMPATIBILITY.md) |
| Browse all real screenshots | [Screenshot gallery](screenshots/README.md) |
| Fix a problem | [Frequently asked questions](docs/TROUBLESHOOTING.md) |
| Undo changes | [Backups and restoration](docs/BACKUPS-AND-RESTORE.md) |
| Check game compatibility and files | [Technical notes](docs/TECHNICAL-NOTES.md) |

**[Download Beta 1.4](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/v3.2-beta.1.4/XNFS-Playlist-Builder-3.2-Beta-1.4-Clean-Public.zip)** · **[Report a problem or idea](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose)**

---

<div align="center">

Made by **valentine**. Original **XNFSMusicPlayer** by **Lovro Pleše (xan1242)**.

<sub>Independent fan-made utility, not affiliated with or endorsed by Electronic Arts. Games and commercial music are not included.</sub>

</div>
