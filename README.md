<div align="center">

# Eliminater74

### Michael H. | Android Systems Developer · PureFusion Tools

**ROM and kernel engineering | Reverse engineering | IPTV platforms | Windows tooling | VR systems**

Largo, Florida · GitHub since 2014 · 280+ public repositories

</div>

---

## What I build

I take systems that are slow, opaque, or locked down and put measurable control back in the operator's
hands. That started as custom Android — kernels, recoveries, ramdisks, device trees — and it is the
same instinct in everything I ship now: IPTV players, Windows device managers, PCVR tray tools,
firmware extractors, and browser extensions.

Latency, stability, and direct control are the requirements. I treat remote-click delay, zap time,
and headset session recovery as engineering problems, not polish. I ship installers, signed betas,
and repeatable GitHub Actions pipelines, not just source trees.

A lot of the current product work is private. Public repos are the tools, SDKs, docs, and utilities
that other people actually run.

---

## Current work

### PureFusion IPTV

Private Android TV / Google TV / handheld **player**. It does not provide channels, playlists, or
subscriptions — you bring your own M3U, Xtream, or Stalker source. Current line is **2.0 Beta-22**,
in Open Testing on Google Play, with a full public launch aimed at early 2027.

[Play Store](https://play.google.com/store/apps/details?id=dev.eliminater.purefusioniptv)
· [Open Beta](https://play.google.com/apps/testing/dev.eliminater.purefusioniptv)
· [Website](https://purefusioniptv.web.app/)
· [Public docs](https://github.com/Eliminater74/PurefusionIPTV-docs)
· [Repo](https://github.com/Eliminater74/PureFusionIPTV) *(private)*

- Media3 / ExoPlayer with two engines: Standard, and **FastZap** (pooled, pre-buffered live surfing)
- Canvas-rendered EPG, D-pad-first navigation, catch-up where the provider actually serves an archive
- Movies / series paging that no longer blocks on counting the whole catalogue
- Local network sync, encrypted backup, Google Drive / WebDAV, PIN-gated Web Admin
- Consent-based crash reports, Stats for Nerds, and a sandboxed plugin runtime with a circuit breaker
- Physically tested on real TVs, not only emulators

**Plugin ecosystem** *(private)* — the host app is closed source; plugins build against the API alone.

| Project | Role |
| --- | --- |
| [Plugin API](https://github.com/Eliminater74/PurefusionIPTV-plugin-api) | Open SDK: `Plugin`, media-server, cloud-storage, and sync contracts |
| [Emby plugin](https://github.com/Eliminater74/PurefusionIPTV-Plugin-emby) | Standalone `MediaServerProvider` for Emby libraries |
| [Google Drive plugin](https://github.com/Eliminater74/PurefusionIPTV-Plugin-googledrive) | Standalone Drive cloud storage / sync provider |

### Meta Quest Tray Tool

Windows tray hub for Meta Quest / Oculus Link and SteamVR OpenXR. Built as a clean C# project, not a
continuation of older Oculus Tray Tool conversions. Current release: **v1.1.35**.

[github.com/Eliminater74/MetaQuestTrayTool](https://github.com/Eliminater74/MetaQuestTrayTool)

- Per-game profiles that auto-apply on launch and restore global defaults on exit
- Link bitrate / encode / sharpening (including high-bitrate presets), OpenXR Meta vs SteamVR
- Bundled ADB headset tweaks (CPU/GPU, refresh, FFR), wireless pairing, Quest-only device trust
- Hotkeys and voice commands for in-headset control when an elevated tray cannot be clicked
- Recover PCVR, Dash → SteamVR over Link, audio routing, power plans, in-app updates

### Android TV Manager

Windows WPF toolbox for Android TV / Google TV boxes. Not an adbLink clone and not a Kodi utility.
Current release: **1.0.0-B19**.

[github.com/Eliminater74/AndroidTVManager](https://github.com/Eliminater74/AndroidTVManager)

- USB, TCP/IP ADB, and Android 11+ wireless debugging, with saved devices that stay visible offline
- Evidence-backed device status, HDMI/HDCP/CEC diagnostics, and a conservative, source-attributed debloat catalog
- App Installer for APK, split APK, APKS, APKM, and XAPK (including OBB copy)
- Recovery / sideload, logcat, scripts, deployment profiles, and disable-first restore journals

### PureFusion Earth

PCVR globe in Unreal Engine + Cesium: grab, scale, and fly a streaming planetary Earth over OpenXR
(SteamVR / Quest Link). **In progress** — Cesium for Unreal is wired; globe, georeference, pawn, and
two-hand interaction are next.

[github.com/Eliminater74/PureFusionEarth](https://github.com/Eliminater74/PureFusionEarth) *(private)*

### Browser tooling

| Project | What it is |
| --- | --- |
| [PureFusion Feed](https://github.com/Eliminater74/PureFusion-Feed) | Manifest V3 Facebook extension: DOM cleanup plus an **on-device** ranking / classification engine. Feed data stays in the browser. |
| [PureFusion Filtration](https://github.com/Eliminater74/PureFusion_Filtration) | Manifest V3 modernization of FB Purity: ads, clutter, themes, tracking-parameter stripping. |
| [PureFusion Torrent Bridge](https://github.com/Eliminater74/Purefusion-TorrentBridge) | Manifest V3 magnet / `.torrent` sender to local or remote BitTorrent clients, rebuilt after Chrome killed older extensions. |

---

## Other shipping products

### Vehicle, firmware, and embedded

| Project | What it is |
| --- | --- |
| [ATOTO Firmware Downloader](https://github.com/Eliminater74/atoto_firmware_downloader) | Most-starred public tool. Finds, downloads, and optionally unpacks firmware for ATOTO S8 / A6 / F7 / P8 / X10 and related head units. v2.4.0. |
| [ATOTO Toolkit 2025](https://github.com/Eliminater74/ATOTO-TOOLKIT_2025) | On-device Android toolkit for ATOTO S8: hardware check, cautious debloat, wireless ADB (including root TCP/IP on Android 10). |
| [AsBuilt Explorer](https://github.com/Eliminater74/AsBuiltExplorer) | Windows toolkit for Ford `.ab` / `.abt` data: SQLite vehicle DB, offline feature matching, side-by-side compare, CRC calculators, NHTSA VIN decode. |
| [PreFusion Firmware Tools](https://github.com/Eliminater74/PreFusion-Firmware-Tools) | Windows Ext2/3/4 + LVM reader, native BinWalk-style scan, Android `payload.bin` / sparse / brotli OTA utilities. |
| [eXtended Parameter Designer](https://github.com/Eliminater74/eXtended-Parameter-Designer) | GUI for Infineon-style e-bike controller parameters (Python 3 port). |

### Windows desktop and VR worlds

| Project | What it is |
| --- | --- |
| [PureFusion IRC](https://github.com/Eliminater74/PureFusionIRC) | Windows WPF IRC client with an mIRC-style layout, IRCv3, JSON themes, JS scripts, reverse DCC. **v1.0.0-B3**. |
| [Redline: Zombie Assault](https://github.com/Eliminater74/Redline_Zombie_Assault_Horizon_worlds) | Meta Horizon Worlds wave survival: TypeScript AI, spawn pooling, XP, five leaderboards. **v26.1.4**. |
| [NTLite presets](https://github.com/Eliminater74/NTLite_Presets_Configs_2023) | Windows image-slim presets and configs. |
| [Android TV AppDrawer](https://github.com/Eliminater74/org.lineageos.appdrawer) | Leanback app drawer so non-ATV apps actually show on Android TV. |

---

## How I got here

The current products sit on about a decade of Android and Linux systems work under **The Nebula
Project**.

**Custom Android (2014–2017).** Kernel governors and I/O schedulers, device trees, recoveries, and
ROM packaging. Named work from that period:

- **Nebula Kernel** and [Nebula Kernel Updater](https://github.com/Eliminater74/Nebula_Kernel_Updater) — performance kernels plus an in-app updater
- [Kernel Tweaks](https://github.com/Eliminater74/Kernel_Tweaks) — governors and I/O schedulers that other trees actually forked
- **MultiROM on LG G3** — [device trees](https://github.com/Eliminater74/multirom_g3_devices) and [kexec hardboot patches](https://github.com/Eliminater74/d851_multirom_patches) across D85X / F400 / LS990 / VS985
- [SpaceX-Pure](https://github.com/Eliminater74/SpaceX-Pure) — root on Android 5.1.1 / 6.0 with a **stock kernel** and SELinux still enforcing; ramdisk only
- Kernel Adiutor forks / [BlackBox Toolkit](https://github.com/Eliminater74/BlackBox-Toolkit), Linaro / SaberMod toolchains, LG G3 and HTC 10 / Samsung Tab S trees

**Firmware, routers, and TV (2018–2022).** OpenWRT GitHub Actions for Linksys WRT3200ACM, private
router images, Android TV launchers and app drawers, Amlogic research tools, NTLite Windows images.

**Product era (2023–now).** The same low-level habits — read the binary, measure the path, automate
the build — applied to shipping apps: PureFusion IPTV, Windows WPF managers, Quest PCVR, ATOTO
firmware, Ford As-Built, Chrome MV3 extensions, Unreal OpenXR, Horizon Worlds.

---

## Technical stack

<div align="center">

![Android](https://img.shields.io/badge/Android-Systems-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-Android-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Java](https://img.shields.io/badge/Java-Android-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![C#](https://img.shields.io/badge/C%23-Windows-239120?style=for-the-badge&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-Desktop-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-Native-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-Tooling-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Systems-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-Automation-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Chrome](https://img.shields.io/badge/Chrome-Extensions-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white)
![Unreal](https://img.shields.io/badge/Unreal-Engine-0E1128?style=for-the-badge&logo=unrealengine&logoColor=white)
![VR](https://img.shields.io/badge/VR-OpenXR-5B5FC7?style=for-the-badge&logo=meta&logoColor=white)

</div>

---

## Specializations

- Android platform work: Kotlin, Java, native code, ADB, recovery, boot images, device trees
- Kernel and ROM engineering: governors, I/O, kexec / MultiROM, ramdisk-only root, SELinux-preserving flows
- Reverse engineering: APK / JADX, firmware (Ext, OTA payload, BinWalk-style scan), As-Built bitfields
- IPTV and Android TV: Media3 playback, EPG, FastZap, Leanback UX, plugin SDKs, Play Integrity / billing
- Windows desktop: C# WPF for device management, PCVR, IRC, and firmware GUIs, with Inno Setup releases
- Embedded and vehicle: ATOTO head-unit firmware, Ford As-Built, Infineon e-bike controllers
- Automation: GitHub Actions, locked restores, tagged Setup.exe / AAB pipelines
- Immersive: OpenXR + Quest Link, Unreal / Cesium, Horizon Worlds TypeScript

---

## GitHub metrics

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

## Development footprint

| Area | Focus |
| --- | --- |
| Android systems | ROMs, platform behavior, ADB, device integration |
| Kernel work | Governors, I/O, boot flows, kexec, low-level debugging |
| Reverse engineering | APKs, firmware images, As-Built, runtime integrations |
| IPTV and media | Playback, EPG, Android TV navigation, plugins, Play beta |
| Windows desktop | WPF device managers, PCVR tray, IRC, firmware readers |
| Vehicle / embedded | ATOTO head units, Ford configs, e-bike controllers |
| Automation | GitHub Actions, repeatable builds, tagged releases |
| Linux and firmware | OpenWRT, Ext/LVM, OTA payloads, router images |
| VR and immersive | OpenXR, Quest Link, Cesium globe, Horizon Worlds |

---

## Engineering principles

- Measure before optimizing
- Keep systems fast, observable, and maintainable
- Prefer direct control over unnecessary abstraction
- Treat UX latency and runtime stability as engineering requirements
- Build tooling that can be repeated, audited, and improved
- Test on the hardware the user actually holds

<div align="center">

**Performance first. Clean systems. Build it right.**

</div>
