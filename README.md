***MOD BOOT SDCARD***

* Buka partisi boot pada sdcard openwrt
* Copy isi repository ini kedalam partisi boot
* Buka folder ```extlinux``` edit ```extlinux.conf``` ganti ```UUID``` sesuai dengan yang ada di ```uEnv.txt```
* Edit dtb sesuai tipe STB pada file ```extlinux.conf``` , ```boot.ini``` dan ```uEnv.txt```
* Ganti nama file ```u-boot-s905x-s912.bin``` menjadi ```u-boot.ext```
* Buat bootcard menggunakan AMLogic bootcardmaker
* Done
