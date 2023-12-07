(from 8th to 12th gen intel i did this)

0. (boot archiso usb stick)
1. configure network with iwctl
1. as root: [installarch](https://github.com/nunq/installarch) start
2. reboot
3. create iwd config files & systemd-networkd config files /etc/iwd/main.conf, /etc/systemd/network/20-default.conf dhcp=ipv4, insert nameserver 1.1.1.1 into etc resolvconf
4. installarch postreboot
5. reboot
6. set modesetting driver in xorg.conf & MODULES append i915 in mkinitcpio.conf
8. get xauthority to spawn in $HOME
9. add DOT server in resolved config
10. borg extract backup to $HOME (should restore all firefox, joplin, etc. settings)
11. reboot
12. restore gpg key
13. diff packages

other things to check for:
* firefox saved passwords
* nextcloud sync settings
* move passwordstore
* luks header backup 
* crontabs
* copy saved iwd connections
* create new borg repo?

