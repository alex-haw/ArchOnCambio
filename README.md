# Arch Linux on RCA Cambio 10.1" (w101 v2)
Installing and configuring Arch Linux on the
[RCA Cambio model w101v2](https://shop.rcaav.com/shop/computing/2-in-1/cambio-w101v2)

## Status

As of about 8/10/2018,  Arch is installed and I have xorg with LXDE working well enough 
that this can be used comfortably enough as a laptop.  I've worked through several issues 
already, and there are plenty remaining, but I'm confident these will all be 
resolved in time and that this will be my everyday device.

## Installation Instructions

- My instructions can be found [here](https://github.com/RayFoulk/ArchOnCambio/blob/master/InstallationInstructions.md)
- These aren't necessarily _the_ way of accomplishing this, just how I did it.  YMMV.

## To Do

- Finish getting touchscreen calibrated
-- It seems to me that no-one has truly 'done the math' on this, including the distinction between the Coordinate Translation Matrix versus the Calibration Matrix 
- Get sound working
- Get auto-rotate working via accelerometer
- Get Front and Rear cameras working (ov2680 on i2c bus)

## Related Projects

- devinsmith's [rca-cambio-linux](https://github.com/devinsmith/rca-cambio-linux)
- onitake's [gsl-firmware](https://github.com/onitake/gsl-firmware/tree/master/firmware/rca/w101v2)

