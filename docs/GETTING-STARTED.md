# 🚀 Let's get your music into Need for Speed

**Never used a game mod before? No problem.** These steps are written for first-time users.

[← Home](../README.md) · [Carbon guide](CARBON.md) · [Most Wanted guide](MOST-WANTED.md)

## What you need

- A computer with **Windows 10 or Windows 11 (64-bit)**.
- Your own **Carbon (2006)** or **Most Wanted (2005)** installation.
- Music files stored on your computer.
- A supported game executable and compatible **ASI loader** for in-game playback.

**What's an ASI loader?** It's a small part of a modded game setup that lets the game load compatible add-ons. If the game has never been modified, you may need to set one up separately. Don't overwrite an existing loader without checking compatibility.

**Before installing game features:** close your game and **make a copy of the game folder** somewhere safe, especially if you already use mods.

## Step 1: Download the real installer

> **Important before downloading:** Most Wanted's full **interactive pursuit-music system was never fully implemented in Beta 1.4**. You can organize a Pursuit playlist, but the dynamic system is unfinished. **The existing installer is unchanged**; no setting or reinstall enables that missing feature. [Read the public clarification](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/2). **Beta 1.5 is still in development, not released.**

**[⬇️ Download XNFS Playlist Builder 3.2 Beta 1.4](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/v3.2-beta.1.4/XNFS-Playlist-Builder-3.2-Beta-1.4-Clean-Public.zip)**

The file you want is **XNFS-Playlist-Builder-3.2-Beta-1.4-Clean-Public.zip**.

In Windows, right-click the downloaded ZIP and choose **Extract All**. Open the extracted folder and run **XNFS-Playlist-Builder-3.2-Beta-1.4-Setup.exe**.

**Avoid the “Source code” ZIPs** generated automatically by GitHub. Those are not the Windows installer.

The Windows installer is unsigned, so Windows may warn about an unknown publisher. Check where you downloaded it and only proceed if you trust it.

## Step 2: Choose your game

Open XNFS Playlist Builder and select **Carbon** or **Most Wanted**.

Use **Game Folder** to select the folder containing your installed game. Try **Auto Detect** if you're unsure where it's installed.

The **XNFS Folder** control can help locate the music-player folder if necessary. Read any compatibility warning instead of forcing an unsupported game executable.

## Step 3: Scan your music

Choose **Music Folder**, select your songs, and press **Scan**.

The app reads available song information, including names, artists, genres, and lengths. It can remember your folder for later.

## Step 4: Make your soundtrack

| In Carbon | In Most Wanted |
| --- | --- |
| **Menu**, **Muscle**, **Tuner**, **Exotic** | **Safe House**, **Free Roam**, **Race**, **Pursuit** |
| Car-class music | Situation-based playlists; **full interactive Pursuit music was not implemented in Beta 1.4** |
| Optional F9 skipping | T to skip while driving |

For Most Wanted, **Safe House includes the menus**, too.

> **Beta 1.4 known limitation:** Although Most Wanted lets you organize a **Pursuit** playlist, **the full interactive pursuit-music feature was never fully implemented in this release**. The visible playlist is not evidence of a complete interactive system. Completing it is being addressed for **Beta 1.5**, which is **not ready for release**. See the [current status note](WHATS-NEW-BETA-1.4.md#known-issue-interactive-pursuit-music).

You can try **Auto-assign tracks by genre**, review unclassified music, change individual assignments, and choose playlist order. Genre suggestions aren't always perfect.

Choose **Install game features** if you want optional in-game playback controls. Read the prompts and check that your setup is compatible.

## Step 5: Save and play

1. **Close your game.**
2. Click **Build / Save**.
3. Let optional music-volume leveling finish if you enabled it. This creates separate copies and can take time.
4. Read the save summary and launch the game.

**Installing the builder alone doesn't immediately modify the game.** Installing game features or saving playlists can change game files. Keep that backup.

## If you need help

[**Troubleshooting and frequently asked questions**](TROUBLESHOOTING.md) · [**Backups and restoration**](BACKUPS-AND-RESTORE.md) · [**All screenshots**](../screenshots/README.md)

**Beta testing reminder:** Not all features, game versions, or mod combinations have been verified. **Most Wanted interactive pursuit music was never fully implemented in Beta 1.4**, and the latest menu/Safe House change still needs a new live-game test.

[← Home](../README.md)
