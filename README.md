Yocto Raspberry Airplay
=======================


About this project
------------------

Builds a Raspberry Pi system with Yocto project.

This image embeds [shairport-sync](https://github.com/mikebrady/shairport-sync),
so the board can act as an Airplay receiver.

The default build settings are for a Raspberry Pi Zero Wifi, to which you need
to add a valid sound output.

My personal choice is [Pimoroni's pHAT DAC](https://shop.pimoroni.com/products/phat-dac),
but you can go much cheaper by doing [your own RC filter](https://learn.adafruit.com/introducing-the-raspberry-pi-zero/audio-outputs)


How to build
------------

Make sure you have at least 20 or 30 GB of disk space available,
downloading and building all the packages will take a lot of space (and time).

```bash
git clone --recursive https://github.com/Youx/yocto-raspberry-airplay
cd yocto-raspberry-airplay
source poky/oe-init-build-env ./build
bitbake core-image-minimal
```
