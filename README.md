# Supperelias2 SBS TV Patches

Unofficial [Morphe](https://morphe.software) patches for the Android TV version
of SBS On Demand.

[Add this source to Morphe](https://morphe.software/add-source?github=Supperelias2/sbs-tv-morphe-patches)
· [Releases](https://github.com/Supperelias2/sbs-tv-morphe-patches/releases)
· [Report a problem](https://github.com/Supperelias2/sbs-tv-morphe-patches/issues)

## Patches

For SBS On Demand for Android TV **6.3.1 (16470)** and **6.4.0 (16690)**:

- **Prefer direct VOD stream** removes the video ads played before and during
  on-demand videos (pre-roll and mid-roll) by using SBS's direct Akamai stream.
- **Prefer direct live stream** removes the extra video ads inserted before or
  during live TV. Ads already present in the broadcast itself remain.
- **Allow sideloaded installation** prevents the Play Store redirect when
  launching the patched TV app.

Ad removal uses the direct stream when SBS supplies one. If it is unavailable,
the app keeps its normal playback path. Location requirements are unchanged.

CLI patching and rebuilding passed for 6.4.0 (16690) and 6.3.1 (16470).
Playback on 6.4.0 still needs device testing.

<!-- PATCHES_START EXPANDED -->
> **[v1.0.2](https://github.com/Supperelias2/sbs-tv-morphe-patches/releases/tag/v1.0.2)**&nbsp;&nbsp;•&nbsp;&nbsp;`main`&nbsp;&nbsp;•&nbsp;&nbsp;4 patches total
<details open>
<summary>📦 SBS On Demand for Android TV&nbsp;&nbsp;•&nbsp;&nbsp;4 patches</summary>
<br>

**🎯 Supported versions:**

| 6.4.0 | 6.3.1 |
| :---: | :---: |

| 💊&nbsp;Patch | 📜&nbsp;Description | ⚙️&nbsp;Options |
|----------|----------------|-----------|
| [Allow sideloaded installation](#allow-sideloaded-installation) | Prevents the Play licensing redirect when launching a sideloaded SBS TV build. |  |
| [Prefer direct VOD stream](#prefer-direct-vod-stream) | Prefers an available Akamai VOD stream over Google DAI. Keeps original selection for live or missing alternatives. Ad removal is not guaranteed. |  |
| [Prefer direct live stream](#prefer-direct-live-stream) | Prefers an available Akamai live stream over Google DAI. Broadcast ads remain. Keeps original selection when no direct stream is available. |  |
| [SBS playback compatibility check](#sbs-playback-compatibility-check) | Checks supported SBS TV playback integration points. Does not remove advertisements. |  |

</details>

<!-- PATCHES_END -->

## Install

Add this repository as a remote source in Morphe, select an original SBS TV
6.3.1 or 6.4.0 APKM and patch it. Both playback patches are enabled by default.

This project does not distribute SBS APKs, account data, stream URLs or signing
keys. It is not affiliated with SBS or Morphe. Licensed under [GPLv3](LICENSE).
