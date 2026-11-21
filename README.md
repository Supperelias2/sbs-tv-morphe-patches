# Supperelias2 SBS TV Patches

Unofficial [Morphe](https://morphe.software) patches for the Android TV version
of SBS On Demand.

[Add this source to Morphe](https://morphe.software/add-source?github=Supperelias2/sbs-tv-morphe-patches)
· [Releases](https://github.com/Supperelias2/sbs-tv-morphe-patches/releases)
· [Report a problem](https://github.com/Supperelias2/sbs-tv-morphe-patches/issues)

## Patches

For SBS On Demand for Android TV **6.3.1 (16470)** and **6.4.0 (16690)**:

- **Prefer direct VOD stream** selects an available direct Akamai HLS stream
  instead of Google DAI for on-demand playback.
- **Prefer direct live stream** does the same for live TV. Ads that are part of
  the broadcast remain.

Both patches retain the original provider selection if no non-empty direct URL
is available. Location requirements are unchanged.

CLI patching and rebuilding passed for 6.4.0 (16690) and 6.3.1 (16470).
Playback on 6.4.0 still needs device testing.

<!-- PATCHES_START EXPANDED -->
> **[v1.0.2-dev.1](https://github.com/Supperelias2/sbs-tv-morphe-patches/releases/tag/v1.0.2-dev.1)**&nbsp;&nbsp;•&nbsp;&nbsp;`dev`&nbsp;&nbsp;•&nbsp;&nbsp;4 patches total
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
