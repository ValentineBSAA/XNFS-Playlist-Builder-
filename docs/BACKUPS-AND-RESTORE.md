# 🛡️ Backups and restoring a game in Beta 1.5

[← Home](../README.md) · [Install guide](GETTING-STARTED.md) · [Troubleshooting](TROUBLESHOOTING.md)

**Before you install any in-game features, copy your entire game folder somewhere safe.** Include any existing mods and your XNFSMusicPlayer files. The builder has tracked backup and rollback tools, but they are not a substitute for an independent backup.

## What changes the game?

**Installing the Windows builder by itself** does **not** automatically modify a game. However, **Install selected features** may replace game player/configuration components, and **Build / Save** writes playlist data (and may prepare separate leveled audio copies).

**Never delete original backup files or replacement records** merely because the builder says the player is installed.

## Backup vs original: two different destinations

| Button | What it attempts | Limit |
| --- | --- | --- |
| **Restore backup** | Return to a **saved prior player/playlist setup** | That save may already contain other mods or earlier customizations |
| **Restore original game** | Preview changes and return to the **first recorded original baseline** | Depends on the integrity of the tracked original files and correctly recorded additions |

A restore may refuse to proceed if an original file was edited outside the builder or a backup record is missing. **Do not force-delete game files to bypass that protection.**

## Safer recovery steps

1. Close the game.
2. Open the builder and select the **correct game/profile/folder**.
3. Visit **Game configuration → Installation** and choose **Check setup**. Read the displayed status.
4. Choose **Restore backup** or **Restore original game**, review the full preview and confirm only if correct.
5. Check that the game launches and the expected files/music are back.
6. Keep your backups until you're satisfied with the result.

**Native original interactive soundtrack caveat (Most Wanted):** the builder deploys a native in-game installer that may generate music files *after* the Windows installer has committed. Complete restoration of every one of those generated files remains an **end-to-end test outstanding in Beta 1.5**. Do not claim one-click original restoration is perfect.

## What if installation closed unexpectedly?

It may have already committed files before the UI closed. **Reopen → Game configuration → Installation → Check setup first**, rather than repeatedly installing. Then use **Open troubleshooting logs** for more information. **Builder installer UI crash hardening was tested in fixtures, not proven to eliminate all crashes.**

Uninstalling the Windows builder does not automatically reverse game changes. Retain app data and tracked restore records until restoration is complete.

[Report a problem](../.github/ISSUE_TEMPLATE/bug_report.yml) · [See tested and untested behavior](WHATS-NEW-BETA-1.5.md)
