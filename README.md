# TWRP Device configuration for Samsung Galaxy A41

## Device specifications :

Basic    | Spec Sheet
--------:|:----------------------
Chipset  | MediaTek Helio P65
CPU      | Octa-core (Cortex-A55 , Cortex-A75)
GPU      | Mali-G52 MC2
Memory   | 4GB , 8GB RAM (LPDDR3 , LPDDR4X)
Storage  | 64GB
Support Model | SM-A415F (global) , SCV48 (jp) , SC-41A (jp) 
Shipped Android version | Android 10 , OneUI 2.5
Codename | a41xx
Battery  | Li-Poly 5000mAh , non-removable
Display  | LCD , 60Hz , 6.1 inch , 1080 × 2400 pixels , 20:9 ratio

[Telegram Support Group](https://t.me/a31nsxx)

## Status :

```diff
+ Mostly Stable.
- Releases tagged as "Pre-release" are considered experimental and may cause more unexpected stuff than the latest release , nobody is forced to support your in older releases.
```
## Theme :

Set the ``TW_CUSTOM_THEME`` flag for a custom theme.

## How to Compile :

```
source build/envsetup.sh; export ALLOW_MISSING_DEPENDENCIES=true; lunch twrp_a41-eng; mka recoveryimage
```

## How to install :

> - Flash the latest .tar release from [releases](https://github.com/Galaxy-MT6768/teamwin_device_samsung_a41xx/releases), it may require Magisk patched vbmeta.img
>
> - Hold the recovery combination (Volume Up + Power) while the .tar is flashing via the odin tool.
>
> - You can now boot into your system and do whatever you want.

## Working Features List :
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
> - [ ] vibrate
> - [x] screenshot
> - [ ] partition SD card

## Special thanks to :

> [TeamWin](https://github.com/TeamWin) for the Recovery Project.
> 
> [Physwizz](https://github.com/physwizz) for his [a145f-S kernel](https://github.com/physwizz/A415f-S) (ligther version was used on this tree).
>
> [Zillion](https://github.com/DevZillion) for owner the device tree.
>
> [Edwin's](https://github.com/EdwinT2) for config.