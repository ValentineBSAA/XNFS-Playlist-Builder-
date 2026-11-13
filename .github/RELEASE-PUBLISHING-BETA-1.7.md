# 🏁 Beta 1.7 | Published release reference and verification handoff

**Release:** XNFS Playlist Builder 3.2 Beta 1.7  
**New tag:** `v3.2-beta.1.7`  
**Target:** `main`  
**Mark:** **Prerelease**  

**Beta 1.7 is already published** under the historical tag **`Beta-1.7`**, with `XNFS-Playlist-Builder-3.2-Beta-1.7-Public.zip` attached. No further ZIP upload or replacement tag is required for this documentation update. The separate Developer ZIP contains editable code and is **not** a public release asset. The screenshot gallery remains unchanged.

## Historical publication checklist (already completed)

1. **Already completed:** [Beta 1.7 published release](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases/tag/Beta-1.7).
2. **Actual published tag:** `Beta-1.7` (not the originally proposed `v3.2-beta.1.7`). Do not create a duplicate tag or move the old historical releases.
3. Published release title: **XNFS Playlist Builder 3.2 beta 1.7**.
4. [GitHub-ready release notes](RELEASE-NOTES-BETA-1.7-FOR-GITHUB.md) now include the **November 13 Windows 11 / Black Edition 1.3 developer verification**; the separate published release description is not automatically synced by this documentation-only GitHub update.
5. The Public ZIP **is already attached** and includes `XNFS-Playlist-Builder-3.2-Beta-1.7-Setup.exe`. Do not attach the Developer ZIP.
6. The release is already published. No new release needs to be created.
7. Confirm the existing public download's name and checksum against the verification below before any future asset replacement.

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
- **Newer PC gameplay confirmation:** developer valentine reports all personally exercised Beta 1.7 features worked on **Windows 11 / Most Wanted Black Edition 1.3 (PC)** on November 13. See [dated PC validation](../docs/PC-VALIDATION-BETA-1.7.md).
- **Packaged testing snapshot:** 10 installer completion-review/return cycles; the original handoff states `gameplay_on_final_exe: false` **at handoff**, prior to the latest reported PC gameplay; exact executable hash for the later test not provided.
- **Not fully verified:** Carbon 1.4, Canyon/Pursuit/Drift event playback, PLAK, selected custom transition paths, first song after changing saves.
- **Not implemented:** independent custom Carbon Canyon/Pursuit music buckets.
- **Unresolved:** Carbon Load Complete crash and heavily modded Most Wanted rendering report.
- **Licensing:** preserve upstream XNFSMusicPlayer MIT attribution; ensure compliance with bundled GPL-enabled FFmpeg and other third-party terms. No blanket project-wide original-builder license has been declared.

## What the repository does automatically

The read-only documentation-validation workflow checks Markdown paths, checksums, essential release files and the original 45-image Beta 1.5 gallery. It does **not** create releases, force-move tags or upload assets. Those steps remain manual.

[Full acceptance table](../docs/WHATS-NEW-BETA-1.7.md) · [Licensing](../docs/LICENSING-AND-CREDITS.md) · [Release notes](../RELEASE_NOTES.md)
