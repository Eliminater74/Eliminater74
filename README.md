<div align="center">

# Eliminater74

### Michael H. | Android Systems Developer

**ROM and kernel engineering | Reverse engineering | IPTV platforms | Automation | VR systems**

I build performance-focused Android and Linux systems, private media tooling, Windows desktop
utilities, automation pipelines, and low-level platform work where latency, stability, and
control matter.

</div>

---

## Current Projects

Recent work that is shipping, in open beta, or actively under development. Several repositories
are private; public repos are linked for source and releases.

### PureFusion IPTV

Private Android TV / Google TV IPTV **player** (not a content service) engineered for fast
playback, responsive guide navigation, and predictable performance on both low-end and high-end
devices. Current line is **2.0 Beta**, with Open Testing on Google Play.

[Play Store](https://play.google.com/store/apps/details?id=dev.eliminater.purefusioniptv)
· [Open Beta](https://play.google.com/apps/testing/dev.eliminater.purefusioniptv)
· [Website](https://purefusioniptv.web.app/)
· [Repo](https://github.com/Eliminater74/PureFusionIPTV) *(private)*

- Media3 / ExoPlayer playback with Standard and FastZap engines
- Fast channel switching, zap-performance tuning, and remote-first D-pad UX
- Canvas-rendered EPG, M3U / Xtream / Stalker playlists, catch-up where the provider supports it
- Cross-device sync, cloud backup, Web Admin, and a sandboxed plugin runtime
- Platform behavior tested against real-world device constraints

**Plugin ecosystem** *(private repos)*

| Project | Role |
| --- | --- |
| [Plugin API](https://github.com/Eliminater74/PurefusionIPTV-plugin-api) | Host SDK: `Plugin`, media-server, cloud-storage, and sync contracts |
| [Emby plugin](https://github.com/Eliminater74/PurefusionIPTV-Plugin-emby) | Standalone `MediaServerProvider` for Emby libraries |
| [Google Drive plugin](https://github.com/Eliminater74/PurefusionIPTV-Plugin-googledrive) | Standalone Drive cloud storage / sync provider |

### Meta Quest Tray Tool

Windows tray hub for Meta Quest / Oculus Link and SteamVR OpenXR. Per-game profiles, Link
bitrate and encode control, ADB headset tweaks, OpenXR switching, audio routing, hotkeys, and
in-headset voice commands. Current release: **v1.1.35**.

[github.com/Eliminater74/MetaQuestTrayTool](https://github.com/Eliminater74/MetaQuestTrayTool)

### Android TV Manager

Windows WPF toolbox for Android TV / Google TV device management: ADB discovery (USB, TCP/IP,
wireless debugging), package inventory, cautious device-aware debloat, App Installer (APK /
split / APKS / APKM / XAPK), recovery/sideload, diagnostics, and scripts. Current release:
**1.0.0-B19**.

[github.com/Eliminater74/AndroidTVManager](https://github.com/Eliminater74/AndroidTVManager)

### PureFusion Earth

PCVR globe in Unreal Engine + Cesium: grab, scale, and fly a streaming planetary Earth over
OpenXR (SteamVR / Quest Link). **In progress** — Cesium for Unreal is wired; globe, georeference,
and VR interaction come next.

[github.com/Eliminater74/PureFusionEarth](https://github.com/Eliminater74/PureFusionEarth) *(private)*

### PureFusion Feed

Privacy-first Chrome extension (Manifest V3) that restructures the Facebook DOM, strips
algorithmic junk, and ranks the timeline with an **on-device** prediction engine. No feed data
leaves the browser.

[github.com/Eliminater74/PureFusion-Feed](https://github.com/Eliminater74/PureFusion-Feed)

### PureFusion Torrent Bridge

Manifest V3 Chrome extension that sends `.torrent` and magnet links to local or remote
BitTorrent clients from the context menu, inline hooks, or a transfer dashboard.

[github.com/Eliminater74/Purefusion-TorrentBridge](https://github.com/Eliminater74/Purefusion-TorrentBridge)

---

## Also Shipping

| Project | What it is |
| --- | --- |
| [PureFusion IRC](https://github.com/Eliminater74/PureFusionIRC) | Windows WPF IRC client (mIRC-style layout, IRCv3, themes, scripts). Beta. |
| [ATOTO Firmware Downloader](https://github.com/Eliminater74/atoto_firmware_downloader) | Tool for downloading firmware for ATOTO car head units. |
| [ATOTO Toolkit 2025](https://github.com/Eliminater74/ATOTO-TOOLKIT_2025) | Android toolkit for ATOTO devices and APK workflows. |
| [AsBuilt Explorer](https://github.com/Eliminater74/AsBuiltExplorer) | Windows tool for exploring Ford As-Built vehicle configuration data. |
| [PureFusion Filtration](https://github.com/Eliminater74/PureFusion_Filtration) | Browser filtration / content-control tooling. |
| [PreFusion Firmware Tools](https://github.com/Eliminater74/PreFusion-Firmware-Tools) | Windows app to read and copy Ext2/3/4 (with LVM) partitions. |
| [IPTV docs](https://github.com/Eliminater74/PurefusionIPTV-docs) | Public documentation for the PureFusion IPTV player. |

---

## Platform History

Longer-running Android and Linux systems work that the current projects sit on top of.

- **PureFusion ROM**: custom Android ROM development
- **Nebula Kernel**: performance-focused Android kernel engineering
- **MultiROM LG G3 Port**: MultiROM support across LG G3 variants
- **Router firmware projects**: automated Linux firmware builds
- **VR / immersive projects**: experimental immersive application work, including Horizon Worlds

---

## Technical Stack

<div align="center">

![Android](https://img.shields.io/badge/Android-Systems-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-Android-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Java](https://img.shields.io/badge/Java-Android-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![C#](https://img.shields.io/badge/C%23-Windows-239120?style=for-the-badge&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-Desktop-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-Native-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Systems-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-Automation-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Chrome](https://img.shields.io/badge/Chrome-Extensions-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white)
![Unreal](https://img.shields.io/badge/Unreal-Engine-0E1128?style=for-the-badge&logo=unrealengine&logoColor=white)
![VR](https://img.shields.io/badge/VR-OpenXR-5B5FC7?style=for-the-badge&logo=meta&logoColor=white)

</div>

---

## Specializations

- Android platform engineering with Kotlin, Java, native code, and system-level debugging
- Reverse engineering with APK analysis, JADX, manifests, runtime behavior, and integration mapping
- ROM, kernel, recovery, boot image, and device-tree workflows
- IPTV, streaming playback, EPG systems, Android TV UX, and plugin SDKs
- Windows desktop tooling in C# / WPF for ADB, PCVR, and device management
- CI/CD automation with GitHub Actions and repeatable build pipelines
- Linux firmware, router workflows, Chrome extensions, and immersive OpenXR experiments

---

## GitHub Metrics

<div align="center">

<img width="100%" src="./github-metrics.svg" alt="GitHub profile overview metrics" />

<br><br>

<img width="100%" src="./metrics.languages.svg" alt="Language activity metrics" />

<br><br>

<img width="100%" src="./metrics.calendar.svg" alt="Contribution calendar metrics" />

<br><br>

<img width="100%" src="./metrics.lines.svg" alt="Lines changed metrics" />

<br><br>

<img width="100%" src="./metrics.stargazers.svg" alt="Stargazers metrics" />

<br><br>

<img width="100%" src="./metrics.notable.svg" alt="Notable contribution metrics" />

<br><br>

<img width="100%" src="./metrics.followup.svg" alt="Issue and pull request follow-up metrics" />

<br><br>

<img width="100%" src="./metrics.reactions.svg" alt="GitHub reactions metrics" />

<br><br>

<img width="100%" src="./metrics.people.svg" alt="People metrics" />

<br><br>

<img width="100%" src="./metrics.topics.svg" alt="Starred topics metrics" />

<br><br>

<img width="100%" src="./metrics.stars.svg" alt="Recently starred repositories metrics" />

<br><br>

<img width="100%" src="./metrics.starlists.svg" alt="Star lists metrics" />

<br><br>

<img width="100%" src="./metrics.discussions.svg" alt="GitHub discussions metrics" />

<br><br>

<img width="100%" src="./metrics.gists.svg" alt="Gists metrics" />

<br><br>

<img width="100%" src="./metrics.traffic.svg" alt="Repository traffic metrics" />

<br><br>

<img width="100%" src="./metrics.skyline.svg" alt="GitHub Skyline metrics" />

</div>

---

## Development Footprint

| Area | Focus |
| --- | --- |
| Android systems | ROMs, platform behavior, device integration |
| Kernel work | Performance tuning, boot flows, low-level debugging |
| Reverse engineering | APK analysis, manifests, app behavior, integrations |
| IPTV and media | Playback, EPG, Android TV navigation, latency, plugins |
| Windows desktop | WPF device managers, PCVR tray tools, IRC, firmware readers |
| Automation | GitHub Actions, repeatable builds, release workflows |
| Linux and firmware | Router firmware, shell workflows, system tooling |
| VR and immersive | OpenXR, Quest Link, Cesium globe, experimental apps |

---

## Engineering Principles

- Measure before optimizing
- Keep systems fast, observable, and maintainable
- Prefer direct control over unnecessary abstraction
- Treat UX latency and runtime stability as engineering requirements
- Build tooling that can be repeated, audited, and improved

<div align="center">

**Performance first. Clean systems. Build it right.**

</div>
