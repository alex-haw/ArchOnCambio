# Installation Instructions

## Perform Windows Hardware Dumps

Note that per the vendor, installing an alternate OS voids the warranty, however I wanted 
assurance that I'd have a path back in the event this experiment didn't work out. 

## Making Bootable USB

## Getting Into the BIOS

The [vendor-provided instructions](https://rcaav.com/faq_support/i-need-to-enter-the-bios-of-the-tablet-w101v2/)
on how to get into the BIOS does _not_ work, at first, because the Windows EFI boot loader 
preempts it.  Hitting ESC seems to work after Windows has been blown away completely, 
however I did discover that holding the Volume-Up and Power-On buttons simultaneously does 
in fact work.  Use this method if you want Windows 10 to never be booted at all, and maybe 
you'll get lucky in claiming a refund from Microsoft, further reducing the cost of your 
low-end tablet :)

## Booting Arch on USB

## Connecting Wireless

## Back Up Original eMMC Image

## Re-Partition the eMMC

## Installation & Configuration Tweaks

grub bootloader default config

## Setting up Encrypted Home on Sdcard

## Calibrating the Touchscreen

## Getting Sound to Work

UPDATE: 2018/08/23 Sound now surprisingly works, either due to a kernel upgrade from 4.17 
to 4.18, or thanks to [plbossart's UCM repo](https://github.com/plbossart/UCM), or both.  
I pulled down this repo and copied the chtnau8824 directory to /usr/share/alsa/ucm and 
then ran alsaucm open chtnau8824, but got an error although it must have made some 
changes.  More TBD later.


