# Q5 Mint ROM

Custom ROM for the Q5 / MT6582 based on Android KitKat, designed as a simple, lightweight, and visually consistent mint-green experience.

This release started from the idea of turning the device into a minimalist MP3 player. Pressing the Home button takes you directly to the music player, creating a more focused experience for listening to music, viewing lyrics, and using the device as a dedicated player. Even so, access to the traditional Android app launcher is still available, so the ROM is not limited to the music player only.

## Personal Note About The Device

I bought this device on AliExpress because it was very cheap and accessible. One curious detail is that the included manual shows an image of another model, the Q5 Timmkoo, and I could not find clear documentation explaining the differences between the variants.

From what I was able to observe, this device seems to use a very similar official base, but with small differences likely made to reduce cost. Unfortunately, this version appears to have been discontinued quickly: I can no longer find the same device for sale on AliExpress, while the more expensive version of this model still seems to be the better-known one.

To distinguish this ROM and this specific device, I use the name "Q5 Mint", since this unit has a very noticeable mint-green color.

## Highlights

- Mint-green interface, with large text and icons for better readability on a small screen.
- Adjusted SystemUI with larger clock, battery percentage, and icons, centered and visually cleaner.
- Music player integrated as the main Home button experience.
- Boot animation and splash timing adjusted for a smoother startup transition.
- Notes app visually adjusted to match the ROM's mint style.
- ROOT access already configured.
- APKs compatible with Android KitKat can still be installed normally when needed.

## Apps And Services

This ROM does not include Google services. Android KitKat is already a discontinued base, so the goal here is to keep the system light and functional within the real limitations of the device.

There is still a limited Google Chrome-based browser, useful for simple browsing, but full compatibility with modern websites should not be expected.

## Separate Exercises APK

There is also a separate exercises APK. It was not included inside `system.img` because it became too large to be convenient as a system app in this release.

The best option is to provide that APK as a separate file on GitHub, alongside the ROM, for manual installation when desired.

## Installation

Use SP Flash Tool with the scatter file included in the package.

Main included files:

- `MT6582_Android_scatter.txt`
- `boot.img`
- `system.img`
- `logo.bin`
- `lk.bin`
- `cache.img`
- `userdata.img`

Important recommendation: do not flash the `preloader` if it appears in another package or backup. This release was prepared to update the required ROM components without touching the preloader.

## Release Package

Recommended file:

`Q5_MINT_ROM_2026-08-27_GITHUB_RELEASE_FIXED.zip`

Hashes:

- SHA256: `2D2C8A9D0E1ECE9D0A7BC8CA743A7E8FB94249F6BD558C4214D2FD70F11F9FD2`
- MD5: `0ECF91A4F7ED6A92EED979A3835329E9`

The previous package without the `FIXED` suffix has been replaced by this one.

## Notes

This ROM was made specifically for the Q5 / MT6582. Use it at your own risk, and keep a backup of the device's original ROM.

Because this is Android 4.4 KitKat, some modern apps may not install or may not work correctly. For best results, use APKs explicitly compatible with KitKat.

⚠️ Pay attention to the two variants of this same TIMMKOO Q5 model. Confusing them will cause the flash to install normally, but it will fail in the following cases:
- Device enters charging mode but does not charge
- Device audio only works with headphones
- Home button does not work
- Volume + and - are inverted.

If for any reason you have this problem, correct it before the battery runs out.
