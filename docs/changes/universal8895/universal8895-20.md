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

## 08.11.2022
- Merged November 2022. Security update
- Switched to new AIDL usb hal
- Switched kernel back to clang toolchain
- Misc performance and stability improvements
- Synced with LineageOS source

## 04.10.2022.
- Merged october 2022. Security update
- Improved UI performance
- Improved stock camera app
- Synced with LineageOS source

## 01.10.2022.
- Fixed samsungs bug with gps where it would start acting up over time
due to time rollover bug
- Synced with LineageOS source

## 28.09.2022.
- Adressed missing symbol in advanced camera effects lib that wouldnt launch without them
- Allowed system to override some bluetooth props
- Performance and stability improvements
- Synced with LineageOS source (Almost all of lineageos features should be there and work now)

## 21.09.2022.
- Switched to Generic FunctionFS usb backend (We used legacy functionfs in past)
- Updated USB hal
- Usb hal will now give notifications on port being wet instead of just disabling it without notice
- Merged few more missing BPF commits to kernel
- Unpinned deprecated updatable media apex jar from ram
- Synced with LineageOS source

## 19.09.2022.
- Updated kernel build flags for new build enviroment
- Misc performance and stability improvements
- Switched to source built Bluetooth interface
- Cleaned up device source
- Synced with LineageOS source

## 07.09.2022.
- Merged September 2022. Security update
- Updated chromium webview to 105.0.5195.79
- Added more customization options powered by Monet
- Misc performance and stability improvements
- Synced with LineageOS source

## 06.09.2022.
- Fixed home button wake

## 05.09.2022.
- Fixed camera on Note 8
- Most of lineageos features have been implemented
- Misc performance and stability improvements
- Synced with LineageOS source

## 01.09.2022.
- Fixed bluetooth audio
- Upreved audio hal to 7.1 from 5.0
- Implemented custom audio service used to load audio hal
- Backported more BPF changes to kernel
- Switched to webview 105.0.5195.68 which is native to T
- Cleaned up the source and patches used to build the rom
- Synced with LineageOS source

## 27.08.2022.
- Initial release

{% include donations.md %}
