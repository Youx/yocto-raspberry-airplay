Yocto Raspberry Airplay
=======================

Builds a Raspberry Pi system with Yocto project.

This image embeds [shairport-sync](https://github.com/mikebrady/shairport-sync),
so the board can act as an Airplay receiver.

The default build settings are for a Raspberry Pi Zero Wifi, to which you need
to add a valid sound output.

My personal choice is [Pimoroni's pHAT DAC](https://shop.pimoroni.com/products/phat-dac),
but you can go much cheaper by doing [your own RC filter](https://learn.adafruit.com/introducing-the-raspberry-pi-zero/audio-outputs)
