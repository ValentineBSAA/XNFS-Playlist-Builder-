# 🔧 Technical notes | Beta 1.7

[← Home](../README.md) · [Test matrix](WHATS-NEW-BETA-1.7.md) · [Checksums](SHA256-OF-BETA-1.7.txt)

## Environment and packaging

**Windows 10/11 x64** compiled Setup EXE; no user-side Python installation required. Players provide their own game copy, local music and compatible existing **ASI loader**. Unknown proxy/loader files are not silently overwritten.

The **Public ZIP** contains a **107125542-byte** Setup EXE, first-run TXT/HTML guides, CHANGELOG and third-party license notices, with a total ZIP size of **107217837 bytes**. It does **not** contain the editable Python/C++ application project or new screenshots. GitHub automatic Source code archives are also documentation snapshots only.

**SHA-256:**
- Public ZIP: `e2ffbf89173ceb01a54211da50ddd0367212a248e4277508c206586807c42609`
- Setup EXE: `d239b491a1d383e21607086da40a95f64543a4756e37719f8aded1b8fbc459fb`

Both were independently recalculated and match the supplied Beta 1.7 Developer ZIP manifest. Both ZIP archives passed CRC tests.

## Most Wanted engine and music controls

The user-defined pools are Safe House (also menus), Free Roam, Race, Pursuit and Shared. Configurable fades, finish-current-complete-song switching and independent **65% default Music gain** apply to relevant custom song paths.

**Developer valentine verified:** **engine volume must be changed manually in Most Wanted's game Audio options → Car Volume**. The builder's music gain does not adjust engine volume. This is an accepted operational limitation, **not an unresolved test**.

**Native original interactive:** the builder installs/arms the native soundtrack installer; actual extraction takes place **inside Most Wanted** using the user's game audio. The original adaptive score cannot be skipped with T. Library-based custom interactive music and its **T** skipping are separate paths.

A modified `speed.exe` can pass compatibility checks only when all **61 native music-hook signatures** match; this alone does not guarantee successful gameplay, especially PLAK. The latest custom pursuit exit fade, natural-song entry fades and save-switch priming still require specific live verification.

## Carbon playback

Menu/Muscle/Tuner/Exotic/Shared routing remains the underlying class-mask structure. Matched binaries exist for inspected **Carbon 1.2 and 1.4**. Earlier 1.2 gameplay confirmed class routing, optional F9 and ducking, but **1.4 gameplay and original event-music options remain unverified**. Independent custom Canyon/Pursuit event buckets have not been implemented. The intermittently reported **Load Complete** crash has no confirmed root cause.

## Installer and audio preparation

Beta 1.7 shows per-song analysis/leveling percentage if sufficient duration data exists, completed file counts, named post-song preparation stages and a conditional ETA. It also avoids redundant source file reads while retaining checks of written output.

**Windows upgrade issue:** Beta 1.6's earlier runtime could leave incompatible Qt/Shiboken DLLs when upgraded in place. The Developer ZIP reports reproduction and subsequent successful in-place repair after using versioned runtime dependencies. It does not prove all native/Qt failures eliminated.

The Developer ZIP records **10 completion-review-and-return cycles**, packaged game view checks and an embedded app icon. Earlier automated tests included a 47-file generated install workflow and 17 core regressions. **At the original packaging-test snapshot**, the final compiled Beta 1.7 EXE was not exercised in actual gameplay (`VERIFICATION.json` had `gameplay_on_final_exe: false`). **Later**, on November 13, developer valentine reported successful hands-on Beta 1.7 gameplay with all personally exercised features on a **Windows 11 PC running Most Wanted Black Edition 1.3**. The latest tested EXE's exact hash was not supplied, so identity with the public installer has not been independently established. [Test chronology](PC-VALIDATION-BETA-1.7.md).

## Loudness leveling and diagnostics

Optional FFmpeg leveling prepares new playback copies at target loudness and peak ceiling; originals remain unchanged. Native original/mapped soundtrack components retain their existing gain.

**Support** presents a reviewable plain-English report and JSON, then exports both into one ZIP, excluding raw logs, personal paths, song titles, actual audio and saved-game files. Sharing is entirely manual.

## Attribution and compliance

Original XNFSMusicPlayer and native in-game installer: **Lovro Pleše (xan1242)**, upstream MIT notice preserved. Other packaged dependencies carry their own licenses. The provided FFmpeg build has **GPL and version 3 enabled**; redistributors should verify full compliance rather than assume the notice alone is sufficient.

[Licensing details](LICENSING-AND-CREDITS.md) · [Backups](BACKUPS-AND-RESTORE.md) · [Report a bug](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose)
