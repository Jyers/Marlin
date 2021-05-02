# Ender 3 V2 Extensible UI

This version of the Extensible UI is customized for my own needs. Using it could harm your device(s). This fork was created from Jyers/Marlin.

### Only these builds are compiled (in High-Speed mode and only for the 4.2.2. board)

- E3V2-UBL-BLTouch-5x5
- E3V2-UBL-BLTouch-10x10
- E3V2-UBL-BLTouch-15x15

### These are the customized settings for these builds:

```
#define DEFAULT_AXIS_STEPS_PER_UNIT { 80, 80, 400, 97.84 }
#define NOZZLE_TO_PROBE_OFFSET { -43, -7, 0 }
#define Z_MAX_POS 230
```
You can change the "e-Steps" within the firmware menu also. This is also the case for the "Nozzle to Probe Offset".

The hight is set to 230mm because I don't print that high. I also had some accidents where I scrolled the wheel to much in the menu and it went to all the way to the top. Because there is no "cancel" button after selecting a X,Y or Z position, I added this as a safety feature to my builds.

## Credits

Ender 3 V2 Extensible UI
https://github.com/Jyers/Marlin


The current Marlin dev team consists of:

 - Scott Lahteine [[@thinkyhead](https://github.com/thinkyhead)] - USA &nbsp; [Donate](https://www.thinkyhead.com/donate-to-marlin) / Flattr: [![Flattr Scott](https://api.flattr.com/button/flattr-badge-small.png)](https://flattr.com/submit/auto?user_id=thinkyhead&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)
 - Roxanne Neufeld [[@Roxy-3D](https://github.com/Roxy-3D)] - USA
 - Chris Pepper [[@p3p](https://github.com/p3p)] - UK
 - Bob Kuhn [[@Bob-the-Kuhn](https://github.com/Bob-the-Kuhn)] - USA
 - João Brazio [[@jbrazio](https://github.com/jbrazio)] - Portugal
 - Erik van der Zalm [[@ErikZalm](https://github.com/ErikZalm)] - Netherlands &nbsp; [![Flattr Erik](https://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=ErikZalm&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)

## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
