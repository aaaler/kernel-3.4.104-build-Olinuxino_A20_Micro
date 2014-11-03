kernel-3.4.104-build-Olinuxino_A20_Micro
========================================

linux-sunxi 3.4.104 build for Olimex Olinuxino A20 Micro

Brief feature list:
* SATA EHCI drivers (can boot rootfs from sata drive)
* sunxi pwm driver (git://github.com/tanzilli/soft_pwm.git)
* sunxi nand drivers
* olimex's sunxi-i2c.patch 100khz patch __NOT__ applied
* soft_pwm module included
* ralink firmware from firmware-ralink debian package
* USB-OTG fix applied (https://www.olimex.com/forum/index.php?topic=1757.msg7922)


Install:

mount /dev/<your boot device> /boot

cp boot/* /boot

cp firmware/* /lib/firmware

cp modules/* /lib/modules


__boot/uEnv.txt__ made to boot from __sata__ drive, 2nd partition. 
change root variable to your rootfs device.
you can just delete this file to boot from 2nd part @ uSD 
