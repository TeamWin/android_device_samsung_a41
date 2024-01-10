# Samsung Galaxy A41 [SM-A415F] [a41xx] - Team Win Recovery Project
[Telegram Support Group](https://t.me/a31nsxx)
```diff
+ TWRP Status: Mostly Stable. 
- Releases tagged as "Pre-release" are considered experimental and may cause more unexpected stuff than the latest release, nobody is forced to support your in older releases.
```

```
git clone https://github.com/EdwinT2/android_device_samsung_a41xx -b android-12.1 device/samsung/a41

source build/envsetup.sh; export ALLOW_MISSING_DEPENDENCIES=true; lunch twrp_a41-eng; mka recoveryimage
```

### Special thanks to:
> [TeamWin](https://github.com/TeamWin) for the Recovery Project.
> 
> [Physwizz](https://github.com/physwizz) for his [A415f-S kernel](https://github.com/physwizz/A415f-S) (ligther version was used on this tree).
>
> [Zillion](https://github.com/DevZillion) for doing the device tree.
>
> [Edwin's](https://github.com/EdwinT2) for fix some issue.

### How to install
> Flash the latest .tar release from [releases](https://github.com/Galaxy-MT6768/android_device_samsung_a41xx/releases), it may require Magisk patched vbmeta.img
> 
> Hold the recovery combination (Volume Up + Power) while the .tar is flashing via the odin tool.
> 
> You can now boot into your system and do whatever you want.

### Working Features List
>
> - [x] Critial Partitions fail to unlock
>
> **Blocking checks**
> - [x] Correct screen/recovery size
> - [x] Working Touch, screen
> - [x] Backup to internal/microSD
> - [x] Restore from internal/microSD
> - [x] reboot to system
> - [x] ADB
>
> **Medium checks**
> - [ ] update.zip sideload
> - [ ] UI colors (red/blue inversions)
> - [x] Screen goes off and on
> - [x] F2FS/EXT4 Support, exFAT/NTFS where supported
> - [x] all important partitions listed in mount/backup lists
> - [x] backup/restore to/from external (USB-OTG) storage
> - [x] backup/restore to/from adb (https://gerrit.omnirom.org/#/c/15943/)
> - [ ] decrypt /data
> - [x] Correct date
>
> **Minor checks**
> - [ ] MTP export
> - [x] reboot to bootloader (download)
> - [x] reboot to recovery
> - [x] poweroff
> - [x] battery level
> - [x] temperature
> - [ ] encrypted backups
> - [x] input devices via USB (USB-OTG) - keyboard, mouse and disks
> - [ ] USB mass storage export
> - [x] set brightness
> - [] vibrate
> - [x] screenshot
> - [ ] partition SD card
