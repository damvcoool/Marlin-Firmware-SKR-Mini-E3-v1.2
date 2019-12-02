<img align="right" width=175 src="buildroot/share/pixmaps/logo/marlin-250.png" />

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

Creality Ender-3 with SKR Mini E3 v1.2 and Creality BLTouch 3.1

## Features Enabled

- BLTouch (Bi-Linear Bed Leveling)
- Custom Status Screen (Ender-3 Default)
- Disable Boot Screens
- Disable Info Screen
- Enabled Slim Menus
- Enabled S Curve Acceleration
- Disable ARC Support (Cura does not have arc support anyway)
- Enabled Linear Advance
- Enabled Square Wave Stepping
- Enabled Hybrid Threshold for TMC2209 Stepper Drivers
- Bed Size is 230x230mm
- Enable Menu to Level Bed Corners (and Center)
- Pre-Heat for "PLA" and "PETG"
- Fix for EEPROM saving issue

## BLTouch Wiring

I will be updating this picture later to be more clear, the BLTouch Probe cables should go in the Dedicated Probe PIN PC14, not on the Z-Endstop as others suggest.

<img src="https://github.com/damvcoool/Marlin-2.0.x-SKR-Mini-E3-v1.2/blob/master/img/SKR%20Mini%20E3%20v1.2%20-%20Ender%203%20-%20Creality%20BLTouch%203.1%20Wiring.png"/>

Please note that ANTCLabs cable colors could be differnet.

## Binary File is in the BIN Folder

Please make sure to go over the configuration of the system before installing this Firmware.

4 Flavors, with self explanatory names, BLTouch use a 5x5 grid to probe, and Manual Bed Leveling uses a 3x3 grid.

- [SKR_Mini_E3_v1.2_256K_BLTouch_v3.1](https://raw.githubusercontent.com/damvcoool/Marlin-2.0.x-SKR-Mini-E3-v1.2/master/bin/SKR_Mini_E3_v1.2_256K_BLTouch_v3.1.bin)
- [SKR_Mini_E3_v1.2_256K_Manual_Bed_Level](https://raw.githubusercontent.com/damvcoool/Marlin-2.0.x-SKR-Mini-E3-v1.2/master/bin/SKR_Mini_E3_v1.2_256K_Manual_Bed_Level.bin)

I am no longer providing 512k variant.

## Credits

The current Marlin dev team consists of:

- Scott Lahteine [[@thinkyhead](https://github.com/thinkyhead)] - USA &nbsp; [Donate](http://www.thinkyhead.com/donate-to-marlin) / Flattr: [![Flattr Scott](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=thinkyhead&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)
- Roxanne Neufeld [[@Roxy-3D](https://github.com/Roxy-3D)] - USA
- Chris Pepper [[@p3p](https://github.com/p3p)] - UK
- Bob Kuhn [[@Bob-the-Kuhn](https://github.com/Bob-the-Kuhn)] - USA
- João Brazio [[@jbrazio](https://github.com/jbrazio)] - Portugal
- Erik van der Zalm [[@ErikZalm](https://github.com/ErikZalm)] - Netherlands &nbsp; [![Flattr Erik](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=ErikZalm&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)

## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
