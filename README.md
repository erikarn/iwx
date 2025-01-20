
iwx - from future crew
----------------------

This iwx driver is a port done by future crew from openbsd
to freebsd.

I've only tested it on the AX210 NIC in my GE76 Raider laptop.

For more information, see the post about it:

 * https://lists.freebsd.org/archives/freebsd-desktop/2024-December/005173.html
 * https://lists.freebsd.org/archives/freebsd-desktop/2024-December/005183.html

I'm doing whatever clean-up is required to get this thing
to build and run fine in FreeBSD-HEAD.

To build - only against FreeBSD-HEAD!

 * run fwget to get the firmware needed in /boot/firmware
 * edit sys/modules/build_module, change the paths
   to the kernel src, kernel obj dirs to your local
   directories.
 * .. and also edit KMODDIR - the path to install it to.
 * then run ./build_modules clean all install
 * the module will be in ../../modules/ , copy it to /boot/modules
 * and load it
 
