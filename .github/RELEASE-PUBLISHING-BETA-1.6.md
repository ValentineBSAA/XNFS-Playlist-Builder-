> **Archived Beta 1.6 reference only.** Do **not** use this file to publish the current release. For Beta 1.7 use [the updated publishing checklist](RELEASE-PUBLISHING-BETA-1.7.md) and [release description](RELEASE-NOTES-BETA-1.7-FOR-GITHUB.md).

# Publish XNFS Playlist Builder 3.2 Beta 1.6

**Documentation state:** Beta 1.6 docs, checksum, support templates and licensing disclosures have been committed. Screenshots are unchanged. The prior Beta 1.5 release and its tag should remain untouched.

## Manual GitHub publishing steps

1. Open **https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/new** while signed into the repository owner account.
2. Choose **Create new tag** `v3.2-beta.1.6` targeting the current `main` branch. Do **not** overwrite or move the historical `Beta-1.5` tag.
3. Release title: **XNFS Playlist Builder 3.2 Beta 1.6**.
4. Copy the prepared, GitHub-link-safe release description from [`.github/RELEASE-NOTES-BETA-1.6-FOR-GITHUB.md`](RELEASE-NOTES-BETA-1.6-FOR-GITHUB.md).
5. Attach **`XNFS-Playlist-Builder-3.2-Beta-1.6-Public.zip`**. This is the only required public downloadable asset: it **already contains** `XNFS-Playlist-Builder-3.2-Beta-1.6-Setup.exe`. A separately attached EXE is optional but not necessary.
6. Mark **Set as a pre-release**. Verify the ZIP asset name and SHA-256, then **Publish release**.
7. After publishing, verify the download from the release page, and that the current README links users to Releases.

## Never attach as the installer

- **Developer ZIP:** contains editable source and internal developer handoff; it is not the public Windows package.
- **Automatic Source code (zip/tar.gz):** documentation and screenshots snapshot only.
- **GitHub-media screenshots:** historical gallery already exists, so no new screenshot upload is necessary.

## Expected checksums

```text
8bf8d69cfaeef2d8759ff172694747fbaebef39661088f1b99bc46110fc3cfd8  XNFS-Playlist-Builder-3.2-Beta-1.6-Public.zip
334ee6a3c55e65e4531bfd8f15036d003a33c20ed71f16133e838c15cdf70511  XNFS-Playlist-Builder-3.2-Beta-1.6-Setup.exe
```

The hashes above were independently recalculated for the provided public ZIP and extracted Setup EXE. The Beta 1.6 developer handoff records clean Windows installation/smoke/uninstallation and runtime fixture tests, but **actual Windows execution was not rerun during this repository documentation update**.

## Compatibility disclosures that must stay visible

- Most Wanted gameplay tests cover specific Safe House, prologue, Free Roam/pursuit and custom T-skip/EA Trax scenarios, including the original-mode pursuit exit fade.
- The revised custom interactive exit fade, every custom boundary fade and first song after changing saves are not fully verified.
- Carbon 1.4 gameplay and original Canyon/Pursuit/Drift modes remain experimental; custom Canyon/Pursuit buckets are unfinished.
- Carbon's intermittent Load Complete crash and the heavily modded Most Wanted rendering issue are unresolved.
- Modified `speed.exe` matching 61 signatures does not prove PLAK game compatibility.
- User-facing third-party notices are included, but redistribution/compliance review of GPL-enabled FFmpeg, Qt/PySide6 and BASS terms is still recommended. See [licensing and credits](../docs/LICENSING-AND-CREDITS.md).

## Release automation

The old Beta 1.5 workflow that updated the older release body and force-moved its tag has been removed. The replacement read-only docs validator does **not** upload release assets or modify tags. The Public ZIP must be attached manually.
