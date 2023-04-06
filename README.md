# Marlin 3D Printer Firmware

[![Build Status](https://travis-ci.org/MarlinFirmware/Marlin.svg?branch=2.0.x)](https://travis-ci.org/MarlinFirmware/Marlin)
![GitHub](https://img.shields.io/github/license/marlinfirmware/marlin.svg)
![GitHub contributors](https://img.shields.io/github/contributors/marlinfirmware/marlin.svg)
![GitHub Release Date](https://img.shields.io/github/release-date/marlinfirmware/marlin.svg)

_Marlin_ is a firmware for RepRap machines, also known as _3D printers_. firmware to the next level by adding support for much faster 32-bit and ARM-based boards while improving support for 8-bit AVR boards through the use of a "hardware abstraction layer."

Additional documentation can be found at the [Marlin Home Page](http://marlinfw.org/).
Please let us know if Marlin misbehaves in any way. Volunteers are standing by!

### BigTreeTech Updated their Firmware, get it here:
https://github.com/bigtreetech/BIGTREETECH-SKR-mini-E3

## Building Marlin 2.0

To build Marlin you'll need [Arduino IDE 1.8.8 or newer](https://www.arduino.cc/en/main/software) or [PlatformIO](http://docs.platformio.org/en/latest/ide.html#platformio-ide) with _[Visual Studio Code](https://code.visualstudio.com/download)_.

- [Installing Marlin (Arduino)](http://marlinfw.org/docs/basics/install_arduino.html)
- [Installing Marlin (VSCode)](http://marlinfw.org/docs/basics/install_platformio_vscode.html).

## Current Target

Creality Ender-3 with SKR Mini E3 v1.2, Creality BLTouch 3.1 and Dualgear Extruder.

## Features Enabled

- BLTouch (Bi-Linear Bed Leveling)
- Assisted Bed Tramming (Using BLTouch)
- Custom Status Screen (Ender-3 Default)
- Disable Boot Screens
- Disable Info Screen
- Enabled S Curve Acceleration
- ARC Support (Install Cura plugin ArcWelder to use it.)
- Enabled Linear Advance
- Enabled Square Wave Stepping
- Bed Size is 228x228mm
- Enable Menu to Level Bed Corners (and Center)
- Enable Probe Offset Wizard
- Assisted Probe to Nozzle Z-Offset
- Pre-Heat for "PLA" and "PETG" and "HOT-PLUG"

## BLTouch Wiring

I will be updating this picture later to be more clear, the BLTouch Probe cables should go in the Dedicated Probe PIN PC14, not on the Z-Endstop as others suggest.

<img src="img/SKR%20Mini%20E3%20v1.2%20-%20Ender%203%20-%20Creality%20BLTouch%203.1%20Wiring.png?raw=true"/>

Please note that ANTCLabs cable colors could be differnet.

## Binary File is in the BIN Folder

Please make sure to go over the configuration of the system before installing this Firmware.

- [SKR_Mini_E3_v1.2_256K_BLTouch_v3.1](bin/SKR_Mini_E3_v1.2_BLTouch_v3.1.bin?raw=true)

## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
