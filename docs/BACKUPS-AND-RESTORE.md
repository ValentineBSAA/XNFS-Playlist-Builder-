# 🛡️ Backups, installation and restore | Beta 1.7

[← Home](../README.md) · [Installation](GETTING-STARTED.md) · [Troubleshooting](TROUBLESHOOTING.md)

**Before installing player features, copy your entire game folder somewhere safe.** Include existing game mods, proxy/ASI loaders, original music banks and any older XNFSMusicPlayer files. The builder's tracked backup is a convenience, not a replacement for your own known-good backup.

## What changes game files?

Installing the **Windows desktop builder** alone does **not** automatically modify either game. Within the app, however, **Install selected features** may write or replace game-side player/configuration files, **Build / Save** writes playlist data, and restoration actions can modify tracked files. The game should be closed for these actions.

| Control | What it attempts | Boundary |
| --- | --- | --- |
| **Restore backup** | Return to a previously saved player/playlist configuration | The snapshot could itself contain mods |
| **Restore original game** | Preview a return to the first recorded game baseline | Requires intact tracked originals and addition records |

**Do not force-delete files or bypass safety prompts** when records are incomplete or changed externally.

## Recovery procedure

1. Close the game and confirm the builder points to the right game and profile.
2. Choose **Game configuration → Installation → Check setup**, particularly if a previous installation seemed to stop or crash.
3. Open the correct restore option and read every file-change preview.
4. Apply restoration only if the expected original files and backups exist.
5. Restart the game and confirm the desired sound and other mods still work.
6. Retain the independent backup and tracking data until you have tested thoroughly.

## New installer feedback in Beta 1.7

Live audio-preparation percentage, completed-song count, post-audio installation stages and ETA (when available) help show that work continues **after the final song is prepared**. Completion review **OK** returns to the main workspace; the developer verification records **10 passing completion/return cycles**. These are UI/fixture tests, not complete game-restoration tests.

A previous Windows app upgrade could leave incompatible **Shiboken** runtime DLLs; the new versioned dependency layout was reported repaired on the affected installation. This is separate from Carbon's unresolved game-side Load Complete crash.

**Native soundtrack caution:** Most Wanted's original score installer may generate soundtrack assets later, **inside the game**, after desktop installation. End-to-end restoration of every native-generated file remains incompletely tested. Uninstalling the desktop builder **does not** undo game modifications.

[Complete Beta 1.7 evidence](WHATS-NEW-BETA-1.7.md) · [Report a problem](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose)
