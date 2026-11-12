# Licensing, third-party components and credits

[← Home](../README.md) · [Release notes](../RELEASE_NOTES.md)

## The project and its source availability

**XNFS Playlist Builder** is a fan-made Windows application maintained by **valentine**. This public GitHub repository currently contains **documentation, templates and screenshots**, not the editable builder/application source code. The public Beta 1.6 ZIP contains a compiled Windows setup installer and bundled third-party notices. Its companion **Developer ZIP with editable source is not being published as a release asset in this documentation update**.

**Do not assume an open-source license for valentine's original builder code or repository content merely because the GitHub repository is public.** No blanket project-wide permission or license for that original content has been declared in the repository. This does not alter the separate licenses of third-party components. A full project-wide licensing decision would need to come from the copyright holder.

## Upstream XNFSMusicPlayer and native installer

- Original **XNFSMusicPlayer** and native in-game soundtrack installer: **Lovro Pleše (xan1242)**, [upstream repository](https://github.com/xan1242/XNFSMusicPlayer).
- The XNFSMusicPlayer source and runtime notices included in the developer/public packages identify an **MIT License, Copyright (c) 2021 Lovro Pleše**. Retain that attribution and copyright/permission notice when redistributing relevant portions. A copy of the upstream license is preserved in [\`licenses/XNFSMusicPlayer-MIT.txt\`](../licenses/XNFSMusicPlayer-MIT.txt).
- This upstream MIT grant **does not** itself assign an MIT license to unrelated valentine-authored builder code or to other dependencies.

## Other bundled components

The **Public ZIP → Third-party notices** directory includes the actual accompanying terms and attributions. Examples:

| Component | Published information / terms to check |
| --- | --- |
| **BASS, BASSFLAC, BASSMIDI** | Un4seen components and bundled text/terms; **not equivalent to an MIT grant** |
| **FFmpeg** (imageio-ffmpeg bundle) | Bundled FFmpeg build configuration reports **GPL and version 3 enabled**; GPL-3.0 text and source links are included |
| **PySide6 / Qt / shiboken6** | Bundled license files and LGPL information; check the terms applying to the exact runtime build |
| **vgmstream interactive decoder** | Its bundled `COPYING`, README and source reference |
| **Python, PyInstaller, Mutagen, imageio-ffmpeg** | Their individual packaged notices and source information |

For source references, see `Third-party notices/Sources.txt` **inside the Public ZIP**. Its Qt libraries are dynamically linked within the installed `_internal` directory so compatible replacements may be possible.

**Compliance note:** having notices and source URLs is not, by itself, proof that every source-provision or redistribution obligation has been satisfied, especially for GPL-enabled FFmpeg, Qt-related packages or BASS licensing. Before further distribution, check the exact component licenses, build provenance, complete corresponding-source obligations and applicable permissions. This page is descriptive, not legal advice.

## Independent fan project

No Need for Speed game binaries, copyrighted EA soundtrack or commercially released song library is included. Users supply their own games and audio. This project is **not affiliated with, supported by, or endorsed by Electronic Arts**.

[Get the public package from Releases](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/releases) · [Report a licensing problem](https://github.com/ValentineBSAA/XNFS-Playlist-Builder-/issues/new/choose)
