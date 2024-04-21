## 21.04.2024.
- Merged April security update
- Synced with LineageOS source

## 19.03.2024.
- Merged March security update
- Synced with LineageOS source

## 18.02.2024.
- Merged February security update
- Synced with LineageOS source

## 16.01.2024.
- Merged January security update
- Synced with LineageOS source

## 12.12.2023.
- Merged December security update
- Synced with LineageOS source

## 20.11.2023.
- Merged November security update
- Synced with LineageOS source
- Fixed OTA updates

## 11.10.2023.
- Merged October 2023. Security Update
- Synced with LineageOS source

## 10.09.2023.
- Merged September 2023. Security update
- Synced with LineageOS source

## 08.08.2023.
- Merged August 2023. Security update
- Synced with LineageOS source

## 10.07.2023.
- Merged July 2023. Security update
- Synced with LineageOS source

## 06.06.2023.
- Merged June 2023. Security update
- Synced with LineageOS source

## 05.05.2023.
- Merged May 2023. Security update
- Misc performance and stability improvements
- Synced with LineageOS source

## 24.04.2023.
- Switched to more source built components from new Exynos 850/Linaro BSP
    - hwcomposer
    - memtrack
    - libion_exynos
    - libGrallocWrapper
    - gralloc
    - libcsc
    - libexynosscaler
    - libexynosgscaler
    - libhwjpeg
    - Whole OMX stack (libOMX.Exynos.*) and stagefrighthw
- cleaned up source and got rid of libutils vndk32 workaround
- Performance, stability and battery life improvements
- Synced with LineageOS source

## 12.04.2023.
- Merged April 2023. Security update
- Synced with LineageOS source

## 17.03.2023.
- Merged March 2023. Security update
- Synced with LineageOS source

## 11.02.2023.
- Merged February 2023. Security update
- Synced with LineageOS source

## 05.01.2023.
- Merged January 2023. Security update
- Misc performance and stability improvements
- Synced with LineageOS source

## 07.12.2022.
- Merged December 2022. Security update
- Synced with LineageOS source


## 09.11.2022.
- Merged November 2022. Security update
- Cleaned up patches list
- Synced with LineageOS source

## 05.10.2022.
- Merged october 2022. Security update
- Fixed samsungs bug with gps where it would start acting up over time
due to time rollover bug
- Synced with LineageOS source

## 07.09.2022.
- Merged September 2022. Security update
- Updated chromium webview to 105.0.5195.79
- Synced with LineageOS source

## 07.08.2022.
- Merged August 2022. Security update
- Synced with LineageOS source

## 07.07.2022.
- Merged July 2022. Security update
- Fixed more keystore issues
- Synced with LineageOS source

## 24.06.2022.
- Fixed issues with keystore present in a lot of bank/secure apps like binance
- Fixed issue where setupwizard would crash when adding fingerprint due to bug in keystore
- Cleaned up patches required for build and removed unneeded ones
- Synced with LineageOS source

## 07.06.2022.
- Merged June 2022. security update
- Merged June 2022. pixel feature drop (SQ3A.220605.009.A1)
- Improved in-call audio quality drastically 
- Addressed few more selinux denials
- Improved general stability and performance
- Cleaned up source
- Synced with LineageOS source

## 26.05.2022.
- Updated libexynosdisplay from BSP to comply with some android 12 changes
- Removed unused build.prop entries
- Fixed few selinux denials related to hwc props
- Improved UI performance and stability
- Cleaned up source
- Removed more unneeded patches for device support
- Synced with LineageOS source

## 18.05.2022.
- Added QR code reader quick settings toggle
- Improved device performance and stability
- Added Custom low power mode power profile for cpu
- Improved A-GNSS (A-GPS) Lock speed
- Exposed device hw revision to settings
- Improved fast/slow charger detection
- Synced with LineageOS source

## 10.05.2022.
- Switched to new libperfmgr power hal which can be configured from /system/vendor/etc/powerhints.json
- Adapted DT2W to new power hal
- Muted phone services gps notif (Thanks google really appreciate you breaking random things for everyone)
- Improved battery life and performance
- Cleaned up all of leftover patches that were used by legacy power hal
- Synced with LineageOS source

## 07.05.2022.
- Improved battery usage logging for display
- Added QR code reader to camera app (Long hold icon and launch it from context menu)
- Misc performance and stability improvements
- Merged May 2022. security update
- Synced with LineageOS source

## 27.04.2022.
- Removed libbfqio dependency from hwc since it was dropped from lineageos 19.1
- Misc performance and stability improvements
- Synced with LineageOS source (same base as official builds + some extras)

## 18.04.2022.
- Fixed bug wehre vibrations were too low on some devices due to inintensity being set to 0
- Fixed bug where apps would show square popup "animation" when launching from icon instead of roudned one
- Cleaned up build patches
- Synced with LineageOS source

## 15.04.2022.
- Updated sepolicy and merged updated common samsung_slsi sepolicy
- Increased microphone gain while recording media (Camcorder, voice recording etc.)
- Added option to disable vibration feedback on fingerprint auth
- Synced with LineageOS source

## 08.04.2022.
- Fixed extended volume panel
- Updated icons for few more stock apps
- Cleaned up patches further
- Misc peroformance improvements
- Synced with LineageOS source

## 06.04.2022.
- Merged April 2022. Security update
- Enabled new LineageOS icons (you might have to clear launcher cache for them to show up)
- Fixed issue where galery app would show black text on black background
- Fixed issue where unlock sound would sometimes play twice
- Misc performance and stability improvements
- Synced with LineageOS source

## 29.03.2022.
- Drastically speed up app launch time [(more info about this here)](https://forum.xda-developers.com/t/lineageos-19-1-android-12l-signature-spoofing-ota-updates-for-s7-exynos.4368995/page-31#post-86657191)
- Imrpoved performance and battery life by disabling some unnecessary logging
- Switched to source built camera provider and removed samsung proprietary one
- Upreved camera provider to 2.5
- Fixed few selinux denials related to NFC trying to raad debug props
- Removed floating_feature.xml which is unused on aosp
- Disabled livedisplay by default
- Cleaned up extra dependencies used for compiling 
- Synced with LOS source

## 22.03.2022.
- Added back configurable audio volume panel location
- Speed up unlock with fingerprint
- Updated a lot of apps to MaterialYou design language
- Fixed issue where touch screen area bellow home button would act as a gesture area even while gestures are disabled
- Improved stability of ADB connection
- Implemented new LineageOS setupwizard
- Cleaned up device tree and list of required patches
- Stability and performance improvements
- Pointed Changelog url in updater app to new page
- Synced with LineageOS source

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

{% include donations.md %}
