# The Sovol SV08 Omnibus

The Sovol SV08 Omnibus attempts to provide complete and extensive
documentation of the Sovol SV08 3D printer.

This repository started as a map of existing efforts to document and
improve this printer, to aid its author in the development of a clean
room operating system image using Yocto.  For more information about
that project, see the
[meta-sovol](https://github.com/zachwelch/meta-sovol) repository.

# Sovol

The [Sovol website](https://sovol3d.com/) provides the official
specifications and support materials.

## SVO8

* [Sovol SV08](https://www.sovol3d.com/products/sovol-sv08-3d-printer)
* [Firmware and Manuals](https://www.sovol3d.com/pages/download)
* [SV08 Open Source](https://github.com/Sovol3d/SV08)

## Support

The official support resources useful for those that want to run the
stock Sovol firmware images, but they are less relevant if you want to
make any mods to the hardware or software:

* [Sovol SV08 Wiki](https://wiki.sovol3d.com/en/SV08)
* [Sovol SV08 Forum](https://forum.sovol3d.com/c/everything-about-sv08/54)
* [Official Sovol Discord server](https://discord.gg/SPSp4Dg992)

# Resources

This section attempts to describe all known community documentation,
modifications, and projects for this printer.

## Documentation

These links offer advice for configuring, extending, tweaking, and upgrading your SV08:

* [https://github.com/Rappetor/Sovol-SV08-Mainline](https://github.com/Rappetor/Sovol-SV08-Mainline)
* [https://github.com/SphaeroX/Sovol-SV08-Tweaks](https://github.com/SphaeroX/Sovol-SV08-Tweaks)
* [https://github.com/asnajder/sv08-config](https://github.com/asnajder/sv08-config)
* [https://github.com/ss1gohan13/SV08-Replacement-Macros](https://github.com/ss1gohan13/SV08-Replacement-Macros)
* [https://github.com/adamrodgers/sv08](https://github.com/adamrodgers/sv08)
* [https://github.com/eric-s-raymond/sovol-SV08-from-scratch](https://github.com/eric-s-raymond/sovol-SV08-from-scratch)

## Modifications

This section provides links to hardware modifications available
for this printer:

### Commercial

Available for purchase:

* [Sovol Accessories and Parts](https://www.sovol3d.com/collections/fdm-parts/For-SV08)

### Community

Available for free:

* [SV08-Modular-Top-Hat](https://github.com/SeeingREDTonight/SV08-Modular-Top-Hat)
* [Printables: SV08](https://www.printables.com/search/models?q=sv08)
  * [SV08 Part Collection](https://www.printables.com/@Zappes_1061978/collections/1395092)
* [Thingiverse: SV08](https://www.thingiverse.com/search?q=sv08)

## Software

There are many kinds of software used in the design and printing
pipeline.  This section provides links to the options best suited
for the Sovol SV08:

### Main Board

The Sovol SV08 mainboard is based on the [BigTreeTech CB1][btt-cb1]
and contains an 64-bit ARM SoC running a custom [Armbian Linux][armbian] image.

[btt-cb1]: https://github.com/bigtreetech/CB1
[armbian]: https://armbian.org/

See the [Armbian page](./armbian.md) for more details about the stock OS image and
how to replace it.

### Printer Software

The printer software itself consists of:

|Project|Code|Docs|Purpose|
|-------|------|----|-------|
|KIAUH|[Code](https://github.com/dw-0/kiauh)||The Klipper Installation And Update Helper manages the remaining packages in this table|
|[Klipper](https://klipper3d.org)|[Code](https://github.com/Klipper3d/klipper)||Controls printer motion via onboard microcontrollers|
|Moonraker|[Code](https://github.com/Arksine/moonraker)|[Docs](https://moonraker.readthedocs.io)|Klipper Web API Server| 
|[Mainsail](https://mailsail.xyz)|[Code](https://github.com/mailsail-crew/mailsail)|[Docs](https://mailsail.xyz)|Klipper Web Interface|
|Mainsail Config|[Code](https://github.com/mailsail-crew/mailsail-config)||Mailsail Configuration Files|
|Moonraker Timelapse|[Code](https://github.com/mainsail-crew/moonraker-timelapse)||Moonraker Timelapse Plugin| 
|Crowsnest|[Code](https://github.com/mainsail-crew/crowsnest)||Webcam service| 
|Fluidd|[Code](https://github.com/fluidd-core/fluidd)|[Docs](https://docs.fluidd.xyz/)|Klipper UI|
|KlipperScreen|[Code](https://github.com/KlipperScreen/KlipperScreen)|[Docs](https://klipperscreen.github.io/KlipperScreen/)|Klipper Touchscreen GUI|

## Desktop Software

The following tools and resources exist to design and slice objects for your printing.

### Modeling

* [OpenSCAD](https://openscad.org)

### Slicing

* [Orcaslicer](https://orcaslicer.com): mainline contains SV08 printer profile
  * [Code](https://github.com/OrcaSlicer/OrcaSlicer)
  * [Sovol's version](https://wiki.sovol3d.com/en/Orca) (older)

## Contributing

If you would like to contribute to this Omnibus, please reach out:

### IRC

Join `#meta-sovol` on `irc.libera.chat`.

### Discord

Join the [Sovol 3D Printers](https://discord.gg/53vPnFMCTw) Discord server.

### GitHub

File issues or PRs, particularly after discussing your request or changes
on IRC or Discord.
