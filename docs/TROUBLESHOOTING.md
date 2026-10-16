# 🛟 Troubleshooting XNFS Playlist Builder 3.2 Beta 1.5

[← Home](../README.md) · [Start guide](GETTING-STARTED.md) · [Current test results](WHATS-NEW-BETA-1.5.md)

**Beta 1.5 is public but experimental.** A feature appearing in a menu or passing an isolated file check does **not** mean that gameplay has been verified.

## Where is the installer?

Download [**XNFS-Playlist-Builder-3.2-Beta-1.5-Public.zip**](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/download/Beta-1.5/XNFS-Playlist-Builder-3.2-Beta-1.5-Public.zip). Extract it with Windows **Extract All**. Run **`XNFS-Playlist-Builder-3.2-Beta-1.5-Setup.exe`**. The screenshots ZIP and automatic GitHub "Source code" ZIP are **not installers**.

## Windows says the publisher is unknown

The app is unsigned. Check that the installer was downloaded from **this project's official release**, compare [SHA-256](SHA256-OF-BETA-1.5.txt) if desired, and only run software you trust.

## I had “No module named 'uuid'” in Beta 1.4

The final Beta 1.5 compiled package **includes** the `uuid` Python standard-library module and related runtime components. Its inclusion passed build/fixture inspection. It does not guarantee that every unrelated installation issue is gone. Download the new Beta 1.5 package, not the old Beta 1.4 ZIP.

## My music doesn't play in game

1. Confirm the **correct game folder and executable version**.
2. Confirm your selected music library and scan results.
3. Review **Game configuration → Manual assignments**, then **Save assignments** if edited.
4. With the game closed, verify required player features are installed and use **Build / Save**.
5. Check that your **compatible ASI loader** works. The builder doesn't silently install or replace unknown loader DLLs.
6. Try a simple category first. If file status passes but game playback doesn't, **report it as unverified gameplay**, not automatically as a broken music file.

## Which Most Wanted pursuit mode should I use?

**Original/default:** uses your own original game soundtrack and the **native in-game XNFS installation/extraction**. **Custom interactive:** songs from your scanned library, with experimental advanced mapping options. **Pursuit playlist:** ordinary track pool. Choose only one pursuit mode at a time. The native original soundtrack **cannot be skipped with T**; T supports ordinary/custom continuous tracks.

**Do original and custom pursuit play on top of each other?** They **should not**, but the latest full-game regression for overlap, transitions, exit and mode-save persistence has **not** been completed. Please report audible overlap with game and mode details.

**Most Wanted police-radio ducking?** Not included.

## Why can't I see Carbon-specific Canyon or Pursuit custom song buckets?

They are **not implemented**. The current custom modes use the existing Muscle/Tuner/Exotic/Menu routing. Original Canyon/Pursuit and Drift configuration controls exist, but need actual events tested. Carbon original music extraction is experimental.

## Carbon freezes or crashes around Load Complete

That intermittent issue is **unresolved** and **not established as a player/plugin bug**. Report your exact Carbon executable version (1.2 or 1.4), other mods, where the game stops, whether it happens without the new components, and any Windows crash details. Preserve your backup.

## The Windows builder closed just after player installation

Some Windows failure evidence implicated Qt animation/lifetime handling **after file changes had already committed**. Beta 1.5 hardens timers, queued UI callbacks and dialog/worker disposal. Fixture tests passed, but the original intermittent crash was not reliably reproduced, so **no universal fix is claimed**.

**Reopen → Game configuration → Installation → Check setup**. If the component is already installed, don't blindly overwrite it. **Open troubleshooting logs** and review the operation summary and any Windows Error Reporting information.

## Why are genres odd or songs in multiple categories?

Automatic suggestions rely on **metadata and balancing**, not listening to the audio. Missing/inaccurate tags need review. Driving pools can overlap, and repeated songs may appear in different contexts. Use **Manual assignments** to refine them, **Save assignments**, then **Build / Save** for the game.

## Can I restore everything perfectly?

**Not guaranteed.** Restore backup/original requires intact tracking and files. In particular, the complete rollback of **media generated later by Most Wanted's native in-game original-score extractor** still needs end-to-end acceptance. Keep your own full game backup. [See restoration guide](BACKUPS-AND-RESTORE.md).

## What should I send with a bug report?

Use [GitHub's bug form](../.github/ISSUE_TEMPLATE/bug_report.yml). Include **application Beta 1.5**, Most Wanted/Carbon and executable version, Windows version and screen scaling, selected pursuit/event options, steps, expected vs actual behavior, screenshot, operations/Qt/Windows error logs if available, and whether restarting changes it.

**Please redact Windows usernames, local paths, music metadata and IP addresses before posting.** A little reproduction detail is much more useful than posting an entire unreviewed log.

[Open a GitHub issue](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose) · [Discuss testing](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/discussions)
