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

## 07.06.2023.
- Merged June 2023. Security update
- Synced with LineageOS source

## 05.05.2023.
- Merged May 2023. Security update
- Synced with LineageOS source

## 12.04.2023.
- Merged April 2023. Security update
- Synced with LineageOS source

## 19.03.2023.
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
- Switched to hidl usb hal from hw/samsung
- Synced with LineageOS source

## 05.10.2022.
- Merged october 2022. Security update
- Fixed samsungs bug with gps where it would start acting up over time
due to time rollover bug
- Adressed missing symbol in advanced camera effects lib that wouldnt launch without them
- Performance and stability improvements
- Switched to Generic FunctionFS usb backend (We used legacy functionfs in past)
- Synced with LineageOS source

## 07.09.2022.
- Switched to a rebased kernel
- Updated kernel to 4.4.302
- Added BPF support to kernel
- Removed no longer needed bpf hacks for system
- Misc performance and stability improvements
- Merged September 2022. Security update
- Updated chromium webview to 105.0.5195.79
- Synced with LineageOS source

## 07.08.2022.
- Merged August 2022. Security update
- Synced with LineageOS source

## 07.07.2022.
- Reverted some changes that caused previous ui performance regression
- Merged July 2022. Security update
- Synced with LineageOS source

## 05.07.2022.
- Improved LMKD behavior
- Improved power hal behaviour and performance boosting
- Tuned surfaceflinger behavior
- Improved ui performance further
- Fixed more keystore issues
- Synced with LineageOS source

## 04.07.2022.
- Fixed HWC
- Improved gcam ports compatibility and post processing speed
- Major battery life and ui performance imporvements
- Synced with LineageOS source

## 23.06.2022.
- Fixed issues with keystore present in a lot of bank/secure apps like binance
- Fixed issue where setupwizard would crash when adding fingerprint due to bug in keystore
- Cleaned up patches required for build and removed unneeded ones
- Synced with LineageOS source

## 08.06.2022.
- Merged June 2022. security update
- Merged June 2022. pixel feature drop (SQ3A.220605.009.A1)
- Cleaned up source
- Synced with LineageOS source

## 27.05.2022.
- Added Dolby audio effects support (from stock) (Access it from quick settings)
- Fixed bixby button mapping that got broken yesterday
- Cleaned up kernel dt2w patches
- Removed broken soundtrigger hal that was causing issues with "Ok Google" detection
- Removed unused audio.playback_record hal
- Synced with LineageOS source

## 26.05.2022.
- Added shim for setLayerBuffer function in hwc, further down the line said shim will be used to fix hwc
- Further improvements for dt2w on devices that previously had issues with it
- Removed more unneeded patches for device support
- Synced with LineageOS source

## 19.05.2022.
- Added WireGuard kernel implementation
- Added QR code reader quick settings toggle
- Improved device performance and stability
- Improved A-GNSS (A-GPS) Lock speed
- Exposed device hw revision to settings
- Improved fast/slow charger detection
- Improved double tap to wake detection on some devices
- Remaped bixby to menu so long hold, short hold and wake actions work
- Long hold on bixby is now handling multitasking
- Improved bluetooth stability
- Synced with LineageOS source

## 11.05.2022.
- Adapted DT2W support (double tap to wake)
- Muted phone services gps notif (Thanks google really appreciate you breaking random things for everyone)
- Improved battery life and performance
- Fixed issue where some devices would not wake up touch after being in sleep mode
- Cleaned up all of leftover patches that were used by legacy power hal
- Synced with LineageOS source
- Released source on https://github.com/8890q/

## 06.05.2022.
- Improved bluetooth in call audio sample rate handling
- Added FB notifier callbacks to kernel
- Added always on display support
- Switched to new power hal with custom fine tuned power profile
- Improved battery usage logging for display
- Added QR code reader to camera app (Long hold icon and launch it from context menu)
- Disabled unneeded debugging in kernel that was slowing things down
- A lot of performance stability and battery life improvements
- Cleaned up device tree
- Merged May 2022. Security update
- Synced with LineageOS source

## 27.04.2022.
- Removed High touch sensitivity (glove mode) support from S8+ build as device lacks proper support for it

## 26.04.2022.
- Included support for High touch sensitivity (glove mode)
- Cleaned up vintf manifest and added target level to it
- Synced with LineageOS source (Same functionas as offical builds of 19.1 have + some extras)

## 18.04.2022.
- Fixed limit for enrolling fingerprint and set it to 4 like on stock
- Improved wifi speed
- Improved battery life
- Fixed auto brightness debounce time to prevent abrupt changes
- Added support for more mDNIe display profiles
- Improved SQLite performance
- Added vibration intensity controls (Under accesibility settings)
- Added multi user support
- Added surfaceflinger and few other services to pinner to keep them in ram
- Enabled 4g+ icon when connected to 4g+ network
- Cleaned up patches used for build
- Synced with LineageOS source

## 14.04.2022.
- Switched to new audio hal that supports interface v5
- Fixed usb audio
- Fixed audio in screen recoidng recording and wireless display sharing
- Improved bluetooth audio stability and compatibility
- Started rewriting sepolicy
- Updated wifi firmware
- Merged latest available kernel source from samsung(G955FXXUCDUD1/G950FXXUCDUD1/N950FXXSGDUG7)
- Merged latest blobs available from samsung(G955FXXUCDUD1/G950FXXUCDUD1/N950FXXSGDUG7)
- Implemented fast charging toggle in battery settings
- Removed unneeded libmemset shim
- Added support for user configurable wireless charging sound
- Added switch to disable vibration on fp unlock
- Removed non-functional srgb toggle from dev options
- Removed liboemcrypto.so to fix L3 drm playback
- updated LPM binaries
- Cleaned up device tree and kernel repo
- A lot of under the hood performacne and stability improvements
- Synced with LineageOS source

## 08.04.2022.
- Fixed extended volume panel
- Fixed build fingerprint for dream2lte and greatlte that was causing safetynet to fail
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

## 31.03.2022.
- Improved app launch speed
- Improved general performance and battery life
- Upreved camera provider to 2.5
- Disabled livedisplay by default
- Cleaned up extra dependencies used for compiling
- Synced with LOS source

## 22.03.2022.
- Added back configurable audio volume panel location
- Speed up unlock with fingerprint
- Updated a lot of apps to MaterialYou design language
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
- Cleaned up source
- Performance and stability improvements
- Updated some stock apps to math with new design
- Synced with LineageOS source

## 11.03.2022.
- Merged March 2022. security and feature updates (Android 12L)
- Fixed status bar network trafic monitor
- Improved zram performance and enabled zram writeback
- Cleaned up patches needed for build
- Fixed network usage monitoring
- Fixed per app network restrictions
- Removed AudioFX which was causing issues
- Decreased microphone gain a bit to mitigate in-call issues
- Updated some device control apps like advanced display settings
- Fixed s-pen pointer offset for note8
- Imrpoved fp sensor response time
- Added cgroup profile config
- A lot of 'under the hood' changes
- Performance improvements
- Merged more previously missing los features
- Implemented OTA updates

## 10.02.2022
- Merged February 2022 security update
- Synced with LOS source

## 09.02.2022.
- Fixed bug where camera would stop working after prolonged use due to file-descriptiors being left open and overflowing
- Fixed torch delay
- Fixed issues with camera auto focus locking up the camera
- Switched to half res boot anim which in turn gives us a slight boost in boot time
- Removed arrow pointer (used for s-pen or mouse input) from non note8 builds and updated pointer for note8 build
- Cleaned up unneeded drm entries in hidl manifest
- Misc performance and stability improvements
- Disabled CONFIG_RT_GROUP_SCHED in kernel in order to remove system hack we previously needed
- Merged some previously missing LOS features
- Synced with LOS source

## 19.01.2022.
- Switched to source built librilutils
- Switched to source built libreference-ril
- Switched to source built secril_config_svc used for dual/single sim detection
- Updatd way samle rates are handled for bt headsets in call
- Misc performance and stability improvements
- Synced with LOS source

## 07.01.2022.
- Fixed volume panel location settings
- Added Advanced Reboot
- Added LiveDisplay entry into settings
- Merged January 2022 Security Update
- Merged most of previously missing LineageOS features
- Misc performance and stability improvements
- Synced with LOS source

## 21.12.2021.
- Fixed wireless display
- Reduced logspam which should imrpove performance a bit
- Misc performance and stability improvements
- Synced with LOS source

## 17.12.2021.
- Merged r18 tag of Android 12 (SQ1D.211205.016.A1)
- Synced with LOS source

## 14.12.2021.
- Disabled legacy configstore which got replaced with props
- Switched to new AIDL Lights hal
- Enabled zram swap
- Misc performance and stability improvements
- Synced with LOS source

## 10.12.2021.
- Fixed issue where system would experience random freezes in some apps

## 09.12.2021.
- Merged December 2021. Security update
- Merged December 2021 pixel feature drop
- Added signature spoofing support which can be used to add microg instead of gapps
- Merged a lot of lineageos features that have been implemented
- Fixed bluetooth sample rate while in call
- Moved device specific ueventd rules to /system/vendor/etc
- Uprevved fp hal to 2.3
- Implemented fingerprint gestures
- fixed system audio recording in apps such as screen recorders
- performance and stability improvements


## 03.12.2021.
- Initial release

{% include donations.md %}
