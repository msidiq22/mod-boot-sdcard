***MOD BOOT SDCARD***

**Cara Pasang Manual:**

* Buka partisi boot pada sdcard openwrt
* Copy isi repository ini kedalam partisi boot
* Buka folder ```extlinux``` edit ```extlinux.conf``` ganti ```UUID``` sesuai dengan yang ada di ```uEnv.txt```
* Edit dtb sesuai tipe STB pada file ```extlinux.conf``` , ```boot.ini``` dan ```uEnv.txt```
* Ganti nama file ```u-boot-s905x-s912.bin``` menjadi ```u-boot.ext```
* Buat bootcard menggunakan AMLogic bootcardmaker
* Done

**Cara Pasang Via Github Action:**

* Fork Repository ini
* Buka Tab Actions Pada Repository yang sudah anda fork
* Pilih Mod SDCard
* Klik Run workflow
* Pilih Tipe STB dan Masukkan Link firmware
* Link yang di support ```Mediafire```, ```GDrive```, ```Mega``` dan ```direct link```
* Setelah workflow dijalankan, Tunggu sekitar 2-5 Menit
* FW Hasil mod sdcard akan muncul di halaman releases
* Done
