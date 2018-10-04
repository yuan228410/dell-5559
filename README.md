# Dell Inspiron 5559

This repo is for the 15" Dell Inspiron 5559 i5-6200U. It should work for the 17" model.

# Supported Versions

`config.plist` has a seperate version for Sierra/High Sierra and Mojave.

# What works (and what doesn't)

* Microphone (webcam/mic commbo, but no webcam)
* Bluetooth (Intel card still present, so no wifi)
* Display brightness
* IGPU
* Sleep
* Touchscreen (Completely independent of the OS. macOS does not natively support multi-touch)
* Touchpad/Trackpad with all gestures
* Speakers
* USB 3 and 2

# Persistent Bugs

At this time you have to rebuild kext cache every few reboots. If not done, the computer will panic and loop until you enter a fake id to boot and then rebuild kext cache. Internet speeds are crippled. With both LAN and USB 3 WiFi adapter. Due these factors I am no longer actively using Mojave. I downgraded to High Sierra.

# How to use

The best way to use this EFI config is visit the [releases page](https://github.com/cbabb/dell-5559/releases). Create an empty `EFI` folder on the mounted EFI partition of the macOS disk. Drag both the `BOOT` and `CLOVER` folders into it. There are no serials present. You will need to generate it with Clover config.

# TO DO

Fix backlight buttons, replace intel wifi card, and enable webcam.
