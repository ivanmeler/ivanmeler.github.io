## 23.04.2023.
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

## 11.04.2023.
- Merged April 2023. Security update
- Updated selinux and removed neverallow rules to make device more secure
- Fixed some issues introduced in QPR2
- Synced with LineageOS source

## 21.03.2023.
- Fixed double tap to wake

## 20.03.2023.
- Merged March 2023. Security update
- Misc performance and stability improvements
- Merged QPR2
- Added aptX HD support
- Synced with LineageOS source

## 23.02.2023
- First public Note FE/7 builds

## 21.02.2023.
- Further Improved UI performance
- Misc performance and stability improvements
- Began process of adding Note FE/7 support to universal8890-common codebase
- Synced with LineageOS source

## 08.02.2023.
- Merged February 2023. Security update
- Improved UI performance
- Misc stability improvements
- Fixed race condition in rotation that would rarely prevent screen from waking up
- Synced with LineageOS source

## 04.01.2023.
- Merged January 2023. Security update
- Camera app improvements
- Misc performance and stability improvements
- Synced with LineageOS source

## 15.12.2022.
- Added back some features that were missing from QPR1
- Misc performance and stability improvements
- Synced with LineageOS source

## 09.12.2022.
- Merged December 2022. Security update
- Merged android QPR1 December update
- Synced with LineageOS source

## 19.11.2022.
- Cleaned up patches used for non-BPF kernel
- Performance stability and battery life improvements
- Synced with LineageOS source

## 09.11.2022
- Merged November 2022. Security update
- Misc performance and stability improvements
- Cleaned up patches source
- Synced with LineageOS source

## 04.10.2022.
- Merged october 2022. Security update
- Improved UI performance
- Fixed issues that were caused by nav bar changes
- Improved stock camera app
- Cleaned up list of patches needed to reproduce builds
- Synced with LineageOS source

## 01.10.2022.
- Fixed samsungs bug with gps where it would start acting up over time
due to time rollover bug
- Implemented gesture navigation settings
- Removed leftover unused blobs
- Updated neural network interface lib
- Synced with LineageOS source

## 28.09.2022.
- Added button backlight control
- Unpinned deprecated updatable media apex jar from ram
- Allowed system to override some bluetooth props
- Performance and stability improvements
- Synced with LineageOS source (Almost all of lineageos features should be there and work now)

## 19.09.2022.
- Removed libhidl hacks and updated libs that required it in past
- Switched to new audio service to remove need for hacks in original one
- Updated kernel build flags for new build enviroment
- Misc performance and stability improvements
- Synced with LineageOS source

## 08.09.2022.
- Merged September 2022. Security update
- Updated chromium webview to 105.0.5195.79
- Added more customization options powered by Monet
- Misc performance and stability improvements
- Synced with LineageOS source

## 06.09.2022.
- Most of lineageos features have been implemented
- Misc performance and stability improvements
- Synced with LineageOS source

## 25.08.2022.
- Initial release

{% include donations.md %}
