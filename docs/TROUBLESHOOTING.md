# 💬 Questions and help

This guide is for **3.2 Beta 1.4**. If you're using the older **3.0 Beta 1.2**, some game options and key bindings are different.

[← Home](../README.md) · [Installation guide](GETTING-STARTED.md)

## Which game works?

**Both Carbon and Most Wanted (2005).** They have different playlist names and in-game options, but both can work with the builder.

## Where do I download Beta 1.4?

**[Download the official Beta 1.4 Windows ZIP](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/v3.2-beta.1.4/XNFS-Playlist-Builder-3.2-Beta-1.4-Clean-Public.zip)**. Extract the Clean-Public ZIP and open Setup.exe inside. Do **not** choose GitHub's “Source code” archives.

## What is an ASI loader?

An ASI loader is a small part of a modded game setup that allows supported game additions to load. This project requires a compatible one for game integration. If you aren't sure whether your game has one, check your game's existing mod installation instructions before proceeding.

## Why does the installer say my game isn't compatible?

The game executable must match a supported version. Check that you selected the correct game folder. Do not try to force an unsupported executable.

## Why isn't my music playing?

Check that you picked the correct **Music Folder**, scanned your songs, reviewed category assignments and completed **Build / Save**. Make sure any required player features were installed, the game was closed during changes, and your ASI loader is working.

## Why don't I see a separate Menu category in Most Wanted?

Most Wanted now uses **Safe House** for both menus and the safe house. This is intentional.

## How do I skip tracks?

**Most Wanted:** Press **T** while driving after installing the T-skip feature. It doesn't use F9.

**Carbon:** F9 works if its optional skip feature is installed and enabled.

## Does Most Wanted change music for pursuits?

**No. Not fully in public Beta 1.4.** The builder includes a **Pursuit** playlist and some underlying playback groundwork, but **the full interactive pursuit-music system was never completely implemented in this beta**. It is unfinished functionality, **not a completed feature that broke**. Earlier tests of other playback behavior do not establish that interactive pursuit music was ever finished. Completing the feature is being addressed for **Beta 1.5**, which is **not ready for release**. Please don't install Beta 1.4 expecting fully functional interactive pursuit music. **If you already installed it, reinstalling or changing options cannot add the unfinished complete system. The current Beta 1.4 installer has not been replaced.** See the [public known-issue notice](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/2).

I'm sorry the earlier feature description incorrectly suggested interactive pursuit music had been implemented and tested. This is a one-developer project, and I cannot test every feature and game setup myself, but the incomplete implementation should have been clearly disclosed.

## Why is audio leveling slow?

The program creates separate copies for more consistent music loudness. Larger libraries need processing time and extra disk space. Your original songs are left unchanged.

## Does it change voices or police-radio volume?

Audio leveling affects music copies, not engine sounds or dialogue. Carbon offers optional music ducking during crew speech. **Most Wanted police-radio ducking is not included.**

## Is Restore backup the same as Restore original game?

No. **Restore backup** returns to a saved player/playlist setup. **Restore original game** aims to undo tracked changes and return the game to its recorded original state. Both depend on good restore data.

[Read the full backup guide](BACKUPS-AND-RESTORE.md).

## Why does Windows warn about an unknown publisher?

The installer is currently unsigned. Make sure it came from the official project's GitHub release and only run it if you trust the source.

## Is Beta 1.4 fully tested?

**No.** Some functions, including Most Wanted T-key skipping, have been tested by the developer; other features and system combinations have limited coverage. **Interactive pursuit music was never fully implemented in Beta 1.4**, rather than simply being an implemented feature that hasn't been tested. Please read the [full testing status](WHATS-NEW-BETA-1.4.md#known-issue-interactive-pursuit-music).

## How do I report a problem?

[**Report it on GitHub**](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose). Include which game and version you're using, your Windows version, what you clicked, and what happened. Remove usernames, personal paths and any other private information from logs and screenshots.

[← Home](../README.md)
