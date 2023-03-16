# HP Probook 440 G4 - OpenCore Configuation

<img align="right" src="https://raw.githubusercontent.com/ssimondev/hackintosh/main/screenshot.png" alt="macOS Ventura running on the HP Probook 440 G4" width="425">

[![macOS](https://img.shields.io/badge/macOS-Ventura-orange.svg)](https://developer.apple.com/documentation/macos-release-notes)

<p align="center">
   <strong>Status: Maintained</strong>
   <br />
   <strong>Version: </strong>1.0.0
   <br />
   <a href="https://github.com/ssimondev/hackintosh/releases"><strong>Download now »</strong></a>
   <br />
   <a href="https://github.com/ssimondev/hackintosh/issues">Report Bug</a>
   ·
   <a href="https://github.com/ssimondev/hackintosh/blob/main/EFI">View EFI</a>
  </p>
</p>
</br>

## ⚠️ Disclaimer
This guide is only for the HP Probook 440 G4. I am NOT responsible for any harm you cause to your device. This guide is provided "as-is" and all steps taken are done at your own risk.

> Style of this README are from [Valnoxy](https://github.com/Valnoxy/t480-oc).

&nbsp;

## Introduction
<details>
<summary><strong>💻 My Hardware</strong></summary>
<br>
These are the Hardware component I use. But this OpenCore configuation <strong>should still work</strong> with your device, even if the components are not equal.

> **Note** Check the model of your WiFi & Bluetooth card. Intel cards should be compatible with itlwm and <a href="https://github.com/OpenIntelWireless/HeliPort/releases"><strong>
HeliPort app</strong></a>. If your card is from another manufacturer, please check if your card supports macOS.

| Category  | Component                            |
| --------- | ------------------------------------ |
| CPU       | Intel Core i5-7200U                  |
| GPU       | Intel HD Graphics 620                |
| SSD       | Samsung MZNTY256HDHP-000H1 SSD       |
| Memory    | 4GB DDR4 2133Mhz                     |
| Camera    | 720p Camera                          |
| WiFi & BT | Intel Dual Band Wireless-AC 7265     |

</details>  

## Post-install (optional)

<details>  
<summary><strong>💾 Install OpenCore to Hard drive</strong></summary>
</br>

1. Press `ALT + SPACE` and open terminal. Type `sudo diskutil mountDisk disk0s1` (where disk0s1 corresponds to the EFI partition of the main disk)
2. Open Finder and copy the EFI folder of your USB device to the main disk's EFI partition.
3. Unplug the USB device and reboot your laptop. Now you can boot macOS without your USB device.

</details>



## Status

<details>  
<summary><strong>✅ What's working</strong></summary>
</br>
 
- [X] Intel WiFi & Bluetooth (thanks to [itlwn](https://github.com/OpenIntelWireless/itlwm))
- [X] Brightness / Volume Control
- [X] Battery Information
- [X] Audio (Audio Jack & Speaker)
- [X] USB Ports & Built-in Camera
- [X] Graphics Acceleration
- [X] PS2 Touchpad
- [X] Power management / Sleep
- [X] FaceTime / iMessage (iServices)
- [X] HDMI
- [X] Handoff / Universal Clipboard
- [X] USB-C

</details>

<details>  
<summary><strong>⚠️ What's not working</strong></summary>
</br>

- [ ] Safari DRM ```Use Chromium powered Browser or Firefox to watch Amazon Prime Video, Netflix, Disney+ and others```
- [ ] AirDrop & Continuity
- [ ] Fingerprint Reader

</details>

<details>  
<summary><strong>🔄 Not tested</strong></summary>
</br>

- [ ] SideCar
- [ ] Automatic OS updates
- [ ] Dualbooting Windows / Linux (with OpenCore)

</details>

### Feel free to download and use my EFI folder :)
