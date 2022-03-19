## 14.03.2022.
- Fixed issue with keystore where apps would crash when invoking it (Security related apps mostly like signal and a lot of work apps)
- Officially rebranded as 19.1
- Updated changelog URL in updater app to point to a valid changelog
- Fixed battery icon styles (Again..)
- Removed invalid zram config.
- Cleaned up source
- Performance and stability improvements
- Updated some stock apps to math with new design
- Synced with LineageOS source

## 10.03.2022.
- Merged March 2022. security and feature updates (Android 12L)
- Fixed status bar network trafic monitor
- Improved zram performance and enabled zram writeback
- Cleaned up patches needed for build
- Fixed network usage monitoring
- Fixed per app network restrictions
- Removed AudioFX which was causing issues
- Decreased microphone and earpiece gain a bit to mitigate in-call issues
- Updated some device control apps like advanced display settings
- Improved vibrator intensity in new hal
- Imrpoved fp sensor response time
- A lot of 'under the hood' changes
- Performance improvements
- Merged more previously missing los features
- Implemented OTA updates

## 10.02.2022.
- Merged February 2022. security update
- Removed broken volume button location toggle
- Synced with LOS source

## 09.02.2022.
- Fixed issue where camera would stop working after prolonged use
- Misc performance and stability improvements
- Merged some more lineageos features that have been posted to gerrit
- Synced with LOS source


## 28.01.2022.
- Fixed developer options crashing on launch
- Added Bluetooth SBC Dual Channel HD audio mode
- Synced with LOS source

## 27.01.2022.
- Added back lineageos setup wizard present on clean installs
- Merged some of previously missing features that have been ported over to LineageOS 19
- Performance and stability improvements
- Synced with LOS source

## 18.01.2022.
- Enabled selinux (Its enforcing now)
- Moved audio hal to vendor
- Fixed confirmation dialog box for button backlight
- Fixed ok button which would go missing for button backlight
- Switched to source built secril_config_svc (used for ds detection)
- Removed obsolete debug.sf.disable_backpressure prop
- Merged latest security updates to kernel from aosp kernel/common
- Cleaned up source
- Cleaned up unused props
- Removed unused custom ld.config.txt that was overriding main one
- Misc performance and stability improvements
- Synced with LOS source

## 06.01.2022.
- Removed duplicate props in vendor and system
- Cleaned up device tree code
- Switched to source built camera provider lib
- Switched to few source built ril related libs
- Addressed more selinux denials
- Fixed volume panel location settings
- Added button backlight
- Added Advanced Reboot
- Added LiveDisplay entry into settings
- Added system side toggle for navigation bar
- Merged January 2022 Security Update
- Merged most of previously missing LineageOS features
- Misc performance and stability improvements
- Synced with LOS source


## 20.12.2021.
- Fixed wireless display
- Reduced logspam which should imrpove performance a bit
- Misc performance and stability improvements
- Synced with LOS source

## 16.12.2021.
- Merged r18 tag of Android 12 (SQ1D.211205.016.A1)
- Removed liboemcrypto which was preventing drm playback in some apps
- Synced with LOS source

## 13.12.2021.
- Updated Clearkey to 1.4
- Addressed most of selinux denials
- Switched to new AIDL Lights hal
- Upreved audio hal to 7.0
- Switched to new AIDL Vibrator hal
- Disabled configstore which got replaced with props
- Upreved fingerprint hal/service to 1.3
- Removed unused kernel defconfig flag
- Synced with LOS source

## 09.12.2021.
- Merged December 2021. Security update
- Merged December 2021 pixel feature drop
- Added signature spoofing support which can be used to add microg instead of gapps
- Merged a lot of lineageos features that have been implemented
- Fixed bluetooth sample rate while in call
- Moved device specific ueventd rules to /system/vendor/etc
- Freed up some ram
- performance and stability improvements

## 30.11.2021.
- Initial release
