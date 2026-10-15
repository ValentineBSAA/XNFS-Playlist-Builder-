# 🔧 Technical notes for experienced players

The main pages are written for beginners. This page collects the setup facts that matter if you already use mods, ASI loaders or custom music players.

[← Home](../README.md) · [Feature comparison](GAMES-AND-COMPATIBILITY.md) · [Download Beta 1.4](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/v3.2-beta.1.4/XNFS-Playlist-Builder-3.2-Beta-1.4-Clean-Public.zip)

## Supported environment

**Windows 10 / 11 (64-bit)**. Bring your own game and locally stored music.

For in-game music playback you need a **supported executable** and a **compatible ASI loader**. Game versions and installed mods may affect behavior. The builder's compatibility checks should be respected, not bypassed.

Carbon **1.2** has received developer live-game testing. Carbon **1.4** has been checked offline and still needs live testing. Some earlier Most Wanted Beta 1.4 playback behavior, **T skipping**, and restoration were tested; the newest merged menu/Safe House routing requires a new acceptance test.

**Known nonworking feature in public Beta 1.4:** Most Wanted **interactive pursuit music** does not currently function as intended. The Pursuit category in the builder does not prove the runtime feature works. The revised implementation is being addressed for **Beta 1.5**, which is **not release-ready**. The sole developer cannot test every game state or mod setup; see the [public status clarification](WHATS-NEW-BETA-1.4.md#known-issue-interactive-pursuit-music).

## What gets changed?

**Installing the Windows application** does not itself immediately modify a game.

**Installing player features** may update or replace supported player components and their configuration. **Build / Save** writes playlists and can generate separate leveled playback copies if selected.

Keep a backup of the original game folder and any pre-existing **XNFSMusicPlayer** installation. Review installation prompts before replacing components.

## Restore paths

**Restore backup** and **Restore original game** mean different things. The first returns to a saved setup, which may already contain mods. The second attempts to reverse tracked changes back to the recorded original state. Restoration cannot be guaranteed when records are incomplete, original files were changed elsewhere, or backups have been removed.

See [Backups and restoring](BACKUPS-AND-RESTORE.md).

## Verifying the release

The intended Windows download is **XNFS-Playlist-Builder-3.2-Beta-1.4-Clean-Public.zip** attached to the official **v3.2-beta.1.4** release. It contains only:

- `XNFS-Playlist-Builder-3.2-Beta-1.4-Setup.exe`
- `READ-ME-FIRST.txt`
- `READ-ME-FIRST.html`

See the [published ZIP and installer SHA-256 checksums](SHA256-OF-BETA-1.4.txt). Checksums verify file consistency; they are not a substitute for deciding whether you trust unsigned software.

The repository hosts user-facing documentation and screenshots, not the full Windows application source code. The source-code archives GitHub automatically generates from this repository **are not installers**.

## Useful support information

When reporting a problem, share the game, game executable version if known, Windows version, other installed mods, and what you tried.

For Carbon playback problems, **XNFSMusicPlayer.log** inside the game's `scripts/XNFSMusicPlayer` folder can be useful when present.

**Remove private user names, full local paths, IP addresses and other sensitive information from screenshots or logs before posting publicly.**

[Report a bug](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose) · [Common questions](TROUBLESHOOTING.md)
