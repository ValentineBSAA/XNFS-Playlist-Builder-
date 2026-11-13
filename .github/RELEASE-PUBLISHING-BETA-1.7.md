# 🏁 Beta 1.7 | GitHub prerelease publishing checklist

**Release:** XNFS Playlist Builder 3.2 Beta 1.7  
**New tag:** `v3.2-beta.1.7`  
**Target:** `main`  
**Mark:** **Prerelease**  

The GitHub repository's documentation is prepared for Beta 1.7. The **Public ZIP is to be uploaded by the repository owner**; the Developer ZIP contains editable code and must not be uploaded as the public installer. Screenshots from the older gallery remain unchanged.

## Publish in GitHub

1. Visit [New release](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/new).
2. Create the new **`v3.2-beta.1.7`** tag from the current `main` branch. Do not move or repurpose the historical Beta 1.5 or Beta 1.6 references.
3. Set title **XNFS Playlist Builder 3.2 Beta 1.7**.
4. Paste the [GitHub-ready release notes](RELEASE-NOTES-BETA-1.7-FOR-GITHUB.md) into the description.
5. Attach **`XNFS-Playlist-Builder-3.2-Beta-1.7-Public.zip`**. It **already contains** `XNFS-Playlist-Builder-3.2-Beta-1.7-Setup.exe`. Do not attach the Developer ZIP.
6. Check **Set as a pre-release** and publish.
7. After publication, verify the download filename, content and SHA-256 on your release page. The README's Releases link should lead to your new release.

A standalone Setup EXE is **optional**, not necessary when distributing the verified Public ZIP.

## Exact tested release hashes

```text
e2ffbf89173ceb01a54211da50ddd0367212a248e4277508c206586807c42609  XNFS-Playlist-Builder-3.2-Beta-1.7-Public.zip
d239b491a1d383e21607086da40a95f64543a4756e37719f8aded1b8fbc459fb  XNFS-Playlist-Builder-3.2-Beta-1.7-Setup.exe
```

Public ZIP size: **107217837 bytes**. ZIP integrity and installer hashes were independently checked against the provided Beta 1.7 Developer ZIP handoff.

## Documentation boundaries

- **Hardware-reported pass:** developer valentine's 45-track Most Wanted custom Pursuit, Safe House and Free Roam gameplay sessions; live preparation percentage and completion.
- **Verified manual setting:** engine sound is adjusted manually via **Most Wanted → Audio options → Car Volume**; builder music gain is separate.
- **Packaged testing:** 10 installer completion-review/return cycles; the handoff states `gameplay_on_final_exe: false`.
- **Not fully verified:** Carbon 1.4, Canyon/Pursuit/Drift event playback, PLAK, selected custom transition paths, first song after changing saves.
- **Not implemented:** independent custom Carbon Canyon/Pursuit music buckets.
- **Unresolved:** Carbon Load Complete crash and heavily modded Most Wanted rendering report.
- **Licensing:** preserve upstream XNFSMusicPlayer MIT attribution; ensure compliance with bundled GPL-enabled FFmpeg and other third-party terms. No blanket project-wide original-builder license has been declared.

## What the repository does automatically

The read-only documentation-validation workflow checks Markdown paths, checksums, essential release files and the original 45-image Beta 1.5 gallery. It does **not** create releases, force-move tags or upload assets. Those steps remain manual.

[Full acceptance table](../docs/WHATS-NEW-BETA-1.7.md) · [Licensing](../docs/LICENSING-AND-CREDITS.md) · [Release notes](../RELEASE_NOTES.md)
