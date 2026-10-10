# 💬 Common questions and help

Here are the answers to the questions people are most likely to have while using **Beta 1.2**.

[**⬇️ Official download**](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/v3.0-beta.1.2/XNFS-Playlist-Builder-3.0-Beta-1.2-Public.zip) · [**🚀 Setup steps**](GETTING-STARTED.md) · [← Home](../README.md)

## Does it work with both games?

**Yes. Both Carbon and Most Wanted (2005) are usable now.** Carbon currently has more features.

**Most Wanted's automatic playlist switching** between Frontend, Free Roam, Race and Pursuit is still being developed. That doesn't mean the Most Wanted part of the builder is unavailable.

## Which download do I choose?

Choose **XNFS-Playlist-Builder-3.0-Beta-1.2-Public.zip** from the [official release](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/tag/v3.0-beta.1.2). Extract it and run the **Setup.exe** inside.

**Don't choose “Source code (zip)” or “Source code (tar.gz)”.** Those are GitHub's automatic repository archives, not the Windows installer.

## Carbon isn't playing my music. What should I check?

- Is the game **Carbon 1.2 or 1.4**? Only those inspected versions are intended for this beta.
- Do you already have a compatible **ASI loader**?
- Did you choose the correct **Game Folder** and **XNFS Folder**?
- Did you select **Install Carbon features**, if needed?
- Did you **Build / Save changes**?
- Is the game **closed** while you make installation changes?

Carbon 1.2 has only been tested in-game on the developer's own PC. Carbon 1.4 still needs live testing.

## Why doesn't Most Wanted automatically change music during a race or pursuit?

That *specific advanced feature* is still under development. You can already build and save Most Wanted playlists, but fully automatic in-game situation switching isn't finished.

## Why are songs in the wrong playlist?

The automatic genre sorter makes suggestions rather than perfect decisions. Tracks without useful genre tags may require manual attention.

Use **Review genres**, **Unclassified tracks**, **Edit genre**, and the song-assignment controls.

## Why is audio leveling taking so long?

When enabled, leveling prepares separate playback copies. First-time preparation of a large library can take time and uses extra disk space. Watch the song counts and progress window.

**Your original music recordings remain unchanged.**

## Does audio leveling control engines or dialogue?

No. It makes the *music tracks* more consistent with one another. It doesn't change engine effects or voices. Crew-voice volume controls have not yet been proven in live play.

## Can I undo something?

There are backup/restore options for supported changes. Restoration depends on backup records being intact. **Back up your original game installation before changing anything.** [Read the restore guide](BACKUPS-AND-RESTORE.md).

## Why does Windows warn me about the installer?

The public beta is not digitally signed. Check that you downloaded it from the official release and make your own decision whether to run it.

## Why can't I see the Now Playing window?

It is a companion window that requires the builder to be running. Some exclusive-fullscreen games may cover it.

## How do I get help or report a bug?

[**Report a problem on GitHub**](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose). Tell us:
1. Which game you're using, and its version if known.
2. What you tried.
3. What happened instead.

You can attach screenshots. For Carbon playback problems, the **XNFSMusicPlayer.log** file inside your game's **scripts/XNFSMusicPlayer** folder may help.

**Before posting logs or screenshots publicly, remove private usernames, full personal paths, addresses and other personal details.**

[← Home](../README.md)
