# 🚀 Let's get your music into Need for Speed

You don't need to be a computer expert. This guide explains the process from start to finish.

[← Home](../README.md) · [Which game is supported?](GAMES-AND-COMPATIBILITY.md) · [I need help](TROUBLESHOOTING.md)

> **Which version can I download right now?** Beta 1.4's new Windows installer is prepared but isn't attached to a published GitHub release yet. Until that upload is finished, the public download is **[Beta 1.2](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/v3.0-beta.1.2/XNFS-Playlist-Builder-3.0-Beta-1.2-Public.zip)**. This guide describes the updated Beta 1.4 controls; some labels may differ in the older beta.

## Before you start

You'll need:
- A PC with **Windows 10 or Windows 11 (64-bit)**.
- Your own installation of **Carbon (2006)** or **Most Wanted (2005)**.
- Some music files stored on your computer.
- A compatible **ASI loader** in the game folder for custom in-game playback. This is a small component that allows the game to load player modifications.

**Make a copy of your game folder** before applying game features or saving playlists. This is particularly important if you already have mods installed.

## Step 1: Download and install

When Beta 1.4 is published, download **XNFS-Playlist-Builder-3.2-Beta-1.4-Clean-Public.zip** (the final release file will be labeled clearly).

Right-click the downloaded ZIP, choose **Extract All**, and run **XNFS-Playlist-Builder-3.2-Beta-1.4-Setup.exe**.

**Do not download the “Source code” ZIP** generated automatically by GitHub. It isn't a Windows installer.

The setup program is unsigned. Windows may ask you to confirm an unknown publisher. Double-check where you got the installer and proceed only if you trust it.

## Step 2: Select your game

Open XNFS Playlist Builder.

Choose **Carbon** or **Most Wanted** at the top of the application.

Select **Game Folder** to show where that game is installed. You can try **Auto Detect** if you don't know the location.

Select **XNFS Folder** if the app needs help finding the game's music-player folder.

The app checks whether the selected game version is compatible before installing features. If the check fails, don't force a different version; read the warning and ask for help.

## Step 3: Find your songs

Select **Music Folder** and choose where you store your music, then click **Scan**.

The app displays titles, artists, track lengths and genre information when available. It remembers your music folder and can scan it again in later sessions.

Missing genres? Use **Review genres**, **Unclassified tracks**, or **Edit genre** to organize them.

## Step 4: Choose your playlists

**Most Wanted:** **Safe House** covers both the menus and safe house. **Free Roam**, **Race**, and **Pursuit** each have their own soundtracks. The automatic driving playlists feature selects music for the active situation when enabled.

**Carbon:** **Menu**, **Muscle**, **Tuner**, and **Exotic** let you tailor the soundtrack to what you drive.

You can enable **Auto-assign tracks by genre** to get suggestions, or select music yourself. The app may balance track counts across categories, so review its suggestions.

Open **Install game features** to choose optional playback settings. Read the options before installing them. Most Wanted lets you use **T** to skip while driving; Carbon offers optional **F9** skipping.

## Step 5: Build and save

**Close the game first.**

Click **Build / Save**.

Wait for any optional loudness leveling to finish. Leveling makes separate playback copies; your original music stays unchanged.

Read the save summary, then start your game.

## Need to restore your game?

Choose **Restore original game** to attempt to return tracked files to the state before the first builder installation. Choose **Restore backup** for a saved player/playlist setup, which may still include mods.

These options work only when the required restore records are intact. [Read the restore guide](BACKUPS-AND-RESTORE.md) before proceeding.

## If something doesn't work

Check the selected folders, installed game features, compatible game version and completed Build / Save. The [common questions](TROUBLESHOOTING.md) page has more help.

[← Back to the homepage](../README.md)
