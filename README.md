# mod-boot-sdcard

-ganti partisi bootloader di sdcard

-aml_autoscript 
if printenv bootfromsd; then exit; fi;
if fatload mmc 0 0x1000000 u-boot.ext; then go 0x1000000; fi;

-boot.ini
if test "${devtype}" = ""; then setenv devtype "/dtb/amlogic/meson-gxl-s905x-p212.dtb"; fi
if fatload ${devtype} ${devnum} 0x1000000 u-boot.ext; then go 0x1000000; fi;

-extlinux.conf
LABEL Armbian
LINUX /"sesuaikan dengan firmware"
INITRD /uInitrd

FDT /dtb/amlogic/"sesuaikan dengan firmware"
APPEND root=LABEL=ROOTFS rootflags=data=writeback rw console=ttyAML0,115200n8 console=tty0 no_console_suspend consoleblank=0 fsck.fix=yes fsck.repair=yes net.ifnames=0
