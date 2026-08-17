# Armbian on Sovol-SV08

The upstream Armbian project contains a board definition for the SV-08.
This document explains how to build and use the latest image.

## Build Armbian Image

On Ubuntu 24 LTS, the following commands should produce a stable image, once
you have installed all of the required dependencies on your build host:

```shell
git clone https://github.com/armbian/build armbian-sv08
cd armbian-sv08
./compile.sh BOARD=sovol-sv08 RELEASE=trixie BRANCH=current BUILD_DESKTOP=no BUILD_MINIMAL=yes KERNEL_CONFIGURE=no
```

The resulting images will be placed in the `output/` folder.

## Sovol Customizations

* [SV08-Armbian-Build-Scripts](https://github.com/mplinuxgeek/SV08-Armbian-Build-Scripts/tree/main)
* [SV08-Armbian-Image](https://github.com/mplinuxgeek/SV08-Armbian-Image/)
