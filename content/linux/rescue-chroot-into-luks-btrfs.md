* have archiso usb stick, boot it
* `luksOpen /dev/sda... /dev/mapper/luks`
* `mount -o subvol=@SUBVOL /dev/mapper/luks /mountpoint`
* mount all the partitions you need
* `chroot /mountpoint`
* do your thing
* leave, unmount, luksClose

## create emergency usb
* if your laptop is "dead" and your raspberry pi breaks, use this [app](https://play.google.com/store/apps/details?id=eu.depau.etchdroid)


mount & luksOpen may be in the wrong order, i forgor
