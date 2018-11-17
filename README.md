# Ubuntu Server 18.04.1 (Bionic) ARM image for Raspberry Pi 3 B+

### Instructions

Burn the image to SD card with dd/etcher/DiskWritter or your favorite tool.

Username: **ubuntu**  
Password: **ubuntu**

SSH is enabled by default, so you can login directly after first boot.

### Notes

* ([#2](https://github.com/AbelCS/ubuntu-server-bionic-rpi-3-b-plus/issues/2)) eth0 (wired) is failing to get routable on boot sometimes, if you have problems with this you can run **sudo netplan  apply** to get it running. You can check with **networkctl**.

* To get wireless connection working on boot you must edit **/etc/netplan/01-rpi-3-network.yaml** present in *cloudimg-rootfs* partition in your sdcard and add your SSID and PASSWORD.

* Filesystem will be expanded to fit your SD Card size on first boot.
