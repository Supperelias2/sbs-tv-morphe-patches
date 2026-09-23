# Supperelias2 SBS TV Patches

Unofficial [Morphe](https://morphe.software) patches for the Android TV version
of SBS On Demand.

[Add this source to Morphe](https://morphe.software/add-source?github=Supperelias2/sbs-tv-morphe-patches)
· [Releases](https://github.com/Supperelias2/sbs-tv-morphe-patches/releases)
· [Report a problem](https://github.com/Supperelias2/sbs-tv-morphe-patches/issues)

## Patches

For SBS On Demand for Android TV **6.3.1 (16470)**:

- **Prefer direct VOD stream** selects an available direct Akamai HLS stream
  instead of Google DAI for on-demand playback.
- **Prefer direct live stream** does the same for live TV. Ads that are part of
  the broadcast remain.

Both patches retain the original provider selection if no non-empty direct URL
is available. Location requirements are unchanged.

<!-- PATCHES_START EXPANDED -->
<!-- PATCHES_END -->

## Install

Add this repository as a remote source in Morphe, select an original SBS TV
6.3.1 APKM and patch it. Both playback patches are enabled by default.

This project does not distribute SBS APKs, account data, stream URLs or signing
keys. It is not affiliated with SBS or Morphe. Licensed under [GPLv3](LICENSE).
