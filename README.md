# Marlin 3D Printer Firmware

## Building Marlin 2.0

To build Marlin 2.0 you'll need [PlatformIO](http://docs.platformio.org/en/latest/ide.html#platformio-ide). We've posted detailed instructions on [Building Marlin with PlatformIO for ReArm](http://marlinfw.org/docs/basics/install_rearm.html) (which applies well to other 32-bit boards).

## Current Target

Creality Ender-3 with SKR Mini E3 v1.3 and Creality BLTouch 3.1

## Features Enabled

- BLTouch (Bi-Linear Bed Leveling)
- Custom Status Screen (Ender-3 Default)
- Disable Boot Screens
- Disable Info Screen
- Enabled Slim Menus
- Disabled Chamber Thermal Protection (I do not use a cage for my Ender-3, it runs free!)
- Enabled S Curve Acceleration
- Disable ARC Support (Cura does not have arc support anyway)
- Enabled Linear Advance 
- Enabled Hybrid Threshold for TMC2209 Stepper Drivers
- Bed Size is 225x225mm
- Enable Menu to Level Bed Corners (and Center)
- Pre-Heat for "Fillament Cold Pull" instead of Pre-heat for ABS
- Fix for EEPROM saving issue
- Using SoftwareSerialM instead to be able to use up-to-date TMCStepper library, instead of BTT outdated library.

## BLTouch Wiring

<img src="https://github.com/damvcoool/Marlin-2.0.x-SKR-Mini-E3-v1.2/blob/master/img/SKR%20Mini%20E3%20v1.2%20-%20Ender%203%20-%20Creality%20BLTouch%203.1%20Wiring.png"/>

Please note that ANTCLabs cable colors could be differnet.

## Binary File is in the BIN Folder

Please make sure to go over the configuration of the system before installing this Firmware.

## Credits

The current Marlin dev team consists of:

 - Scott Lahteine [[@thinkyhead](https://github.com/thinkyhead)] - USA &nbsp; [![Flattr Scott](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=thinkyhead&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)
 - Roxanne Neufeld [[@Roxy-3D](https://github.com/Roxy-3D)] - USA
 - Bob Kuhn [[@Bob-the-Kuhn](https://github.com/Bob-the-Kuhn)] - USA
 - Chris Pepper [[@p3p](https://github.com/p3p)] - UK
 - João Brazio [[@jbrazio](https://github.com/jbrazio)] - Portugal
 - Erik van der Zalm [[@ErikZalm](https://github.com/ErikZalm)] - Netherlands &nbsp; [![Flattr Erik](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=ErikZalm&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)

## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
