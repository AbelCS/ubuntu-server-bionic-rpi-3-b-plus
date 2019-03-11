# Ubuntu Server 18.04.2 (Bionic) ARM image for Raspberry Pi 3 B+

### Instructions

Burn the image to SD card with dd/etcher/DiskWritter or your favorite tool.

Username: **ubuntu**  
Password: **ubuntu**

SSH is enabled by default, so you can login directly after first boot.

### Notes

* To get wireless connection working on boot you must edit **/etc/netplan/01-rpi-3-network.yaml** present in *cloudimg-rootfs* partition in your sdcard and add your SSID and PASSWORD.

* Filesystem will be expanded to fit your SD Card size on first boot.
