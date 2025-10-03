# arch rescue chroot
for (regular) ext4 fs. no btrfs shenanigans

- have archiso stick, boot it
- (setup internet access with `iwctl` if you need it)
- open luks container `cryptsetup luksOpen /dev/nvme0n1pX luks`
- `mount /dev/mapper/luks /mnt/`
- arch-chroot into /mnt
- do your thing
- leave, unmount, luksClose

## create emergency usb
- if your laptop is "dead" and your raspberry pi breaks, use this [android app](https://play.google.com/store/apps/details?id=eu.depau.etchdroid)
