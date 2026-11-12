# 🛡️ Backups and restore | Beta 1.6

[← Home](../README.md) · [Installation](GETTING-STARTED.md) · [Troubleshooting](TROUBLESHOOTING.md)

**Make an independent copy of the entire game folder first.** Preserve installed ASI loaders, other mods and any original XNFSMusicPlayer files. Automated tracking is helpful, but it is not a replacement for your own known-good baseline.

## What modifies games?

**Installing the Windows desktop builder alone does not automatically modify game files.** Using **Install selected features** can install/replace game-side files; **Build / Save** writes playlists and can prepare separate playback copies; restore commands may replace or remove tracked files.

| Function | Intention | Limitation |
| --- | --- | --- |
| **Restore backup** | Restore a previously saved setup / playlist snapshot | Snapshot may already include mods or custom player files |
| **Restore original game** | Preview and attempt to restore the first tracked baseline | Only as reliable as tracked originals and file-change records |

A restore may stop to protect files that changed outside the builder. **Do not bypass conflicts by deleting files blindly.**

## Suggested recovery

1. Close the game and verify the correct game/profile/folder.
2. Open **Game configuration → Installation → Check setup** before attempting more changes.
3. Review the chosen backup/original restoration preview.
4. Confirm only the files that match your intended baseline.
5. Launch the game and test the relevant music modes.
6. Keep copies and tracking data until you confirm full recovery.

**Special Most Wanted limitation:** the native original-score installer can generate music assets **later, inside the game**, after the desktop builder has committed. Complete end-to-end removal/restoration of *every* generated file has **not** been confirmed. Keep a full pre-install backup.

**If the builder appears to crash after installing components:** file changes may have already succeeded. Reopen → **Check setup** rather than reinstalling immediately. The Beta 1.6 handoff reports clean Windows Setup install/uninstall and 10 disposable game installer cycles, but those results do not prove every crash or recovery scenario is solved.

**Uninstalling the desktop application does not undo in-game changes.** Recover files first, and retain your backup/receipt records.

[Testing evidence](WHATS-NEW-BETA-1.6.md) · [Open a bug report](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose)
