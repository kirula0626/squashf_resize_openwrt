# squashf_resize_openwrt
Flash image to SD as normal with the firmware selector (I added packages to mine)
ssh into router
## opkg update && opkg install cfdisk resize2fs
## cfdisk /dev/mmcblk0
Select /dev/mmcblk0p2 and RESIZE it. The default entries will take the whole space.
Reboot
ssh into router
## resize2fs /dev/loop0
Success!
