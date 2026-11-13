# Beta 1.7 | Developer PC Gameplay Verification

[← Home](../README.md) · [Beta 1.7 complete test record](WHATS-NEW-BETA-1.7.md) · [Most Wanted](MOST-WANTED.md)

## November 13, 2026: Developer-confirmed hardware gameplay

**Tester:** valentine (project developer)  
**Application under test:** XNFS Playlist Builder **3.2 Beta 1.7**  
**Computer:** Physical Windows PC  
**Operating system:** **Windows 11**  
**Game:** **Need for Speed: Most Wanted (2005) Black Edition, version 1.3**  
**Test method:** Hands-on gameplay and use of the running application on the developer's PC  
**Reported outcome:** **PASS.** The developer reports that everything they tested worked correctly in this configuration, with no issues observed in that test session.

This is a **direct, subsequent developer verification**, not an automated fixture or hypothetical compatibility statement. It adds a real-world PC configuration to the existing Beta 1.7 evidence.

### How this relates to earlier verification

The original Developer ZIP's `VERIFICATION.json` captured the packaging-test state at handoff and explicitly included `gameplay_on_final_exe: false`. **That historical field must not be rewritten:** it accurately describes what had been tested *at the time the file was generated*.

**On November 13, valentine supplied additional, later hands-on Beta 1.7 PC gameplay confirmation.** Accordingly, it is now inaccurate to describe Beta 1.7 as lacking *any* subsequent developer gameplay verification.

The developer has not provided an exact SHA-256 for the executable used in this latest session, so the new statement **does not independently establish that the tested executable is byte-for-byte identical to the Public ZIP's installed EXE**. It verifies the **Beta 1.7 version on the specified hardware and game**.

Earlier documented 45-track Custom Pursuit, 45-track Safe House and 45-track Free Roam playback tests remain separate recorded developer tests. This new broad confirmation **does not assert that those exact song-count tests were individually rerun**.

### Scope and boundaries

- **Confirmed:** the features the developer personally exercised in Beta 1.7 behaved correctly on Windows 11 with Most Wanted Black Edition 1.3 in the latest hands-on test.
- **Not claimed:** universal compatibility on Windows 10, all regional/modified game executables, PLAK, other computers or other players' mod stacks.
- **Not newly verified by this report:** Carbon 1.2 / 1.4 gameplay, original Carbon Canyon/Pursuit/Drift events, and features the developer did not explicitly identify as part of their latest session.
- **Existing open reports:** Carbon's intermittent Load Complete crash and a heavily modded Most Wanted rendering issue do not become resolved solely because this PC configuration passed.
- **Manual audio requirement remains:** Most Wanted's **Car Volume** is adjusted through the game's own Audio options; builder Music gain is separate.

### Reproducibility

This entry records **developer testimony**, not independent third-party confirmation. No new per-feature diagnostic log, video, test checklist, installed-binary hash or cross-PC regression record accompanied the November 13 report. Future independent confirmation, including from the original Discord reporter, would further strengthen the compatibility record.

**Verdict:** Beta 1.7 is **developer gameplay-verified for the stated Windows 11 + Most Wanted Black Edition 1.3 PC configuration**, without a blanket declaration of universal stability.

[Release notes](../RELEASE_NOTES.md) · [Compatibility guide](GAMES-AND-COMPATIBILITY.md) · [Report a compatibility issue](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose)
