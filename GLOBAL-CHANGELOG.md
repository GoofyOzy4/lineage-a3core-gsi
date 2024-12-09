# V1 - First release
## Vanilla :
- First Release
- Added optimizations in phh-on-boot , phh-on-data , /system/bin/one-boot.sh .
- Added Samsung A03 Core info props. (build.prop and /product/build.prop).
- Added optimizations in build.prop and fixed 4:45 bootloops on Samsung A03 Core.
- Offline charging "fixed" . Instead of stuck on samsung logo - you get reboot.
- Disabled background activity by default for these apps:
   - Camera / Aperture
   - Calendar
   - Gallery
   - Android Documents UI
   - Calculator
- Hided treble settings option.
- Removed ~420 useless treble overlays.
## Gapps :
- First release.
- Same changelog as Vanilla build.
- Added Google Services and etc. for stable work (Thanks to LiteGApps)
---
# Changelog for V2 (2024-12-05) :
## Vanilla:
- Removed 4 treble overlays
- Debloated rw-system.sh (1144>435 lines) , and small on-data, on-boot debloat(~20  lines total in both files).
- Debloated useless stuff in /system/phh.
- Edited build.prop (removed oneplus orange status).
- Now it's "user" repack instead of "user-debug".
- Removed alot useless bin and etc from other phones.
- Removed CPU V-Sync Disabler tweak.
## Gapps:
- Same as Vanilla
- Maybe dropping gapps build in next update, because i can't check both builds.
- not tested
---
# What new here (changelog for V3, 2024-12-09) :
- Dropped GApps variant.
- Android update(Lineage OS 21).
- "Keeping" default build info.