Grub-holdshift
==============
About
-----

Simple GRUB script to make grub skip it's menu if you aren't holding
shift.

The script is mostly made up of bit canibalized from Ubuntu's os_prober
script.

Installation
------------

Copy 31_hold_shift to ```/etc/grub.d/```.

For the master branch, that's all that needs to be done.

For the branch ```optional```, you'll need to add
```GRUB_FORCE_HIDDEN_MENU="true"``` to ```/etc/default/grub``` and re-run
grub-mkconfig (generally, ```grub-mkconfig -o /boot/grub/grub.cfg```, though
this may vary depending on your distribution. Consult your distributions
manual if in doubt).

The latter branch has been designed to be integrated into upstream, or
distribution packages without altering the default grub behaviour.