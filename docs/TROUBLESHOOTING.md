# 💬 Questions and troubleshooting

## Carbon isn't playing music

Check that you have a supported Carbon **1.2 or 1.4** executable, an appropriate existing ASI loader, the right game and XNFSMusicPlayer folders, and that you actually installed the optional Carbon features and saved the playlist. Close the game before changing files.

Only **Carbon 1.2** has been confirmed during actual play on the developer's own PC. Carbon 1.4 still needs live testing.

## Why doesn't Most Wanted change music when I start a race or pursuit?

**Most Wanted remains under development.** You can organize and export playlists, but automatic switching among Frontend, Free Roam, Race and Pursuit isn't finished in this beta.

## Why are songs in unexpected categories?

The app offers genre-based suggestions, and balancing can place songs outside their preferred category. Missing or unfamiliar genre tags may require a manual choice. Use **Review genres**, **Unclassified tracks**, **Edit genre**, and assignment controls to tidy up before saving.

## Why does volume leveling take a while?

It prepares separate playback copies of songs and may need extra time and disk space for the first scan. You can watch song-by-song progress; long tracks may make the progress bar appear to pause. Later passes can reuse verified copies.

## Does leveling turn down the engine or character dialogue?

No. It adjusts the loudness of the music copies, not the engine, effects or in-game dialogue. The separate crew-volume control has not yet been proven effective during live play.

## What about my original music?

Your own source recordings stay unchanged when optional leveling is used.

## Where is Now Playing?

It's a companion window; keep the builder open to use it. Exclusive-fullscreen games might cover it.

## Can I undo game modifications?

Use the backup and restore controls when valid backup records are available. See [Backups and restore](BACKUPS-AND-RESTORE.md).

## Windows warns about an unknown publisher

The beta installer is not digitally signed. Confirm that you downloaded the intended release and review Windows warnings.

## How should I report a bug?

Open [a GitHub issue](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose). Include which game and game version, your Windows version, what you clicked, what you expected and what happened.

If Carbon playback fails, the `XNFSMusicPlayer.log` file in `scripts/XNFSMusicPlayer` may be helpful. **Remove usernames, private paths, IP addresses and personal information** from screenshots and logs before posting them publicly.

[← Back to the homepage](../README.md)
