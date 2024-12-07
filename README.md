<p align="center">
  <img src="https://raw.githubusercontent.com/OrangeFoxRecovery/.github/fox/profile/OrangeFox.jpg" alt="OrangeFox Logo" width="400">
</p>

<h1 align="center">OrangeFox for m31s</h1>

## Overview

This repository contains the OrangeFox Recovery Project build for the Samsung Galaxy M31s (m31s).

## Features

- Custom recovery based on TWRP
- Enhanced user interface
- Advanced backup and restore options
- Customizable themes
- Support for decryption

## Installation

1. Download the latest release
2. Boot into download mode (make sure you have the disabled vbmeta.img)
4.  - Flash the recovery using Odin or heimdall (could do using the img after renaming the OrangeFox .img to recovery.img and tarring)
    - Flash the zip from the official TWRP
5. Reboot into recovery

## Building

To build OrangeFox for m31s, Check the workflow action for reference:

For detailed instructions, please refer to the [OrangeFox documentation](https://wiki.orangefox.tech/en/home).

## Issues and Support

If you encounter any issues or need support, please open an issue in this repository.

## Credits

This project wouldn't be possible without the following:

- [OrangeFox Recovery Project](https://orangefox.download/)
- [TWRP](https://twrp.me/)
- [Exynos 9611 GitLab Repository](https://gitlab.com/OrangeFox/device/exynos9611)

Special thanks to all contributors and maintainers of the Exynos 9611 GitLab repository for their valuable work and resources.

## Flashing a Custom ROM 

> Old version of Alphadroid (where RIL worked) doesnt work through install zip or adb sideload, can use lineageOS (May, only using sideload) for that. 

You can flash a custom rom like qnttechh's [Alphadroid](https://sourceforge.net/projects/qnttechh/files/samsung/m31s/AlphaDroid-V2.4/) using below steps

- Format data -> yes
- Reboot to recovery (optional)
- Flash the rom and Gapps (Optional, used this version of [MindtheGapps](https://github.com/MindTheGapps/14.0.0-arm64/releases/download/MindTheGapps-14.0.0-arm64-20240612_135921/MindTheGapps-14.0.0-arm64-20240612_135921.zip), But can try latest version, Dirty flashing/Flashing after booting -> No Play Integrity, Normal -> Meets Basic Integrity)
- Use the Kernel from [here](https://github.com/mlm-games/kernel_samsung_exynos_9611) for KSU and then can use the Play Integrity Fix module for play store cert.

Tested AlphaDroid on m31s and has few bugs like
- RIL (mobile network and calls are very unstable)
- NFC (Doesnt disable it for phones released in different regions)
- Auto Rotate (Doesnt work)

This project is licensed under [GPL-3.0](LICENSE).
