# fdroid-priv-magisk
Magisk package to install F-Droid privileged extension.
Based on the documentation by topjohnwu at https://topjohnwu.github.io/Magisk/guides.html#magisk-modules, using the official release from https://github.com/f-droid/privileged-extension/

## Two Caveats
1. Security concerns: While a Magisk package can receive automatic updates, you should not accept those from an untrusted source like me! Magisk enables us to do all sorts of things with root privileges. It wouldn't be too difficult to create an update that installs some kind of malware on your phone. A far better approach would be what I ended up doing: Create your own package, where you know exactly what it contains, and what it does with this contents.
2. Compatibility: This package has been tested with only two phones, a Xiaomi RedMi Note 8 (A-only device, real partitions), runnning LineageOS 18.1, and a Pixel 3a (A/B device with dynamic partitions), running LineageOS 20, both rooted with Magisk 26.4. The extension apk is installed to /system/app-priv/, which should also work for most other devices, but this hasn't been tested and is out of scope for this package. Please note that some custom roms (for example LineageOS for microG) already include the extension. Installing this package _should_ not break anything, but again: It hasn't been tested.

## Prerequisites
A phone rooted with Magisk, version 26.4 or higher is recommended. (Actually, always running the latest Magisk release is recommended - and you should always get it directly from the source at https://github.com/topjohnwu/Magisk/tags/) 

## Usage
Copy the zip package to your phone and load it as a module in Magisk. Reboot. That's it, thanks to topjohnwu :-)
