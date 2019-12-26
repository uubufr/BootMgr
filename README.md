# BootMgr
Script for generate simple Grub2 configuration

Warning: Only tested on Fedora 30 and 31!

Features:

- Add Current kernel, and previous kernel
- Admin menu for rescue access
- Add restart - stop - System Setup
- Add user passwords
- Try to add Windows on Dual Boot System
- Install theme
- Sign modules

## How to:

First, install it:

    git clone https://github.com/uubufr/BootMgr
    cd BootMgr
    chmod u+x BootMgr
    ./BootMgr install

Next review /etc/BootMgr/BootMgr_.conf

then test:

    BootMgr test

This create bootmgr.cfg and don't change grub.cfg. Restart, and in grub prompt use 'configfile' to load bootmgr.cfg. If all is ok, you can install in with:

    BootMgr update

You can install themes in /var/lib/BootMgr/themes/ and select theme with:

    BootMgr theme <theme name>

Note: I don't provide any support
