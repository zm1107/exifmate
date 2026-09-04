<div align="center">

<img src="assets/img/logo.png" width="170" alt="ExifMate">

# ExifMate

**Photo & video metadata — see it all, fix it in bulk, undo anything.**

A fully offline EXIF viewer / repair / batch editor for Windows.

**🛡️ Fully offline &nbsp;·&nbsp; 🔄 Lifetime history &nbsp;·&nbsp; 🎬 Video support &nbsp;·&nbsp; ⚡ Multithreaded &nbsp;·&nbsp; 📅 Batch date repair &nbsp;·&nbsp; 🕐 Timestamp write-back &nbsp;·&nbsp; ✏️ Templated rename**

`Windows 10 / 11` · `Free + Full Edition`

[Website exifmate.com](https://exifmate.com) · [Microsoft Store](https://apps.microsoft.com/search?query=ExifMate) · [Privacy Policy](https://exifmate.com/privacy/) · [Feedback](https://github.com/zm1107/exifmate/issues)

☕ [Buy me a coffee](#buy-me-a-coffee)

<!-- TODO: replace with the official store listing URL once published; add a screenshot here -->

</div>

<p align="center"><a href="README.md">简体中文</a> · <b>English</b></p>

## What it solves

| The problem | ExifMate's answer |
|---|---|
| Camera clock was wrong — thousands of photos with wrong dates | Shift or set capture dates in bulk; sync file timestamps to match |
| Old scans with no date metadata sink to the bottom | Smart filename recognition writes missing dates back; RAW+JPG pairs cross-fill |
| Batch editing means command-line tutorials | A GUI covering all of ExifTool — write any tag visually, in bulk |
| You notice the mistake after the batch ran | Every operation is snapshotted — restore any step or batch with one click |
| Video metadata (phone / drone clips) has no tooling | Native support for MP4 / MOV / MKV / MTS and a dozen more formats |
| Photos leak your location when shared | Strip GPS and device serials in one click — or batch-write copyright info |

## Features

- **See everything** — grouped tree view of all metadata, before/after diff highlighting, RAW embedded-JPEG preview, inline video playback
- **Multithreaded throughout** — hashing, EXIF reading, batch writing and renaming each run in their own thread pools, so large batches stay fluid
- **Undo anything, history kept for life** — every operation is permanently stored in a local log (file hashes + before/after snapshots); it survives restarts, and any step or historical batch can be restored with one click
- **Timestamp write-back** — batch-set a file's **creation & modification times** from its date taken (or a date recognized from the filename; creation time via Windows system API) — Explorer sorting and backup archives snap into place
- **Templated batch rename** — combine date taken, camera model, sequence number, original name and extension into output templates (e.g. `{Y4}{M2}{D2}_{h}{m}{s}_{相机型号}`); same-second shots auto-suffix `_01/_02`; full preview before renaming
- **Smart recognition** — filename-recognition placeholder syntax (`{Y4}{M2}{D2}_{h}{m}{s}`, wildcards `{seg}` `{*}`), multi-template ordered matching
- **Fully offline** — zero networking, zero accounts, zero telemetry. Privacy by architecture, not promise

**Formats**: JPEG / PNG / GIF / BMP / TIFF / WebP / HEIC; major RAW (CR2 / CR3 / NEF / NRW / ARW / RAF / PEF / SRW / DNG); video: MP4 / M4V / MOV / AVI / MKV / WMV / FLV / WebM / MTS / M2TS / MOD / MPG.

## Free vs Full Edition

| | Free | Full Edition |
|---|---|---|
| All features | ✓ | ✓ |
| Files per batch | ≤ 10 | Unlimited |
| Priority support | — | ✓ |
| Price | Free | One-time purchase |

Purchased on the [Microsoft Store](https://apps.microsoft.com/search?query=ExifMate); free updates through 1.x.

## Privacy

ExifMate runs **fully offline**: no networking code, no personal data collection — your photos never leave your PC. See the [privacy policy](https://exifmate.com/privacy/).

## Feedback

- 🐛 [GitHub Issues](https://github.com/zm1107/exifmate/issues) (recommended, English & Chinese)
- 📧 dev@exifmate.com

## About this repository

This repository hosts the source of the official website (exifmate.com). The app ships as closed source, built on [ExifTool](https://exiftool.org) (Artistic License 2.0) and other open-source components; license notices ship with the software.

## Acknowledgments

ExifMate stands on the shoulders of these excellent open-source projects — our sincere thanks to their authors and to the open-source community:

| Project | Used for | License | Home |
|---|---|---|---|
| [ExifTool](https://exiftool.org) | EXIF / XMP / QuickTime metadata engine | Artistic License 2.0 | Copyright 2003-2026, Phil Harvey |
| [Qt / PySide6](https://www.qt.io) | GUI framework | LGPL-3.0 | The Qt Company |
| [Pillow](https://python-pillow.org) | Image decoding & preview | MIT-CMU | Python Pillow community |
| [pillow-heif](https://github.com/bigcat88/pillow_heif) | HEIC / HEIF support | MIT | bigcat88 |
| [xxHash](https://github.com/Cyan4973/xxHash) | File hashing (restore verification) | BSD-2-Clause | Yann Collet |
| [SQLite](https://www.sqlite.org) | Local operation-history database | Public Domain | SQLite developers |
| [Python](https://www.python.org) | Runtime | PSF License | Python Software Foundation |
| [cryptography](https://github.com/pyca/cryptography) | Integrity verification signing | Apache-2.0 | pyca |

Thank you to all open-source contributors — you make it possible for an independent developer to build professional-grade tools.

## Buy me a coffee

If ExifMate has been useful to you, consider buying the developer a coffee ☕ — your support fuels continued updates.

<p align="center">
  <img src="assets/img/coffee-wx.jpg" alt="WeChat QR code" width="260">
</p>

> Scan the QR code above with WeChat to chip in — every bit is appreciated.
