# Installing Linux on the RCA Cambio
This is my *reboot* of the parent repo. I'll be using Debian 10 because it's what I prefer.

## Conclusions from my experiments:
* The i386 installation image must be used. I believe that this device could use the amd64 version, but the 32-bit BIOS can't recognize it.
* Debian *can* run without any modifications, but some part of the display manager causes the system to stick in an unusable state.
* The screen orientation can be fixed by modifying your kernel parameters in GRUB.

## My recommendations:
* Use the [unofficial i386 iso](https://cdimage.debian.org/debian-cd/current/i386/bt-dvd/), including firmware to support its network hardware.
* Prevent the x-server from trying to start: change default kernel parameters from `quiet` to `fbcon=rotate:1 text splash nomodeset 3`.

## To Do:
* Fix desktop environment bug
* Install [Phosh](https://puri.sm/posts/phosh-overview/)
* Fix screen calibration (inherited)
* Build Coreboot to replace stock BIOS
* Driver stuff?
