# mkinitcpio-ps4
This hook makes your PS4 autoboot with the default mkinitcpio initramfs.



## Usage:
Here is an extract from my `/etc/mkinitcpio.conf`
```
HOOKS=(base udev autodetect keyboard keymap modconf block encrypt ps4 filesystems)
```
**MAKE SURE TO INCLUDE *encrypt* HOOK BEFORE *ps4* HOOK!!!!**
