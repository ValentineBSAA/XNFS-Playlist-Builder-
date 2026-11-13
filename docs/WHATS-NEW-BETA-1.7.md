# Beta 1.7 release verification and gameplay record

[← Home](../README.md) · [Release notes](../RELEASE_NOTES.md) · [Help](TROUBLESHOOTING.md)

**XNFS Playlist Builder 3.2 Beta 1.7 · Windows public prerelease**

This page separates (a) actual gameplay reported by the **developer valentine**, (b) results carried forward from earlier versions, (c) packaged/automated checks and (d) outstanding compatibility or unimplemented features. The data comes from the Beta 1.7 Developer ZIP: `GITHUB-HANDOFF.json`, `GITHUB-HANDOFF.txt`, `VERIFICATION.json` and the distribution's `CHANGELOG.md`, supplemented by valentine's direct engine-volume confirmation.

## New developer verification: Windows 11 + Most Wanted Black Edition 1.3

**Reported November 13, 2026 by valentine:** XNFS Playlist Builder **3.2 Beta 1.7** was tested during actual gameplay on a Windows 11 PC using **Need for Speed: Most Wanted (2005) Black Edition, version 1.3**. The developer confirms **every feature exercised in that session worked correctly**, with no observed problems on that configuration.

This is a newer developer hardware test that occurred **after** the Developer ZIP's packaging-verification snapshot. The snapshot's `gameplay_on_final_exe: false` refers to its original test run, not a permanent claim that no subsequent Beta 1.7 gameplay ever occurred. The latest session did **not include a tested EXE checksum**, so byte-for-byte equivalence to the published Public ZIP's installed executable is unverified. The report also does not enumerate each individually exercised feature, and must not be presented as an independent third-party test.

[Read the full dated developer PC validation record](PC-VALIDATION-BETA-1.7.md).

## What's changed from Beta 1.6

- **Live per-song loudness leveling and preparation percentage** when source duration is available, plus completed-file count, named install stages and an ETA once sufficient progress exists.
- **Completion review workflow:** after successful player installation, choose **OK** and return to the main workspace. The handoff records **10 successful packaged completion-review/return cycles**.
- **Application identity:** embedded Windows icon with taskbar and shortcut consistency.
- **Custom pursuit installation:** fewer repeated reads of the source audio; verification of generated audio remains; post-audio restore, cleanup and player-install stages are now visible.
- **Upgrade repair:** older runtime DLLs left behind during an upgrade were implicated in a reproduced Shiboken load failure. A versioned runtime dependency directory plus an in-place installer repair passed the reported verification.
- **Larger Most Wanted playlist gameplay:** **45 custom Pursuit, 45 Safe House, 45 Free Roam tracks** were played successfully according to valentine's reported tests; the custom Pursuit group included an additional manually selected song.

## Verified developer operating note: engine volume

**Status: developer verified in gameplay; manual adjustment required.**

In **Need for Speed: Most Wanted (2005)**, **car engine sound volume must be adjusted manually using the game's own Audio options → Car Volume**. The XNFS builder's independent **Music** volume does **not** automatically adjust engine loudness. The builder's **65% default music level** was accepted as an initial music/engine/police-radio balance, but the correct car volume depends on the player's game settings and audio setup.

**Classification:** expected manual configuration, **not** a pending implementation, unresolved defect, or untested suggestion.

## Most Wanted gameplay test matrix

| Scenario | Evidence / test source | Classification |
| --- | --- | --- |
| Overall Beta 1.7 gameplay on Windows 11, MW Black Edition 1.3 PC | Developer reports all personally exercised features behaved correctly on November 13; individual feature list and EXE hash not supplied | **Latest developer hardware pass for this configuration** |
| Custom interactive Pursuit, 45 songs | Developer reports completed real-game playback, including a manually added selection | **Developer-confirmed pass, Beta 1.7 handoff** |
| Safe House, 45 tracks | Developer reports working playlist playback | **Developer-confirmed pass, Beta 1.7 handoff** |
| Free Roam, 45 tracks | Developer reports working playlist playback | **Developer-confirmed pass, Beta 1.7 handoff** |
| Live processing percentage | Developer observed progress during 45 custom pursuit song preparation and completed install | **Developer-confirmed pass** |
| Car engine loudness | Developer verified manual **Car Volume** control in game's Audio settings | **Developer-confirmed operating requirement** |
| Safe House song fades | First three song excerpts audibly faded in earlier sessions | **Earlier gameplay pass** |
| Prologue soundtrack | Music became audible after independent gain adjustment | **Earlier gameplay pass** |
| Free Roam → ordinary Pursuit | Existing song finished; Pursuit track selected; prior log shows 0.65 applied gain | **Earlier gameplay pass** |
| Custom interactive song selection | Earlier three-song test logged 39 node requests, intended indices and no logged playback errors | **Earlier gameplay pass** |
| Custom continuous-song T skip | Confirmed by user in earlier hardware gameplay | **Earlier gameplay pass** |
| EA Trax notifications | Correct custom song titles shown in earlier game test | **Earlier gameplay pass** |
| Original adaptive pursuit score | Earlier playback confirmed; revised exit handoff audibly faded back to Free Roam | **Earlier gameplay pass**, exit timing may feel slow |
| Latest custom-mode exit fade | Revised custom handoff not separately listened to after final change | **Needs targeted gameplay test** |
| Fade-in at every natural custom-song boundary | BASS fixture checked endpoints, not every real-game boundary | **Needs targeted gameplay test** |
| First track after switching saves | Fresh-scene logic compiled/fixture tested; end-to-end gameplay not confirmed | **Needs gameplay test** |
| Modified/PLAK game executable | All 61 music signatures can match, but no verified PLAK game playthrough | **No PLAK gameplay verification** |
| Heavily modded car-body rendering | Issue observed; read-only inspection inconclusive, XNFS causality not established | **Open / unrelated cause unproven** |

**Important:** these are specific real-playback claims, not a general guarantee of correct behavior on all editions, computers, save games or mod stacks.

## Carbon compatibility matrix

| Scenario | Evidence | Classification |
| --- | --- | --- |
| Carbon 1.2 car-class routing | Earlier real gameplay confirmed class music | **Earlier gameplay pass** |
| F9 skip and crew-speech ducking | Earlier gameplay reported on 1.2 | **Earlier gameplay pass** |
| Inspected 1.2 and 1.4 player payloads | Version-matched packaging and isolated installer fixtures | **Isolated / automated pass** |
| Carbon 1.4 runtime playback | No complete in-game acceptance | **Not verified** |
| Original Canyon/Pursuit and Drift options | Configuration / installation combinations tested, not full event listening | **Experimental / needs gameplay** |
| Independent custom Canyon/Pursuit pools | Current runtime still uses class pools | **Not implemented** |
| Intermittent Load Complete crash | Historical report, root cause/fix not established | **Unresolved** |

## Installer / packaged verification

| Test | Result / interpretation |
| --- | --- |
| ZIP integrity | Public ZIP and Developer ZIP CRC **passed** |
| Public ZIP SHA-256 | **e2ffbf89173ceb01a54211da50ddd0367212a248e4277508c206586807c42609** |
| Setup EXE SHA-256 | **d239b491a1d383e21607086da40a95f64543a4756e37719f8aded1b8fbc459fb** |
| Embedded icon | **true** in developer verification |
| Packaged views | Most Wanted and Carbon pass in developer verification |
| Completion-review and main-window return | **10 cycles** in developer verification |
| Overall packaged verification | `passed: true` in developer `VERIFICATION.json` |
| Actual gameplay on final packaged EXE **at original handoff** | `gameplay_on_final_exe: false` in original developer `VERIFICATION.json`; **newer Windows 11 + Black Edition 1.3 gameplay confirmation received November 13**, but exact tested EXE hash not provided |
| Previous core regression suite | 17 tests reported passing in earlier handoff, **not newly run here** |
| 47-file generated custom installer | Earlier isolated regression passed; original 1.4 GB source workload not fully rerun in that fixture |
| Native hook layout | 61 signature checks can accept a matching modified executable, without proving gameplay |

The published checksums were **independently recalculated** from the supplied Beta 1.7 Public ZIP and its Setup EXE during GitHub-documentation preparation. A ZIP integrity check and the handoff's test summary **do not certify that the installer is free from other defects**.

## Restoration and data safety

Installing the **Windows application** is different from installing the **game-side player**. With the game closed, **Install selected features** and **Build / Save** may modify game files. **Restore backup** returns to a tracked saved setup; **Restore original game** attempts to undo recorded changes. Neither can guarantee complete recovery if another mod changed files or originals are missing.

Most Wanted's original adaptive soundtrack installation/extraction happens **inside the running game**, after the relevant native installer has been enabled. Full restoration of all native-generated files remains incompletely covered.

## What remains genuinely open

A majority of the *reported* Most Wanted scenarios are working. The remaining explicitly unverified items are **Carbon 1.4**, experimental Carbon Canyon/Pursuit/Drift event playback, PLAK gameplay, the first song after save switching, certain custom pursuit fade paths, and full-game restoration of native-generated audio. Independent custom Canyon/Pursuit buckets are **not implemented**. The intermittent Carbon Load Complete crash and the heavily modded Most Wanted rendering report have no verified root cause.

The manual **Car Volume** requirement is **not** an open issue. The later Windows 11 + Black Edition 1.3 success report is **configuration-specific**; remaining entries denote missing isolated/other-game verification, not failures observed on that tested PC.

[Detailed Most Wanted guide](MOST-WANTED.md) · [Carbon](CARBON.md) · [Compatibility](GAMES-AND-COMPATIBILITY.md) · [Troubleshooting](TROUBLESHOOTING.md) · [Checksum](SHA256-OF-BETA-1.7.txt) · [Previous Beta 1.6 record](WHATS-NEW-BETA-1.6.md)
