# Skylake Desktop Hackintosh (i5 6600K)

OpenCore bootloader config files for my workstation hackintosh.

Intel iGPU is used for primary display even though my rig has a NVIDIA RTX 2080 since it doesn't have supported drivers 😞. I should sell my RTX and buy a compatible AMD card.

## System Information

| Name     |                    Model |
| :------- | -----------------------: |
| CPU      | Intel i5 6600K (Skylake) |
| GPU      |             Intel HD 530 |
| SSD      |           M.2 SATA 256GB |
| WiFi     | TP-Link T9E (BCM driver) |
| Board    |     ASUS Z170 Pro gaming |
| Ethernet |              Intel I219V |

- OpenCore: v0.6.3
- MacOS: v11.1 BigSur
- OpenCanopy theme: <https://github.com/tekteq/opencanopy-minimal-theme>

## Guide

<https://dortania.github.io/OpenCore-Install-Guide/prerequisites.html>
<https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html>

### SMBIOS

Selected: `iMac17,1`

Don't forget to change device uuid, board serials and network mac address
Go to <https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html#platforminfo> For information on setting up SMBIOS platform info

## Kexts Used

| Package               | Version |
| :-------------------- | ------: |
| AppleALC              |   1.5.5 |
| Lilu                  |   1.5.0 |
| WhateverGreen         |   1.4.5 |
| VirtualSMC            |   1.1.9 |
| SMCProcessor          |   1.1.9 |
| SMCSuperIO            |   1.1.9 |
| AirportBcrmFixup      |   1.4.5 |
| IntelMausi            |     xxx |
| CPUFriendDataProvider |     xxx |

## What's not working

- Sleep wake not working with Intel HD 530. (Turn off auto sleep/poweroff in settings)

## Post Install

- Change OpenCore to release version
- Upgrade OpenCore versions
  