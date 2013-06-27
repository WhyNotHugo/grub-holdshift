Grub-holdshift
==============
About
-----

Simple GRUB script to make grub skip it's menu if you aren't holding
shift.
Script is mostly made up of bit canibalized from Ubuntu's os_prober
script.

Installation
------------

Copy 31_hold_shift to ```/etc/grub.d/```.

You'll need to add ```GRUB_FORCE_HIDDEN_MENU="true"'``` to
/etc/default/grub and re-run grub-mkconfig (generally, ```grub-mkconfig
-o /boot/grub/grub.cfg```, though this may vary depending on your
distribution. Consult your distributions manual if in doubt).
