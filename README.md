# Arch Linux on RCA Cambio 10.1" (w101 v2)
Installing and configuring Arch Linux on the
[RCA Cambio model w101v2](https://shop.rcaav.com/shop/computing/2-in-1/cambio-w101v2)

## Status

UPDATE: 2/18/2019
This project is an unfinished Work In Progress!  I have not had time to work on it in several months.  In brief: for those considering buying this tablet and attempting to install Linux on it (any flavor), I would recommend spending the additional money on a different model tablet as the time you will save in configuring it will be more than worth it.  This project is for those who are not afraid to hack the kernel, submit patches, and spend _weeks_ doggedly trying to get a specific driver working.  You have been warned.  

As of about 8/10/2018,  Arch is installed and I have xorg with LXDE working well enough 
that this can be used comfortably enough as a laptop.  I've worked through several issues 
already, and there are plenty remaining, but I'm confident these will all be 
resolved in time and that this will be my everyday device.

## Installation Instructions

- My instructions can be found [here](https://github.com/RayFoulk/ArchOnCambio/blob/master/InstallationInstructions.md)
- These aren't necessarily _the_ way of accomplishing this, just how I did it.  YMMV.

## To Do

- Finish getting touchscreen calibrated
  - It seems that no-one has really solved the general case here, although there is 
    lots of work being done on xinput_calibrator, so that's hopeful.
  - xorg configuration files in /etc/X11/xorg.conf.d use a slightly different nomenclature
    for key/type/value than xinput, which can be confusing.
- Get sound working
- Get auto-rotate working via accelerometer
- Get Front and Rear cameras working (ov2680 on i2c bus)
  - Arch kernels have not yet picked up ov2680 module
  - Linus' kernel.org git repo for 4.18 contains the ov2680 module, which builds and 
modprobe loads it, but there are no /dev/videoN devices created.  Suspect udev script 
needs to be modified or do mknod manually might fix this.


## Related Projects

- devinsmith: [rca-cambio-linux](https://github.com/devinsmith/rca-cambio-linux)
- onitake: [gsl-firmware](https://github.com/onitake/gsl-firmware/tree/master/firmware/rca/w101v2)
- plbossart: [UCM](https://github.com/plbossart/UCM)
- reinderien: [xcal](https://github.com/reinderien/xcal)



