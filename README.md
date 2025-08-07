# Customized Marlin 3D Printer Firmware for Ender-3 V3 SE

This repository contains customized Marlin 2.0 firmware specifically for the _Ender-3 V3 SE_ 3D Printer.

It includes the following customizations from the Stock firmware released by Creality:

- Raise max nozzle temp from 260°C to 300°C
    - NOTE: Requires Ceramic Hotend upgrade to use max temp safely
- Raise max bed temp from 100°C to 110°C
- Increase Z homing speed
- Increase max speeds and accelerations
- Enable host action commands (OctoPrint)
- Enable Linear Advance
   - Backported from mainline Marlin by [queeup](https://github.com/queeup-Forks/Ender-3V3-SE)
- Extend auto-levelling to use 7x7 grid
   - Patch by [aschmitt1909](https://github.com/aschmitt1909/Ender-3V3-SE)

To build run:

```
> make firmware
```

This will execute the build using dockerised plaformio. Build artifacts will be written to `.pio/build/STM32F103RET6_creality`.


# Marlin 3D Printer Firmware

<img align="right" width=175 src="buildroot/share/pixmaps/logo/marlin-250.png" />

Additional documentation can be found at the [Marlin Home Page](https://marlinfw.org/).

This repository is a customized fork and is not representative of the Official Marlin 2.0 project.


## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
