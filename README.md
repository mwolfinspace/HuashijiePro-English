# Huashijie Pro 3.4.6 — English portable edition

🇻🇳 Hướng dẫn tiếng Việt: [HUONG-DAN-VI.md](HUONG-DAN-VI.md)

A fully English, **install-free** Windows build of Huashijie Pro 3.4.6.
Extract the zip, double-click one file, start drawing.

## Download

| File | Size | SHA-256 |
|---|---|---|
| `HuashijiePro-English-3.4.6-win64.zip` | 257 MiB | `cdb9baeb9a370573da93ad819f47c7ccecb3779d923d70ab3a84723ee9293916` |

Get it from the [latest release](../../releases/latest).

## How to run

1. Download the zip and **extract the whole folder** (right-click → *Extract All…*).
2. Open the folder and double-click **`Start Huashijie Pro (English).exe`**.
3. Windows may warn about an unsigned app: *More info* → *Run anyway*.

That is all. No installer, no admin rights, no account required to draw.

The launcher seeds the translated brush library into `%LOCALAPPDATA%\HuashijiePro`
on the first run and then starts `hsjpro.exe`. Afterwards you can start
`hsjpro.exe` directly — the launcher only does the one-time seeding.

## What is translated

- Every menu, panel, dialog, tooltip, tool option popup and status line.
- Brush categories, 359 brush preset names, shortcut presets.
- Hotkey names, theme names, country and dial-code lists.
- Logo lockups.

Not translated on purpose: the WeChat/phone **login web page** (vendor HTML from
the vendor's server), vendor promo art, licence text, and source comments.

## Also fixed

An existing selection now **follows Flip Canvas** (the vendor's flip task only
flipped the pixels). This is a native patch in `hsjpro_engine.dll`: the flip
worker mirrors the selection mask and its rectangle, and fails soft on any
unexpected state.

## Requirements

Windows 10/11, 64-bit. Qt, the codecs and the MSVC runtime are bundled; nothing
else needs to be installed. ~1.6 GB free disk after extraction.

## Good to know

- Drawings and settings live in `%LOCALAPPDATA%\HuashijiePro` — that folder is
  your work; back it up.
- Drawing, filters, layers and export (PNG/JPG/PSD/TIFF/PDF/GIF/MP4) work offline.
  Cloud sync, login and sharing need the vendor's servers.
- **Do not use *Check for updates*** — an update replaces the English binaries
  with the vendor's Chinese ones. Download a new English build instead.

## Build provenance

The binaries are produced deterministically from the vendor's own 3.4.6 files by
a small translation kit (`VERDICT: OK`: identical file size and PE headers, zero
untranslated UI literals, zero slot overflows).

```
hsjpro.exe          8a193bbeae34f7dd564e215838d05ea5d69d1f551b7a607c88667c95b716993d
hsjpro_engine.dll   7333407ddc2ade86a4cecb0ded5f1300d43bb5a6c6829f1a20bd59c471b98874
```

## Disclaimer

Unofficial localisation for personal use. Huashijie Pro and all of its assets
belong to their original authors. This repository contains no vendor source
code, only a packaged copy of the vendor's distributed files with translated
strings and the selection fix. No warranty of any kind.
